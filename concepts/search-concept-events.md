---
title: 搜索日历事件
description: 您可以在用户自己的日历中进行搜索。
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 1b749c0b45b8250d011589e20b05a3d715b40bcb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939556"
---
# <a name="search-calendar-events"></a><span data-ttu-id="cd743-103">搜索日历事件</span><span class="sxs-lookup"><span data-stu-id="cd743-103">Search calendar events</span></span>

<span data-ttu-id="cd743-104">您的应用程序可以在用户自己的主日历中。</span><span class="sxs-lookup"><span data-stu-id="cd743-104">You app can in a user’s own primary calendar.</span></span> <span data-ttu-id="cd743-105">用于搜索的用户标识基于授权令牌。</span><span class="sxs-lookup"><span data-stu-id="cd743-105">The user identity used to search is based on the Authorization Token.</span></span>

## <a name="example"></a><span data-ttu-id="cd743-106">示例</span><span class="sxs-lookup"><span data-stu-id="cd743-106">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd743-107">请求</span><span class="sxs-lookup"><span data-stu-id="cd743-107">Request</span></span>

<span data-ttu-id="cd743-108">本示例将在用户的日历中搜索关键字 "contoso"，并检索最大25个结果。</span><span class="sxs-lookup"><span data-stu-id="cd743-108">This example searches in the user's calendar for the keyword "contoso", and will retrieve up to 25 results.</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
       "entityTypes": ["microsoft.graph.event"],
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

## <a name="known-limitations"></a><span data-ttu-id="cd743-109">已知限制</span><span class="sxs-lookup"><span data-stu-id="cd743-109">Known limitations</span></span>

<span data-ttu-id="cd743-110">您只能访问用户自己的日历。</span><span class="sxs-lookup"><span data-stu-id="cd743-110">You can only access user’s own calendar.</span></span> <span data-ttu-id="cd743-111">共享日历，不支持委派访问权限。</span><span class="sxs-lookup"><span data-stu-id="cd743-111">Shared Calendar, delegated access is not supported.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cd743-112">后续步骤</span><span class="sxs-lookup"><span data-stu-id="cd743-112">Next steps</span></span>

<span data-ttu-id="cd743-113">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="cd743-113">Find out more about:</span></span>

- [<span data-ttu-id="cd743-114">使用搜索 API</span><span class="sxs-lookup"><span data-stu-id="cd743-114">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)