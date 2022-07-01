---
title: 使用 Microsoft 搜索 API 搜索 Outlook 消息
description: 可以使用 Microsoft Graph 中的 Microsoft 搜索 API 搜索电子邮件中的信息，并返回按相关性排名的消息。
author: knightsu
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 1769bda3a6d4f4ed2fed6fc8294b7dc049749482
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436972"
---
# <a name="use-the-microsoft-search-api-to-search-outlook-messages"></a>使用 Microsoft 搜索 API 搜索 Outlook 消息

使用 Microsoft Graph 中的 Microsoft 搜索 API 搜索电子邮件中的信息，返回按相关性排名的消息，并呈现专用搜索体验。 搜索适用于登录用户自己的邮箱中邮件的正文和附件。

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

搜索查询可以包含最终用户在 Outlook 的 **“搜索**”文本框中输入的 [筛选器](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da)。

消息搜索结果按 **receivedDateTime** 按降序排序。

消息搜索适用于工作或学校帐户。 用户可以搜索自己的邮箱，但无法搜索委派邮箱。 有关详细信息，请参阅 [已知的限制](#known-limitations)。

消息搜索还会查找附件。 消息附件搜索 [支持的文件类型](/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) 与 SharePoint Online 搜索的文件类型相同。

## <a name="example-1-search-messages-in-a-users-mailbox"></a>示例 1：搜索用户邮箱中的邮件

以下示例查询登录用户邮箱中包含邮件任意部分的字符串“contoso”的邮件 (发件人名称、主题、邮件正文或) 的任何附件。 查询返回前 25 个结果。 搜索结果按 **DateTime** 降序排序。

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

下面是响应的示例，其中包含一条与搜索条件匹配的消息。

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

## <a name="example-2-search-top-results-messages"></a>示例 2：搜索热门结果消息

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

### <a name="response"></a>响应

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

- 只能访问已登录用户自己的邮箱。 不支持搜索委派邮箱。
- 对于消息，[searchHitsContainer](/graph/api/resources/searchhitscontainer) 类型的 **总** 属性包含页面上的结果数，而不是匹配结果的总数。
- 事件不支持对结果进行排序。 请求中的 sort 子句将在响应中返回错误的请求错误代码。

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview)
