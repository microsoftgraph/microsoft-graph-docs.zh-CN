---
title: 列出 accessReviewInstance
description: 检索 accessReviewInstance 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 52844146764ffb85be50a9c8d8609b466a88ba2e
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030522"
---
# <a name="list-accessreviewinstance"></a><span data-ttu-id="31caf-103">列出 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="31caf-103">List accessReviewInstance</span></span>

<span data-ttu-id="31caf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31caf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31caf-105">检索特定[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)的[accessReviewInstance](../resources/accessreviewinstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="31caf-105">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects for a specific [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="31caf-106">返回零个或多个 **accessReviewInstance** 对象的列表，包括其所有嵌套属性。</span><span class="sxs-lookup"><span data-stu-id="31caf-106">A list of zero or more **accessReviewInstance** objects are returned, including all of their nested properties.</span></span> <span data-ttu-id="31caf-107">返回的对象不包括关联的 accessReviewInstanceDecisionItems。</span><span class="sxs-lookup"><span data-stu-id="31caf-107">Returned objects do not include associated accessReviewInstanceDecisionItems.</span></span> <span data-ttu-id="31caf-108">若要检索有关实例的决策，请使用 [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md)。</span><span class="sxs-lookup"><span data-stu-id="31caf-108">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

>[!NOTE]
><span data-ttu-id="31caf-109">此 API 的默认页面大小为 100 accessReviewInstance 对象。</span><span class="sxs-lookup"><span data-stu-id="31caf-109">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="31caf-110">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="31caf-110">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="31caf-111">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="31caf-111">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="31caf-112">权限</span><span class="sxs-lookup"><span data-stu-id="31caf-112">Permissions</span></span>
<span data-ttu-id="31caf-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31caf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31caf-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="31caf-115">Permission type</span></span>                        | <span data-ttu-id="31caf-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31caf-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="31caf-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31caf-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="31caf-118">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31caf-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="31caf-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="31caf-119">Application</span></span>                            | <span data-ttu-id="31caf-120">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31caf-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="31caf-121">登录用户还必须具有允许其读取访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="31caf-121">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="31caf-122">若要查看仅向已登录用户分配审阅者的实例，请参阅列出待处理 [的访问评审实例](accessreviewinstance-pendingaccessreviewinstances.md)</span><span class="sxs-lookup"><span data-stu-id="31caf-122">To view just the instances that the signed-in user is assigned the reviewer on, see [List pending access review instances](accessreviewinstance-pendingaccessreviewinstances.md)</span></span>

## <a name="http-request"></a><span data-ttu-id="31caf-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31caf-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31caf-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="31caf-124">Optional query parameters</span></span>
<span data-ttu-id="31caf-125">此方法支持 `$select` 、 、 、 和 OData 查询参数 `$filter` `$orderBy` `$skip` `$top` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="31caf-125">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="31caf-126">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="31caf-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="31caf-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="31caf-127">Request headers</span></span>
<span data-ttu-id="31caf-128">无。</span><span class="sxs-lookup"><span data-stu-id="31caf-128">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="31caf-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="31caf-129">Request body</span></span>
<span data-ttu-id="31caf-130">不提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="31caf-130">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="31caf-131">响应</span><span class="sxs-lookup"><span data-stu-id="31caf-131">Response</span></span>
<span data-ttu-id="31caf-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstance](../resources/accessreviewinstance.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="31caf-132">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31caf-133">示例</span><span class="sxs-lookup"><span data-stu-id="31caf-133">Examples</span></span>
### <a name="request"></a><span data-ttu-id="31caf-134">请求</span><span class="sxs-lookup"><span data-stu-id="31caf-134">Request</span></span>
<span data-ttu-id="31caf-135">以下示例显示检索定义的所有访问评审实例的请求。</span><span class="sxs-lookup"><span data-stu-id="31caf-135">The following example shows a request to retrieve all the access review instances for a definition.</span></span>


# <a name="http"></a>[<span data-ttu-id="31caf-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="31caf-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="31caf-137">C#</span><span class="sxs-lookup"><span data-stu-id="31caf-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31caf-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31caf-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31caf-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31caf-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31caf-140">Java</span><span class="sxs-lookup"><span data-stu-id="31caf-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="31caf-141">响应</span><span class="sxs-lookup"><span data-stu-id="31caf-141">Response</span></span>
><span data-ttu-id="31caf-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="31caf-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('8564a649-4f67-4e09-88e7-55def6530e88')/instances",
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
        },
        {
            "id": "f1f35945-3f42-4941-9f7b-465e545f6f99",
            "startDateTime": "2021-03-09T23:10:28.83Z",
            "endDateTime": "2021-03-09T23:10:28.83Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/f4ac55b3-3b3c-417e-85bd-183bbda3ccf2/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="31caf-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="31caf-143">See also</span></span>

- [<span data-ttu-id="31caf-144">列出 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="31caf-144">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="31caf-145">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="31caf-145">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


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
