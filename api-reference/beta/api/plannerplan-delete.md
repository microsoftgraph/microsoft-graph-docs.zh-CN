---
title: 删除 plannerPlan
description: 删除 **plannerPlan**。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 82d9ccfa20dd5852280e0d4b579c6dc4c71fec9d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361714"
---
# <a name="delete-plannerplan"></a><span data-ttu-id="3f387-103">删除 plannerPlan</span><span class="sxs-lookup"><span data-stu-id="3f387-103">Delete plannerPlan</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f387-104">删除 **plannerPlan**。</span><span class="sxs-lookup"><span data-stu-id="3f387-104">Delete **plannerPlan**.</span></span>
## <a name="permissions"></a><span data-ttu-id="3f387-105">权限</span><span class="sxs-lookup"><span data-stu-id="3f387-105">Permissions</span></span>
<span data-ttu-id="3f387-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f387-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f387-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f387-108">Permission type</span></span>      | <span data-ttu-id="3f387-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f387-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f387-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f387-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3f387-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f387-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3f387-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f387-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f387-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f387-113">Not supported.</span></span>    |
|<span data-ttu-id="3f387-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f387-114">Application</span></span> | <span data-ttu-id="3f387-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f387-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f387-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f387-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/plans/<id>

```
## <a name="request-headers"></a><span data-ttu-id="3f387-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f387-117">Request headers</span></span>
| <span data-ttu-id="3f387-118">名称</span><span class="sxs-lookup"><span data-stu-id="3f387-118">Name</span></span>       | <span data-ttu-id="3f387-119">说明</span><span class="sxs-lookup"><span data-stu-id="3f387-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3f387-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f387-120">Authorization</span></span>  | <span data-ttu-id="3f387-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3f387-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3f387-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="3f387-123">If-Match</span></span>  | <span data-ttu-id="3f387-p103">要删除的 **plannerPlan** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="3f387-p103">Last known ETag value for the **plannerPlan** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f387-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f387-126">Request body</span></span>
<span data-ttu-id="3f387-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3f387-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f387-128">响应</span><span class="sxs-lookup"><span data-stu-id="3f387-128">Response</span></span>

<span data-ttu-id="3f387-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3f387-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="3f387-p105">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="3f387-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="3f387-134">示例</span><span class="sxs-lookup"><span data-stu-id="3f387-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f387-135">请求</span><span class="sxs-lookup"><span data-stu-id="3f387-135">Request</span></span>
<span data-ttu-id="3f387-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f387-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3f387-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3f387-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_plannerplan"
}-->
```http
DELETE https://graph.microsoft.com/beta/planner/plans/<id>
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3f387-138">C#</span><span class="sxs-lookup"><span data-stu-id="3f387-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f387-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f387-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3f387-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="3f387-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3f387-141">Java</span><span class="sxs-lookup"><span data-stu-id="3f387-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3f387-142">响应</span><span class="sxs-lookup"><span data-stu-id="3f387-142">Response</span></span>
<span data-ttu-id="3f387-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3f387-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
