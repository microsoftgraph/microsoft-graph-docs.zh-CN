---
title: 更新 plannerUser
description: 更新 plannerUser 对象的属性。 可以使用此操作在用户最喜爱的计划列表中添加或删除计划，并指示用户最近查看的计划。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 20c50b423962e9c8289ba3c00556deeba22b50e4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474029"
---
# <a name="update-planneruser"></a><span data-ttu-id="28fc3-104">更新 plannerUser</span><span class="sxs-lookup"><span data-stu-id="28fc3-104">Update plannerUser</span></span>

<span data-ttu-id="28fc3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28fc3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28fc3-106">更新 [plannerUser 对象](../resources/planneruser.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="28fc3-106">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="28fc3-107">可以使用此操作在用户最喜爱的计划列表中添加或删除计划，并指示用户最近查看的计划。</span><span class="sxs-lookup"><span data-stu-id="28fc3-107">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="28fc3-108">权限</span><span class="sxs-lookup"><span data-stu-id="28fc3-108">Permissions</span></span>
<span data-ttu-id="28fc3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28fc3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28fc3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="28fc3-111">Permission type</span></span>      | <span data-ttu-id="28fc3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28fc3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28fc3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28fc3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="28fc3-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28fc3-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="28fc3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28fc3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28fc3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="28fc3-116">Not supported.</span></span>    |
|<span data-ttu-id="28fc3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="28fc3-117">Application</span></span> | <span data-ttu-id="28fc3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="28fc3-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28fc3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28fc3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="28fc3-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="28fc3-120">Optional request headers</span></span>
| <span data-ttu-id="28fc3-121">名称</span><span class="sxs-lookup"><span data-stu-id="28fc3-121">Name</span></span>       | <span data-ttu-id="28fc3-122">说明</span><span class="sxs-lookup"><span data-stu-id="28fc3-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="28fc3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="28fc3-123">Authorization</span></span>  | <span data-ttu-id="28fc3-124">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="28fc3-124">Bearer {code}.</span></span> <span data-ttu-id="28fc3-125">必需。</span><span class="sxs-lookup"><span data-stu-id="28fc3-125">Required.</span></span>|
| <span data-ttu-id="28fc3-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="28fc3-126">If-Match</span></span>  | <span data-ttu-id="28fc3-127">要更新的 **plannerUser** 的上次已知 ETag 值。</span><span class="sxs-lookup"><span data-stu-id="28fc3-127">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="28fc3-128">必填。</span><span class="sxs-lookup"><span data-stu-id="28fc3-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="28fc3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="28fc3-129">Request body</span></span>
<span data-ttu-id="28fc3-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="28fc3-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="28fc3-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="28fc3-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="28fc3-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="28fc3-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="28fc3-133">属性</span><span class="sxs-lookup"><span data-stu-id="28fc3-133">Property</span></span>     | <span data-ttu-id="28fc3-134">类型</span><span class="sxs-lookup"><span data-stu-id="28fc3-134">Type</span></span>   |<span data-ttu-id="28fc3-135">说明</span><span class="sxs-lookup"><span data-stu-id="28fc3-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28fc3-136">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="28fc3-136">favoritePlanReferences</span></span>|[<span data-ttu-id="28fc3-137">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="28fc3-137">plannerFavoritePlanReferenceCollection</span></span>](../resources/plannerfavoriteplanreferencecollection.md)|<span data-ttu-id="28fc3-138">对包含用户标记为收藏夹的计划的引用的集合的更改。</span><span class="sxs-lookup"><span data-stu-id="28fc3-138">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="28fc3-139">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="28fc3-139">recentPlanReferences</span></span>|[<span data-ttu-id="28fc3-140">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="28fc3-140">plannerRecentPlanReferenceCollection</span></span>](../resources/plannerrecentplanreferencecollection.md)|<span data-ttu-id="28fc3-141">对包含用户最近查看的计划的引用的集合的更改。</span><span class="sxs-lookup"><span data-stu-id="28fc3-141">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="28fc3-142">响应</span><span class="sxs-lookup"><span data-stu-id="28fc3-142">Response</span></span>
<span data-ttu-id="28fc3-143">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和更新 [的 plannerUser](../resources/planneruser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="28fc3-143">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="28fc3-p107">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="28fc3-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="28fc3-147">示例</span><span class="sxs-lookup"><span data-stu-id="28fc3-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28fc3-148">请求</span><span class="sxs-lookup"><span data-stu-id="28fc3-148">Request</span></span>
<span data-ttu-id="28fc3-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="28fc3-149">The following is an example of the request.</span></span> <span data-ttu-id="28fc3-150">此请求将 ID 为"jd8S5gOaFk2S8aWCIAJz42QAAxtD"的计划添加为用户的收藏夹，并将 ID 为"7oTB5aMIAE2rVo-1N-L7RmQAGX2q"的计划从收藏夹列表中删除。</span><span class="sxs-lookup"><span data-stu-id="28fc3-150">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="28fc3-151">它还更新计划"jd8S5gOaFk2S8aWCIAJz42QAAxtD"的最后一次查看时间。</span><span class="sxs-lookup"><span data-stu-id="28fc3-151">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>

# <a name="http"></a>[<span data-ttu-id="28fc3-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="28fc3-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="c"></a>[<span data-ttu-id="28fc3-153">C#</span><span class="sxs-lookup"><span data-stu-id="28fc3-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-planneruser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28fc3-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28fc3-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-planneruser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28fc3-155">响应</span><span class="sxs-lookup"><span data-stu-id="28fc3-155">Response</span></span>
<span data-ttu-id="28fc3-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="28fc3-156">The following is an example of the response.</span></span> 

><span data-ttu-id="28fc3-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="28fc3-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
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
  "suppressions": []
}
-->


