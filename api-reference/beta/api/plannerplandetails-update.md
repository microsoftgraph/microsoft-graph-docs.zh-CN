---
title: 更新 plannerplandetails
description: 更新 **plannerplandetails** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: fd42196238fb103021debf8a4fee2f658053a255
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950135"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="69ba0-103">更新 plannerplandetails</span><span class="sxs-lookup"><span data-stu-id="69ba0-103">Update plannerplandetails</span></span>

> <span data-ttu-id="69ba0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="69ba0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69ba0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="69ba0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="69ba0-106">更新 **plannerplandetails** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="69ba0-106">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="69ba0-107">权限</span><span class="sxs-lookup"><span data-stu-id="69ba0-107">Permissions</span></span>
<span data-ttu-id="69ba0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69ba0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69ba0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="69ba0-110">Permission type</span></span>      | <span data-ttu-id="69ba0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69ba0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69ba0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69ba0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="69ba0-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ba0-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="69ba0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69ba0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69ba0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="69ba0-115">Not supported.</span></span>    |
|<span data-ttu-id="69ba0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="69ba0-116">Application</span></span> | <span data-ttu-id="69ba0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="69ba0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="69ba0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69ba0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="69ba0-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="69ba0-119">Optional request headers</span></span>
| <span data-ttu-id="69ba0-120">名称</span><span class="sxs-lookup"><span data-stu-id="69ba0-120">Name</span></span>       | <span data-ttu-id="69ba0-121">说明</span><span class="sxs-lookup"><span data-stu-id="69ba0-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="69ba0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="69ba0-122">Authorization</span></span>  | <span data-ttu-id="69ba0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69ba0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69ba0-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="69ba0-125">If-Match</span></span>  | <span data-ttu-id="69ba0-p104">要更新的 plannerPlanDetails 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="69ba0-p104">Last known ETag value for the plannerPlanDetails to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69ba0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="69ba0-128">Request body</span></span>
<span data-ttu-id="69ba0-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="69ba0-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="69ba0-132">属性</span><span class="sxs-lookup"><span data-stu-id="69ba0-132">Property</span></span>     | <span data-ttu-id="69ba0-133">类型</span><span class="sxs-lookup"><span data-stu-id="69ba0-133">Type</span></span>   |<span data-ttu-id="69ba0-134">说明</span><span class="sxs-lookup"><span data-stu-id="69ba0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69ba0-135">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="69ba0-135">categoryDescriptions</span></span>|[<span data-ttu-id="69ba0-136">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="69ba0-136">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="69ba0-137">指定可与计划中的任务相关联的六个类别的描述的对象</span><span class="sxs-lookup"><span data-stu-id="69ba0-137">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="69ba0-138">sharedWith</span><span class="sxs-lookup"><span data-stu-id="69ba0-138">sharedWith</span></span>|[<span data-ttu-id="69ba0-139">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="69ba0-139">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="69ba0-p106">此计划共享的用户 id 集合。如果你正在利用 Office 365 组，使用组 API 管理组成员身份以共享[组的](../resources/group.md)计划。你还可以将现有的组成员添加到此集合，尽管他们无需访问组拥有的计划。</span><span class="sxs-lookup"><span data-stu-id="69ba0-p106">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="69ba0-143">响应</span><span class="sxs-lookup"><span data-stu-id="69ba0-143">Response</span></span>

<span data-ttu-id="69ba0-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerPlanDetails](../resources/plannerplandetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="69ba0-144">If successful, this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="69ba0-p107">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="69ba0-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="69ba0-148">示例</span><span class="sxs-lookup"><span data-stu-id="69ba0-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69ba0-149">请求</span><span class="sxs-lookup"><span data-stu-id="69ba0-149">Request</span></span>
<span data-ttu-id="69ba0-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69ba0-150">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="69ba0-151">响应</span><span class="sxs-lookup"><span data-stu-id="69ba0-151">Response</span></span>
<span data-ttu-id="69ba0-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69ba0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplandetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
