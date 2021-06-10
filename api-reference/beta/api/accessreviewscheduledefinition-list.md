---
title: 列出 accessReviewScheduleDefinitions
description: 检索 accessReviewScheduleDefinition 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bbc014075f1dc72970ef64add9555d6067cbe0f0
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870022"
---
# <a name="list-accessreviewscheduledefinition"></a><span data-ttu-id="ad189-103">列出 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="ad189-103">List accessReviewScheduleDefinition</span></span>

<span data-ttu-id="ad189-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad189-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad189-105">检索 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ad189-105">Retrieve the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects.</span></span> <span data-ttu-id="ad189-106">对于创建的每个访问评审系列，将返回零个或多个 accessReviewScheduleDefinition 对象的列表，包括它们的所有嵌套属性。</span><span class="sxs-lookup"><span data-stu-id="ad189-106">A list of zero or more accessReviewScheduleDefinition objects are returned, including all of their nested properties, for each access review series created.</span></span> <span data-ttu-id="ad189-107">这不包括关联的 accessReviewInstance 对象。</span><span class="sxs-lookup"><span data-stu-id="ad189-107">This does not include the associated accessReviewInstance objects.</span></span>

>[!NOTE]
><span data-ttu-id="ad189-108">此 API 的默认页面大小为 100 accessReviewScheduleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="ad189-108">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="ad189-109">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="ad189-109">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="ad189-110">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="ad189-110">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad189-111">权限</span><span class="sxs-lookup"><span data-stu-id="ad189-111">Permissions</span></span>
<span data-ttu-id="ad189-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad189-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad189-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad189-114">Permission type</span></span>                        | <span data-ttu-id="ad189-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad189-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad189-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad189-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad189-117">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad189-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="ad189-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad189-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad189-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad189-119">Not supported.</span></span>|
|<span data-ttu-id="ad189-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad189-120">Application</span></span>                            | <span data-ttu-id="ad189-121">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad189-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="ad189-122">登录用户还必须具有允许其读取访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="ad189-122">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="ad189-123">请参阅访问评审 [角色和应用程序权限授权检查](../resources/accessreviewsv2-root.md#role-and-application-permission-authorization-checks)。</span><span class="sxs-lookup"><span data-stu-id="ad189-123">See access review [role and application permission authorization checks](../resources/accessreviewsv2-root.md#role-and-application-permission-authorization-checks).</span></span>

## <a name="http-request"></a><span data-ttu-id="ad189-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad189-124">HTTP request</span></span>

<span data-ttu-id="ad189-125">列出所有 accessReviewScheduleDefinitions：</span><span class="sxs-lookup"><span data-stu-id="ad189-125">To list all your accessReviewScheduleDefinitions:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad189-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ad189-126">Optional query parameters</span></span>
<span data-ttu-id="ad189-127">此方法支持 `$select` 、 `$top` 、 和 `$skip` `$filter` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ad189-127">This method supports the `$select`, `$top`, `$skip`, and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ad189-128">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ad189-128">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="use-the-filter-query-parameter"></a><span data-ttu-id="ad189-129">使用 $filter 查询参数</span><span class="sxs-lookup"><span data-stu-id="ad189-129">Use the $filter query parameter</span></span>
<span data-ttu-id="ad189-130">`$filter` `contains` accessReviewScheduleDefinition 的 **scope** 属性支持具有 运算符的查询参数。</span><span class="sxs-lookup"><span data-stu-id="ad189-130">The `$filter` query parameter with the `contains` operator is supported on the **scope** property of accessReviewScheduleDefinition.</span></span> <span data-ttu-id="ad189-131">对请求使用以下格式：</span><span class="sxs-lookup"><span data-stu-id="ad189-131">Use the following format for the request:</span></span>

```http
GET /identityGovernance/accessReviews/definitions?$filter=contains(scope/microsoft.graph.accessReviewQueryScope/query, '{object}')
```

<span data-ttu-id="ad189-132">的值 `{object}` 可以是下列值之一：</span><span class="sxs-lookup"><span data-stu-id="ad189-132">The value of `{object}` can be one of the following:</span></span>

|<span data-ttu-id="ad189-133">值</span><span class="sxs-lookup"><span data-stu-id="ad189-133">Value</span></span>|<span data-ttu-id="ad189-134">说明</span><span class="sxs-lookup"><span data-stu-id="ad189-134">Description</span></span>|
|:---     |:---       |
|<span data-ttu-id="ad189-135">/groups</span><span class="sxs-lookup"><span data-stu-id="ad189-135">/groups</span></span>  |<span data-ttu-id="ad189-136">列出各个组上的每个 accessReviewScheduleDefinition (不包括作用域为具有来宾用户的所有Microsoft 365组的定义) 。</span><span class="sxs-lookup"><span data-stu-id="ad189-136">List every accessReviewScheduleDefinition on individual groups (excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>|
|<span data-ttu-id="ad189-137">/groups/{group id}</span><span class="sxs-lookup"><span data-stu-id="ad189-137">/groups/{group id}</span></span>  |<span data-ttu-id="ad189-138">列出特定组上的每个 accessReviewScheduleDefinition (不包括作用域为具有来宾用户的所有 Microsoft 365 组) 。</span><span class="sxs-lookup"><span data-stu-id="ad189-138">List every accessReviewScheduleDefinition on a specific group (excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>|
|<span data-ttu-id="ad189-139">./members</span><span class="sxs-lookup"><span data-stu-id="ad189-139">./members</span></span>  |<span data-ttu-id="ad189-140">列出每个作用域为来宾用户的所有 Microsoft 365 AccessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="ad189-140">List every accessReviewScheduleDefinition scoped to all Microsoft 365 groups with guest users.</span></span>|
|<span data-ttu-id="ad189-141">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="ad189-141">accessPackageAssignments</span></span>  |<span data-ttu-id="ad189-142">列出访问包上的每个 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="ad189-142">List every accessReviewScheduleDefinition on an access package.</span></span>|
|<span data-ttu-id="ad189-143">roleAssignmentScheduleInstances</span><span class="sxs-lookup"><span data-stu-id="ad189-143">roleAssignmentScheduleInstances</span></span>  |<span data-ttu-id="ad189-144">列出分配给特权角色的服务主体的每个 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="ad189-144">List every accessReviewScheduleDefinition for service principals assigned to a privileged role.</span></span>|

<span data-ttu-id="ad189-145">`$filter` **accessReviewInactiveUserQueryScope** 或 **principalResourceMembershipScope 不支持查询参数**。</span><span class="sxs-lookup"><span data-stu-id="ad189-145">The `$filter` query parameter is not supported on **accessReviewInactiveUserQueryScope** or **principalResourceMembershipScope**.</span></span>


## <a name="request-headers"></a><span data-ttu-id="ad189-146">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad189-146">Request headers</span></span>
<span data-ttu-id="ad189-147">无。</span><span class="sxs-lookup"><span data-stu-id="ad189-147">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="ad189-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad189-148">Request body</span></span>
<span data-ttu-id="ad189-149">不提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="ad189-149">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="ad189-150">响应</span><span class="sxs-lookup"><span data-stu-id="ad189-150">Response</span></span>
<span data-ttu-id="ad189-151">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="ad189-151">If successful, this method returns a `200 OK` response code and an array of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ad189-152">示例</span><span class="sxs-lookup"><span data-stu-id="ad189-152">Examples</span></span>

### <a name="example-1-list-the-first-one-hundred-access-review-definitions"></a><span data-ttu-id="ad189-153">示例 1：列出前 100 个访问评审定义</span><span class="sxs-lookup"><span data-stu-id="ad189-153">Example 1: List the first one hundred access review definitions</span></span>

#### <a name="request"></a><span data-ttu-id="ad189-154">请求</span><span class="sxs-lookup"><span data-stu-id="ad189-154">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ad189-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad189-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="ad189-156">C#</span><span class="sxs-lookup"><span data-stu-id="ad189-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad189-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad189-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad189-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad189-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad189-159">Java</span><span class="sxs-lookup"><span data-stu-id="ad189-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ad189-160">响应</span><span class="sxs-lookup"><span data-stu-id="ad189-160">Response</span></span>
><span data-ttu-id="ad189-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ad189-161">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions",
    "@odata.count": 1,
    "value": [
        {
            "id": "98dcebed-c7f6-46f4-bcf3-4a3fccdb3e2a",
            "displayName": "Access Review",
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


### <a name="example-2-retrieve-all-access-review-definitions-scoped-to-all-microsoft-365-groups-in-a-tenant"></a><span data-ttu-id="ad189-162">示例 2：检索范围为租户中Microsoft 365组的所有访问评审定义</span><span class="sxs-lookup"><span data-stu-id="ad189-162">Example 2: Retrieve all access review definitions scoped to all Microsoft 365 groups in a tenant</span></span>

#### <a name="request"></a><span data-ttu-id="ad189-163">请求</span><span class="sxs-lookup"><span data-stu-id="ad189-163">Request</span></span>
<span data-ttu-id="ad189-164">以下示例显示一个请求，请求检索范围为租户中所有Microsoft 365组的所有访问评审系列。</span><span class="sxs-lookup"><span data-stu-id="ad189-164">The following example shows a request to retrieve all the access review series scoped to all Microsoft 365 groups in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad189-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad189-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition_allgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions?$filter=contains(scope/microsoft.graph.accessReviewQueryScope/query, './members')
```
# <a name="c"></a>[<span data-ttu-id="ad189-166">C#</span><span class="sxs-lookup"><span data-stu-id="ad189-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-allgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad189-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad189-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-allgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad189-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad189-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-allgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad189-169">Java</span><span class="sxs-lookup"><span data-stu-id="ad189-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-allgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ad189-170">响应</span><span class="sxs-lookup"><span data-stu-id="ad189-170">Response</span></span>
><span data-ttu-id="ad189-171">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ad189-171">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions",
    "@odata.count": 1,
    "value": [
        {
            "id": "cc701697-762c-439a-81f5-f58d680fde76",
            "displayName": "Review guest access across Microsoft 365 groups",
            "status": "InProgress",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph"
            },
            "instanceEnumerationScope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
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
                "defaultDecisionEnabled": true,
                "defaultDecision": "Recommendation",
                "instanceDurationInDays": 25,
                "autoApplyDecisionsEnabled": true,
                "recommendationsEnabled": true,
                "recurrence": {
                    "pattern": {
                        "type": "absoluteMonthly",
                        "interval": 3,
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
                        "startDate": "2021-04-27",
                        "endDate": "9999-12-31"
                    }
                },
                "applyActions": [
                    {
                        "@odata.type": "#microsoft.graph.removeAccessApplyAction"
                    }
                ]
            },
            "instances@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('cc701697-762c-439a-81f5-f58d680fde76')/instances",
            "instances": []
        }
    ]
}

```


## <a name="see-also"></a><span data-ttu-id="ad189-172">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ad189-172">See also</span></span>

- [<span data-ttu-id="ad189-173">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="ad189-173">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)


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
