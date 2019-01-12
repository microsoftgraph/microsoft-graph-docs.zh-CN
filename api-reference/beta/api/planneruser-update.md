---
title: 更新 plannerUser
description: 更新 plannerUser 对象的属性。 此操作可用于添加或删除计划从用户的收藏夹计划列表中，并以指示该计划用户具有最近查看。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 733743ffee8e29d66f2ebe411d127161e7e8eb2a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925887"
---
# <a name="update-planneruser"></a><span data-ttu-id="5a906-104">更新 plannerUser</span><span class="sxs-lookup"><span data-stu-id="5a906-104">Update plannerUser</span></span>

> <span data-ttu-id="5a906-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5a906-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a906-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5a906-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a906-107">更新[plannerUser](../resources/planneruser.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5a906-107">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="5a906-108">此操作可用于添加或删除计划从用户的收藏夹计划列表中，并以指示该计划用户具有最近查看。</span><span class="sxs-lookup"><span data-stu-id="5a906-108">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a906-109">权限</span><span class="sxs-lookup"><span data-stu-id="5a906-109">Permissions</span></span>
<span data-ttu-id="5a906-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a906-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a906-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a906-112">Permission type</span></span>      | <span data-ttu-id="5a906-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a906-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a906-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a906-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5a906-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a906-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5a906-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a906-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a906-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a906-117">Not supported.</span></span>    |
|<span data-ttu-id="5a906-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a906-118">Application</span></span> | <span data-ttu-id="5a906-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a906-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a906-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a906-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="5a906-121">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="5a906-121">Optional request headers</span></span>
| <span data-ttu-id="5a906-122">名称</span><span class="sxs-lookup"><span data-stu-id="5a906-122">Name</span></span>       | <span data-ttu-id="5a906-123">说明</span><span class="sxs-lookup"><span data-stu-id="5a906-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5a906-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a906-124">Authorization</span></span>  | <span data-ttu-id="5a906-p105">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a906-p105">Bearer {code}. Required.</span></span>|
| <span data-ttu-id="5a906-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="5a906-127">If-Match</span></span>  | <span data-ttu-id="5a906-128">最后的**plannerUser**要更新的已知的 ETag 值。</span><span class="sxs-lookup"><span data-stu-id="5a906-128">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="5a906-129">必需。</span><span class="sxs-lookup"><span data-stu-id="5a906-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a906-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a906-130">Request body</span></span>
<span data-ttu-id="5a906-131">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="5a906-131">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5a906-132">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="5a906-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5a906-133">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5a906-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5a906-134">属性</span><span class="sxs-lookup"><span data-stu-id="5a906-134">Property</span></span>     | <span data-ttu-id="5a906-135">类型</span><span class="sxs-lookup"><span data-stu-id="5a906-135">Type</span></span>   |<span data-ttu-id="5a906-136">说明</span><span class="sxs-lookup"><span data-stu-id="5a906-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a906-137">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="5a906-137">favoritePlanReferences</span></span>|[<span data-ttu-id="5a906-138">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="5a906-138">plannerFavoritePlanReferenceCollection</span></span>](../resources/plannerfavoriteplanreferencecollection.md)|<span data-ttu-id="5a906-139">对包含用户已标记为收藏计划引用的集合。</span><span class="sxs-lookup"><span data-stu-id="5a906-139">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="5a906-140">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="5a906-140">recentPlanReferences</span></span>|[<span data-ttu-id="5a906-141">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="5a906-141">plannerRecentPlanReferenceCollection</span></span>](../resources/plannerrecentplanreferencecollection.md)|<span data-ttu-id="5a906-142">对包含对用户具有最近查看的计划的引用的集合。</span><span class="sxs-lookup"><span data-stu-id="5a906-142">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="5a906-143">响应</span><span class="sxs-lookup"><span data-stu-id="5a906-143">Response</span></span>
<span data-ttu-id="5a906-144">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[plannerUser](../resources/planneruser.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5a906-144">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="5a906-p108">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="5a906-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="5a906-148">示例</span><span class="sxs-lookup"><span data-stu-id="5a906-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a906-149">请求</span><span class="sxs-lookup"><span data-stu-id="5a906-149">Request</span></span>
<span data-ttu-id="5a906-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5a906-150">The following is an example of the request.</span></span> <span data-ttu-id="5a906-151">此请求将作为用户的收藏夹中添加 ID"jd8S5gOaFk2S8aWCIAJz42QAAxtD"计划"下一版本讨论"，并从最喜爱的计划列表中删除 id 为"7oTB5aMIAE2rVo 1N L7RmQAGX2q"计划。</span><span class="sxs-lookup"><span data-stu-id="5a906-151">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="5a906-152">它还更新计划"jd8S5gOaFk2S8aWCIAJz42QAAxtD"的视图上次。</span><span class="sxs-lookup"><span data-stu-id="5a906-152">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_planneruser"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/planner
Content-type: application/json
Content-length: 504
If-Match: W/"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc="

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": " !",
      "planTitle": "Next Release Discussion"
    },
    "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": null
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    }
  }
}
```
##### <a name="response"></a><span data-ttu-id="5a906-153">响应</span><span class="sxs-lookup"><span data-stu-id="5a906-153">Response</span></span>
<span data-ttu-id="5a906-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5a906-154">The following is an example of the response.</span></span> 

><span data-ttu-id="5a906-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5a906-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586866870001551087",
      "planTitle": "Next Release Discussion"
    },
    "uZWtCtli30CGoWLIWSat1mQAC0ai": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586888705198093378",
      "planTitle": "Product Support"
    }
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    },
    "XYE5pqNJu0uuRC2PM4ZQrmQAF2Pn": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-01T19:39:17.57Z",
      "planTitle": "Success Metrics"
    }
  },
  "id": "-YPnMJRiIUSKFyaVjYEkBWQAAc47"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update planneruser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
