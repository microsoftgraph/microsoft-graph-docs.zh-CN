---
title: 列出 accessReviewInstance
description: 检索 accessReviewInstance 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 155c77e5a7b7fc8c81c5595dd2d504febd14673f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439190"
---
# <a name="list-accessreviewinstance"></a><span data-ttu-id="bfdc8-103">列出 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="bfdc8-103">List accessReviewInstance</span></span>

<span data-ttu-id="bfdc8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfdc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfdc8-105">检索 [特定 accessReviewScheduleDefinition 的 accessReviewInstance](../resources/accessreviewinstance.md) [对象](../resources/accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-105">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects for a specific [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="bfdc8-106">返回零个或多个 **accessReviewInstance** 对象的列表，包括所有嵌套属性。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-106">A list of zero or more **accessReviewInstance** objects are returned, including all of their nested properties.</span></span> <span data-ttu-id="bfdc8-107">返回的对象不包括关联的 accessReviewInstanceDecisionItems。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-107">Returned objects do not include associated accessReviewInstanceDecisionItems.</span></span> <span data-ttu-id="bfdc8-108">若要检索有关实例的决策，请使用 [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md)。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-108">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

>[!NOTE]
><span data-ttu-id="bfdc8-109">如果返回了许多 **accessReviewInstances，** 为了提高效率并避免超时，请检索页面中的 结果集，方法为在请求中同时包括页面大小最多为 100 的 $top 查询参数和 $skip=0 查询参数。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-109">If many **accessReviewInstances** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="bfdc8-110">当结果集多个页面时，Microsoft Graph 在响应中返回包含下一页结果 URL 的 @odata.nextLink 属性的页面。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-110">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="bfdc8-111">如果存在该属性，请在每个响应中继续使用 @odata.nextLink URL 提出其他请求，直到返回所有结果，如应用中分页 Microsoft Graph 数据中所述。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-111">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="bfdc8-112">如果未提供查询参数且结果超过 100 个，Microsoft Graph 将自动对结果进行分页，每页结果为 100 个。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-112">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfdc8-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="bfdc8-113">Permissions</span></span>
<span data-ttu-id="bfdc8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfdc8-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfdc8-116">Permission type</span></span>                        | <span data-ttu-id="bfdc8-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bfdc8-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfdc8-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfdc8-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="bfdc8-119">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfdc8-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="bfdc8-120">Application</span><span class="sxs-lookup"><span data-stu-id="bfdc8-120">Application</span></span>                            | <span data-ttu-id="bfdc8-121">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfdc8-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="bfdc8-122">登录用户还必须具有允许其读取访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-122">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="bfdc8-123">若要查看已登录用户分配审阅者的实例，请参阅 ["列出待处理的访问评审实例"](accessreviewinstance-pendingaccessreviewinstances.md)</span><span class="sxs-lookup"><span data-stu-id="bfdc8-123">To view just the instances that the signed-in user is assigned the reviewer on, see [List pending access review instances](accessreviewinstance-pendingaccessreviewinstances.md)</span></span>

## <a name="http-request"></a><span data-ttu-id="bfdc8-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfdc8-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances
```
## <a name="request-headers"></a><span data-ttu-id="bfdc8-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfdc8-125">Request headers</span></span>
<span data-ttu-id="bfdc8-126">无。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-126">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="bfdc8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfdc8-127">Request body</span></span>
<span data-ttu-id="bfdc8-128">不提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-128">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="bfdc8-129">响应</span><span class="sxs-lookup"><span data-stu-id="bfdc8-129">Response</span></span>
<span data-ttu-id="bfdc8-130">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [accessReviewInstance](../resources/accessreviewinstance.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-130">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bfdc8-131">示例</span><span class="sxs-lookup"><span data-stu-id="bfdc8-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="bfdc8-132">请求</span><span class="sxs-lookup"><span data-stu-id="bfdc8-132">Request</span></span>
<span data-ttu-id="bfdc8-133">以下示例显示检索定义的所有访问评审实例的请求。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-133">The following example shows a request to retrieve all the access review instances for a definition.</span></span>


# <a name="http"></a>[<span data-ttu-id="bfdc8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfdc8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04f34444/instances?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="bfdc8-135">C#</span><span class="sxs-lookup"><span data-stu-id="bfdc8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfdc8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfdc8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfdc8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfdc8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfdc8-138">Java</span><span class="sxs-lookup"><span data-stu-id="bfdc8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bfdc8-139">响应</span><span class="sxs-lookup"><span data-stu-id="bfdc8-139">Response</span></span>
><span data-ttu-id="bfdc8-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bfdc8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "12490cdb-6a18-4c08-ba2c-44442f0a0138",
            "startDateTime": "2020-09-21T20:03:36Z",
            "endDateTime": "2020-09-23T20:03:36Z",
            "status": "NotStarted",
            "scope": {
                "query": "/groups/b7a04444-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        },
        {
            "id": "64444761-b89f-4d9c-afb9-fcfc8bb9cf45",
            "startDateTime": "2020-09-14T20:03:36.74Z",
            "endDateTime": "2020-09-16T20:03:36.74Z",
            "status": "Completed",
            "scope": {
                "query": "/groups/b7a04444-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="bfdc8-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bfdc8-142">See also</span></span>

- [<span data-ttu-id="bfdc8-143">列出 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="bfdc8-143">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="bfdc8-144">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="bfdc8-144">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
