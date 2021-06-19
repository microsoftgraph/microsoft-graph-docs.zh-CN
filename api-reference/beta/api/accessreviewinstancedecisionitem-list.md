---
title: 列出 accessReviewInstanceDecisionItem
description: 检索 accessReviewInstanceDecisionItem 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a89f6a1bc91f2449a280fe3bfcfaab918cd92e16
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030430"
---
# <a name="list-accessreviewinstancedecisionitem"></a><span data-ttu-id="f20f0-103">列出 accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="f20f0-103">List accessReviewInstanceDecisionItem</span></span>

<span data-ttu-id="f20f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f20f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f20f0-105">检索 [特定 accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的 [AccessReviewInstance](../resources/accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="f20f0-105">Retrieve the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects for a specific [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="f20f0-106">返回零个或多个 accessReviewInstanceDecisionItem 对象的列表，包括其所有嵌套属性。</span><span class="sxs-lookup"><span data-stu-id="f20f0-106">A list of zero or more accessReviewInstanceDecisionItem objects are returned, including all of their nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="f20f0-107">此 API 的默认页面大小为 100 accessReviewInstanceDecisionItem 对象。</span><span class="sxs-lookup"><span data-stu-id="f20f0-107">The default page size for this API is 100 accessReviewInstanceDecisionItem objects.</span></span> <span data-ttu-id="f20f0-108">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="f20f0-108">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="f20f0-109">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="f20f0-109">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="f20f0-110">权限</span><span class="sxs-lookup"><span data-stu-id="f20f0-110">Permissions</span></span>
<span data-ttu-id="f20f0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f20f0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f20f0-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="f20f0-113">Permission type</span></span>                        | <span data-ttu-id="f20f0-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f20f0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f20f0-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f20f0-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="f20f0-116">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f20f0-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="f20f0-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f20f0-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f20f0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f20f0-118">Not supported.</span></span>|
|<span data-ttu-id="f20f0-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="f20f0-119">Application</span></span>                            | <span data-ttu-id="f20f0-120">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f20f0-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="f20f0-121">登录用户还必须具有允许其读取访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="f20f0-121">The signed-in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="f20f0-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f20f0-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/decisions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f20f0-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f20f0-123">Optional query parameters</span></span>
<span data-ttu-id="f20f0-124">此方法支持 `$select` 、 、 、 和 OData 查询参数 `$filter` `$orderBy` `$skip` `$top` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f20f0-124">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="f20f0-125">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f20f0-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f20f0-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="f20f0-126">Request headers</span></span>
<span data-ttu-id="f20f0-127">无。</span><span class="sxs-lookup"><span data-stu-id="f20f0-127">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="f20f0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f20f0-128">Request body</span></span>
<span data-ttu-id="f20f0-129">不提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="f20f0-129">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="f20f0-130">响应</span><span class="sxs-lookup"><span data-stu-id="f20f0-130">Response</span></span>
<span data-ttu-id="f20f0-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="f20f0-131">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f20f0-132">示例</span><span class="sxs-lookup"><span data-stu-id="f20f0-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="f20f0-133">请求</span><span class="sxs-lookup"><span data-stu-id="f20f0-133">Request</span></span>
<span data-ttu-id="f20f0-134">以下示例显示检索有关访问评审实例的所有决策的请求。</span><span class="sxs-lookup"><span data-stu-id="f20f0-134">The following example shows a request to retrieve all the decisions on an instance of an access review.</span></span>


# <a name="http"></a>[<span data-ttu-id="f20f0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f20f0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/14444cdb-6a18-4c08-ba2c-48c02f0a0138/decisions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="f20f0-136">C#</span><span class="sxs-lookup"><span data-stu-id="f20f0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f20f0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f20f0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f20f0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f20f0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f20f0-139">Java</span><span class="sxs-lookup"><span data-stu-id="f20f0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="f20f0-140">响应</span><span class="sxs-lookup"><span data-stu-id="f20f0-140">Response</span></span>
><span data-ttu-id="f20f0-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f20f0-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0')/instances('6444d4fd-ab55-4608-8cf9-c6702d172bcc')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "e6cafba0-cbf0-4748-8868-0810c7f4cc06",
            "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
                "userDisplayName": "Diego Siciliani",
                "userPrincipalName": "DiegoS@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
                "displayName": "Diego Siciliani",
                "userPrincipalName": "DiegoS@contoso.com"
            }
        },
        {
            "id": "4bde8d40-9224-4aa3-936b-08d73e1baf47",
            "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/11feb738-0039-4a6c-a045-dcb91a47969a",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "11feb738-0039-4a6c-a045-dcb91a47969a",
                "userDisplayName": "Johanna Lorenz",
                "userPrincipalName": "JohannaL@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "11feb738-0039-4a6c-a045-dcb91a47969a",
                "displayName": "Johanna Lorenz",
                "userPrincipalName": "JohannaL@contoso.com"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="f20f0-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f20f0-142">See also</span></span>

- [<span data-ttu-id="f20f0-143">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="f20f0-143">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="f20f0-144">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="f20f0-144">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstanceDecisionItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
