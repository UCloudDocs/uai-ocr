{{indexmenu_n>20}}

====创建票据识别任务====

**请求方式 POST http://api.uai.ucloud.cn/v1/ocr/bill**

**Signature使用参数**

- PublicKey： Header参数
- ResourceId： Header参数
- Timestamp： Header参数
- Url： 请求参数， 若无，则不放入该字段

生成Signature签名算法流程包括四步：  
（1）将请求参数按照名进行升序排列；  
（2）构造被签名参数串；  
（3）计算签名；  
（4）使用签名组合HTTP请求。  

*具体内容请参考签名文档：https://docs.ucloud.cn/api/summary/signature*

**请求Header参数**

| 参数 | 类型 | 说明 | 是否必须 |
| Signature | String | 签名 | 是 |
| PublicKey | String | 公钥 | 是 |
| ResourceId | String | 资源ID | 是 |
| Timestamp | String | 当前unix时间戳 | 是 |

**请求参数(Multipart/Form-data)**

| 参数 | 类型 | 说明 | 是否必须 |
| Method | String | 请求方式，可选方式：url - 图像url方式，file - 图像二进制文件方式 | 是 |
| Url | String | 图像Url, Method='url'时必填 | 否 |
| Image | Binary | 图像二进制文件，Method='file'时必填 | 否 |


**响应参数(JSON)**

| 参数 | 类型 | 说明 |
| RetCode | Int | 错误码 |
| Message | String | 错误信息 |
| Timestamp | Int | unix时间戳 |
| Result | Result | 结果对象 |

**Result:**

| 参数          | 类型      | 说明      |
| ExpireDate  | String  | 票据过期时间  |
| TicketId    | String  | 票据ID    |
| Money       | String  | 票据金额    |
| BankId      | String  | 银行ID    |