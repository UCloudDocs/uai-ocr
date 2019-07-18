{{indexmenu_n>10}}

====接入流程====


- **在ucloud.cn上注册账号**
- **在console上创建项目**
- **创建资源**

 创建资源提供[[ai:uai-ocr:api:resource:create-resource|Http API]]和[[ai:uai-ocr:pysdk:resource|Python SDK]]两种方式。
 
 API和SDK的使用都需要填充ProjectId字段, ProjectId的查询步骤如下：
 
  - 登陆控制台：https://console.ucloud.cn/dashboard
  - ProjectId如下图红框所示

    {{:ai:uai-censor:获取projectid.png |}}
 

- **开始图像OCR**

 图像OCR提供两种调用方式：

 - [[ai:uai-ocr:api:ocr|Restful API]]
 - [[ai:uai-ocr:pysdk:ocr|Python SDK]]