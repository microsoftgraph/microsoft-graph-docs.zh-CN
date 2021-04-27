---
title: accessReviewInstance：pendingAccessReviewInstances
description: 通过调用用户检索等待审批的 accessReviewInstance 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 581ade7ffd620a105dfbb2e6f5c8e9854aab76dc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048412"
---
# <a name="accessreviewinstance-pendingaccessreviewinstances"></a><span data-ttu-id="51dd1-103">accessReviewInstance：pendingAccessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="51dd1-103">accessReviewInstance: pendingAccessReviewInstances</span></span>

<span data-ttu-id="51dd1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51dd1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51dd1-105">检索 [调用用户等待审批的 accessReviewInstance](../resources/accessreviewinstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51dd1-105">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects pending approval by the calling user.</span></span> <span data-ttu-id="51dd1-106">返回零个或多个 accessReviewInstance 对象的列表，其中调用用户是分配的审阅者。</span><span class="sxs-lookup"><span data-stu-id="51dd1-106">A list of zero or more accessReviewInstance objects are returned, of which the calling user is an assigned reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="51dd1-107">如果返回了许多 **accessReviewInstances，** 为了提高效率并避免超时，请检索页面中的 结果集，方法包括页面大小最多为 100 的 $top 查询参数和请求中的 $skip=0 查询参数。</span><span class="sxs-lookup"><span data-stu-id="51dd1-107">If many **accessReviewInstances** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="51dd1-108">当结果集跨多个页面时，Microsoft Graph 在响应中返回包含指向下一页结果的 URL 的 @odata.nextLink 属性的页面。</span><span class="sxs-lookup"><span data-stu-id="51dd1-108">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="51dd1-109">如果存在该属性，请继续在每个响应中通过 @odata.nextLink URL 提出其他请求，直到返回所有结果，如在应用中分页 Microsoft Graph 数据中所述。</span><span class="sxs-lookup"><span data-stu-id="51dd1-109">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="51dd1-110">如果未提供查询参数且结果超过 100 个，Microsoft Graph将按每页 100 个结果自动对结果分页。</span><span class="sxs-lookup"><span data-stu-id="51dd1-110">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="51dd1-111">权限</span><span class="sxs-lookup"><span data-stu-id="51dd1-111">Permissions</span></span>
<span data-ttu-id="51dd1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51dd1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51dd1-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="51dd1-114">Permission type</span></span>                        | <span data-ttu-id="51dd1-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="51dd1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="51dd1-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51dd1-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="51dd1-117">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51dd1-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |

 <span data-ttu-id="51dd1-118">登录用户仅在实例的 accessReviewScheduleDefinition 中查看为其分配审阅者的实例。</span><span class="sxs-lookup"><span data-stu-id="51dd1-118">The signed-in user only sees instances of which they are assigned reviewer in the accessReviewScheduleDefinition of the instance.</span></span>

## <a name="http-request"></a><span data-ttu-id="51dd1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51dd1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances
```
## <a name="request-headers"></a><span data-ttu-id="51dd1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="51dd1-120">Request headers</span></span>
<span data-ttu-id="51dd1-121">无。</span><span class="sxs-lookup"><span data-stu-id="51dd1-121">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="51dd1-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="51dd1-122">Request body</span></span>
<span data-ttu-id="51dd1-123">不提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="51dd1-123">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="51dd1-124">响应</span><span class="sxs-lookup"><span data-stu-id="51dd1-124">Response</span></span>
<span data-ttu-id="51dd1-125">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstance](../resources/accessreviewinstance.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="51dd1-125">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51dd1-126">示例</span><span class="sxs-lookup"><span data-stu-id="51dd1-126">Examples</span></span>
### <a name="request"></a><span data-ttu-id="51dd1-127">请求</span><span class="sxs-lookup"><span data-stu-id="51dd1-127">Request</span></span>
<span data-ttu-id="51dd1-128">以下示例显示检索租户中所有访问评审系列的请求。</span><span class="sxs-lookup"><span data-stu-id="51dd1-128">The following example shows a request to retrieve all the access review series in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="51dd1-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="51dd1-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances?$expand=definition&$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="51dd1-130">C#</span><span class="sxs-lookup"><span data-stu-id="51dd1-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51dd1-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51dd1-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51dd1-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51dd1-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51dd1-133">Java</span><span class="sxs-lookup"><span data-stu-id="51dd1-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="51dd1-134">响应</span><span class="sxs-lookup"><span data-stu-id="51dd1-134">Response</span></span>
><span data-ttu-id="51dd1-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="51dd1-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.count": 1,
    "value": [
        {
            "id": "70a68410-67f3-4d4c-b946-6989e050be19",
            "startDateTime": "2020-09-09T15:57:56Z",
            "endDateTime": "2020-10-08T15:57:56Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/04b3d70b-c770-46cb-b751-d857d2beedff/transitiveMembers",
                "queryType": "MicrosoftGraph"
            },
            "definition": {
                "id": "70a68410-67f3-4d4c-b946-6989e050be19",
                "displayName": "review of leadership",
                "createdDateTime": "2020-09-08T15:59:06Z",
                "lastModifiedDateTime": "2020-09-09T15:58:24Z",
                "status": "InProgress",
                "descriptionForAdmins": "review of leadership",
                "descriptionForReviewers": "",
                "createdBy": {
                    "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@msft.com"
                },
                "scope": {
                    "query": "/groups/04b3d70b-c770-46cb-b751-d857d2beedff/transitiveMembers",
                    "queryType": "MicrosoftGraph"
                },
                "instanceEnumerationScope": {
                    "query": "/groups/04b3d70b-c770-46cb-b751-d857d2beedff",
                    "queryType": "MicrosoftGraph"
                },
                "reviewers": [
                    {
                        "query": "/users/957f1027-c0ee-460d-9269-b8828e59e0fe",
                        "queryType": "MicrosoftGraph",
                        "queryRoot": null
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
                        "pattern": null,
                        "range": {
                            "type": "numbered",
                            "numberOfOccurrences": 0,
                            "recurrenceTimeZone": null,
                            "startDate": "2020-09-09",
                            "endDate": "2020-10-08"
                        }
                    },
                    "applyActions": [
                        {
                            "@odata.type": "#microsoft.graph.removeAccessApplyAction"
                        }
                    ]
                }
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="51dd1-136">另请参阅</span><span class="sxs-lookup"><span data-stu-id="51dd1-136">See also</span></span>

- [<span data-ttu-id="51dd1-137">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="51dd1-137">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)
- [<span data-ttu-id="51dd1-138">获取 accessReviewInstanceDecisionItems 待审批</span><span class="sxs-lookup"><span data-stu-id="51dd1-138">Get accessReviewInstanceDecisionItems pending approval</span></span>](accessreviewinstancedecisionitem-listpendingapproval.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstance pendingApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
