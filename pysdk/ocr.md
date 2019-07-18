{{indexmenu_n>30}}

====OCR====

####使用说明

```
python ocr_tool.py ocr {idcard,bill} ...
```

####参数说明

| 参数名称 | 参数类型 | 参数说明 |
| public\_key | String | 用户的公钥 |
| resource\_id | String | 资源ID|
| timestamp | Int | 时间戳信息|
| signature | String | 签名信息 |
| method | String | 图片输入方法，可选项{url,file}|
| image | String | 图片内容 |
| url | String | 图片地址 |

####1. 创建OCR身份证识别任务

```
python ocr_tool.py ocr idcard  --signature SIGNATURE \
  				--public_key PUBLIC_KEY \
  				--resource_id RESOURCE_ID \
  				--timestamp TIMESTAMP \
  				--method {url, file} \
  				[--image IMAGE] \
  				[--url URL]
```

####2. 创建OCR票据识别任务

```
python ocr_tool.py ocr bill  --signature SIGNATURE \
  				--public_key PUBLIC_KEY \
  				--resource_id RESOURCE_ID \
  				--timestamp TIMESTAMP \
  				--method {url, file} \
  				[--image IMAGE] \
  				[--url URL]
```