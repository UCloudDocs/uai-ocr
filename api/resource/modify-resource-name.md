{{indexmenu_n>30}}

### 修改资源名称

**请求方式 GET <https://api.ucloud.cn>**

**请求参数(拼在Url后面)**

|              |        |                              |                                                  |
| ------------ | ------ | ---------------------------- | ------------------------------------------------ |
| 字段名          | 字段类型   | 说明                           | 是否必须                                             |
| Action       | String | 固定值：ModifyUAIOcrResourceName | 是                                                |
| PublicKey    | String | 私钥                           | 是                                                |
| Signature    | String | 签名                           | 签名参照https://docs.ucloud.cn/api/summary/signature |
| Region       | String | 地域信息,可选地域：cn-bj2             | 是                                                |
| ProjectId    | String | 项目ID。不填写则为默认项目               | 否                                                |
| ResourceId   | String | 待修改资源ID                      | 是                                                |
| ResourceName | String | 修改后的资源名称                     | 是                                                |

**响应参数**

|         |        |      |
| ------- | ------ | ---- |
| 字段名     | 字段类型   | 说明   |
| Action  | String | 操作名称 |
| RetCode | Int    | 返回码  |
| Message | String | 返回信息 |