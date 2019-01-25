---
title: 更新 plannerUser
description: 更新 plannerUser 对象的属性。 此操作可用于添加或删除计划从用户的收藏夹计划列表中，并以指示该计划用户具有最近查看。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 95c631d39fb650dea0b87871bdd10d92a3ab31eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508921"
---
# <a name="update-planneruser"></a><span data-ttu-id="9d37c-104">更新 plannerUser</span><span class="sxs-lookup"><span data-stu-id="9d37c-104">Update plannerUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d37c-105">更新[plannerUser](../resources/planneruser.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9d37c-105">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="9d37c-106">此操作可用于添加或删除计划从用户的收藏夹计划列表中，并以指示该计划用户具有最近查看。</span><span class="sxs-lookup"><span data-stu-id="9d37c-106">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d37c-107">权限</span><span class="sxs-lookup"><span data-stu-id="9d37c-107">Permissions</span></span>
<span data-ttu-id="9d37c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d37c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d37c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d37c-110">Permission type</span></span>      | <span data-ttu-id="9d37c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d37c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d37c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d37c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d37c-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d37c-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9d37c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d37c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d37c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d37c-115">Not supported.</span></span>    |
|<span data-ttu-id="9d37c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d37c-116">Application</span></span> | <span data-ttu-id="9d37c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d37c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d37c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d37c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="9d37c-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="9d37c-119">Optional request headers</span></span>
| <span data-ttu-id="9d37c-120">名称</span><span class="sxs-lookup"><span data-stu-id="9d37c-120">Name</span></span>       | <span data-ttu-id="9d37c-121">说明</span><span class="sxs-lookup"><span data-stu-id="9d37c-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9d37c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d37c-122">Authorization</span></span>  | <span data-ttu-id="9d37c-p104">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="9d37c-p104">Bearer {code}. Required.</span></span>|
| <span data-ttu-id="9d37c-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="9d37c-125">If-Match</span></span>  | <span data-ttu-id="9d37c-126">最后的**plannerUser**要更新的已知的 ETag 值。</span><span class="sxs-lookup"><span data-stu-id="9d37c-126">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="9d37c-127">必需。</span><span class="sxs-lookup"><span data-stu-id="9d37c-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d37c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d37c-128">Request body</span></span>
<span data-ttu-id="9d37c-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="9d37c-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9d37c-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="9d37c-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9d37c-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9d37c-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9d37c-132">属性</span><span class="sxs-lookup"><span data-stu-id="9d37c-132">Property</span></span>     | <span data-ttu-id="9d37c-133">类型</span><span class="sxs-lookup"><span data-stu-id="9d37c-133">Type</span></span>   |<span data-ttu-id="9d37c-134">说明</span><span class="sxs-lookup"><span data-stu-id="9d37c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d37c-135">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="9d37c-135">favoritePlanReferences</span></span>|[<span data-ttu-id="9d37c-136">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="9d37c-136">plannerFavoritePlanReferenceCollection</span></span>](../resources/plannerfavoriteplanreferencecollection.md)|<span data-ttu-id="9d37c-137">对包含用户已标记为收藏计划引用的集合。</span><span class="sxs-lookup"><span data-stu-id="9d37c-137">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="9d37c-138">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="9d37c-138">recentPlanReferences</span></span>|[<span data-ttu-id="9d37c-139">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="9d37c-139">plannerRecentPlanReferenceCollection</span></span>](../resources/plannerrecentplanreferencecollection.md)|<span data-ttu-id="9d37c-140">对包含对用户具有最近查看的计划的引用的集合。</span><span class="sxs-lookup"><span data-stu-id="9d37c-140">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="9d37c-141">响应</span><span class="sxs-lookup"><span data-stu-id="9d37c-141">Response</span></span>
<span data-ttu-id="9d37c-142">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[plannerUser](../resources/planneruser.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9d37c-142">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="9d37c-p107">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="9d37c-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="9d37c-146">示例</span><span class="sxs-lookup"><span data-stu-id="9d37c-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d37c-147">请求</span><span class="sxs-lookup"><span data-stu-id="9d37c-147">Request</span></span>
<span data-ttu-id="9d37c-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9d37c-148">The following is an example of the request.</span></span> <span data-ttu-id="9d37c-149">此请求将作为用户的收藏夹中添加 ID"jd8S5gOaFk2S8aWCIAJz42QAAxtD"计划"下一版本讨论"，并从最喜爱的计划列表中删除 id 为"7oTB5aMIAE2rVo 1N L7RmQAGX2q"计划。</span><span class="sxs-lookup"><span data-stu-id="9d37c-149">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="9d37c-150">它还更新计划"jd8S5gOaFk2S8aWCIAJz42QAAxtD"的视图上次。</span><span class="sxs-lookup"><span data-stu-id="9d37c-150">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>
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
##### <a name="response"></a><span data-ttu-id="9d37c-151">响应</span><span class="sxs-lookup"><span data-stu-id="9d37c-151">Response</span></span>
<span data-ttu-id="9d37c-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9d37c-152">The following is an example of the response.</span></span> 

><span data-ttu-id="9d37c-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9d37c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Update planneruser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
