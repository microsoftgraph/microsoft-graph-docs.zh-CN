---
title: 更新 plannerUser
description: 更新 plannerUser 对象的属性。 可以使用此操作在用户最喜爱的计划列表中添加或删除计划，并指示用户最近查看过的计划。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 0555d7ccfd843fbfac3cf51fe43c61e16930421a
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473925"
---
# <a name="update-planneruser"></a><span data-ttu-id="07b27-104">更新 plannerUser</span><span class="sxs-lookup"><span data-stu-id="07b27-104">Update plannerUser</span></span>

<span data-ttu-id="07b27-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07b27-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07b27-106">更新 [plannerUser 对象](../resources/planneruser.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="07b27-106">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="07b27-107">可以使用此操作在用户最喜爱的计划列表中添加或删除计划，并指示用户最近查看过的计划。</span><span class="sxs-lookup"><span data-stu-id="07b27-107">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="07b27-108">权限</span><span class="sxs-lookup"><span data-stu-id="07b27-108">Permissions</span></span>
<span data-ttu-id="07b27-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07b27-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07b27-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="07b27-111">Permission type</span></span>      | <span data-ttu-id="07b27-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07b27-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07b27-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07b27-113">Delegated (work or school account)</span></span> | <span data-ttu-id="07b27-114">Tasks.ReadWrite、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07b27-114">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="07b27-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07b27-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07b27-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="07b27-116">Not supported.</span></span>    |
|<span data-ttu-id="07b27-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="07b27-117">Application</span></span> | <span data-ttu-id="07b27-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="07b27-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07b27-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07b27-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="07b27-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="07b27-120">Optional request headers</span></span>
| <span data-ttu-id="07b27-121">名称</span><span class="sxs-lookup"><span data-stu-id="07b27-121">Name</span></span>       | <span data-ttu-id="07b27-122">说明</span><span class="sxs-lookup"><span data-stu-id="07b27-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="07b27-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07b27-123">Authorization</span></span>  | <span data-ttu-id="07b27-124">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="07b27-124">Bearer {code}.</span></span> <span data-ttu-id="07b27-125">必需。</span><span class="sxs-lookup"><span data-stu-id="07b27-125">Required.</span></span>|
| <span data-ttu-id="07b27-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="07b27-126">If-Match</span></span>  | <span data-ttu-id="07b27-127">要更新的 **plannerUser** 的上次已知 ETag 值。</span><span class="sxs-lookup"><span data-stu-id="07b27-127">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="07b27-128">必需。</span><span class="sxs-lookup"><span data-stu-id="07b27-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="07b27-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="07b27-129">Request body</span></span>
<span data-ttu-id="07b27-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="07b27-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="07b27-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="07b27-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="07b27-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="07b27-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="07b27-133">属性</span><span class="sxs-lookup"><span data-stu-id="07b27-133">Property</span></span>     | <span data-ttu-id="07b27-134">类型</span><span class="sxs-lookup"><span data-stu-id="07b27-134">Type</span></span>   |<span data-ttu-id="07b27-135">说明</span><span class="sxs-lookup"><span data-stu-id="07b27-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07b27-136">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="07b27-136">favoritePlanReferences</span></span>|[<span data-ttu-id="07b27-137">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="07b27-137">plannerFavoritePlanReferenceCollection</span></span>](../resources/plannerfavoriteplanreferencecollection.md)|<span data-ttu-id="07b27-138">对集合所做的更改，该集合包含对用户已标记为收藏的计划的引用。</span><span class="sxs-lookup"><span data-stu-id="07b27-138">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="07b27-139">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="07b27-139">recentPlanReferences</span></span>|[<span data-ttu-id="07b27-140">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="07b27-140">plannerRecentPlanReferenceCollection</span></span>](../resources/plannerrecentplanreferencecollection.md)|<span data-ttu-id="07b27-141">对包含用户最近查看的计划的引用的集合的更改。</span><span class="sxs-lookup"><span data-stu-id="07b27-141">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="07b27-142">响应</span><span class="sxs-lookup"><span data-stu-id="07b27-142">Response</span></span>
<span data-ttu-id="07b27-143">如果成功，此方法将返回 `204 No Content` 响应和空内容。</span><span class="sxs-lookup"><span data-stu-id="07b27-143">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="07b27-144">如果请求指定具有首选项的标头，则此方法在响应正文中返回 响应代码和更新的 `Prefer` `return=representation` `200 OK` [plannerUser](../resources/planneruser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07b27-144">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="07b27-p108">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="07b27-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="07b27-148">示例</span><span class="sxs-lookup"><span data-stu-id="07b27-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07b27-149">请求</span><span class="sxs-lookup"><span data-stu-id="07b27-149">Request</span></span>
<span data-ttu-id="07b27-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="07b27-150">The following is an example of the request.</span></span> <span data-ttu-id="07b27-151">此请求将 ID 为"jd8S5gOaFk2S8aWCIAJz42QAAxtD"的计划添加为用户最喜爱的计划，并从收藏夹计划列表中删除 ID 为"7oTB5aMIAE2rVo-1N-L7RmQAGX2q"的计划。</span><span class="sxs-lookup"><span data-stu-id="07b27-151">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="07b27-152">它还更新计划"jd8S5gOaFk2S8aWCIAJz42QAAxtD"的最后查看时间。</span><span class="sxs-lookup"><span data-stu-id="07b27-152">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>

# <a name="http"></a>[<span data-ttu-id="07b27-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="07b27-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_planneruser"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/planner
Content-type: application/json
Content-length: 504
Prefer: return=representation
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
# <a name="c"></a>[<span data-ttu-id="07b27-154">C#</span><span class="sxs-lookup"><span data-stu-id="07b27-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-planneruser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07b27-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07b27-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-planneruser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="07b27-156">响应</span><span class="sxs-lookup"><span data-stu-id="07b27-156">Response</span></span>
<span data-ttu-id="07b27-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="07b27-157">The following is an example of the response.</span></span> 

><span data-ttu-id="07b27-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="07b27-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


