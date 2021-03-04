---
title: 列出 accessReviewScheduleDefinitions
description: 检索 accessReviewScheduleDefinition 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 983ecadb7bf60258ee531ad252c4c67325e97802
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439042"
---
# <a name="list-accessreviewscheduledefinition"></a><span data-ttu-id="6e2ce-103">列出 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="6e2ce-103">List accessReviewScheduleDefinition</span></span>

<span data-ttu-id="6e2ce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e2ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e2ce-105">检索 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-105">Retrieve the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects.</span></span> <span data-ttu-id="6e2ce-106">对于创建的每个访问评审系列，将返回零个或多个 accessReviewScheduleDefinition 对象的列表，包括所有其嵌套属性。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-106">A list of zero or more accessReviewScheduleDefinition objects are returned, including all of their nested properties, for each access review series created.</span></span> <span data-ttu-id="6e2ce-107">这不包括关联的 accessReviewInstances。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-107">This does not include associated accessReviewInstances.</span></span>

>[!NOTE]
><span data-ttu-id="6e2ce-108">如果返回了许多 **accessReviewScheduleDefinitions，** 为了提高效率并避免超时，请检索页面中的 结果集，方法为在请求中同时包括页面大小最多为 100 的 $top 查询参数和 $skip=0 查询参数。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-108">If many **accessReviewScheduleDefinitions** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="6e2ce-109">当结果集多个页面时，Microsoft Graph 在响应中返回包含下一页结果 URL 的 @odata.nextLink 属性的页面。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-109">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="6e2ce-110">如果存在该属性，请在每个响应中继续使用 @odata.nextLink URL 提出其他请求，直到返回所有结果，如应用中分页 Microsoft Graph 数据中所述。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-110">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="6e2ce-111">如果未提供查询参数且结果超过 100 个，Microsoft Graph 将自动对结果进行分页，每页结果为 100 个。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-111">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>


## <a name="permissions"></a><span data-ttu-id="6e2ce-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="6e2ce-112">Permissions</span></span>
<span data-ttu-id="6e2ce-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e2ce-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e2ce-115">Permission type</span></span>                        | <span data-ttu-id="6e2ce-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e2ce-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e2ce-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e2ce-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e2ce-118">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e2ce-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="6e2ce-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e2ce-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e2ce-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-120">Not supported.</span></span>|
|<span data-ttu-id="6e2ce-121">Application</span><span class="sxs-lookup"><span data-stu-id="6e2ce-121">Application</span></span>                            | <span data-ttu-id="6e2ce-122">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e2ce-122">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="6e2ce-123">登录用户还必须具有允许其读取访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-123">The signed-in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="6e2ce-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e2ce-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a><span data-ttu-id="6e2ce-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e2ce-125">Request headers</span></span>
<span data-ttu-id="6e2ce-126">无。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-126">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="6e2ce-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e2ce-127">Request body</span></span>
<span data-ttu-id="6e2ce-128">不提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-128">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="6e2ce-129">响应</span><span class="sxs-lookup"><span data-stu-id="6e2ce-129">Response</span></span>
<span data-ttu-id="6e2ce-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-130">If successful, this method returns a `200 OK` response code and an array of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e2ce-131">示例</span><span class="sxs-lookup"><span data-stu-id="6e2ce-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="6e2ce-132">请求</span><span class="sxs-lookup"><span data-stu-id="6e2ce-132">Request</span></span>
<span data-ttu-id="6e2ce-133">以下示例显示检索租户中所有访问评审系列的请求。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-133">The following example shows a request to retrieve all the access review series in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="6e2ce-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e2ce-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="6e2ce-135">C#</span><span class="sxs-lookup"><span data-stu-id="6e2ce-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e2ce-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e2ce-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e2ce-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e2ce-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e2ce-138">Java</span><span class="sxs-lookup"><span data-stu-id="6e2ce-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="6e2ce-139">响应</span><span class="sxs-lookup"><span data-stu-id="6e2ce-139">Response</span></span>
><span data-ttu-id="6e2ce-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6e2ce-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 1,
    "value": [
        {
            "id": "98dcebed-c7f6-46f4-bcf3-4a3fccdb3e2a",
            "displayName": "Access Review",
            "createdDateTime": "2020-09-09T14:27:59Z",
            "lastModifiedDateTime": "2020-09-11T12:02:50Z",
            "status": "InProgress",
            "descriptionForAdmins": "",
            "descriptionForReviewers": "",
            "createdBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "admin@contoso.com"
            },
            "scope": {
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b/transitiveMembers",
                "queryType": "MicrosoftGraph"
            },
            "instanceEnumerationScope": {
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b",
                "queryType": "MicrosoftGraph"
            },
            "reviewers": [
                {
                    "query": "./manager",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": "decisions"
                }
            ],
            "settings": {
                "mailNotificationsEnabled": true,
                "reminderNotificationsEnabled": true,
                "justificationRequiredOnApproval": true,
                "defaultDecisionEnabled": false,
                "defaultDecision": "None",
                "instanceDurationInDays": 0,
                "autoApplyDecisionsEnabled": false,
                "recommendationsEnabled": true,
                "recurrence": {
                    "pattern": {
                        "type": "weekly",
                        "interval": 1,
                        "month": 0,
                        "dayOfMonth": 0,
                        "daysOfWeek": [],
                        "firstDayOfWeek": "sunday",
                        "index": "first"
                    },
                    "range": {
                        "type": "numbered",
                        "numberOfOccurrences": 0,
                        "recurrenceTimeZone": null,
                        "startDate": "2020-09-11",
                        "endDate": "9999-12-31"
                    }
                }
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="6e2ce-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6e2ce-142">See also</span></span>

- [<span data-ttu-id="6e2ce-143">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="6e2ce-143">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
