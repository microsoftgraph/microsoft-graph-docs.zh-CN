---
title: 删除 timeOffReason
description: 通过设置 isActive 属性将 timeOffReason 标记为非活动状态。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1e71e976167b94d144037d93bf9bb3dff59cc5b7
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44154421"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="931aa-103">删除 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="931aa-103">Delete timeOffReason</span></span>

<span data-ttu-id="931aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="931aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="931aa-105">通过设置**isActive**属性将[timeOffReason](../resources/timeoffreason.md)标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="931aa-105">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span> <span data-ttu-id="931aa-106">每个团队必须至少包含一个**timeOffReason**。</span><span class="sxs-lookup"><span data-stu-id="931aa-106">Every team must include at least one **timeOffReason**.</span></span>

<span data-ttu-id="931aa-107">此方法不会删除指定的**timeOffReason**实例。</span><span class="sxs-lookup"><span data-stu-id="931aa-107">This method does not remove the specified **timeOffReason** instance.</span></span> <span data-ttu-id="931aa-108">已分配此原因的[timeOffItem](../resources/timeoffitem.md)实例仍将被分配给此原因。</span><span class="sxs-lookup"><span data-stu-id="931aa-108">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="931aa-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="931aa-109">Permissions</span></span>

<span data-ttu-id="931aa-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="931aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="931aa-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="931aa-112">Permission type</span></span>      | <span data-ttu-id="931aa-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="931aa-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="931aa-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="931aa-114">Delegated (work or school account)</span></span> | <span data-ttu-id="931aa-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="931aa-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="931aa-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="931aa-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="931aa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="931aa-117">Not supported.</span></span>    |
|<span data-ttu-id="931aa-118">Application</span><span class="sxs-lookup"><span data-stu-id="931aa-118">Application</span></span> | <span data-ttu-id="931aa-119">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="931aa-119">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="931aa-120">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="931aa-120">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="931aa-121">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="931aa-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="931aa-122">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="931aa-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="931aa-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="931aa-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="931aa-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="931aa-124">Request headers</span></span>

| <span data-ttu-id="931aa-125">标头</span><span class="sxs-lookup"><span data-stu-id="931aa-125">Header</span></span>       | <span data-ttu-id="931aa-126">值</span><span class="sxs-lookup"><span data-stu-id="931aa-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="931aa-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="931aa-127">Authorization</span></span>  | <span data-ttu-id="931aa-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="931aa-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="931aa-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="931aa-130">Request body</span></span>
<span data-ttu-id="931aa-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="931aa-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="931aa-132">响应</span><span class="sxs-lookup"><span data-stu-id="931aa-132">Response</span></span>

<span data-ttu-id="931aa-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="931aa-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="931aa-135">示例</span><span class="sxs-lookup"><span data-stu-id="931aa-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="931aa-136">请求</span><span class="sxs-lookup"><span data-stu-id="931aa-136">Request</span></span>

<span data-ttu-id="931aa-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="931aa-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="931aa-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="931aa-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="931aa-139">C#</span><span class="sxs-lookup"><span data-stu-id="931aa-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="931aa-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="931aa-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="931aa-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="931aa-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="931aa-142">响应</span><span class="sxs-lookup"><span data-stu-id="931aa-142">Response</span></span>

<span data-ttu-id="931aa-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="931aa-143">The following is an example of the response.</span></span> 

><span data-ttu-id="931aa-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="931aa-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
