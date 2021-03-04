---
title: 列出 accessReviewInstanceDecisionItem
description: 检索 accessReviewInstanceDecisionItem 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1d2ec913e3ef942f76c26c86df74493819c2d790
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439133"
---
# <a name="list-accessreviewinstancedecisionitem"></a><span data-ttu-id="00828-103">列出 accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="00828-103">List accessReviewInstanceDecisionItem</span></span>

<span data-ttu-id="00828-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00828-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00828-105">检索 [特定 accessReviewInstance 的 accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) [对象](../resources/accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="00828-105">Retrieve the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects for a specific [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="00828-106">返回零个或多个 accessReviewInstanceDecisionItem 对象的列表，包括所有嵌套属性。</span><span class="sxs-lookup"><span data-stu-id="00828-106">A list of zero or more accessReviewInstanceDecisionItem objects are returned, including all of their nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="00828-107">如果返回了许多 **accessReviewInstanceDecisionItems，** 为了提高效率并避免超时，请检索页面中的 结果集，方法为在请求中同时包括页面大小最多为 100 的 $top 查询参数和 $skip=0 查询参数。</span><span class="sxs-lookup"><span data-stu-id="00828-107">If many **accessReviewInstanceDecisionItems** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="00828-108">当结果集多个页面时，Microsoft Graph 在响应中返回包含下一页结果 URL 的 @odata.nextLink 属性的页面。</span><span class="sxs-lookup"><span data-stu-id="00828-108">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="00828-109">如果存在该属性，请在每个响应中继续使用 @odata.nextLink URL 提出其他请求，直到返回所有结果，如应用中分页 Microsoft Graph 数据中所述。</span><span class="sxs-lookup"><span data-stu-id="00828-109">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="00828-110">如果未提供查询参数且结果超过 100 个，Microsoft Graph 将自动对结果进行分页，每页结果为 100 个。</span><span class="sxs-lookup"><span data-stu-id="00828-110">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="00828-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="00828-111">Permissions</span></span>
<span data-ttu-id="00828-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00828-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00828-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="00828-114">Permission type</span></span>                        | <span data-ttu-id="00828-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00828-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="00828-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00828-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="00828-117">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00828-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="00828-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00828-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00828-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="00828-119">Not supported.</span></span>|
|<span data-ttu-id="00828-120">Application</span><span class="sxs-lookup"><span data-stu-id="00828-120">Application</span></span>                            | <span data-ttu-id="00828-121">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00828-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="00828-122">登录用户还必须具有允许其读取访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="00828-122">The signed-in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="00828-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00828-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="00828-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="00828-124">Request headers</span></span>
<span data-ttu-id="00828-125">无。</span><span class="sxs-lookup"><span data-stu-id="00828-125">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="00828-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="00828-126">Request body</span></span>
<span data-ttu-id="00828-127">不提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="00828-127">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="00828-128">响应</span><span class="sxs-lookup"><span data-stu-id="00828-128">Response</span></span>
<span data-ttu-id="00828-129">如果成功，此方法在响应正文中返回 `200 OK` [响应代码和 accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="00828-129">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00828-130">示例</span><span class="sxs-lookup"><span data-stu-id="00828-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="00828-131">请求</span><span class="sxs-lookup"><span data-stu-id="00828-131">Request</span></span>
<span data-ttu-id="00828-132">以下示例显示检索有关访问评审实例的所有决策的请求。</span><span class="sxs-lookup"><span data-stu-id="00828-132">The following example shows a request to retrieve all the decisions on an instance of an access review.</span></span>


# <a name="http"></a>[<span data-ttu-id="00828-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="00828-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/14444cdb-6a18-4c08-ba2c-48c02f0a0138/decisions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="00828-134">C#</span><span class="sxs-lookup"><span data-stu-id="00828-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00828-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00828-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00828-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00828-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00828-137">Java</span><span class="sxs-lookup"><span data-stu-id="00828-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="00828-138">响应</span><span class="sxs-lookup"><span data-stu-id="00828-138">Response</span></span>
><span data-ttu-id="00828-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="00828-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="00828-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="00828-141">See also</span></span>

- [<span data-ttu-id="00828-142">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="00828-142">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="00828-143">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="00828-143">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


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
