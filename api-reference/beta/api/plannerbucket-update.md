---
title: 更新 plannerbucket
description: 更新 **plannerbucket** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: ccc7b6054c309919a0181ea0dd40a764ae7ded69
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978360"
---
# <a name="update-plannerbucket"></a><span data-ttu-id="340c4-103">更新 plannerbucket</span><span class="sxs-lookup"><span data-stu-id="340c4-103">Update plannerbucket</span></span>

<span data-ttu-id="340c4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="340c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="340c4-105">更新 **plannerbucket** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="340c4-105">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="340c4-106">权限</span><span class="sxs-lookup"><span data-stu-id="340c4-106">Permissions</span></span>
<span data-ttu-id="340c4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="340c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="340c4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="340c4-109">Permission type</span></span>      | <span data-ttu-id="340c4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="340c4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="340c4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="340c4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="340c4-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="340c4-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="340c4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="340c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="340c4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="340c4-114">Not supported.</span></span>    |
|<span data-ttu-id="340c4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="340c4-115">Application</span></span> | <span data-ttu-id="340c4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="340c4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="340c4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="340c4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="340c4-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="340c4-118">Optional request headers</span></span>
| <span data-ttu-id="340c4-119">名称</span><span class="sxs-lookup"><span data-stu-id="340c4-119">Name</span></span>       | <span data-ttu-id="340c4-120">说明</span><span class="sxs-lookup"><span data-stu-id="340c4-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="340c4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="340c4-121">Authorization</span></span>  | <span data-ttu-id="340c4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="340c4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="340c4-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="340c4-124">If-Match</span></span>  | <span data-ttu-id="340c4-p103">要更新的 **plannerBucket** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="340c4-p103">Last known ETag value for the **plannerBucket** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="340c4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="340c4-127">Request body</span></span>
<span data-ttu-id="340c4-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="340c4-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="340c4-131">属性</span><span class="sxs-lookup"><span data-stu-id="340c4-131">Property</span></span>     | <span data-ttu-id="340c4-132">类型</span><span class="sxs-lookup"><span data-stu-id="340c4-132">Type</span></span>   |<span data-ttu-id="340c4-133">说明</span><span class="sxs-lookup"><span data-stu-id="340c4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="340c4-134">name</span><span class="sxs-lookup"><span data-stu-id="340c4-134">name</span></span>|<span data-ttu-id="340c4-135">String</span><span class="sxs-lookup"><span data-stu-id="340c4-135">String</span></span>|<span data-ttu-id="340c4-136">存储桶的名称。</span><span class="sxs-lookup"><span data-stu-id="340c4-136">Name of the bucket.</span></span>|
|<span data-ttu-id="340c4-137">orderHint</span><span class="sxs-lookup"><span data-stu-id="340c4-137">orderHint</span></span>|<span data-ttu-id="340c4-138">String</span><span class="sxs-lookup"><span data-stu-id="340c4-138">String</span></span>|<span data-ttu-id="340c4-p105">用于为列表视图中的此类型项目排序的提示。此格式在[使用规划器中的排序提示](../resources/planner-order-hint-format.md)定义中。</span><span class="sxs-lookup"><span data-stu-id="340c4-p105">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="340c4-141">planId</span><span class="sxs-lookup"><span data-stu-id="340c4-141">planId</span></span>|<span data-ttu-id="340c4-142">String</span><span class="sxs-lookup"><span data-stu-id="340c4-142">String</span></span>|<span data-ttu-id="340c4-143">此存储桶所属的计划 id。</span><span class="sxs-lookup"><span data-stu-id="340c4-143">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="340c4-144">响应</span><span class="sxs-lookup"><span data-stu-id="340c4-144">Response</span></span>

<span data-ttu-id="340c4-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerBucket](../resources/plannerbucket.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="340c4-145">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="340c4-p106">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="340c4-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="340c4-149">示例</span><span class="sxs-lookup"><span data-stu-id="340c4-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="340c4-150">请求</span><span class="sxs-lookup"><span data-stu-id="340c4-150">Request</span></span>
<span data-ttu-id="340c4-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="340c4-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="340c4-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="340c4-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR
Content-type: application/json
Content-length: 27
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "name": "Development"
}
```
# <a name="c"></a>[<span data-ttu-id="340c4-153">C#</span><span class="sxs-lookup"><span data-stu-id="340c4-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerbucket-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="340c4-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="340c4-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerbucket-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="340c4-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="340c4-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerbucket-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="340c4-156">Java</span><span class="sxs-lookup"><span data-stu-id="340c4-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerbucket-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="340c4-157">响应</span><span class="sxs-lookup"><span data-stu-id="340c4-157">Response</span></span>
<span data-ttu-id="340c4-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="340c4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "name": "Development",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerbucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


