---
title: 删除 timeOffReason
description: 通过设置 isActive 属性将 timeOffReason 标记为非活动状态
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 45df0c9644e9845b9d86c591fb6871af455502ee
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270532"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="47680-103">删除 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="47680-103">Delete timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47680-104">通过设置**isActive**属性将[timeOffReason](../resources/timeoffreason.md)标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="47680-104">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span>

<span data-ttu-id="47680-105">此方法不会删除指定的[timeOffReason](../resources/timeoffreason.md)实例。</span><span class="sxs-lookup"><span data-stu-id="47680-105">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="47680-106">已分配此原因的[timeOffItem](../resources/timeoffitem.md)实例仍将被分配给此原因。</span><span class="sxs-lookup"><span data-stu-id="47680-106">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="47680-107">权限</span><span class="sxs-lookup"><span data-stu-id="47680-107">Permissions</span></span>

<span data-ttu-id="47680-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47680-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47680-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="47680-110">Permission type</span></span>      | <span data-ttu-id="47680-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47680-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47680-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47680-112">Delegated (work or school account)</span></span> | <span data-ttu-id="47680-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47680-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="47680-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47680-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47680-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="47680-115">Not supported.</span></span>    |
|<span data-ttu-id="47680-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="47680-116">Application</span></span> | <span data-ttu-id="47680-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="47680-117">Not supported.</span></span> |

> <span data-ttu-id="47680-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="47680-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="47680-119">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="47680-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="47680-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47680-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="47680-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="47680-121">Request headers</span></span>

| <span data-ttu-id="47680-122">标头</span><span class="sxs-lookup"><span data-stu-id="47680-122">Header</span></span>       | <span data-ttu-id="47680-123">值</span><span class="sxs-lookup"><span data-stu-id="47680-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47680-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="47680-124">Authorization</span></span>  | <span data-ttu-id="47680-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="47680-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="47680-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47680-127">Content-Type</span></span>  | <span data-ttu-id="47680-128">application/json</span><span class="sxs-lookup"><span data-stu-id="47680-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47680-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="47680-129">Request body</span></span>
<span data-ttu-id="47680-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="47680-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47680-131">响应</span><span class="sxs-lookup"><span data-stu-id="47680-131">Response</span></span>

<span data-ttu-id="47680-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="47680-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47680-134">示例</span><span class="sxs-lookup"><span data-stu-id="47680-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="47680-135">请求</span><span class="sxs-lookup"><span data-stu-id="47680-135">Request</span></span>

<span data-ttu-id="47680-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="47680-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

#### <a name="response"></a><span data-ttu-id="47680-137">响应</span><span class="sxs-lookup"><span data-stu-id="47680-137">Response</span></span>

<span data-ttu-id="47680-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="47680-138">The following is an example of the response.</span></span> 

><span data-ttu-id="47680-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="47680-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="47680-141">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="47680-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="47680-142">C#</span><span class="sxs-lookup"><span data-stu-id="47680-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/timeoffreason-delete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="47680-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="47680-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/timeoffreason-delete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="47680-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="47680-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/timeoffreason-delete-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Marks a timeOffReason as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoffreason-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/timeoffreason-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/timeoffreason-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
