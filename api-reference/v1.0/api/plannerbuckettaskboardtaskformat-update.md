---
title: 更新 plannerBucketTaskBoardTaskFormat
description: 更新 **plannerBucketTaskBoardTaskFormat** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: f204de1d662b898b69d8ae0b5d5ba344c5e13212
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055846"
---
# <a name="update-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="618eb-103">更新 plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="618eb-103">Update plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="618eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="618eb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="618eb-105">更新 **plannerBucketTaskBoardTaskFormat** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="618eb-105">Update the properties of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="618eb-106">权限</span><span class="sxs-lookup"><span data-stu-id="618eb-106">Permissions</span></span>
<span data-ttu-id="618eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="618eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="618eb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="618eb-109">Permission type</span></span>      | <span data-ttu-id="618eb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="618eb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="618eb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="618eb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="618eb-112">Tasks.ReadWrite，Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="618eb-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="618eb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="618eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="618eb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="618eb-114">Not supported.</span></span>    |
|<span data-ttu-id="618eb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="618eb-115">Application</span></span> | <span data-ttu-id="618eb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="618eb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="618eb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="618eb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/bucketTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="618eb-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="618eb-118">Optional request headers</span></span>
| <span data-ttu-id="618eb-119">名称</span><span class="sxs-lookup"><span data-stu-id="618eb-119">Name</span></span>       | <span data-ttu-id="618eb-120">说明</span><span class="sxs-lookup"><span data-stu-id="618eb-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="618eb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="618eb-121">Authorization</span></span>  | <span data-ttu-id="618eb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="618eb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="618eb-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="618eb-124">If-Match</span></span>  | <span data-ttu-id="618eb-p103">要更新的 **plannerBucketTaskBoardTaskFormat** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="618eb-p103">Last known ETag value for the **plannerBucketTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="618eb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="618eb-127">Request body</span></span>
<span data-ttu-id="618eb-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="618eb-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="618eb-131">属性</span><span class="sxs-lookup"><span data-stu-id="618eb-131">Property</span></span>     | <span data-ttu-id="618eb-132">类型</span><span class="sxs-lookup"><span data-stu-id="618eb-132">Type</span></span>   |<span data-ttu-id="618eb-133">说明</span><span class="sxs-lookup"><span data-stu-id="618eb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="618eb-134">orderHint</span><span class="sxs-lookup"><span data-stu-id="618eb-134">orderHint</span></span>|<span data-ttu-id="618eb-135">String</span><span class="sxs-lookup"><span data-stu-id="618eb-135">String</span></span>|<span data-ttu-id="618eb-p105">用于为任务板存储桶视图中的任务进行排序的提示。[此处](../resources/planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="618eb-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="618eb-138">响应</span><span class="sxs-lookup"><span data-stu-id="618eb-138">Response</span></span>

<span data-ttu-id="618eb-139">如果成功，此方法将返回 `204 No Content` 响应和空内容。</span><span class="sxs-lookup"><span data-stu-id="618eb-139">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="618eb-140">如果请求指定具有首选项的标头，则此方法在响应正文中返回 响应代码和更新的 `Prefer` `return=representation` `200 OK` [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="618eb-140">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="618eb-p107">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="618eb-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="618eb-144">示例</span><span class="sxs-lookup"><span data-stu-id="618eb-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="618eb-145">请求</span><span class="sxs-lookup"><span data-stu-id="618eb-145">Request</span></span>
<span data-ttu-id="618eb-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="618eb-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="618eb-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="618eb-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerbuckettaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/bucketTaskBoardFormat
Content-type: application/json
Content-length: 34
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
# <a name="c"></a>[<span data-ttu-id="618eb-148">C#</span><span class="sxs-lookup"><span data-stu-id="618eb-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerbuckettaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="618eb-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="618eb-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerbuckettaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="618eb-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="618eb-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerbuckettaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="618eb-151">Java</span><span class="sxs-lookup"><span data-stu-id="618eb-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerbuckettaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="618eb-152">响应</span><span class="sxs-lookup"><span data-stu-id="618eb-152">Response</span></span>
<span data-ttu-id="618eb-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="618eb-153">Here is an example of the response.</span></span> <span data-ttu-id="618eb-154">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="618eb-154">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 68

{
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "orderHint": "C3665D"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerbuckettaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

