---
title: accessReviewInstance：filterByCurrentUser
description: 检索给定审阅者的所有 accessReviewInstance 对象。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: eefc7b1fe375dbc9712cf342b9d68e1a13c9b315
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031072"
---
# <a name="accessreviewinstance-filterbycurrentuser"></a><span data-ttu-id="8c449-103">accessReviewInstance：filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="8c449-103">accessReviewInstance: filterByCurrentUser</span></span>
<span data-ttu-id="8c449-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c449-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c449-105">检索给定[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)上的所有[accessReviewInstance](../resources/accessreviewinstance.md)对象，其中调用用户是一个或多个[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)对象的审阅者。</span><span class="sxs-lookup"><span data-stu-id="8c449-105">Retrieve all [accessReviewInstance](../resources/accessreviewinstance.md) objects on a given [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) where the calling user is a reviewer on one or more [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects.</span></span>

>[!NOTE]
><span data-ttu-id="8c449-106">此 API 的默认页面大小为 100 accessReviewInstance 对象。</span><span class="sxs-lookup"><span data-stu-id="8c449-106">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="8c449-107">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="8c449-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="8c449-108">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="8c449-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c449-109">权限</span><span class="sxs-lookup"><span data-stu-id="8c449-109">Permissions</span></span>
<span data-ttu-id="8c449-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c449-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c449-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c449-112">Permission type</span></span>|<span data-ttu-id="8c449-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c449-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c449-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c449-114">Delegated (work or school account)</span></span>|<span data-ttu-id="8c449-115">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c449-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="8c449-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c449-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c449-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c449-117">Not supported.</span></span>|
|<span data-ttu-id="8c449-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c449-118">Application</span></span>|<span data-ttu-id="8c449-119">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c449-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c449-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c449-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c449-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8c449-121">Optional query parameters</span></span>
<span data-ttu-id="8c449-122">此方法支持 `$select` 、 、 、 和 OData 查询参数 `$filter` `$orderBy` `$skip` `$top` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8c449-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="8c449-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="8c449-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c449-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c449-124">Request headers</span></span>
|<span data-ttu-id="8c449-125">名称</span><span class="sxs-lookup"><span data-stu-id="8c449-125">Name</span></span>|<span data-ttu-id="8c449-126">说明</span><span class="sxs-lookup"><span data-stu-id="8c449-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8c449-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c449-127">Authorization</span></span>|<span data-ttu-id="8c449-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8c449-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c449-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c449-130">Request body</span></span>
<span data-ttu-id="8c449-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8c449-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c449-132">响应</span><span class="sxs-lookup"><span data-stu-id="8c449-132">Response</span></span>

<span data-ttu-id="8c449-133">如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [accessReviewInstance](../resources/accessreviewinstance.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="8c449-133">If successful, this function returns a `200 OK` response code and a [accessReviewInstance](../resources/accessreviewinstance.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c449-134">示例</span><span class="sxs-lookup"><span data-stu-id="8c449-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c449-135">请求</span><span class="sxs-lookup"><span data-stu-id="8c449-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/filterByCurrentUser(on='reviewer')
```


### <a name="response"></a><span data-ttu-id="8c449-136">响应</span><span class="sxs-lookup"><span data-stu-id="8c449-136">Response</span></span>
><span data-ttu-id="8c449-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8c449-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(accessReviewInstance)",
    "@odata.count": 1,
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
        }
    ]
}
```
