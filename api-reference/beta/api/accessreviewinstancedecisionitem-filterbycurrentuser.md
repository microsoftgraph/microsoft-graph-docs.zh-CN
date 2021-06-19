---
title: accessReviewInstanceDecisionItem：filterByCurrentUser
description: 检索调用用户是审阅者的 accessReviewInstance 上的所有 accessReviewInstanceDecisionItem 对象。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f4f045ac67e1b98179f64a5a09102c975a2f0374
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031441"
---
# <a name="accessreviewinstancedecisionitem-filterbycurrentuser"></a><span data-ttu-id="5dd72-103">accessReviewInstanceDecisionItem：filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="5dd72-103">accessReviewInstanceDecisionItem: filterByCurrentUser</span></span>
<span data-ttu-id="5dd72-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dd72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dd72-105">检索调用用户作为审阅者的给定 accessReviewInstance 上的所有[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)对象。 [](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="5dd72-105">Retrieves all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects on a given [accessReviewInstance](../resources/accessreviewinstance.md) for which the calling user is the reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="5dd72-106">此 API 的默认页面大小为 100 accessReviewInstanceDecisionItem 对象。</span><span class="sxs-lookup"><span data-stu-id="5dd72-106">The default page size for this API is 100 accessReviewInstanceDecisionItem objects.</span></span> <span data-ttu-id="5dd72-107">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="5dd72-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="5dd72-108">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="5dd72-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="5dd72-109">权限</span><span class="sxs-lookup"><span data-stu-id="5dd72-109">Permissions</span></span>
<span data-ttu-id="5dd72-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5dd72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dd72-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5dd72-112">Permission type</span></span>|<span data-ttu-id="5dd72-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5dd72-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dd72-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5dd72-114">Delegated (work or school account)</span></span>|<span data-ttu-id="5dd72-115">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dd72-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="5dd72-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5dd72-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dd72-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5dd72-117">Not supported.</span></span>|
|<span data-ttu-id="5dd72-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5dd72-118">Application</span></span>|<span data-ttu-id="5dd72-119">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dd72-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dd72-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5dd72-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5dd72-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5dd72-121">Optional query parameters</span></span>
<span data-ttu-id="5dd72-122">此方法支持 `$select` 、 、 、 和 OData 查询参数 `$filter` `$orderBy` `$skip` `$top` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5dd72-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="5dd72-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5dd72-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5dd72-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="5dd72-124">Request headers</span></span>
|<span data-ttu-id="5dd72-125">名称</span><span class="sxs-lookup"><span data-stu-id="5dd72-125">Name</span></span>|<span data-ttu-id="5dd72-126">说明</span><span class="sxs-lookup"><span data-stu-id="5dd72-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5dd72-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dd72-127">Authorization</span></span>|<span data-ttu-id="5dd72-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5dd72-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dd72-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5dd72-130">Request body</span></span>
<span data-ttu-id="5dd72-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5dd72-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dd72-132">响应</span><span class="sxs-lookup"><span data-stu-id="5dd72-132">Response</span></span>

<span data-ttu-id="5dd72-133">如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="5dd72-133">If successful, this function returns a `200 OK` response code and a [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5dd72-134">示例</span><span class="sxs-lookup"><span data-stu-id="5dd72-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5dd72-135">请求</span><span class="sxs-lookup"><span data-stu-id="5dd72-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstancedecisionitem_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-5678-ae36-41b923c3bf87/decisions/filterByCurrentUser(on='reviewer')
```


### <a name="response"></a><span data-ttu-id="5dd72-136">响应</span><span class="sxs-lookup"><span data-stu-id="5dd72-136">Response</span></span>
><span data-ttu-id="5dd72-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5dd72-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewInstanceDecisionItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewInstanceDecisionItem)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
            "id": "139166ec-d214-4835-95aa-3c1d89581e51",
            "accessReviewId": "8d035c9d-798d-47fa-beb4-f986a4b8126f",
            "reviewedDateTime": "2021-05-03T19:28:25.02Z",
            "decision": "Approve",
            "justification": "Kathleen still needs access to the Marketing group as she works in the Marketing organization.",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "principalLink": "https://graph.microsoft.com/v1.0/users/1800bb2c-955d-4205-8471-3a6c3116435d",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "36c4c56e-fce3-4e2d-b28e-4ac0c7d2fa10",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "userDisplayName": "guest example",
                "userPrincipalName": "guest@guest.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "displayName": "guest example",
                "userPrincipalName": "guest@contoso.com"
            }
        }
    ]
}
```
