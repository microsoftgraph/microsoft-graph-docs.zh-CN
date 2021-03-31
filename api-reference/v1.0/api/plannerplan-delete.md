---
title: 删除 plannerPlan
description: 删除 **plannerPlan**。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 50a6eb577ac895ab33abf7d3cf1d9d1930eeb379
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473141"
---
# <a name="delete-plannerplan"></a><span data-ttu-id="b6ca2-103">删除 plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b6ca2-103">Delete plannerPlan</span></span>

<span data-ttu-id="b6ca2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6ca2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6ca2-105">删除 **plannerPlan**。</span><span class="sxs-lookup"><span data-stu-id="b6ca2-105">Delete **plannerPlan**.</span></span>
## <a name="permissions"></a><span data-ttu-id="b6ca2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b6ca2-106">Permissions</span></span>
<span data-ttu-id="b6ca2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6ca2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6ca2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6ca2-109">Permission type</span></span>      | <span data-ttu-id="b6ca2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b6ca2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6ca2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6ca2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b6ca2-112">Tasks.ReadWrite、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6ca2-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b6ca2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6ca2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6ca2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6ca2-114">Not supported.</span></span>    |
|<span data-ttu-id="b6ca2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6ca2-115">Application</span></span> | <span data-ttu-id="b6ca2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6ca2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6ca2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6ca2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/plans/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b6ca2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6ca2-118">Request headers</span></span>
| <span data-ttu-id="b6ca2-119">名称</span><span class="sxs-lookup"><span data-stu-id="b6ca2-119">Name</span></span>       | <span data-ttu-id="b6ca2-120">说明</span><span class="sxs-lookup"><span data-stu-id="b6ca2-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b6ca2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6ca2-121">Authorization</span></span>  | <span data-ttu-id="b6ca2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b6ca2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b6ca2-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="b6ca2-124">If-Match</span></span>  | <span data-ttu-id="b6ca2-p103">要删除的 **plannerPlan** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="b6ca2-p103">Last known ETag value for the **plannerPlan** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6ca2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6ca2-127">Request body</span></span>
<span data-ttu-id="b6ca2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b6ca2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6ca2-129">响应</span><span class="sxs-lookup"><span data-stu-id="b6ca2-129">Response</span></span>

<span data-ttu-id="b6ca2-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b6ca2-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="b6ca2-p105">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="b6ca2-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="b6ca2-135">示例</span><span class="sxs-lookup"><span data-stu-id="b6ca2-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6ca2-136">请求</span><span class="sxs-lookup"><span data-stu-id="b6ca2-136">Request</span></span>
<span data-ttu-id="b6ca2-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b6ca2-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b6ca2-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6ca2-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_plannerplan"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/plans/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
# <a name="c"></a>[<span data-ttu-id="b6ca2-139">C#</span><span class="sxs-lookup"><span data-stu-id="b6ca2-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6ca2-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6ca2-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6ca2-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6ca2-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6ca2-142">Java</span><span class="sxs-lookup"><span data-stu-id="b6ca2-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b6ca2-143">响应</span><span class="sxs-lookup"><span data-stu-id="b6ca2-143">Response</span></span>
<span data-ttu-id="b6ca2-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b6ca2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

