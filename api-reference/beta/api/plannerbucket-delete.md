---
title: 删除 plannerBucket
description: 删除 **plannerBucket**。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 286514d878be65638b267369ff70073c8c736b77
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876595"
---
# <a name="delete-plannerbucket"></a><span data-ttu-id="aed6d-103">删除 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="aed6d-103">Delete plannerBucket</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aed6d-104">删除 **plannerBucket**。</span><span class="sxs-lookup"><span data-stu-id="aed6d-104">Delete **plannerBucket**.</span></span>
## <a name="permissions"></a><span data-ttu-id="aed6d-105">权限</span><span class="sxs-lookup"><span data-stu-id="aed6d-105">Permissions</span></span>
<span data-ttu-id="aed6d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aed6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aed6d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="aed6d-108">Permission type</span></span>      | <span data-ttu-id="aed6d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aed6d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aed6d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aed6d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aed6d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aed6d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="aed6d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aed6d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aed6d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="aed6d-113">Not supported.</span></span>    |
|<span data-ttu-id="aed6d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="aed6d-114">Application</span></span> | <span data-ttu-id="aed6d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="aed6d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aed6d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aed6d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/buckets/<id>
```
## <a name="request-headers"></a><span data-ttu-id="aed6d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="aed6d-117">Request headers</span></span>
| <span data-ttu-id="aed6d-118">名称</span><span class="sxs-lookup"><span data-stu-id="aed6d-118">Name</span></span>       | <span data-ttu-id="aed6d-119">说明</span><span class="sxs-lookup"><span data-stu-id="aed6d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aed6d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="aed6d-120">Authorization</span></span>  | <span data-ttu-id="aed6d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aed6d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aed6d-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="aed6d-123">If-Match</span></span>  | <span data-ttu-id="aed6d-p103">要删除的 **plannerBucket** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="aed6d-p103">Last known ETag value for the **plannerBucket** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aed6d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aed6d-126">Request body</span></span>
<span data-ttu-id="aed6d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aed6d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aed6d-128">响应</span><span class="sxs-lookup"><span data-stu-id="aed6d-128">Response</span></span>

<span data-ttu-id="aed6d-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="aed6d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="aed6d-p105">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="aed6d-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="aed6d-134">示例</span><span class="sxs-lookup"><span data-stu-id="aed6d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aed6d-135">请求</span><span class="sxs-lookup"><span data-stu-id="aed6d-135">Request</span></span>
<span data-ttu-id="aed6d-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aed6d-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="aed6d-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="aed6d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_plannerbucket"
}-->
```http
DELETE https://graph.microsoft.com/beta/planner/buckets/<id>
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aed6d-138">C#</span><span class="sxs-lookup"><span data-stu-id="aed6d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-plannerbucket-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aed6d-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="aed6d-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-plannerbucket-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aed6d-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="aed6d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-plannerbucket-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="aed6d-141">Java</span><span class="sxs-lookup"><span data-stu-id="aed6d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-plannerbucket-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="aed6d-142">响应</span><span class="sxs-lookup"><span data-stu-id="aed6d-142">Response</span></span>
<span data-ttu-id="aed6d-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aed6d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
