---
title: accessReviewInstance：filterByCurrentUser
description: 返回给定审阅者的所有 accessReviewInstance 对象。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 67d2ae1c3a2abafe16d519e9cb5a3f1035b6e23a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207608"
---
# <a name="accessreviewinstance-filterbycurrentuser"></a><span data-ttu-id="e14e6-103">accessReviewInstance：filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="e14e6-103">accessReviewInstance: filterByCurrentUser</span></span>
<span data-ttu-id="e14e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e14e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e14e6-105">返回给定[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)上的所有[accessReviewInstance](../resources/accessreviewinstance.md)对象，其中调用用户是一个或多个[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)对象的审阅者。</span><span class="sxs-lookup"><span data-stu-id="e14e6-105">Returns all [accessReviewInstance](../resources/accessreviewinstance.md) objects on a given [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) where the calling user is a reviewer on one or more [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects.</span></span>

>[!NOTE]
><span data-ttu-id="e14e6-106">此 API 的默认页面大小为 100 accessReviewInstance 对象。</span><span class="sxs-lookup"><span data-stu-id="e14e6-106">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="e14e6-107">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="e14e6-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="e14e6-108">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="e14e6-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="e14e6-109">权限</span><span class="sxs-lookup"><span data-stu-id="e14e6-109">Permissions</span></span>
<span data-ttu-id="e14e6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e14e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e14e6-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e14e6-112">Permission type</span></span>|<span data-ttu-id="e14e6-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e14e6-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e14e6-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e14e6-114">Delegated (work or school account)</span></span>|<span data-ttu-id="e14e6-115">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e14e6-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="e14e6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e14e6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e14e6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e14e6-117">Not supported.</span></span>|
|<span data-ttu-id="e14e6-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e14e6-118">Application</span></span>|<span data-ttu-id="e14e6-119">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e14e6-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e14e6-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e14e6-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e14e6-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e14e6-121">Optional query parameters</span></span>
<span data-ttu-id="e14e6-122">此方法支持 `$select` 、 `$filter` `$orderBy` 、 和 `$skip` `$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e14e6-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="e14e6-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e14e6-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e14e6-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="e14e6-124">Request headers</span></span>
|<span data-ttu-id="e14e6-125">名称</span><span class="sxs-lookup"><span data-stu-id="e14e6-125">Name</span></span>|<span data-ttu-id="e14e6-126">说明</span><span class="sxs-lookup"><span data-stu-id="e14e6-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e14e6-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e14e6-127">Authorization</span></span>|<span data-ttu-id="e14e6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e14e6-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e14e6-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e14e6-130">Request body</span></span>
<span data-ttu-id="e14e6-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e14e6-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e14e6-132">响应</span><span class="sxs-lookup"><span data-stu-id="e14e6-132">Response</span></span>

<span data-ttu-id="e14e6-133">如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [accessReviewInstance](../resources/accessreviewinstance.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="e14e6-133">If successful, this function returns a `200 OK` response code and a [accessReviewInstance](../resources/accessreviewinstance.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e14e6-134">示例</span><span class="sxs-lookup"><span data-stu-id="e14e6-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e14e6-135">请求</span><span class="sxs-lookup"><span data-stu-id="e14e6-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e14e6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e14e6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/08531375-eff6-4e21-b1a8-de0eb37ec913/instances/filterByCurrentUser(on='reviewer')
```
# <a name="c"></a>[<span data-ttu-id="e14e6-137">C#</span><span class="sxs-lookup"><span data-stu-id="e14e6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e14e6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e14e6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e14e6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e14e6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e14e6-140">Java</span><span class="sxs-lookup"><span data-stu-id="e14e6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e14e6-141">响应</span><span class="sxs-lookup"><span data-stu-id="e14e6-141">Response</span></span>
><span data-ttu-id="e14e6-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e14e6-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
