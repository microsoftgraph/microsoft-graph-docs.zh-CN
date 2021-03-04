---
title: 列出 accessReviewInstanceDecisionItem 待审批
description: 检索等待调用用户批准的 accessReviewInstanceDecisionItem 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 426abc674df2b14b19dee6ef838d3b7d5fe31a3c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439126"
---
# <a name="list-accessreviewinstancedecisionitems-pending-approval"></a><span data-ttu-id="7f89b-103">列出待审批的 accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="7f89b-103">List accessReviewInstanceDecisionItems pending approval</span></span>

<span data-ttu-id="7f89b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f89b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f89b-105">检索 [特定 accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) 对象的 [accessReviewInstance](../resources/accessreviewscheduledefinition.md) 等待调用用户批准。</span><span class="sxs-lookup"><span data-stu-id="7f89b-105">Retrieve the [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects for a specific [accessReviewInstance](../resources/accessreviewscheduledefinition.md) pending approval by the calling user.</span></span> <span data-ttu-id="7f89b-106">返回零个或多个 accessReviewInstanceDecisionItem 对象的列表，包括所有嵌套属性。</span><span class="sxs-lookup"><span data-stu-id="7f89b-106">A list of zero or more accessReviewInstanceDecisionItem objects are returned, including all of their nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="7f89b-107">如果返回了许多 **accessReviewInstanceDecisionItems，** 为了提高效率并避免超时，请检索页面中的 结果集，方法为在请求中同时包括页面大小最多为 100 的 $top 查询参数和 $skip=0 查询参数。</span><span class="sxs-lookup"><span data-stu-id="7f89b-107">If many **accessReviewInstanceDecisionItems** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="7f89b-108">当结果集多个页面时，Microsoft Graph 在响应中返回包含下一页结果 URL 的 @odata.nextLink 属性的页面。</span><span class="sxs-lookup"><span data-stu-id="7f89b-108">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="7f89b-109">如果存在该属性，请在每个响应中继续使用 @odata.nextLink URL 提出其他请求，直到返回所有结果，如应用中分页 Microsoft Graph 数据中所述。</span><span class="sxs-lookup"><span data-stu-id="7f89b-109">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="7f89b-110">如果未提供查询参数且结果超过 100 个，Microsoft Graph 将自动对结果进行分页，每页结果为 100 个。</span><span class="sxs-lookup"><span data-stu-id="7f89b-110">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f89b-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="7f89b-111">Permissions</span></span>
<span data-ttu-id="7f89b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f89b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f89b-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f89b-114">Permission type</span></span>                        | <span data-ttu-id="7f89b-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f89b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f89b-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f89b-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f89b-117">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f89b-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="7f89b-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f89b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f89b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f89b-119">Not supported.</span></span>|

<span data-ttu-id="7f89b-120">登录用户还将仅看到在决定实例的 accessReviewScheduleDefinition 中为其分配审阅者的决策。</span><span class="sxs-lookup"><span data-stu-id="7f89b-120">The signed-in user will also only see decisions of which they are assigned reviewer in that decision's instance's accessReviewScheduleDefinition.</span></span>

## <a name="http-request"></a><span data-ttu-id="7f89b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f89b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances/{instance-id}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="7f89b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f89b-122">Request headers</span></span>
<span data-ttu-id="7f89b-123">无。</span><span class="sxs-lookup"><span data-stu-id="7f89b-123">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="7f89b-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f89b-124">Request body</span></span>
<span data-ttu-id="7f89b-125">不提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f89b-125">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="7f89b-126">响应</span><span class="sxs-lookup"><span data-stu-id="7f89b-126">Response</span></span>
<span data-ttu-id="7f89b-127">如果成功，此方法在响应正文中返回 `200 OK` [响应代码和 accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="7f89b-127">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7f89b-128">示例</span><span class="sxs-lookup"><span data-stu-id="7f89b-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="7f89b-129">请求</span><span class="sxs-lookup"><span data-stu-id="7f89b-129">Request</span></span>
<span data-ttu-id="7f89b-130">以下示例显示一个请求，请求检索有关访问评审实例的所有决策，等待呼叫用户的审批。</span><span class="sxs-lookup"><span data-stu-id="7f89b-130">The following example shows a request to retrieve all the decisions on an instance of an access review pending the calling user's approval.</span></span>


# <a name="http"></a>[<span data-ttu-id="7f89b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f89b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="7f89b-132">C#</span><span class="sxs-lookup"><span data-stu-id="7f89b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f89b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f89b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f89b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f89b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f89b-135">Java</span><span class="sxs-lookup"><span data-stu-id="7f89b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="7f89b-136">响应</span><span class="sxs-lookup"><span data-stu-id="7f89b-136">Response</span></span>
><span data-ttu-id="7f89b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7f89b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.count": 2,
    "value": [
        {
            "id": "654b34e7-b48f-4772-a2d4-08f1d0dd014c",
            "accessReviewId": "70a68410-67f3-4d4c-b946-6989e050be19",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
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
                "userId": "7eae986b-d425-48b2-adf2-3c777f6256f3",
                "userDisplayName": "Adele Vance",
                "userPrincipalName": "AdeleV@contoso.com"
            }
        },
        {
            "id": "0311dba4-c60c-412e-ac77-14e1da23daf1",
            "accessReviewId": "70a68410-67f3-4d4c-b946-6989e050be19",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
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
                "userId": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "userDisplayName": "MOD Administrator",
                "userPrincipalName": "admin@contoso.com"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="7f89b-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7f89b-139">See also</span></span>

- [<span data-ttu-id="7f89b-140">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="7f89b-140">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="7f89b-141">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="7f89b-141">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstanceDecisionItem pendingApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
