---
title: 列出 accessReviewInstance
description: 检索 accessReviewInstance 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 844564c383b065adc80672cad727807cbb590ca7
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000810"
---
# <a name="list-accessreviewinstance"></a><span data-ttu-id="4e6c0-103">列出 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="4e6c0-103">List accessReviewInstance</span></span>

<span data-ttu-id="4e6c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e6c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e6c0-105">检索特定[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)的[accessReviewInstance](../resources/accessreviewinstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-105">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects for a specific [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="4e6c0-106">返回零个或多个 **accessReviewInstance** 对象的列表，包括它们的所有嵌套属性。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-106">A list of zero or more **accessReviewInstance** objects are returned, including all of their nested properties.</span></span> <span data-ttu-id="4e6c0-107">返回的对象不包含关联的 accessReviewInstanceDecisionItems。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-107">Returned objects do not include associated accessReviewInstanceDecisionItems.</span></span> <span data-ttu-id="4e6c0-108">若要检索有关实例的决策，请使用 [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md)。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-108">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

>[!NOTE]
><span data-ttu-id="4e6c0-109">如果返回多个 **accessReviewInstances** ，则要提高效率并避免超时，请在页面中检索结果集，方法是在页面大小最多为100的情况下包括 $top 查询参数以及请求中的 $skip = 0 查询参数。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-109">If many **accessReviewInstances** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="4e6c0-110">当结果集跨越多个页面时，Microsoft Graph 将在包含指向结果下一页的 URL 的响应中的 nextLink 属性返回该页面，其中包含一个 @odata。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-110">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="4e6c0-111">如果该属性存在，则继续在每个响应中 @odata 使用 nextLink URL 进行额外请求，直到返回所有结果，如您的应用程序中分页 Microsoft Graph 数据中所述。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-111">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="4e6c0-112">如果未提供查询参数，且结果多于100，则 Microsoft Graph 将自动对结果进行分页，每页100个结果。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-112">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e6c0-113">权限</span><span class="sxs-lookup"><span data-stu-id="4e6c0-113">Permissions</span></span>
<span data-ttu-id="4e6c0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e6c0-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e6c0-116">Permission type</span></span>                        | <span data-ttu-id="4e6c0-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e6c0-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e6c0-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e6c0-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e6c0-119">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="4e6c0-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="4e6c0-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e6c0-120">Application</span></span>                            | <span data-ttu-id="4e6c0-121">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="4e6c0-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="4e6c0-122">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-122">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="4e6c0-123">若要仅查看已登录用户为其分配审阅者的实例，请参阅 [列出挂起的访问审核实例](accessreviewinstance-pendingaccessreviewinstances.md)</span><span class="sxs-lookup"><span data-stu-id="4e6c0-123">To view just the instances that the signed-in user is assigned the reviewer on, see [List pending access review instances](accessreviewinstance-pendingaccessreviewinstances.md)</span></span>

## <a name="http-request"></a><span data-ttu-id="4e6c0-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e6c0-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances
```
## <a name="request-headers"></a><span data-ttu-id="4e6c0-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e6c0-125">Request headers</span></span>
<span data-ttu-id="4e6c0-126">无。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-126">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="4e6c0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e6c0-127">Request body</span></span>
<span data-ttu-id="4e6c0-128">请勿提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-128">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="4e6c0-129">响应</span><span class="sxs-lookup"><span data-stu-id="4e6c0-129">Response</span></span>
<span data-ttu-id="4e6c0-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的数组。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-130">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4e6c0-131">示例</span><span class="sxs-lookup"><span data-stu-id="4e6c0-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="4e6c0-132">请求</span><span class="sxs-lookup"><span data-stu-id="4e6c0-132">Request</span></span>
<span data-ttu-id="4e6c0-133">下面的示例演示检索定义的所有访问评审实例的请求。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-133">The following example shows a request to retrieve all the access review instances for a definition.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04f34444/instances?$top=100&$skip=0
```

### <a name="response"></a><span data-ttu-id="4e6c0-134">响应</span><span class="sxs-lookup"><span data-stu-id="4e6c0-134">Response</span></span>
><span data-ttu-id="4e6c0-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4e6c0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4e6c0-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4e6c0-137">See also</span></span>

- [<span data-ttu-id="4e6c0-138">列出 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="4e6c0-138">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="4e6c0-139">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="4e6c0-139">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


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
