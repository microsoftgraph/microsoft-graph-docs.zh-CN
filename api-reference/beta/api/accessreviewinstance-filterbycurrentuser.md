---
title: accessReviewInstance：filterByCurrentUser
description: 返回给定审阅者的所有 accessReviewInstance 对象。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: db6de64071645fe97d5fffa4e3968ea63db5578e
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031444"
---
# <a name="accessreviewinstance-filterbycurrentuser"></a><span data-ttu-id="0cb72-103">accessReviewInstance：filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="0cb72-103">accessReviewInstance: filterByCurrentUser</span></span>
<span data-ttu-id="0cb72-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cb72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cb72-105">返回给定[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)上的所有[accessReviewInstance](../resources/accessreviewinstance.md)对象，其中调用用户是一个或多个[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)对象的审阅者。</span><span class="sxs-lookup"><span data-stu-id="0cb72-105">Returns all [accessReviewInstance](../resources/accessreviewinstance.md) objects on a given [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) where the calling user is a reviewer on one or more [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects.</span></span>

>[!NOTE]
><span data-ttu-id="0cb72-106">此 API 的默认页面大小为 100 accessReviewInstance 对象。</span><span class="sxs-lookup"><span data-stu-id="0cb72-106">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="0cb72-107">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="0cb72-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="0cb72-108">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="0cb72-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="0cb72-109">权限</span><span class="sxs-lookup"><span data-stu-id="0cb72-109">Permissions</span></span>
<span data-ttu-id="0cb72-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0cb72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cb72-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0cb72-112">Permission type</span></span>|<span data-ttu-id="0cb72-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0cb72-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cb72-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0cb72-114">Delegated (work or school account)</span></span>|<span data-ttu-id="0cb72-115">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cb72-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="0cb72-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0cb72-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cb72-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cb72-117">Not supported.</span></span>|
|<span data-ttu-id="0cb72-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0cb72-118">Application</span></span>|<span data-ttu-id="0cb72-119">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cb72-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cb72-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0cb72-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0cb72-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0cb72-121">Optional query parameters</span></span>
<span data-ttu-id="0cb72-122">此方法支持 `$select` 、 `$filter` `$orderBy` 、 和 `$skip` `$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0cb72-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="0cb72-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0cb72-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0cb72-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="0cb72-124">Request headers</span></span>
|<span data-ttu-id="0cb72-125">名称</span><span class="sxs-lookup"><span data-stu-id="0cb72-125">Name</span></span>|<span data-ttu-id="0cb72-126">说明</span><span class="sxs-lookup"><span data-stu-id="0cb72-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0cb72-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cb72-127">Authorization</span></span>|<span data-ttu-id="0cb72-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0cb72-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cb72-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="0cb72-130">Request body</span></span>
<span data-ttu-id="0cb72-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0cb72-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cb72-132">响应</span><span class="sxs-lookup"><span data-stu-id="0cb72-132">Response</span></span>

<span data-ttu-id="0cb72-133">如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [accessReviewInstance](../resources/accessreviewinstance.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="0cb72-133">If successful, this function returns a `200 OK` response code and a [accessReviewInstance](../resources/accessreviewinstance.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0cb72-134">示例</span><span class="sxs-lookup"><span data-stu-id="0cb72-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0cb72-135">请求</span><span class="sxs-lookup"><span data-stu-id="0cb72-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/08531375-eff6-4e21-b1a8-de0eb37ec913/instances/filterByCurrentUser(on='reviewer')
```

### <a name="response"></a><span data-ttu-id="0cb72-136">响应</span><span class="sxs-lookup"><span data-stu-id="0cb72-136">Response</span></span>
><span data-ttu-id="0cb72-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0cb72-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewInstance)",
    "@odata.count": 2,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstance",
            "id": "7ca879f0-77ea-4386-b110-776dec898935",
            "startDateTime": "2021-04-20T00:45:51.627Z",
            "endDateTime": "2021-04-23T00:45:51.627Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/6b7b9930-38a0-4f93-a107-3bc9904c83d7/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        },
        {
            "@odata.type": "#microsoft.graph.accessReviewInstance",
            "id": "00ef5dba-4a32-48b3-b18a-57b244c0c4ba",
            "startDateTime": "2021-04-13T00:45:51.627Z",
            "endDateTime": "2021-04-16T00:45:51.627Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/6b7b9930-38a0-4f93-a107-3bc9904c83d7/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        }
    ]
}
```
