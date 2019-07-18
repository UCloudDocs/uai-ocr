{{indexmenu_n>10}}

====环境准备====

####环境要求

- Python 2.7
- UAI-Ocr SDK
  - git clone https://github.com/ucloud/uai-saas-sdk.git
  - sudo python setup.py install


####UAI-OCR 工具一览

| 命令子类       | 命令名称        | 命令说明         |
| resource   | create      | 创建资源         |
|            | delete      | 删除资源         |
|            | modifyname  | 修改资源名称信息     |
|            | modifymemo  | 修改资源备注信息     |
|            | list        | 获取资源列表       |
|            | listtype    | 获取资源类型列表     |
|            | listrecord  | 获取资源请求记录     |
| signature  | gen         | 生成signature  |
| ocr        | idcard      | 创建身份证识别任务    |
|            | bill        | 创建票据识别任务     |