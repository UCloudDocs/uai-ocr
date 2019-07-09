{{indexmenu_n>20}}

### 资源管理

\#\#\#\#使用说明

\`\`\` python ocr\_tool.py resource
{create,delete,modifyname,modifymemo,list,listrecord,listtype} ...
\`\`\`

\*注：\[\]表示可选\*

\#\#\#\#参数说明

|                   |        |                    |
| ----------------- | ------ | ------------------ |
| 参数名称              | 参数类型   | 参数说明               |
| public\\\_key     | String | 用户的公钥              |
| private\\\_key    | String | 用户的私钥              |
| project\\\_id     | String | bitmap的具体含义        |
| region            | String | 地域信息，默认cn-bj2      |
| zone              | String | 可用区信息，默认cn-bj2     |
| resource\\\_types | String | 资源类型，若含多种资源，用","隔开 |
| resource\\\_name  | String | 资源名称               |
| resource\\\_memo  | String | 资源备注               |
| limit             | String | 查询记录总数             |
| offset            | String | 首条记录的偏移量           |

\#\#\#\#1. 创建资源

\`\`\` python ocr\_tool.py resource create --public\_key PUBLIC\_KEY \\

``` 
                                --private_key PRIVATE_KEY \
                                [--project_id PROJECT_ID] \
                                [--region REGION] \
                                [--zone ZONE] \
                                --resource_types RESOURCE_TYPES \
                                [--resource_name RESOURCE_NAME] \
                                [--resource_memo RESOURCE_MEMO]
```

\`\`\`

\#\#\#\#2. 删除资源

\`\`\` python ocr\_tool.py resource delete --public\_key PUBLIC\_KEY \\

``` 
                                --private_key PRIVATE_KEY \
                                [--project_id PROJECT_ID] \
                                [--region REGION] \
                                [--zone ZONE] \
                                --resource_id RESOURCE_ID
```

\`\`\`

\#\#\#\#3. 修改资源名称

\`\`\` python ocr\_tool.py resource modifyname --public\_key PUBLIC\_KEY
\\

``` 
                                --private_key PRIVATE_KEY \
                                [--project_id PROJECT_ID] \
                                [--region REGION] \
                                [--zone ZONE] \
                                --resource_id RESOURCE_ID \
                                --resource_name RESOURCE_NAME
```

\`\`\`

\#\#\#\#4. 修改资源备注

\`\`\` python ocr\_tool.py resource modifymemo --public\_key PUBLIC\_KEY
\\

``` 
                                    --private_key PRIVATE_KEY \
                                    [--project_id PROJECT_ID] \
                                    [--region REGION] \
                                    [--zone ZONE] \
                                    --resource_id RESOURCE_ID \
                                    --resource_memo RESOURCE_MEMO
```

\`\`\`

\#\#\#\#5. 获取已创建资源列表

\`\`\` python ocr\_tool.py resource list --public\_key PUBLIC\_KEY \\

``` 
                                    --private_key PRIVATE_KEY \
                                    [--project_id PROJECT_ID] \
                                    [--region REGION] \
                                    [--zone ZONE] \
                                    [--limit LIMIT] \
                                    [--offset OFFSET]
```

\`\`\`

\#\#\#\#6. 获取可用资源类型

\`\`\` python ocr\_tool.py resource listtype --public\_key PUBLIC\_KEY
\\

``` 
                                  --private_key PRIVATE_KEY \
                                  [--project_id PROJECT_ID] \
                                  [--region REGION] \
                                  [--zone ZONE] \
```

\`\`\`

\#\#\#\#7. 获取资源使用记录信息

\`\`\` python ocr\_tool.py resource listrecord --public\_key PUBLIC\_KEY
\\

``` 
                                      --private_key PRIVATE_KEY \
                                      [--project_id PROJECT_ID] \
                                      [--region REGION] \
                                      [--zone ZONE] \
                                      --begin_time BEGIN_TIME \
                                      --end_time END_TIME \
                                      [--resource_id RESOURCE_ID]
```

\`\`\`
