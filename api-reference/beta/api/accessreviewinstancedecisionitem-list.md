---
title: 列出 accessReviewInstanceDecisionItem
description: 检索 accessReviewInstanceDecisionItem 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aa7389c8779d667d401f6f7ca421ea0d405d5d33
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000806"
---
# <a name="list-accessreviewinstancedecisionitem"></a><span data-ttu-id="aae02-103">列出 accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="aae02-103">List accessReviewInstanceDecisionItem</span></span>

<span data-ttu-id="aae02-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aae02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aae02-105">检索特定[accessReviewInstance](../resources/accessreviewinstance.md)的[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aae02-105">Retrieve the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects for a specific [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="aae02-106">返回零个或多个 accessReviewInstanceDecisionItem 对象的列表，包括它们的所有嵌套属性。</span><span class="sxs-lookup"><span data-stu-id="aae02-106">A list of zero or more accessReviewInstanceDecisionItem objects are returned, including all of their nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="aae02-107">如果返回多个 **accessReviewInstanceDecisionItems** ，则要提高效率并避免超时，请在页面中检索结果集，方法是在页面大小最多为100的情况下包括 $top 查询参数以及请求中的 $skip = 0 查询参数。</span><span class="sxs-lookup"><span data-stu-id="aae02-107">If many **accessReviewInstanceDecisionItems** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="aae02-108">当结果集跨越多个页面时，Microsoft Graph 将在包含指向结果下一页的 URL 的响应中的 nextLink 属性返回该页面，其中包含一个 @odata。</span><span class="sxs-lookup"><span data-stu-id="aae02-108">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="aae02-109">如果该属性存在，则继续在每个响应中 @odata 使用 nextLink URL 进行额外请求，直到返回所有结果，如您的应用程序中分页 Microsoft Graph 数据中所述。</span><span class="sxs-lookup"><span data-stu-id="aae02-109">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="aae02-110">如果未提供查询参数，且结果多于100，则 Microsoft Graph 将自动对结果进行分页，每页100个结果。</span><span class="sxs-lookup"><span data-stu-id="aae02-110">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="aae02-111">权限</span><span class="sxs-lookup"><span data-stu-id="aae02-111">Permissions</span></span>
<span data-ttu-id="aae02-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aae02-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aae02-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="aae02-114">Permission type</span></span>                        | <span data-ttu-id="aae02-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aae02-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="aae02-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aae02-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="aae02-117">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="aae02-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="aae02-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aae02-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aae02-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="aae02-119">Not supported.</span></span>|
|<span data-ttu-id="aae02-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="aae02-120">Application</span></span>                            | <span data-ttu-id="aae02-121">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="aae02-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="aae02-122">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="aae02-122">The signed-in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="aae02-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aae02-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="aae02-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="aae02-124">Request headers</span></span>
<span data-ttu-id="aae02-125">无。</span><span class="sxs-lookup"><span data-stu-id="aae02-125">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="aae02-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aae02-126">Request body</span></span>
<span data-ttu-id="aae02-127">请勿提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="aae02-127">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="aae02-128">响应</span><span class="sxs-lookup"><span data-stu-id="aae02-128">Response</span></span>
<span data-ttu-id="aae02-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) 对象的数组。</span><span class="sxs-lookup"><span data-stu-id="aae02-129">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aae02-130">示例</span><span class="sxs-lookup"><span data-stu-id="aae02-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="aae02-131">请求</span><span class="sxs-lookup"><span data-stu-id="aae02-131">Request</span></span>
<span data-ttu-id="aae02-132">下面的示例演示了一个请求，以检索对 access 评审实例的所有决策。</span><span class="sxs-lookup"><span data-stu-id="aae02-132">The following example shows a request to retrieve all the decisions on an instance of an access review.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/14444cdb-6a18-4c08-ba2c-48c02f0a0138/decisions?$top=100&$skip=0
```

---

### <a name="response"></a><span data-ttu-id="aae02-133">响应</span><span class="sxs-lookup"><span data-stu-id="aae02-133">Response</span></span>
><span data-ttu-id="aae02-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aae02-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.count": 4,
    "value": [
        {
            "id": "77a61af9-3bef-4bbf-b00b-04734d6d5eae",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
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
                "userId": "3736c87b-dc21-4290-8802-d6fef5fa3a08",
                "userDisplayName": "Irvin Sayers",
                "userPrincipalName": "IrvinS@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "f30b68ef-b843-4479-86b8-0a3a2f4bb209",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:08.377Z",
            "decision": "Approve",
            "justification": "This employee needs access for reason X",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "ecd78419-3f1e-4f07-9bd9-7c77137af4f1",
                "userDisplayName": "Bianca Pisani",
                "userPrincipalName": "BiancaP@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "037b737f-e8ca-4507-b126-5a0620ba2c18",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:28.473Z",
            "decision": "Deny",
            "justification": "This employee changed roles and no longer needs access",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "5f16b75b-031c-4944-9691-070f03273079",
                "userDisplayName": "Delia Dennis",
                "userPrincipalName": "DeliaD@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "7032f455-10a3-4d04-bf02-66fb65d26d10",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:44.38Z",
            "decision": "DontKnow",
            "justification": "I do not know what this employee needs",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "4169762e-895f-4350-a13d-e5b09b1efcfa",
                "userDisplayName": "Isaiah Langer",
                "userPrincipalName": "IsaiahL@M365x471116.OnMicrosoft.com"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="aae02-136">另请参阅</span><span class="sxs-lookup"><span data-stu-id="aae02-136">See also</span></span>

- [<span data-ttu-id="aae02-137">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="aae02-137">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="aae02-138">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="aae02-138">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


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
