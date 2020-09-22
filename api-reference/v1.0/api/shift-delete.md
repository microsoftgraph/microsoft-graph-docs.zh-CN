---
title: 删除班次
description: 从计划中删除班次轮换。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e68d6727c61c36a8e7a8471f36713c1768106f1e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013004"
---
# <a name="delete-shift"></a><span data-ttu-id="cf617-103">删除班次</span><span class="sxs-lookup"><span data-stu-id="cf617-103">Delete shift</span></span>

<span data-ttu-id="cf617-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf617-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cf617-105">从计划中删除 [班次轮换](../resources/shift.md) 。</span><span class="sxs-lookup"><span data-stu-id="cf617-105">Delete a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf617-106">权限</span><span class="sxs-lookup"><span data-stu-id="cf617-106">Permissions</span></span>

<span data-ttu-id="cf617-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf617-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf617-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf617-109">Permission type</span></span>      | <span data-ttu-id="cf617-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf617-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf617-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf617-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cf617-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="cf617-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf617-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf617-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf617-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf617-114">Not supported.</span></span>    |
|<span data-ttu-id="cf617-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf617-115">Application</span></span> | <span data-ttu-id="cf617-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="cf617-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="cf617-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="cf617-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cf617-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="cf617-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cf617-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf617-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="cf617-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf617-120">Request headers</span></span>

| <span data-ttu-id="cf617-121">标头</span><span class="sxs-lookup"><span data-stu-id="cf617-121">Header</span></span>       | <span data-ttu-id="cf617-122">值</span><span class="sxs-lookup"><span data-stu-id="cf617-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cf617-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf617-123">Authorization</span></span>  | <span data-ttu-id="cf617-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf617-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf617-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf617-126">Request body</span></span>
<span data-ttu-id="cf617-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf617-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf617-128">响应</span><span class="sxs-lookup"><span data-stu-id="cf617-128">Response</span></span>

<span data-ttu-id="cf617-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cf617-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf617-131">示例</span><span class="sxs-lookup"><span data-stu-id="cf617-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cf617-132">请求</span><span class="sxs-lookup"><span data-stu-id="cf617-132">Request</span></span>

<span data-ttu-id="cf617-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cf617-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cf617-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf617-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="cf617-135">C#</span><span class="sxs-lookup"><span data-stu-id="cf617-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf617-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf617-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf617-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf617-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf617-138">Java</span><span class="sxs-lookup"><span data-stu-id="cf617-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a><span data-ttu-id="cf617-139">响应</span><span class="sxs-lookup"><span data-stu-id="cf617-139">Response</span></span>

<span data-ttu-id="cf617-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cf617-140">The following is an example of the response.</span></span> 

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
  "description": "Deletes a shift from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

