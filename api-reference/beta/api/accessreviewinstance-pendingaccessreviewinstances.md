---
title: accessReviewInstance：pendingAccessReviewInstances
description: 通过调用用户检索等待审批的 accessReviewInstance 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c62f954ea7fe70d46ff4a46879b4d568d619226c
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030524"
---
# <a name="accessreviewinstance-pendingaccessreviewinstances-deprecated"></a><span data-ttu-id="9be02-103">accessReviewInstance：pendingAccessReviewInstances (弃) </span><span class="sxs-lookup"><span data-stu-id="9be02-103">accessReviewInstance: pendingAccessReviewInstances (deprecated)</span></span>

<span data-ttu-id="9be02-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9be02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="9be02-105">此方法将弃用，并将于 2023 年 5 月 19 日停止返回数据。</span><span class="sxs-lookup"><span data-stu-id="9be02-105">This method will be deprecated and will stop returning data on May 19, 2023.</span></span> <span data-ttu-id="9be02-106">它已被 [filterByCurrentUser 取代](accessreviewinstance-filterbycurrentuser.md)。</span><span class="sxs-lookup"><span data-stu-id="9be02-106">It has been replaced by [filterByCurrentUser](accessreviewinstance-filterbycurrentuser.md).</span></span>

>[!NOTE]
><span data-ttu-id="9be02-107">此 API 的默认页面大小为 100 accessReviewInstance 对象。</span><span class="sxs-lookup"><span data-stu-id="9be02-107">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="9be02-108">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="9be02-108">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="9be02-109">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="9be02-109">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="9be02-110">检索 [调用用户等待审批的 accessReviewInstance](../resources/accessreviewinstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9be02-110">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects pending approval by the calling user.</span></span> <span data-ttu-id="9be02-111">返回零个或多个 accessReviewInstance 对象的列表，其中调用用户是分配的审阅者。</span><span class="sxs-lookup"><span data-stu-id="9be02-111">A list of zero or more accessReviewInstance objects are returned, of which the calling user is an assigned reviewer.</span></span>

## <a name="permissions"></a><span data-ttu-id="9be02-112">权限</span><span class="sxs-lookup"><span data-stu-id="9be02-112">Permissions</span></span>
<span data-ttu-id="9be02-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9be02-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9be02-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="9be02-115">Permission type</span></span>                        | <span data-ttu-id="9be02-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9be02-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9be02-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9be02-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="9be02-118">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9be02-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |

 <span data-ttu-id="9be02-119">登录用户仅在实例的 accessReviewScheduleDefinition 中查看为其分配审阅者的实例。</span><span class="sxs-lookup"><span data-stu-id="9be02-119">The signed-in user only sees instances of which they are assigned reviewer in the accessReviewScheduleDefinition of the instance.</span></span>

## <a name="http-request"></a><span data-ttu-id="9be02-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9be02-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9be02-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9be02-121">Optional query parameters</span></span>
<span data-ttu-id="9be02-122">此方法支持 `$skip` `$top` 和 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9be02-122">This method supports `$skip` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="9be02-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9be02-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9be02-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="9be02-124">Request headers</span></span>
<span data-ttu-id="9be02-125">无。</span><span class="sxs-lookup"><span data-stu-id="9be02-125">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="9be02-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9be02-126">Request body</span></span>
<span data-ttu-id="9be02-127">不提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="9be02-127">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="9be02-128">响应</span><span class="sxs-lookup"><span data-stu-id="9be02-128">Response</span></span>
<span data-ttu-id="9be02-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstance](../resources/accessreviewinstance.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="9be02-129">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9be02-130">示例</span><span class="sxs-lookup"><span data-stu-id="9be02-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="9be02-131">请求</span><span class="sxs-lookup"><span data-stu-id="9be02-131">Request</span></span>
<span data-ttu-id="9be02-132">以下示例显示检索租户中所有访问评审系列的请求。</span><span class="sxs-lookup"><span data-stu-id="9be02-132">The following example shows a request to retrieve all the access review series in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="9be02-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9be02-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances?$expand=definition&$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="9be02-134">C#</span><span class="sxs-lookup"><span data-stu-id="9be02-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9be02-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9be02-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9be02-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9be02-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9be02-137">Java</span><span class="sxs-lookup"><span data-stu-id="9be02-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9be02-138">响应</span><span class="sxs-lookup"><span data-stu-id="9be02-138">Response</span></span>
><span data-ttu-id="9be02-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9be02-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="9be02-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9be02-140">See also</span></span>

- [<span data-ttu-id="9be02-141">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="9be02-141">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)
- [<span data-ttu-id="9be02-142">获取 accessReviewInstanceDecisionItems 待审批</span><span class="sxs-lookup"><span data-stu-id="9be02-142">Get accessReviewInstanceDecisionItems pending approval</span></span>](accessreviewinstancedecisionitem-listpendingapproval.md)


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
