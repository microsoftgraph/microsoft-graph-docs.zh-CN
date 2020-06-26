---
title: 更新 plannerplandetails
description: 更新 **plannerplandetails** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 904826370ecd5d75dbdce73cad1de820e7363d2a
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896537"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="45200-103">更新 plannerplandetails</span><span class="sxs-lookup"><span data-stu-id="45200-103">Update plannerplandetails</span></span>

<span data-ttu-id="45200-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45200-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45200-105">更新 **plannerplandetails** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="45200-105">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="45200-106">权限</span><span class="sxs-lookup"><span data-stu-id="45200-106">Permissions</span></span>
<span data-ttu-id="45200-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="45200-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="45200-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45200-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45200-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="45200-109">Permission type</span></span>      | <span data-ttu-id="45200-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45200-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45200-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45200-111">Delegated (work or school account)</span></span> | <span data-ttu-id="45200-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45200-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="45200-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45200-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45200-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="45200-114">Not supported.</span></span>    |
|<span data-ttu-id="45200-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="45200-115">Application</span></span> | <span data-ttu-id="45200-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="45200-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45200-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45200-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="45200-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="45200-118">Optional request headers</span></span>
| <span data-ttu-id="45200-119">名称</span><span class="sxs-lookup"><span data-stu-id="45200-119">Name</span></span>       | <span data-ttu-id="45200-120">说明</span><span class="sxs-lookup"><span data-stu-id="45200-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="45200-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="45200-121">Authorization</span></span>  | <span data-ttu-id="45200-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="45200-122">Bearer {token}.</span></span> <span data-ttu-id="45200-123">Required.</span><span class="sxs-lookup"><span data-stu-id="45200-123">Required.</span></span> |
| <span data-ttu-id="45200-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="45200-124">If-Match</span></span>  | <span data-ttu-id="45200-125">Last known ETag value for the plannerPlanDetails to be updated.</span><span class="sxs-lookup"><span data-stu-id="45200-125">Last known ETag value for the plannerPlanDetails to be updated.</span></span> <span data-ttu-id="45200-126">Required.</span><span class="sxs-lookup"><span data-stu-id="45200-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45200-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="45200-127">Request body</span></span>
<span data-ttu-id="45200-128">In the request body, supply the values for relevant fields that should be updated.</span><span class="sxs-lookup"><span data-stu-id="45200-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="45200-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span><span class="sxs-lookup"><span data-stu-id="45200-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="45200-130">For best performance you shouldn't include existing values that haven't changed.</span><span class="sxs-lookup"><span data-stu-id="45200-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="45200-131">属性</span><span class="sxs-lookup"><span data-stu-id="45200-131">Property</span></span>     | <span data-ttu-id="45200-132">类型</span><span class="sxs-lookup"><span data-stu-id="45200-132">Type</span></span>   |<span data-ttu-id="45200-133">说明</span><span class="sxs-lookup"><span data-stu-id="45200-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45200-134">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="45200-134">categoryDescriptions</span></span>|[<span data-ttu-id="45200-135">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="45200-135">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="45200-136">指定可与计划中的任务相关联的六个类别的描述的对象</span><span class="sxs-lookup"><span data-stu-id="45200-136">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="45200-137">sharedWith</span><span class="sxs-lookup"><span data-stu-id="45200-137">sharedWith</span></span>|[<span data-ttu-id="45200-138">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="45200-138">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="45200-139">与之共享此计划的用户 id 集。</span><span class="sxs-lookup"><span data-stu-id="45200-139">Set of user ids that this plan is shared with.</span></span> <span data-ttu-id="45200-140">如果您利用的是 Microsoft 365 组，请使用组 API 来管理组成员身份，以共享[组的](../resources/group.md)计划。</span><span class="sxs-lookup"><span data-stu-id="45200-140">If you are leveraging Microsoft 365 groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan.</span></span> <span data-ttu-id="45200-141">您还可以将组的现有成员添加到此集合中，但它们不需要他们访问该组拥有的计划。</span><span class="sxs-lookup"><span data-stu-id="45200-141">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="45200-142">响应</span><span class="sxs-lookup"><span data-stu-id="45200-142">Response</span></span>

<span data-ttu-id="45200-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerPlanDetails](../resources/plannerplandetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45200-143">If successful, this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="45200-144">This method can return any of the [HTTP status codes](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="45200-144">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="45200-145">The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses.</span><span class="sxs-lookup"><span data-stu-id="45200-145">The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses.</span></span> <span data-ttu-id="45200-146">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="45200-146">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="45200-147">示例</span><span class="sxs-lookup"><span data-stu-id="45200-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45200-148">请求</span><span class="sxs-lookup"><span data-stu-id="45200-148">Request</span></span>
<span data-ttu-id="45200-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45200-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45200-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="45200-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerplandetails"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
Content-type: application/json
Content-length: 212
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
# <a name="c"></a>[<span data-ttu-id="45200-151">C#</span><span class="sxs-lookup"><span data-stu-id="45200-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerplandetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45200-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45200-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerplandetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45200-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45200-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerplandetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="45200-154">响应</span><span class="sxs-lookup"><span data-stu-id="45200-154">Response</span></span>
<span data-ttu-id="45200-155">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="45200-155">Here is an example of the response.</span></span> <span data-ttu-id="45200-156">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="45200-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="45200-157">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="45200-157">All of the properties will be returned from an actual call.</span></span>
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
