---
title: 搜索邮件
description: Microsoft Search API 允许应用搜索电子邮件中的信息，返回相关性排名的邮件，并呈现专用搜索体验。
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 985da47e5a7b96cead416e8e5cda32dae0357adb
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38303130"
---
# <a name="search-messages"></a>搜索邮件

Microsoft Search API 允许应用搜索电子邮件中的信息，返回相关性排名的邮件，并呈现专用搜索体验。 搜索适用于用户自己的邮箱中邮件的正文和附件。

搜索查询可以包含最终用户在 Outlook 的 "**搜索**" 文本框中输入的[筛选器](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da)。

邮件搜索结果按**receivedDateTime**降序排列。

邮件搜索适用于工作或学校帐户。 用户可以搜索其自己的邮箱，但不能搜索委派邮箱中的邮箱。 请参阅下面的[已知限制](#known-limitations)。

邮件搜索还会查找附件。 [附件支持的文件类型](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types)与 SharePoint Online 中的文件类型相同。

## <a name="examples"></a>示例

### <a name="example-1"></a>示例 1

下面的示例查询登录用户邮箱中的邮件，其中包含邮件的任何部分（发件人姓名、主题、邮件正文或任何附件）中的字符串 "contoso"。 查询返回前25个结果。 搜索结果按日期/降序进行排序。

#### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [{
      "entityTypes": ["microsoft.graph.message"],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

#### <a name="response"></a>响应 

以下是包含一条与搜索条件相匹配的邮件的响应示例。 

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
    "value": [
        {
            "searchTerms": [
                "contoso"
            ],
            "hitsContainers": [
                {
                    "total": 1,
                    "moreResultsAvailable": false,
                    "hits": [
                        {
                            "_id": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
                            "_score": 1,
                            "_sortField": "DateTime",
                            "_summary": "Here is a summary of your messages from last week",
                            "_source": {
                                "@odata.type": "#microsoft.graph.message",
                                "createdDateTime": "2019-10-07T10:00:08Z",
                                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                                "receivedDateTime": "2019-10-07T10:00:09Z",
                                "sentDateTime": "2019-10-07T09:59:52Z",
                                "hasAttachments": false,
                                "subject": "Weekly digest: Office 365 changes",
                                "bodyPreview": "Here is a summary of your messages from last week -   New Feature: Live captions in English-US a",
                                "importance": "normal",
                                "replyTo": [
                                    {
                                        "emailAddress": {
                                            "name": "Goncalo Torres"
                                        }
                                    }
                                ],
                                "sender": {
                                    "emailAddress": {
                                        "name": "Office365 Message Center",
                                        "address": "gtorres@contoso.com"
                                    }
                                },
                                "from": {
                                    "emailAddress": {
                                        "name": "Office365 Message Center",
                                        "address": "gtorres@contoso.com",
                                    }
                                }
                            }
                        }
                    ]
                }
            ]
        }
    ]
}
```

### <a name="example-2-search-top-results-messages"></a>示例2搜索热门结果邮件
下面的示例使用与[示例 1](#example-1)相同的搜索查询，并按相关性对结果进行排序。 

#### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
    "requests": [{
        "entityTypes": ["microsoft.graph.message"],
        "query": {
            "query_string": {
                "query": "contoso"
            }
        },
        "from": 0,
        "size": 15,
        "enableTopResults": true
    }]
}
```

## <a name="known-limitations"></a>已知限制

- 您只能访问用户自己的邮箱。 不支持搜索委派的邮箱 

- 对于邮件， [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta)类型的**total**属性包含页面上的结果数，而不是匹配结果的总数。

## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [使用搜索 API](/graph/api/resources/search-api-overview?view=graph-rest-beta)
