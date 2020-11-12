---
title: 列出 accessReviewInstanceDecisionItem 待审批
description: 检索由呼叫用户等待审批的 accessReviewInstanceDecisionItem 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e245d58966b1fa6e206dff1c7a29f38a3146ac21
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000759"
---
# <a name="list-accessreviewinstancedecisionitems-pending-approval"></a><span data-ttu-id="21cce-103">列出 accessReviewInstanceDecisionItems 待审批</span><span class="sxs-lookup"><span data-stu-id="21cce-103">List accessReviewInstanceDecisionItems pending approval</span></span>

<span data-ttu-id="21cce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21cce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21cce-105">检索由呼叫用户等待审批的特定[accessReviewInstance](../resources/accessreviewscheduledefinition.md)的[accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="21cce-105">Retrieve the [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects for a specific [accessReviewInstance](../resources/accessreviewscheduledefinition.md) pending approval by the calling user.</span></span> <span data-ttu-id="21cce-106">返回零个或多个 accessReviewInstanceDecisionItem 对象的列表，包括它们的所有嵌套属性。</span><span class="sxs-lookup"><span data-stu-id="21cce-106">A list of zero or more accessReviewInstanceDecisionItem objects are returned, including all of their nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="21cce-107">如果返回多个 **accessReviewInstanceDecisionItems** ，则要提高效率并避免超时，请在页面中检索结果集，方法是在页面大小最多为100的情况下包括 $top 查询参数以及请求中的 $skip = 0 查询参数。</span><span class="sxs-lookup"><span data-stu-id="21cce-107">If many **accessReviewInstanceDecisionItems** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="21cce-108">当结果集跨越多个页面时，Microsoft Graph 将在包含指向结果下一页的 URL 的响应中的 nextLink 属性返回该页面，其中包含一个 @odata。</span><span class="sxs-lookup"><span data-stu-id="21cce-108">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="21cce-109">如果该属性存在，则继续在每个响应中 @odata 使用 nextLink URL 进行额外请求，直到返回所有结果，如您的应用程序中分页 Microsoft Graph 数据中所述。</span><span class="sxs-lookup"><span data-stu-id="21cce-109">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="21cce-110">如果未提供查询参数，且结果多于100，则 Microsoft Graph 将自动对结果进行分页，每页100个结果。</span><span class="sxs-lookup"><span data-stu-id="21cce-110">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="21cce-111">权限</span><span class="sxs-lookup"><span data-stu-id="21cce-111">Permissions</span></span>
<span data-ttu-id="21cce-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21cce-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21cce-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="21cce-114">Permission type</span></span>                        | <span data-ttu-id="21cce-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="21cce-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="21cce-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21cce-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="21cce-117">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="21cce-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="21cce-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21cce-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21cce-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="21cce-119">Not supported.</span></span>|

<span data-ttu-id="21cce-120">登录用户还将仅在该决策的 instance's accessReviewScheduleDefinition 中查看为其分配了审阅者的决定。</span><span class="sxs-lookup"><span data-stu-id="21cce-120">The signed-in user will also only see decisions of which they are assigned reviewer in that decision's instance's accessReviewScheduleDefinition.</span></span>

## <a name="http-request"></a><span data-ttu-id="21cce-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21cce-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances/{instance-id}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="21cce-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="21cce-122">Request headers</span></span>
<span data-ttu-id="21cce-123">无。</span><span class="sxs-lookup"><span data-stu-id="21cce-123">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="21cce-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="21cce-124">Request body</span></span>
<span data-ttu-id="21cce-125">请勿提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="21cce-125">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="21cce-126">响应</span><span class="sxs-lookup"><span data-stu-id="21cce-126">Response</span></span>
<span data-ttu-id="21cce-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) 对象的数组。</span><span class="sxs-lookup"><span data-stu-id="21cce-127">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="21cce-128">示例</span><span class="sxs-lookup"><span data-stu-id="21cce-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="21cce-129">请求</span><span class="sxs-lookup"><span data-stu-id="21cce-129">Request</span></span>
<span data-ttu-id="21cce-130">下面的示例演示了一个请求，以检索对 access 评审实例的所有决策，以等待调用用户的批准。</span><span class="sxs-lookup"><span data-stu-id="21cce-130">The following example shows a request to retrieve all the decisions on an instance of an access review pending the calling user's approval.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions?$top=100&$skip=0
```

---


### <a name="response"></a><span data-ttu-id="21cce-131">响应</span><span class="sxs-lookup"><span data-stu-id="21cce-131">Response</span></span>
><span data-ttu-id="21cce-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="21cce-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
                "userPrincipalName": "AdeleV@microsoft.com"
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
                "userPrincipalName": "admin@microsoft.com"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="21cce-134">另请参阅</span><span class="sxs-lookup"><span data-stu-id="21cce-134">See also</span></span>

- [<span data-ttu-id="21cce-135">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="21cce-135">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="21cce-136">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="21cce-136">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


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
