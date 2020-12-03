---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索日历事件
description: 您可以在用户自己的日历中进行搜索。
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: bedad2dcf94df6024bcba7f0760dbe5c1cf97c18
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49521906"
---
# <a name="use-the-microsoft-search-api-to-search-calendar-events"></a><span data-ttu-id="c90b8-103">使用 Microsoft 搜索 API 搜索日历事件</span><span class="sxs-lookup"><span data-stu-id="c90b8-103">Use the Microsoft Search API to search calendar events</span></span>

<span data-ttu-id="c90b8-104">使用 Microsoft 搜索 API 搜索登录用户的主日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="c90b8-104">Use the Microsoft Search API to search for events in the signed-in user’s primary calendar.</span></span> <span data-ttu-id="c90b8-105">搜索的用户标识基于身份验证令牌。</span><span class="sxs-lookup"><span data-stu-id="c90b8-105">The user identity for the search is based on the auth token.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

## <a name="example"></a><span data-ttu-id="c90b8-106">示例</span><span class="sxs-lookup"><span data-stu-id="c90b8-106">Example</span></span>

### <a name="request"></a><span data-ttu-id="c90b8-107">请求</span><span class="sxs-lookup"><span data-stu-id="c90b8-107">Request</span></span>

<span data-ttu-id="c90b8-108">本示例将在用户的日历中搜索关键字 "contoso"，并返回最大25个结果。</span><span class="sxs-lookup"><span data-stu-id="c90b8-108">This example searches in the user's calendar for the keyword "contoso", and will return up to 25 results.</span></span>

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

#### <a name="response"></a><span data-ttu-id="c90b8-109">响应</span><span class="sxs-lookup"><span data-stu-id="c90b8-109">Response</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="c90b8-110">已知限制</span><span class="sxs-lookup"><span data-stu-id="c90b8-110">Known limitations</span></span>

- <span data-ttu-id="c90b8-111">您只能访问登录用户自己的邮箱。</span><span class="sxs-lookup"><span data-stu-id="c90b8-111">You can access only the signed-in user’s own mailbox.</span></span> <span data-ttu-id="c90b8-112">不支持搜索委派的邮箱。</span><span class="sxs-lookup"><span data-stu-id="c90b8-112">Searching delegated mailboxes is not supported.</span></span>
- <span data-ttu-id="c90b8-113">对于事件， [searchHitsContainer](/graph/api/resources/searchhitscontainer)类型的 **total** 属性包含页面上的结果数，而不是匹配结果的总数。</span><span class="sxs-lookup"><span data-stu-id="c90b8-113">For events, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer) type contains the number of results on the page, not the total number of matching results.</span></span>
- <span data-ttu-id="c90b8-114">事件不支持排序结果。</span><span class="sxs-lookup"><span data-stu-id="c90b8-114">Sorting results is not supported for events.</span></span> <span data-ttu-id="c90b8-115">请求中的 sort 子句将在响应中返回错误的请求错误代码。</span><span class="sxs-lookup"><span data-stu-id="c90b8-115">A sort clause in the request will return a Bad Request error code in the response.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c90b8-116">后续步骤</span><span class="sxs-lookup"><span data-stu-id="c90b8-116">Next steps</span></span>

- [<span data-ttu-id="c90b8-117">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="c90b8-117">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview)
