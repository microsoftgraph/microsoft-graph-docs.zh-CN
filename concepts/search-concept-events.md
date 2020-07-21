---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索日历事件
description: 您可以在用户自己的日历中进行搜索。
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 8cafb01337581d1b1d2e355363aec14f658ee4f6
ms.sourcegitcommit: 79267b6d78c3510ef609953c5a664e692794caaa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/21/2020
ms.locfileid: "45196825"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-calendar-events"></a><span data-ttu-id="61632-103">在 Microsoft Graph 中使用 Microsoft Search API 搜索日历事件</span><span class="sxs-lookup"><span data-stu-id="61632-103">Use the Microsoft Search API in Microsoft Graph to search calendar events</span></span>

<span data-ttu-id="61632-104">您可以使用 Microsoft 搜索 API 在用户的主日历中搜索事件。</span><span class="sxs-lookup"><span data-stu-id="61632-104">You can use the Microsoft Search API to search for events in a user’s primary calendar.</span></span> <span data-ttu-id="61632-105">搜索的用户标识基于身份验证令牌。</span><span class="sxs-lookup"><span data-stu-id="61632-105">The user identity for the search is based on the auth token.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="example"></a><span data-ttu-id="61632-106">示例</span><span class="sxs-lookup"><span data-stu-id="61632-106">Example</span></span>

### <a name="request"></a><span data-ttu-id="61632-107">请求</span><span class="sxs-lookup"><span data-stu-id="61632-107">Request</span></span>

<span data-ttu-id="61632-108">本示例将在用户的日历中搜索关键字 "contoso"，并返回最大25个结果。</span><span class="sxs-lookup"><span data-stu-id="61632-108">This example searches in the user's calendar for the keyword "contoso", and will return up to 25 results.</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "event"
      ],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

## <a name="known-limitations"></a><span data-ttu-id="61632-109">已知限制</span><span class="sxs-lookup"><span data-stu-id="61632-109">Known limitations</span></span>

<span data-ttu-id="61632-110">您只能访问用户自己的日历。</span><span class="sxs-lookup"><span data-stu-id="61632-110">You can only access user’s own calendar.</span></span> <span data-ttu-id="61632-111">不支持共享日历和委派访问方案。</span><span class="sxs-lookup"><span data-stu-id="61632-111">Shared calendar and delegated access scenarios are not supported.</span></span>

## <a name="next-steps"></a><span data-ttu-id="61632-112">后续步骤</span><span class="sxs-lookup"><span data-stu-id="61632-112">Next steps</span></span>

- [<span data-ttu-id="61632-113">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="61632-113">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
