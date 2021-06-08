---
title: 替换 timeCard
description: 更新现有 timeCard 条目。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 095c5fcdda15496ab41570aa940ad09585f9a633
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787847"
---
# <a name="replace-timecard"></a><span data-ttu-id="786f7-103">替换 timeCard</span><span class="sxs-lookup"><span data-stu-id="786f7-103">Replace timeCard</span></span>

<span data-ttu-id="786f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="786f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="786f7-105">将现有的 [timeCard 替换为](../resources/timecard.md) 更新的值。</span><span class="sxs-lookup"><span data-stu-id="786f7-105">Replace an existing [timeCard](../resources/timecard.md) with updated values.</span></span>

## <a name="permissions"></a><span data-ttu-id="786f7-106">权限</span><span class="sxs-lookup"><span data-stu-id="786f7-106">Permissions</span></span>

<span data-ttu-id="786f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="786f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="786f7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="786f7-109">Permission type</span></span>      | <span data-ttu-id="786f7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="786f7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="786f7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="786f7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="786f7-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="786f7-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="786f7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="786f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="786f7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="786f7-114">Not supported.</span></span>    |
|<span data-ttu-id="786f7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="786f7-115">Application</span></span> | <span data-ttu-id="786f7-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="786f7-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="786f7-117">\***重要提示：** 使用应用程序权限时，必须在请求 `MS-APP-ACTS-AS` 中包括 标头。</span><span class="sxs-lookup"><span data-stu-id="786f7-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="786f7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="786f7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timecards/{timeCardID}
```

## <a name="request-headers"></a><span data-ttu-id="786f7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="786f7-119">Request headers</span></span>

| <span data-ttu-id="786f7-120">标头</span><span class="sxs-lookup"><span data-stu-id="786f7-120">Header</span></span>       | <span data-ttu-id="786f7-121">值</span><span class="sxs-lookup"><span data-stu-id="786f7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="786f7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="786f7-122">Authorization</span></span>  | <span data-ttu-id="786f7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="786f7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="786f7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="786f7-125">Content-Type</span></span>  | <span data-ttu-id="786f7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="786f7-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="786f7-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="786f7-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="786f7-129">应用代表其操作的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="786f7-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="786f7-130">使用应用程序权限范围时是必需的。</span><span class="sxs-lookup"><span data-stu-id="786f7-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="786f7-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="786f7-131">Request body</span></span>

<span data-ttu-id="786f7-132">在请求正文中，提供 [timeCard](../resources/timecard.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="786f7-132">In the request body, supply a JSON representation of a [timeCard](../resources/timecard.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="786f7-133">响应</span><span class="sxs-lookup"><span data-stu-id="786f7-133">Response</span></span>

<span data-ttu-id="786f7-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="786f7-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="786f7-135">示例</span><span class="sxs-lookup"><span data-stu-id="786f7-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="786f7-136">请求</span><span class="sxs-lookup"><span data-stu-id="786f7-136">Request</span></span>

<span data-ttu-id="786f7-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="786f7-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timecard_replace"
}-->

```http
PUT https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_3cd7413f-0337-433b-9a49-da0923185b3f
Content-type: application/json

{
    "userId": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    "state": "clockedOut",
    "confirmedBy": "None",
    "notes": null,
    "clockInEvent": {
        "dateTime": "2021-05-21T21:58:41.327Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "update sample notes"
        }
    },
    "clockOutEvent": {
        "dateTime": "2021-05-21T22:01:46.205Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "update sample notes"
        }
    },
    "breaks": [
        {
            "breakId": "BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f",
            "notes": null,
            "start": {
                "dateTime": "2021-05-21T21:59:59.328Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "update sample notes"
                }
            },
            "end": {
                "dateTime": "2021-05-21T22:01:10.205Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "update sample notes"
                }
            }
        }
    ]
}
```

### <a name="response"></a><span data-ttu-id="786f7-138">响应</span><span class="sxs-lookup"><span data-stu-id="786f7-138">Response</span></span>

<span data-ttu-id="786f7-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="786f7-139">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "timecard_replace"
} -->

```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
