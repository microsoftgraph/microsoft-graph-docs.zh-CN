---
title: 删除 timeOffReason
description: 通过设置 isActive 属性将 timeOffReason 标记为非活动状态。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4a53a677187373105e6a6b1cd3b884c6aa5e928e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787427"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="63967-103">删除 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="63967-103">Delete timeOffReason</span></span>

<span data-ttu-id="63967-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63967-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63967-105">通过设置 **isActive** 属性将 [timeOffReason](../resources/timeoffreason.md)标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="63967-105">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span> <span data-ttu-id="63967-106">每个团队必须至少包括一个请到时间原因。</span><span class="sxs-lookup"><span data-stu-id="63967-106">Every team must include at least one timeoff reason.</span></span>

<span data-ttu-id="63967-107">此方法不会删除指定的 [timeOffReason](../resources/timeoffreason.md) 实例。</span><span class="sxs-lookup"><span data-stu-id="63967-107">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="63967-108">已分配此原因的[timeOffItem](../resources/timeoffitem.md)实例仍分配给此原因。</span><span class="sxs-lookup"><span data-stu-id="63967-108">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="63967-109">权限</span><span class="sxs-lookup"><span data-stu-id="63967-109">Permissions</span></span>

<span data-ttu-id="63967-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63967-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63967-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="63967-112">Permission type</span></span>      | <span data-ttu-id="63967-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63967-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63967-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63967-114">Delegated (work or school account)</span></span> | <span data-ttu-id="63967-115">Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63967-115">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="63967-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63967-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63967-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="63967-117">Not supported.</span></span>    |
|<span data-ttu-id="63967-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="63967-118">Application</span></span> | <span data-ttu-id="63967-119">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63967-119">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="63967-120">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="63967-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="63967-121">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="63967-121">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="63967-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63967-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="63967-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="63967-123">Request headers</span></span>

| <span data-ttu-id="63967-124">标头</span><span class="sxs-lookup"><span data-stu-id="63967-124">Header</span></span>       | <span data-ttu-id="63967-125">值</span><span class="sxs-lookup"><span data-stu-id="63967-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="63967-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="63967-126">Authorization</span></span>  | <span data-ttu-id="63967-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63967-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63967-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="63967-129">Request body</span></span>
<span data-ttu-id="63967-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63967-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63967-131">响应</span><span class="sxs-lookup"><span data-stu-id="63967-131">Response</span></span>

<span data-ttu-id="63967-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="63967-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63967-134">示例</span><span class="sxs-lookup"><span data-stu-id="63967-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="63967-135">请求</span><span class="sxs-lookup"><span data-stu-id="63967-135">Request</span></span>

<span data-ttu-id="63967-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="63967-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="63967-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="63967-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="63967-138">C#</span><span class="sxs-lookup"><span data-stu-id="63967-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63967-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63967-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63967-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63967-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63967-141">Java</span><span class="sxs-lookup"><span data-stu-id="63967-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffreason-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="63967-142">响应</span><span class="sxs-lookup"><span data-stu-id="63967-142">Response</span></span>

<span data-ttu-id="63967-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63967-143">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
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

