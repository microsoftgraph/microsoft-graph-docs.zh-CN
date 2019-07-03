---
title: 更新 plannerBucketTaskBoardTaskFormat
description: 更新 **plannerBucketTaskBoardTaskFormat** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: efae23d2247ff1f504cc4ff9cc1155431575e0c2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445833"
---
# <a name="update-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="64b97-103">更新 plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="64b97-103">Update plannerBucketTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64b97-104">更新 **plannerBucketTaskBoardTaskFormat** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="64b97-104">Update the properties of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="64b97-105">权限</span><span class="sxs-lookup"><span data-stu-id="64b97-105">Permissions</span></span>
<span data-ttu-id="64b97-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64b97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64b97-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="64b97-108">Permission type</span></span>      | <span data-ttu-id="64b97-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64b97-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64b97-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64b97-110">Delegated (work or school account)</span></span> | <span data-ttu-id="64b97-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64b97-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="64b97-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64b97-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64b97-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="64b97-113">Not supported.</span></span>    |
|<span data-ttu-id="64b97-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="64b97-114">Application</span></span> | <span data-ttu-id="64b97-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="64b97-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64b97-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64b97-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/bucketTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="64b97-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="64b97-117">Optional request headers</span></span>
| <span data-ttu-id="64b97-118">名称</span><span class="sxs-lookup"><span data-stu-id="64b97-118">Name</span></span>       | <span data-ttu-id="64b97-119">说明</span><span class="sxs-lookup"><span data-stu-id="64b97-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="64b97-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="64b97-120">Authorization</span></span>  | <span data-ttu-id="64b97-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64b97-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64b97-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="64b97-123">If-Match</span></span>  | <span data-ttu-id="64b97-p103">要更新的 **plannerBucketTaskBoardTaskFormat** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="64b97-p103">Last known ETag value for the **plannerBucketTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64b97-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="64b97-126">Request body</span></span>
<span data-ttu-id="64b97-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="64b97-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="64b97-130">属性</span><span class="sxs-lookup"><span data-stu-id="64b97-130">Property</span></span>     | <span data-ttu-id="64b97-131">类型</span><span class="sxs-lookup"><span data-stu-id="64b97-131">Type</span></span>   |<span data-ttu-id="64b97-132">说明</span><span class="sxs-lookup"><span data-stu-id="64b97-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64b97-133">orderHint</span><span class="sxs-lookup"><span data-stu-id="64b97-133">orderHint</span></span>|<span data-ttu-id="64b97-134">String</span><span class="sxs-lookup"><span data-stu-id="64b97-134">String</span></span>|<span data-ttu-id="64b97-p105">用于为任务板存储桶视图中的任务进行排序的提示。[此处](../resources/planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="64b97-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="64b97-137">响应</span><span class="sxs-lookup"><span data-stu-id="64b97-137">Response</span></span>

<span data-ttu-id="64b97-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64b97-138">If successful, this method returns a `200 OK` response code and updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="64b97-p106">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="64b97-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="64b97-142">示例</span><span class="sxs-lookup"><span data-stu-id="64b97-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64b97-143">请求</span><span class="sxs-lookup"><span data-stu-id="64b97-143">Request</span></span>
<span data-ttu-id="64b97-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64b97-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="64b97-145">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="64b97-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerbuckettaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="64b97-146">C#</span><span class="sxs-lookup"><span data-stu-id="64b97-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerbuckettaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64b97-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="64b97-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerbuckettaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="64b97-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="64b97-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerbuckettaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="64b97-149">响应</span><span class="sxs-lookup"><span data-stu-id="64b97-149">Response</span></span>
<span data-ttu-id="64b97-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64b97-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerbuckettaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
