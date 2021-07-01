---
title: 列出 accessReviewScheduleDefinitions
description: 获取 accessReviewScheduleDefinition 对象及其属性的列表。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 34c58be8c3fa0c580e91a74baee2ddafbed3e738
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208685"
---
# <a name="list-accessreviewscheduledefinitions"></a><span data-ttu-id="0b3bd-103">列出 accessReviewScheduleDefinitions</span><span class="sxs-lookup"><span data-stu-id="0b3bd-103">List accessReviewScheduleDefinitions</span></span>
<span data-ttu-id="0b3bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b3bd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b3bd-105">获取 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-105">Get a list of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects and their properties.</span></span>

>[!NOTE]
><span data-ttu-id="0b3bd-106">此 API 的默认页面大小为 100 accessReviewScheduleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="0b3bd-107">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="0b3bd-108">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b3bd-109">权限</span><span class="sxs-lookup"><span data-stu-id="0b3bd-109">Permissions</span></span>
<span data-ttu-id="0b3bd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b3bd-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b3bd-112">Permission type</span></span>|<span data-ttu-id="0b3bd-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b3bd-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b3bd-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b3bd-114">Delegated (work or school account)</span></span>|<span data-ttu-id="0b3bd-115">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b3bd-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="0b3bd-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b3bd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b3bd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-117">Not supported.</span></span>|
|<span data-ttu-id="0b3bd-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b3bd-118">Application</span></span>|<span data-ttu-id="0b3bd-119">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b3bd-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

 <span data-ttu-id="0b3bd-120">登录用户还必须具有允许其读取访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-120">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="0b3bd-121">请参阅访问评审 [角色和应用程序权限授权检查](../resources/accessreviewsv2-root.md#role-and-application-permission-authorization-checks)。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-121">See access review [role and application permission authorization checks](../resources/accessreviewsv2-root.md#role-and-application-permission-authorization-checks).</span></span>

## <a name="http-request"></a><span data-ttu-id="0b3bd-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b3bd-122">HTTP request</span></span>

<span data-ttu-id="0b3bd-123">列出所有 accessReviewScheduleDefinitions：</span><span class="sxs-lookup"><span data-stu-id="0b3bd-123">To list all your accessReviewScheduleDefinitions:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b3bd-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0b3bd-124">Optional query parameters</span></span>
<span data-ttu-id="0b3bd-125">此方法支持使用 `$select` 、 、 、 和 OData 查询参数 `$top` `$skip` `$orderBy` `$filter` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-125">This method supports the `$select`, `$top`, `$skip`,`$orderBy`, and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="0b3bd-126">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="use-the-filter-query-parameter"></a><span data-ttu-id="0b3bd-127">使用 $filter 查询参数</span><span class="sxs-lookup"><span data-stu-id="0b3bd-127">Use the $filter query parameter</span></span>
<span data-ttu-id="0b3bd-128">`$filter` `contains` accessReviewScheduleDefinition 的 **scope** 属性支持具有 运算符的查询参数。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-128">The `$filter` query parameter with the `contains` operator is supported on the **scope** property of accessReviewScheduleDefinition.</span></span> <span data-ttu-id="0b3bd-129">对请求使用以下格式：</span><span class="sxs-lookup"><span data-stu-id="0b3bd-129">Use the following format for the request:</span></span>

```http
GET /identityGovernance/accessReviews/definitions?$filter=contains(scope/microsoft.graph.accessReviewQueryScope/query, '{object}')
```

<span data-ttu-id="0b3bd-130">的值 `{object}` 可以是下列值之一：</span><span class="sxs-lookup"><span data-stu-id="0b3bd-130">The value of `{object}` can be one of the following:</span></span>

|<span data-ttu-id="0b3bd-131">值</span><span class="sxs-lookup"><span data-stu-id="0b3bd-131">Value</span></span>|<span data-ttu-id="0b3bd-132">说明</span><span class="sxs-lookup"><span data-stu-id="0b3bd-132">Description</span></span>|
|:---     |:---       |
|`/groups`  |<span data-ttu-id="0b3bd-133">列出各个组上的每个 accessReviewScheduleDefinition (不包括作用域为具有来宾用户的所有Microsoft 365组的定义) 。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-133">List every accessReviewScheduleDefinition on individual groups (excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>|
|`/groups/{group id}`  |<span data-ttu-id="0b3bd-134">列出特定组上的每个 accessReviewScheduleDefinition (不包括作用域为具有来宾用户的所有 Microsoft 365 组) 。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-134">List every accessReviewScheduleDefinition on a specific group (excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>|
|`./members`  |<span data-ttu-id="0b3bd-135">列出每个作用域为来宾用户的所有 Microsoft 365 AccessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-135">List every accessReviewScheduleDefinition scoped to all Microsoft 365 groups with guest users.</span></span>|
|`accessPackageAssignments`  |<span data-ttu-id="0b3bd-136">列出访问包上的每个 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-136">List every accessReviewScheduleDefinition on an access package.</span></span>|
|`roleAssignmentScheduleInstances`  |<span data-ttu-id="0b3bd-137">列出分配给特权角色的服务主体的每个 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-137">List every accessReviewScheduleDefinition for service principals assigned to a privileged role.</span></span>|

<span data-ttu-id="0b3bd-138">`$filter` **accessReviewInactiveUserQueryScope** 或 **principalResourceMembershipScope 不支持查询参数**。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-138">The `$filter` query parameter is not supported on **accessReviewInactiveUserQueryScope** or **principalResourceMembershipScope**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b3bd-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b3bd-139">Request headers</span></span>
|<span data-ttu-id="0b3bd-140">名称</span><span class="sxs-lookup"><span data-stu-id="0b3bd-140">Name</span></span>|<span data-ttu-id="0b3bd-141">说明</span><span class="sxs-lookup"><span data-stu-id="0b3bd-141">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0b3bd-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b3bd-142">Authorization</span></span>|<span data-ttu-id="0b3bd-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b3bd-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b3bd-145">Request body</span></span>
<span data-ttu-id="0b3bd-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b3bd-147">响应</span><span class="sxs-lookup"><span data-stu-id="0b3bd-147">Response</span></span>

<span data-ttu-id="0b3bd-148">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-148">If successful, this method returns a `200 OK` response code and a collection of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b3bd-149">示例</span><span class="sxs-lookup"><span data-stu-id="0b3bd-149">Examples</span></span>

### <a name="example-1-list-the-first-one-hundred-access-review-definitions"></a><span data-ttu-id="0b3bd-150">示例 1：列出前 100 个访问评审定义</span><span class="sxs-lookup"><span data-stu-id="0b3bd-150">Example 1: List the first one hundred access review definitions</span></span>

#### <a name="request"></a><span data-ttu-id="0b3bd-151">请求</span><span class="sxs-lookup"><span data-stu-id="0b3bd-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0b3bd-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b3bd-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition"
}-->
```
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="0b3bd-153">C#</span><span class="sxs-lookup"><span data-stu-id="0b3bd-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b3bd-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b3bd-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b3bd-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b3bd-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b3bd-156">Java</span><span class="sxs-lookup"><span data-stu-id="0b3bd-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b3bd-157">响应</span><span class="sxs-lookup"><span data-stu-id="0b3bd-157">Response</span></span>
><span data-ttu-id="0b3bd-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions",
    "@odata.count": 1,
    "value": [
        {
            "id": "98dcebed-c7f6-46f4-bcf3-4a3fccdb3e2a",
            "displayName": "Access Review",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b/transitiveMembers",
                "queryType": "MicrosoftGraph"
            },
            "instanceEnumerationScope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
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

### <a name="example-2-retrieve-all-access-review-definitions-scoped-to-all-microsoft-365-groups-in-a-tenant"></a><span data-ttu-id="0b3bd-159">示例 2：检索范围为租户中Microsoft 365组的所有访问评审定义</span><span class="sxs-lookup"><span data-stu-id="0b3bd-159">Example 2: Retrieve all access review definitions scoped to all Microsoft 365 groups in a tenant</span></span>

#### <a name="request"></a><span data-ttu-id="0b3bd-160">请求</span><span class="sxs-lookup"><span data-stu-id="0b3bd-160">Request</span></span>
<span data-ttu-id="0b3bd-161">以下示例显示一个请求，请求检索范围为租户中所有Microsoft 365组的所有访问评审系列。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-161">The following example shows a request to retrieve all the access review series scoped to all Microsoft 365 groups in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="0b3bd-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b3bd-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition_allgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions?$filter=contains(scope/microsoft.graph.accessReviewQueryScope/query, './members')
```
# <a name="c"></a>[<span data-ttu-id="0b3bd-163">C#</span><span class="sxs-lookup"><span data-stu-id="0b3bd-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-allgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b3bd-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b3bd-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-allgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b3bd-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b3bd-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-allgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b3bd-166">Java</span><span class="sxs-lookup"><span data-stu-id="0b3bd-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-allgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b3bd-167">响应</span><span class="sxs-lookup"><span data-stu-id="0b3bd-167">Response</span></span>
><span data-ttu-id="0b3bd-168">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b3bd-168">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions",
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
            "instances@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('cc701697-762c-439a-81f5-f58d680fde76')/instances",
            "instances": []
        }
    ]
}

```
