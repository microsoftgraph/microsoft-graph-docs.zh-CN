---
title: 更新 plannerplandetails
description: 更新 **plannerplandetails** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: ee12fd4607f4f3b2fad4f32e0473698fbe95b601
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473582"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="86934-103">更新 plannerplandetails</span><span class="sxs-lookup"><span data-stu-id="86934-103">Update plannerplandetails</span></span>

<span data-ttu-id="86934-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86934-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86934-105">更新 **plannerplandetails** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="86934-105">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="86934-106">权限</span><span class="sxs-lookup"><span data-stu-id="86934-106">Permissions</span></span>
<span data-ttu-id="86934-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86934-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86934-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="86934-109">Permission type</span></span>      | <span data-ttu-id="86934-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86934-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86934-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86934-111">Delegated (work or school account)</span></span> | <span data-ttu-id="86934-112">Tasks.ReadWrite、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86934-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="86934-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86934-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86934-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="86934-114">Not supported.</span></span>    |
|<span data-ttu-id="86934-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="86934-115">Application</span></span> | <span data-ttu-id="86934-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86934-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86934-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86934-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="86934-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="86934-118">Optional request headers</span></span>
| <span data-ttu-id="86934-119">名称</span><span class="sxs-lookup"><span data-stu-id="86934-119">Name</span></span>       | <span data-ttu-id="86934-120">说明</span><span class="sxs-lookup"><span data-stu-id="86934-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="86934-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="86934-121">Authorization</span></span>  | <span data-ttu-id="86934-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="86934-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="86934-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="86934-124">If-Match</span></span>  | <span data-ttu-id="86934-p103">要更新的 plannerPlanDetails 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="86934-p103">Last known ETag value for the plannerPlanDetails to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86934-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="86934-127">Request body</span></span>
<span data-ttu-id="86934-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="86934-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="86934-131">属性</span><span class="sxs-lookup"><span data-stu-id="86934-131">Property</span></span>     | <span data-ttu-id="86934-132">类型</span><span class="sxs-lookup"><span data-stu-id="86934-132">Type</span></span>   |<span data-ttu-id="86934-133">说明</span><span class="sxs-lookup"><span data-stu-id="86934-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86934-134">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="86934-134">categoryDescriptions</span></span>|[<span data-ttu-id="86934-135">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="86934-135">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="86934-136">指定可与计划中的任务相关联的六个类别的描述的对象</span><span class="sxs-lookup"><span data-stu-id="86934-136">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="86934-137">sharedWith</span><span class="sxs-lookup"><span data-stu-id="86934-137">sharedWith</span></span>|[<span data-ttu-id="86934-138">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="86934-138">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="86934-139">此计划共享的用户 ID 集。</span><span class="sxs-lookup"><span data-stu-id="86934-139">Set of user ids that this plan is shared with.</span></span> <span data-ttu-id="86934-140">如果你要利用 Microsoft 365 组，请使用组 API 管理组成员身份以 [共享组计划](../resources/group.md) 。</span><span class="sxs-lookup"><span data-stu-id="86934-140">If you are leveraging Microsoft 365 groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan.</span></span> <span data-ttu-id="86934-141">您还可以将组的现有成员添加到此集合中，尽管他们无需访问组所拥有的计划。</span><span class="sxs-lookup"><span data-stu-id="86934-141">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="86934-142">响应</span><span class="sxs-lookup"><span data-stu-id="86934-142">Response</span></span>

<span data-ttu-id="86934-143">如果成功，此方法将返回 `204 No Content` 响应和空内容。</span><span class="sxs-lookup"><span data-stu-id="86934-143">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="86934-144">如果请求指定具有首选项的标头，则此方法在响应正文中返回 响应代码和更新的 `Prefer` `return=representation` `200 OK` [plannerPlanDetails](../resources/plannerplandetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86934-144">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="86934-p107">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="86934-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="86934-148">示例</span><span class="sxs-lookup"><span data-stu-id="86934-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86934-149">请求</span><span class="sxs-lookup"><span data-stu-id="86934-149">Request</span></span>
<span data-ttu-id="86934-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86934-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="86934-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="86934-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerplandetails"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
Content-type: application/json
Content-length: 212
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "sharedWith": {
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true,
    "d95e6152-f683-4d78-9ff5-67ad180fea4a" : false,
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category3": null,
  }
}
```
# <a name="c"></a>[<span data-ttu-id="86934-152">C#</span><span class="sxs-lookup"><span data-stu-id="86934-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerplandetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86934-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86934-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerplandetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86934-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86934-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerplandetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86934-155">Java</span><span class="sxs-lookup"><span data-stu-id="86934-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerplandetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="86934-156">响应</span><span class="sxs-lookup"><span data-stu-id="86934-156">Response</span></span>
<span data-ttu-id="86934-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86934-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerplandetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


