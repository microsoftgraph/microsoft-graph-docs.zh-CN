---
title: 更新 plannerUser
description: 更新 plannerUser 对象的属性。 您可以使用此操作在用户的 "收藏夹计划" 列表中添加或删除计划, 并指示用户最近查看过的计划。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 95c631d39fb650dea0b87871bdd10d92a3ab31eb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538751"
---
# <a name="update-planneruser"></a><span data-ttu-id="938fd-104">更新 plannerUser</span><span class="sxs-lookup"><span data-stu-id="938fd-104">Update plannerUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="938fd-105">更新[plannerUser](../resources/planneruser.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="938fd-105">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="938fd-106">您可以使用此操作在用户的 "收藏夹计划" 列表中添加或删除计划, 并指示用户最近查看过的计划。</span><span class="sxs-lookup"><span data-stu-id="938fd-106">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="938fd-107">权限</span><span class="sxs-lookup"><span data-stu-id="938fd-107">Permissions</span></span>
<span data-ttu-id="938fd-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="938fd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="938fd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="938fd-110">Permission type</span></span>      | <span data-ttu-id="938fd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="938fd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="938fd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="938fd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="938fd-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="938fd-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="938fd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="938fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="938fd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="938fd-115">Not supported.</span></span>    |
|<span data-ttu-id="938fd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="938fd-116">Application</span></span> | <span data-ttu-id="938fd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="938fd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="938fd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="938fd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="938fd-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="938fd-119">Optional request headers</span></span>
| <span data-ttu-id="938fd-120">名称</span><span class="sxs-lookup"><span data-stu-id="938fd-120">Name</span></span>       | <span data-ttu-id="938fd-121">说明</span><span class="sxs-lookup"><span data-stu-id="938fd-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="938fd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="938fd-122">Authorization</span></span>  | <span data-ttu-id="938fd-123">持有者 {代码}。</span><span class="sxs-lookup"><span data-stu-id="938fd-123">Bearer {code}.</span></span> <span data-ttu-id="938fd-124">必需。</span><span class="sxs-lookup"><span data-stu-id="938fd-124">Required.</span></span>|
| <span data-ttu-id="938fd-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="938fd-125">If-Match</span></span>  | <span data-ttu-id="938fd-126">要更新的**plannerUser**的最新已知 ETag 值。</span><span class="sxs-lookup"><span data-stu-id="938fd-126">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="938fd-127">必需。</span><span class="sxs-lookup"><span data-stu-id="938fd-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="938fd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="938fd-128">Request body</span></span>
<span data-ttu-id="938fd-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="938fd-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="938fd-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="938fd-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="938fd-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="938fd-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="938fd-132">属性</span><span class="sxs-lookup"><span data-stu-id="938fd-132">Property</span></span>     | <span data-ttu-id="938fd-133">类型</span><span class="sxs-lookup"><span data-stu-id="938fd-133">Type</span></span>   |<span data-ttu-id="938fd-134">说明</span><span class="sxs-lookup"><span data-stu-id="938fd-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="938fd-135">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="938fd-135">favoritePlanReferences</span></span>|[<span data-ttu-id="938fd-136">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="938fd-136">plannerFavoritePlanReferenceCollection</span></span>](../resources/plannerfavoriteplanreferencecollection.md)|<span data-ttu-id="938fd-137">对集合所做的更改, 其中包含对用户已标记为收藏的计划的引用。</span><span class="sxs-lookup"><span data-stu-id="938fd-137">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="938fd-138">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="938fd-138">recentPlanReferences</span></span>|[<span data-ttu-id="938fd-139">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="938fd-139">plannerRecentPlanReferenceCollection</span></span>](../resources/plannerrecentplanreferencecollection.md)|<span data-ttu-id="938fd-140">对集合的更改, 其中包含对用户最近查看过的计划的引用。</span><span class="sxs-lookup"><span data-stu-id="938fd-140">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="938fd-141">响应</span><span class="sxs-lookup"><span data-stu-id="938fd-141">Response</span></span>
<span data-ttu-id="938fd-142">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[plannerUser](../resources/planneruser.md)对象。</span><span class="sxs-lookup"><span data-stu-id="938fd-142">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="938fd-p107">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="938fd-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="938fd-146">示例</span><span class="sxs-lookup"><span data-stu-id="938fd-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="938fd-147">请求</span><span class="sxs-lookup"><span data-stu-id="938fd-147">Request</span></span>
<span data-ttu-id="938fd-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="938fd-148">The following is an example of the request.</span></span> <span data-ttu-id="938fd-149">此请求将 id 为 "jd8S5gOaFk2S8aWCIAJz42QAAxtD" 的计划 "下一次发布讨论" 添加为用户的收藏夹, 并从 "收藏夹计划" 列表中删除 id 为 "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" 的计划。</span><span class="sxs-lookup"><span data-stu-id="938fd-149">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="938fd-150">它还更新了计划 "jd8S5gOaFk2S8aWCIAJz42QAAxtD" 的上次查看时间。</span><span class="sxs-lookup"><span data-stu-id="938fd-150">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>
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
##### <a name="response"></a><span data-ttu-id="938fd-151">响应</span><span class="sxs-lookup"><span data-stu-id="938fd-151">Response</span></span>
<span data-ttu-id="938fd-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="938fd-152">The following is an example of the response.</span></span> 

><span data-ttu-id="938fd-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="938fd-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
