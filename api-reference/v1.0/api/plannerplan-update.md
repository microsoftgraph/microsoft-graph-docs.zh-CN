---
title: 更新 plannerPlan
description: 更新**plannerPlan**对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: a1b4ef284a243135ad26a01dbed662f37bdfbd33
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35452324"
---
# <a name="update-plannerplan"></a><span data-ttu-id="30f4e-103">更新 plannerPlan</span><span class="sxs-lookup"><span data-stu-id="30f4e-103">Update plannerPlan</span></span>

<span data-ttu-id="30f4e-104">更新**plannerPlan**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="30f4e-104">Update the properties of **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="30f4e-105">权限</span><span class="sxs-lookup"><span data-stu-id="30f4e-105">Permissions</span></span>
<span data-ttu-id="30f4e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30f4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30f4e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="30f4e-108">Permission type</span></span>      | <span data-ttu-id="30f4e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30f4e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30f4e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30f4e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="30f4e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30f4e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="30f4e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30f4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30f4e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="30f4e-113">Not supported.</span></span>    |
|<span data-ttu-id="30f4e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="30f4e-114">Application</span></span> | <span data-ttu-id="30f4e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="30f4e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="30f4e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30f4e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}
```

## <a name="request-headers"></a><span data-ttu-id="30f4e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="30f4e-117">Request headers</span></span>

| <span data-ttu-id="30f4e-118">名称</span><span class="sxs-lookup"><span data-stu-id="30f4e-118">Name</span></span>       | <span data-ttu-id="30f4e-119">说明</span><span class="sxs-lookup"><span data-stu-id="30f4e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="30f4e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="30f4e-120">Authorization</span></span>  | <span data-ttu-id="30f4e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="30f4e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="30f4e-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="30f4e-123">If-Match</span></span>  | <span data-ttu-id="30f4e-p103">要更新的 plannerPlan 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="30f4e-p103">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30f4e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="30f4e-126">Request body</span></span>
<span data-ttu-id="30f4e-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="30f4e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="30f4e-130">属性</span><span class="sxs-lookup"><span data-stu-id="30f4e-130">Property</span></span>     | <span data-ttu-id="30f4e-131">类型</span><span class="sxs-lookup"><span data-stu-id="30f4e-131">Type</span></span>   |<span data-ttu-id="30f4e-132">说明</span><span class="sxs-lookup"><span data-stu-id="30f4e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30f4e-133">owner</span><span class="sxs-lookup"><span data-stu-id="30f4e-133">owner</span></span>|<span data-ttu-id="30f4e-134">String</span><span class="sxs-lookup"><span data-stu-id="30f4e-134">String</span></span>|<span data-ttu-id="30f4e-p105">拥有计划的[组](../resources/group.md)`id`。必须存在有效的组才能设置此字段。设置后，只能由所有者更新此字段。</span><span class="sxs-lookup"><span data-stu-id="30f4e-p105">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="30f4e-138">title</span><span class="sxs-lookup"><span data-stu-id="30f4e-138">title</span></span>|<span data-ttu-id="30f4e-139">String</span><span class="sxs-lookup"><span data-stu-id="30f4e-139">String</span></span>|<span data-ttu-id="30f4e-140">计划的标题。</span><span class="sxs-lookup"><span data-stu-id="30f4e-140">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="30f4e-141">响应</span><span class="sxs-lookup"><span data-stu-id="30f4e-141">Response</span></span>

<span data-ttu-id="30f4e-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerPlan](../resources/plannerplan.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="30f4e-142">If successful, this method returns a `200 OK` response code and updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="30f4e-p106">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="30f4e-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="30f4e-146">示例</span><span class="sxs-lookup"><span data-stu-id="30f4e-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30f4e-147">请求</span><span class="sxs-lookup"><span data-stu-id="30f4e-147">Request</span></span>
<span data-ttu-id="30f4e-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="30f4e-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="30f4e-149">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="30f4e-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/{plan-id}
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="30f4e-150">C#</span><span class="sxs-lookup"><span data-stu-id="30f4e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="30f4e-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="30f4e-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="30f4e-152">目标-C</span><span class="sxs-lookup"><span data-stu-id="30f4e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="30f4e-153">响应</span><span class="sxs-lookup"><span data-stu-id="30f4e-153">Response</span></span>
<span data-ttu-id="30f4e-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="30f4e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
