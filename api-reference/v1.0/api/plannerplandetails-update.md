---
title: 更新 plannerplandetails
description: 更新 **plannerplandetails** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 73d238775eb138c2bc978f75790220e445fb4872
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274149"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="17b39-103">更新 plannerplandetails</span><span class="sxs-lookup"><span data-stu-id="17b39-103">Update plannerplandetails</span></span>

<span data-ttu-id="17b39-104">更新 **plannerplandetails** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="17b39-104">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="17b39-105">权限</span><span class="sxs-lookup"><span data-stu-id="17b39-105">Permissions</span></span>
<span data-ttu-id="17b39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17b39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17b39-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="17b39-108">Permission type</span></span>      | <span data-ttu-id="17b39-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17b39-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17b39-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17b39-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17b39-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17b39-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="17b39-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17b39-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17b39-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="17b39-113">Not supported.</span></span>    |
|<span data-ttu-id="17b39-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="17b39-114">Application</span></span> | <span data-ttu-id="17b39-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="17b39-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17b39-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17b39-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="17b39-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="17b39-117">Optional request headers</span></span>
| <span data-ttu-id="17b39-118">名称</span><span class="sxs-lookup"><span data-stu-id="17b39-118">Name</span></span>       | <span data-ttu-id="17b39-119">说明</span><span class="sxs-lookup"><span data-stu-id="17b39-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="17b39-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="17b39-120">Authorization</span></span>  | <span data-ttu-id="17b39-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17b39-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="17b39-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="17b39-123">If-Match</span></span>  | <span data-ttu-id="17b39-p103">要更新的 plannerPlanDetails 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="17b39-p103">Last known ETag value for the plannerPlanDetails to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="17b39-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="17b39-126">Request body</span></span>
<span data-ttu-id="17b39-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="17b39-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="17b39-130">属性</span><span class="sxs-lookup"><span data-stu-id="17b39-130">Property</span></span>     | <span data-ttu-id="17b39-131">类型</span><span class="sxs-lookup"><span data-stu-id="17b39-131">Type</span></span>   |<span data-ttu-id="17b39-132">说明</span><span class="sxs-lookup"><span data-stu-id="17b39-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17b39-133">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="17b39-133">categoryDescriptions</span></span>|[<span data-ttu-id="17b39-134">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="17b39-134">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="17b39-135">指定可与计划中的任务相关联的六个类别的描述的对象</span><span class="sxs-lookup"><span data-stu-id="17b39-135">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="17b39-136">sharedWith</span><span class="sxs-lookup"><span data-stu-id="17b39-136">sharedWith</span></span>|[<span data-ttu-id="17b39-137">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="17b39-137">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="17b39-p105">此计划共享的用户 id 集合。如果你正在利用 Office 365 组，使用组 API 管理组成员身份以共享[组的](../resources/group.md)计划。你还可以将现有的组成员添加到此集合，尽管他们无需访问组拥有的计划。</span><span class="sxs-lookup"><span data-stu-id="17b39-p105">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="17b39-141">响应</span><span class="sxs-lookup"><span data-stu-id="17b39-141">Response</span></span>

<span data-ttu-id="17b39-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerPlanDetails](../resources/plannerplandetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="17b39-142">If successful, this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="17b39-p106">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="17b39-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="17b39-146">示例</span><span class="sxs-lookup"><span data-stu-id="17b39-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17b39-147">请求</span><span class="sxs-lookup"><span data-stu-id="17b39-147">Request</span></span>
<span data-ttu-id="17b39-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17b39-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplandetails"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/details
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
##### <a name="response"></a><span data-ttu-id="17b39-149">响应</span><span class="sxs-lookup"><span data-stu-id="17b39-149">Response</span></span>
<span data-ttu-id="17b39-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="17b39-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="17b39-153">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="17b39-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="17b39-154">C#</span><span class="sxs-lookup"><span data-stu-id="17b39-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_plannerplandetails-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17b39-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="17b39-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_plannerplandetails-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="17b39-156">目标-C</span><span class="sxs-lookup"><span data-stu-id="17b39-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_plannerplandetails-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplandetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/plannerplandetails-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/plannerplandetails-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/plannerplandetails-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
