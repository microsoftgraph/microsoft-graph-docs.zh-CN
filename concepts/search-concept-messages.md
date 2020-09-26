---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索邮件
description: 您可以使用 Microsoft 搜索 API 搜索电子邮件中的信息，返回按相关性排序的邮件，并呈现专用搜索体验。
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: e9917b8153946161168e90f78399f29b6a7f3df3
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288824"
---
# <a name="use-the-microsoft-search-api-to-search-outlook-messages"></a>使用 Microsoft 搜索 API 搜索 Outlook 邮件

使用 Microsoft Search API 搜索电子邮件中的信息，返回相关性排名的邮件，并呈现专用搜索体验。 搜索适用于登录用户自己的邮箱中的邮件的正文和附件。

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

搜索查询可以包含最终用户在 Outlook 的 "**搜索**" 文本框中输入的[筛选器](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da)。

邮件搜索结果按 **receivedDateTime** 降序排列。

邮件搜索适用于工作或学校帐户。 用户可以搜索其自己的邮箱，但不能搜索委派的邮箱。 有关详细信息，请参阅 [已知限制](#known-limitations)。

邮件搜索还会查找附件。 邮件附件搜索支持的文件类型与 SharePoint Online 搜索所 [支持的文件类型](/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) 相同。

## <a name="example-1-search-messages-in-a-users-mailbox"></a>示例1：搜索用户邮箱中的邮件

下面的示例在登录用户的邮箱中查询邮件的任何部分中包含字符串 "contoso" 的邮件， (发件人姓名、主题、邮件正文或任何附件) 。 查询返回前25个结果。 搜索结果按 **日期/** 降序进行排序。

### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/beta/search/query
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

下面是一个响应示例，其中包含一个与搜索条件相匹配的邮件。

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
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

## <a name="example-2-search-top-results-messages"></a>示例2：搜索排名靠前的结果邮件

下面的示例使用示例1中所示的搜索查询，并按相关性对结果进行排序。 

<!-- markdownlint-disable MD024 -->
### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/beta/search/query
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
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

- 您只能访问登录用户自己的邮箱。 不支持搜索委派的邮箱。
- 对于邮件， [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta&preserve-view=true)类型的**total**属性包含页面上的结果数，而不是匹配结果的总数。
- 事件不支持排序结果。 请求中的 sort 子句将在响应中返回错误的请求错误代码。

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)