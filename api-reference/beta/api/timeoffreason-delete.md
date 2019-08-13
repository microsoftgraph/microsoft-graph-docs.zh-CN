---
title: 删除 timeOffReason
description: 通过设置 isActive 属性将 timeOffReason 标记为非活动状态
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1c09b46927f5779f7c3ed6b456a5bb783a5eec7c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362620"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="6305f-103">删除 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="6305f-103">Delete timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6305f-104">通过设置**isActive**属性将[timeOffReason](../resources/timeoffreason.md)标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="6305f-104">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span>

<span data-ttu-id="6305f-105">此方法不会删除指定的[timeOffReason](../resources/timeoffreason.md)实例。</span><span class="sxs-lookup"><span data-stu-id="6305f-105">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="6305f-106">已分配此原因的[timeOffItem](../resources/timeoffitem.md)实例仍将被分配给此原因。</span><span class="sxs-lookup"><span data-stu-id="6305f-106">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="6305f-107">权限</span><span class="sxs-lookup"><span data-stu-id="6305f-107">Permissions</span></span>

<span data-ttu-id="6305f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6305f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6305f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6305f-110">Permission type</span></span>      | <span data-ttu-id="6305f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6305f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6305f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6305f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6305f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6305f-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6305f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6305f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6305f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6305f-115">Not supported.</span></span>    |
|<span data-ttu-id="6305f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6305f-116">Application</span></span> | <span data-ttu-id="6305f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6305f-117">Not supported.</span></span> |

> <span data-ttu-id="6305f-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="6305f-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6305f-119">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="6305f-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6305f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6305f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="6305f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6305f-121">Request headers</span></span>

| <span data-ttu-id="6305f-122">标头</span><span class="sxs-lookup"><span data-stu-id="6305f-122">Header</span></span>       | <span data-ttu-id="6305f-123">值</span><span class="sxs-lookup"><span data-stu-id="6305f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6305f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6305f-124">Authorization</span></span>  | <span data-ttu-id="6305f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6305f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6305f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6305f-127">Content-Type</span></span>  | <span data-ttu-id="6305f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6305f-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6305f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6305f-129">Request body</span></span>
<span data-ttu-id="6305f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6305f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6305f-131">响应</span><span class="sxs-lookup"><span data-stu-id="6305f-131">Response</span></span>

<span data-ttu-id="6305f-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6305f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6305f-134">示例</span><span class="sxs-lookup"><span data-stu-id="6305f-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6305f-135">请求</span><span class="sxs-lookup"><span data-stu-id="6305f-135">Request</span></span>

<span data-ttu-id="6305f-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6305f-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6305f-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6305f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6305f-138">C#</span><span class="sxs-lookup"><span data-stu-id="6305f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6305f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6305f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6305f-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="6305f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6305f-141">Java</span><span class="sxs-lookup"><span data-stu-id="6305f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffreason-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6305f-142">响应</span><span class="sxs-lookup"><span data-stu-id="6305f-142">Response</span></span>

<span data-ttu-id="6305f-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6305f-143">The following is an example of the response.</span></span> 

><span data-ttu-id="6305f-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6305f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
