---
title: 使用 Microsoft Microsoft 搜索中的 Graph API 搜索日历事件
description: 您可以在用户自己的日历中搜索。
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 277c46e6298aa532d300b23fcba707c678e38e035007d2ef63fa249951afa633
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54171971"
---
# <a name="use-the-microsoft-search-api-to-search-calendar-events"></a>使用 Microsoft 搜索 API 搜索日历事件

使用 Microsoft 搜索 API 搜索登录用户的主日历中的事件。 搜索的用户标识基于身份验证令牌。

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

## <a name="example"></a>示例

### <a name="request"></a>请求

本示例在用户的日历中搜索关键字"contoso"，最多返回 25 个结果。

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "event"
      ],
      "query": {
        "queryString":"contoso"
      },
      "from": 0,
      "size": 25
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
   "@odata.type": "#microsoft.graph.searchResponse",
   "searchTerms": [
    "contoso"
   ],
   "hitsContainers": [
    {
     "@odata.type": "#microsoft.graph.searchHitsContainer",
     "hits": [
      {
       "@odata.type": "#microsoft.graph.searchHit",
       "hitId": "AAMkADEwODY2NzllLTQ3MmEtNGRlMC05ZTUyLTE4ZDRhYmU1ZGM3NABGAAAAAAA3+iYQBnJnQabRVDelNhnzBwAejhWkAOAxQ6M4c1c9NwfrAAAAAAENAAAejhWkAOAxQ6M4c1c9NwfrAABbUZLJAAA=",
       "rank": 1,
       "summary": "Here is a summary of your events from last week",
       "resource": {
        "@odata.type": "#microsoft.graph.event",
        "end": {
         "dateTime": "2020-06-16T04:15:00Z",
         "timeZone": "UTC"
        },
        "hasAttachments": false,
        "iCalUId": "040000008200E00074C5B7101A82E008000000007093FDD79B3AD60100000000000000001000000036DAA2262EB4E04DA27DA77985FB8251",
        "isAllDay": false,
        "sensitivity": "Normal",
        "start": {
         "dateTime": "2020-06-16T03:30:00Z",
         "timeZone": "UTC"
        },
        "subject": "Weekly digest: Microsoft 365 changes",
        "type": "Single"
       }
      }
     ],
     "total": 1,
     "moreResultsAvailable": false
    }
   ]
  }
 ]
}
```

## <a name="known-limitations"></a>已知限制

- 只能访问登录用户自己的邮箱。 不支持搜索委派邮箱。
- 对于事件[，searchHitsContainer](/graph/api/resources/searchhitscontainer)类型的 total 属性包含页面上的结果数，而不是匹配结果的总数。 
- 事件不支持对结果进行排序。 请求中的 sort 子句将在响应中返回错误请求错误代码。

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview)
