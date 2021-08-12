---
title: 使用 Microsoft Microsoft 搜索中的 Graph API 搜索邮件
description: 您可以使用 Microsoft 搜索 API 在电子邮件中搜索信息，返回按相关性排名的邮件，并呈现专用的搜索体验。
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 1edc75cab2192fd000a29e565869e2534ecf4032540fbe3073b1b2dccdd39d76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54165516"
---
# <a name="use-the-microsoft-search-api-to-search-outlook-messages"></a>使用 Microsoft 搜索 API 搜索Outlook消息

使用 Microsoft 搜索 API 在电子邮件中搜索信息，返回按相关性排名的邮件，并呈现专用的搜索体验。 搜索适用于已登录用户自己的邮箱中邮件的正文和附件。

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

搜索查询可以包含[最终用户](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da)在"搜索"文本框中输入的筛选器Outlook。

邮件搜索结果按 **receivedDateTime** 按降序排序。

邮件搜索适用于工作或学校帐户。 用户可以搜索自己的邮箱，但不能搜索委派邮箱。 有关详细信息，请参阅 [已知限制](#known-limitations)。

邮件搜索还会查找附件。 邮件[附件搜索](/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types)支持的文件类型与用于联机搜索SharePoint相同。

## <a name="example-1-search-messages-in-a-users-mailbox"></a>示例 1：搜索用户邮箱中的邮件

以下示例查询已登录用户的邮箱中的邮件，该邮箱包含邮件任何部分包含字符串"contoso" (发件人名称、主题、邮件正文或任何附件) 。 查询将返回前 25 个结果。 搜索结果按 **DateTime** 降序排序。

### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "message"
      ],
      "query": {
        "queryString": "contoso"
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

### <a name="response"></a>响应

下面是一个响应示例，其中包含一条匹配搜索条件的邮件。

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
              "rank": 1,
              "summary": "Here is a summary of your messages from last week",
              "resource": {
                "@odata.type": "#microsoft.graph.message",
                "createdDateTime": "2019-10-07T10:00:08Z",
                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                "receivedDateTime": "2019-10-07T10:00:09Z",
                "sentDateTime": "2019-10-07T09:59:52Z",
                "hasAttachments": false,
                "subject": "Weekly digest: Microsoft 365 changes",
                "bodyPreview": "Here is a summary of your messages from last week -   New Feature: Live captions in English-US a",
                "importance": "normal",
                "replyTo": [
                  {
                    "emailAddress": {
                      "name": "Goncalo Torres"
                    }
                  }
                ],
                "sender": {
                  "emailAddress": {
                    "name": "Office365 Message Center",
                    "address": "gtorres@contoso.com"
                  }
                },
                "from": {
                  "emailAddress": {
                    "name": "Office365 Message Center",
                    "address": "gtorres@contoso.com"
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

## <a name="example-2-search-top-results-messages"></a>示例 2：搜索热门结果邮件

以下示例使用示例 1 中显示的搜索查询，并按相关性对结果进行排序。 

<!-- markdownlint-disable MD024 -->
### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "message"
      ],
      "query": {
        "queryString": "contoso"
      },
      "from": 0,
      "size": 15,
      "enableTopResults": true
    }
  ]
}
```

#### <a name="response"></a>响应
```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
              "rank": 1,
              "summary": "Here is a summary of your messages from last week",
              "resource": {
                "@odata.type": "#microsoft.graph.message",
                "createdDateTime": "2019-10-07T10:00:08Z",
                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                "receivedDateTime": "2019-10-07T10:00:09Z",
                "sentDateTime": "2019-10-07T09:59:52Z",
                "hasAttachments": false,
                "subject": "Weekly digest: Microsoft 365 changes",
                "bodyPreview": "Here is a summary of your messages from last week -   New Feature: Live captions in English-US a",
                "importance": "normal",
                "replyTo": [
                  {
                    "emailAddress": {
                      "name": "Goncalo Torres"
                    }
                  }
                ],
                "sender": {
                  "emailAddress": {
                    "name": "Office365 Message Center",
                    "address": "gtorres@contoso.com"
                  }
                },
                "from": {
                  "emailAddress": {
                    "name": "Office365 Message Center",
                    "address": "gtorres@contoso.com"
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

## <a name="known-limitations"></a>已知限制

- 只能访问登录用户自己的邮箱。 不支持搜索委派邮箱。
- 对于邮件[，searchHitsContainer](/graph/api/resources/searchhitscontainer)类型的 total 属性包含页面上的结果数，而不是匹配结果的总数。 
- 事件不支持对结果进行排序。 请求中的 sort 子句将在响应中返回错误请求错误代码。

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API](/graph/api/resources/search-api-overview)