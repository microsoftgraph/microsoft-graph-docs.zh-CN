---
title: 更新 plannerPlan
description: 更新 **plannerPlan 对象** 的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 9ff3eb5d6cb39a16a3c18f3475ec685558bef200
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035097"
---
# <a name="update-plannerplan"></a><span data-ttu-id="cd633-103">更新 plannerPlan</span><span class="sxs-lookup"><span data-stu-id="cd633-103">Update plannerPlan</span></span>

<span data-ttu-id="cd633-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd633-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd633-105">更新 **plannerPlan 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="cd633-105">Update the properties of a **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd633-106">权限</span><span class="sxs-lookup"><span data-stu-id="cd633-106">Permissions</span></span>
<span data-ttu-id="cd633-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd633-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd633-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd633-109">Permission type</span></span>      | <span data-ttu-id="cd633-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd633-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd633-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd633-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cd633-112">Tasks.ReadWrite，Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd633-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cd633-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd633-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd633-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd633-114">Not supported.</span></span>    |
|<span data-ttu-id="cd633-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd633-115">Application</span></span> | <span data-ttu-id="cd633-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd633-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd633-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd633-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{plan-id}
```

## <a name="request-headers"></a><span data-ttu-id="cd633-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd633-118">Request headers</span></span>

| <span data-ttu-id="cd633-119">名称</span><span class="sxs-lookup"><span data-stu-id="cd633-119">Name</span></span>       | <span data-ttu-id="cd633-120">说明</span><span class="sxs-lookup"><span data-stu-id="cd633-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cd633-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd633-121">Authorization</span></span>  | <span data-ttu-id="cd633-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd633-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd633-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="cd633-124">If-Match</span></span>  | <span data-ttu-id="cd633-p103">要更新的 plannerPlan 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="cd633-p103">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd633-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd633-127">Request body</span></span>
<span data-ttu-id="cd633-128">在请求正文中，提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="cd633-128">In the request body, supply the values for relevant fields to updated.</span></span> <span data-ttu-id="cd633-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="cd633-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="cd633-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="cd633-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cd633-131">属性</span><span class="sxs-lookup"><span data-stu-id="cd633-131">Property</span></span>     | <span data-ttu-id="cd633-132">类型</span><span class="sxs-lookup"><span data-stu-id="cd633-132">Type</span></span>   |<span data-ttu-id="cd633-133">说明</span><span class="sxs-lookup"><span data-stu-id="cd633-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd633-134">owner</span><span class="sxs-lookup"><span data-stu-id="cd633-134">owner</span></span>|<span data-ttu-id="cd633-135">String</span><span class="sxs-lookup"><span data-stu-id="cd633-135">String</span></span>|<span data-ttu-id="cd633-p105">拥有计划的[组](../resources/group.md)`id`。必须存在有效的组才能设置此字段。设置后，只能由所有者更新此字段。</span><span class="sxs-lookup"><span data-stu-id="cd633-p105">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="cd633-139">title</span><span class="sxs-lookup"><span data-stu-id="cd633-139">title</span></span>|<span data-ttu-id="cd633-140">String</span><span class="sxs-lookup"><span data-stu-id="cd633-140">String</span></span>|<span data-ttu-id="cd633-141">计划的标题。</span><span class="sxs-lookup"><span data-stu-id="cd633-141">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="cd633-142">响应</span><span class="sxs-lookup"><span data-stu-id="cd633-142">Response</span></span>

<span data-ttu-id="cd633-143">如果成功，此方法将返回 `204 No Content` 响应和空内容。</span><span class="sxs-lookup"><span data-stu-id="cd633-143">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="cd633-144">如果请求指定具有首选项的标头，则此方法在响应正文中返回 响应代码和更新的 `Prefer` `return=representation` `200 OK` [plannerPlan](../resources/plannerplan.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd633-144">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and an updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="cd633-p107">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="cd633-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="cd633-148">示例</span><span class="sxs-lookup"><span data-stu-id="cd633-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd633-149">请求</span><span class="sxs-lookup"><span data-stu-id="cd633-149">Request</span></span>
<span data-ttu-id="cd633-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd633-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cd633-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd633-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/{plan-id}
Content-type: application/json
Content-length: 29
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
# <a name="c"></a>[<span data-ttu-id="cd633-152">C#</span><span class="sxs-lookup"><span data-stu-id="cd633-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd633-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd633-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd633-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd633-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd633-155">Java</span><span class="sxs-lookup"><span data-stu-id="cd633-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cd633-156">响应</span><span class="sxs-lookup"><span data-stu-id="cd633-156">Response</span></span>
<span data-ttu-id="cd633-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cd633-157">Here is an example of the response.</span></span> 

><span data-ttu-id="cd633-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cd633-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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

