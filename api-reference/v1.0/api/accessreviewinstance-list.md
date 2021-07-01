---
title: 列出 accessReviewInstances
description: 获取 accessReviewInstance 对象及其属性的列表。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 60b5ba7e35acfb72f033f90cd37d4fd32c8a3d8b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210575"
---
# <a name="list-accessreviewinstances"></a><span data-ttu-id="7daab-103">列出 accessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="7daab-103">List accessReviewInstances</span></span>
<span data-ttu-id="7daab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7daab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7daab-105">获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="7daab-105">Get a list of the [accessReviewInstance](../resources/accessreviewinstance.md) objects and their properties.</span></span>

>[!NOTE]
><span data-ttu-id="7daab-106">此 API 的默认页面大小为 100 accessReviewScheduleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="7daab-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="7daab-107">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="7daab-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="7daab-108">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="7daab-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="7daab-109">权限</span><span class="sxs-lookup"><span data-stu-id="7daab-109">Permissions</span></span>
<span data-ttu-id="7daab-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7daab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7daab-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7daab-112">Permission type</span></span>|<span data-ttu-id="7daab-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7daab-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7daab-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7daab-114">Delegated (work or school account)</span></span>|<span data-ttu-id="7daab-115">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7daab-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="7daab-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7daab-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7daab-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7daab-117">Not supported.</span></span>|
|<span data-ttu-id="7daab-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7daab-118">Application</span></span>|<span data-ttu-id="7daab-119">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7daab-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7daab-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7daab-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7daab-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7daab-121">Optional query parameters</span></span>
<span data-ttu-id="7daab-122">此方法支持 `$select` 、 、 、 和 OData 查询参数 `$filter` `$orderBy` `$skip` `$top` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7daab-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="7daab-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7daab-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7daab-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="7daab-124">Request headers</span></span>
|<span data-ttu-id="7daab-125">名称</span><span class="sxs-lookup"><span data-stu-id="7daab-125">Name</span></span>|<span data-ttu-id="7daab-126">说明</span><span class="sxs-lookup"><span data-stu-id="7daab-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7daab-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7daab-127">Authorization</span></span>|<span data-ttu-id="7daab-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7daab-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7daab-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="7daab-130">Request body</span></span>
<span data-ttu-id="7daab-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7daab-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7daab-132">响应</span><span class="sxs-lookup"><span data-stu-id="7daab-132">Response</span></span>

<span data-ttu-id="7daab-133">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstance](../resources/accessreviewinstance.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7daab-133">If successful, this method returns a `200 OK` response code and a collection of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7daab-134">示例</span><span class="sxs-lookup"><span data-stu-id="7daab-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7daab-135">请求</span><span class="sxs-lookup"><span data-stu-id="7daab-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7daab-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7daab-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstance"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances
```
# <a name="c"></a>[<span data-ttu-id="7daab-137">C#</span><span class="sxs-lookup"><span data-stu-id="7daab-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7daab-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7daab-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7daab-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7daab-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7daab-140">Java</span><span class="sxs-lookup"><span data-stu-id="7daab-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7daab-141">响应</span><span class="sxs-lookup"><span data-stu-id="7daab-141">Response</span></span>
><span data-ttu-id="7daab-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7daab-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('8564a649-4f67-4e09-88e7-55def6530e88')/instances",
    "@odata.count": 2,
    "value": [
        {
            "id": "7bc18cf4-3d70-4009-bc8e-a7c5adb30849",
            "startDateTime": "2021-03-09T23:10:28.83Z",
            "endDateTime": "2021-03-09T23:10:28.83Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/f661fdd0-f0f7-42c0-8281-e89c6527ac63/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        }
    ]
}
```
