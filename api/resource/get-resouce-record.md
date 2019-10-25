

# 获取资源的OCR记录

**请求方式 GET https://api.ucloud.cn**

**请求参数(拼在Url后面)**

| 字段名 | 字段类型 | 说明 | 是否必须 |
| ------ | -------- | ---- | -------- |
| Action | String | 固定值：GetUAIOcrResourceRecordInfo | 是 |
| PublicKey | String | 私钥 | 是 |
| Signature | String | 签名 | 签名参照https://docs.ucloud.cn/api/summary/signature |
| Region | String | 地域信息,可选地域：cn-bj2 | 是 |
| ProjectId | String | 项目ID。不填写则为默认项目 | 否 |
| BeginTime | Int64 | 开始查询时间 | 是 |
| EndTime | Int64 | 结束查询时间 | 是 |
| ResourceId | String | 需要查询的资源ID；若不提供，默认获取当前用户所有资源的请求记录 | 否 |

**响应参数**

| 字段名 | 字段类型 | 说明 |
| ------ | -------- | ---- |
| Action | String | 操作名称 |
| RetCode | Int | 返回码|
| Message | String | 返回信息 |
| TotalRecordCount | Int | 资源请求记录总数 |
| TotalOcrCount | Int | 请求总数 |
| DataSet | Array of UAIOcrResourceRecordInfo | 资源请求记录的具体信息 |

**UAIOcrResourceRecordInfo**

| 字段名 | 字段类型 | 说明 |
| ------ | -------- | ---- |
| ResourceId | String | 资源ID |
| Status | String | 资源状态 |
| OcrCount | Int | 文字识别请求数 |
| LatestRecordTime | Int | 最新请求记录创建时间 |

