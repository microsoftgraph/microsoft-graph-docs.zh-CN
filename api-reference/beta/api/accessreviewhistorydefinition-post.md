---
title: 创建 accessReviewHistoryDefinition
description: 创建新的 accessReviewHistoryDefinition 对象。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3c0a1309ae67a2f4aa3f066deb5fe8adeec84119
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474106"
---
# <a name="create-accessreviewhistorydefinition"></a><span data-ttu-id="d6b67-103">创建 accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="d6b67-103">Create accessReviewHistoryDefinition</span></span>

<span data-ttu-id="d6b67-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6b67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6b67-105">创建新的 [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6b67-105">Create a new [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6b67-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6b67-106">Permissions</span></span>

<span data-ttu-id="d6b67-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6b67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6b67-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6b67-109">Permission type</span></span>|<span data-ttu-id="d6b67-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6b67-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6b67-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6b67-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6b67-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6b67-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="d6b67-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6b67-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6b67-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6b67-114">Not supported.</span></span>|
|<span data-ttu-id="d6b67-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6b67-115">Application</span></span>|<span data-ttu-id="d6b67-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6b67-116">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="d6b67-117">登录用户还必须是允许其读取访问评审以检索任何数据的目录角色。</span><span class="sxs-lookup"><span data-stu-id="d6b67-117">The signed-in user must also be in a directory role that permits them to read an access review to retrieve any data.</span></span>  <span data-ttu-id="d6b67-118">有关详细信息，请参阅访问评审的角色和 [权限要求](../resources/accessreviewsv2-root.md)。</span><span class="sxs-lookup"><span data-stu-id="d6b67-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="d6b67-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6b67-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/historyDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="d6b67-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6b67-120">Request headers</span></span>

|<span data-ttu-id="d6b67-121">名称</span><span class="sxs-lookup"><span data-stu-id="d6b67-121">Name</span></span>|<span data-ttu-id="d6b67-122">说明</span><span class="sxs-lookup"><span data-stu-id="d6b67-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d6b67-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6b67-123">Authorization</span></span>|<span data-ttu-id="d6b67-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6b67-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d6b67-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6b67-126">Content-Type</span></span>|<span data-ttu-id="d6b67-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d6b67-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6b67-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6b67-129">Request body</span></span>

<span data-ttu-id="d6b67-130">在请求正文中，提供 [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6b67-130">In the request body, supply a JSON representation of the [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.</span></span>

<span data-ttu-id="d6b67-131">下表显示用于创建 [accessReviewHistoryDefinition 所需的属性](../resources/accessreviewhistorydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="d6b67-131">The following table shows the required properties used to create an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md).</span></span>

|<span data-ttu-id="d6b67-132">属性</span><span class="sxs-lookup"><span data-stu-id="d6b67-132">Property</span></span>|<span data-ttu-id="d6b67-133">类型</span><span class="sxs-lookup"><span data-stu-id="d6b67-133">Type</span></span>|<span data-ttu-id="d6b67-134">说明</span><span class="sxs-lookup"><span data-stu-id="d6b67-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6b67-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d6b67-135">displayName</span></span> | <span data-ttu-id="d6b67-136">String</span><span class="sxs-lookup"><span data-stu-id="d6b67-136">String</span></span>  | <span data-ttu-id="d6b67-137">访问评审历史记录数据收集的名称。</span><span class="sxs-lookup"><span data-stu-id="d6b67-137">Name for the access review history data collection.</span></span> <span data-ttu-id="d6b67-138">必需。</span><span class="sxs-lookup"><span data-stu-id="d6b67-138">Required.</span></span> |
|<span data-ttu-id="d6b67-139">reviewHistoryPeriodStartDateTime</span><span class="sxs-lookup"><span data-stu-id="d6b67-139">reviewHistoryPeriodStartDateTime</span></span>  | <span data-ttu-id="d6b67-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6b67-140">DateTimeOffset</span></span>  | <span data-ttu-id="d6b67-141">时间戳、在此日期当天或之后开始审阅将包含在提取的历史记录数据中。</span><span class="sxs-lookup"><span data-stu-id="d6b67-141">Timestamp, reviews starting on or after this date will be included in the fetched history data.</span></span> <span data-ttu-id="d6b67-142">必需。</span><span class="sxs-lookup"><span data-stu-id="d6b67-142">Required.</span></span>  |
|<span data-ttu-id="d6b67-143">reviewHistoryPeriodEndDateTime</span><span class="sxs-lookup"><span data-stu-id="d6b67-143">reviewHistoryPeriodEndDateTime</span></span>  | <span data-ttu-id="d6b67-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6b67-144">DateTimeOffset</span></span>  | <span data-ttu-id="d6b67-145">时间戳、在此日期或之前开始审阅将包含在提取的历史记录数据中。</span><span class="sxs-lookup"><span data-stu-id="d6b67-145">Timestamp, reviews starting on or before this date will be included in the fetched history data.</span></span> <span data-ttu-id="d6b67-146">必需。</span><span class="sxs-lookup"><span data-stu-id="d6b67-146">Required.</span></span>  |
|<span data-ttu-id="d6b67-147">scopes</span><span class="sxs-lookup"><span data-stu-id="d6b67-147">scopes</span></span>|<span data-ttu-id="d6b67-148">microsoft.graph.accessReviewQueryScope 集合</span><span class="sxs-lookup"><span data-stu-id="d6b67-148">microsoft.graph.accessReviewQueryScope collection</span></span>| <span data-ttu-id="d6b67-149">用于筛选包含在提取的历史记录数据中的审阅。</span><span class="sxs-lookup"><span data-stu-id="d6b67-149">Used to filter which reviews are included in the fetched history data.</span></span> <span data-ttu-id="d6b67-150">获取其范围与提供的范围匹配的审阅。</span><span class="sxs-lookup"><span data-stu-id="d6b67-150">Fetches reviews whose scope matches with this provided scope.</span></span> <span data-ttu-id="d6b67-151">必需。</span><span class="sxs-lookup"><span data-stu-id="d6b67-151">Required.</span></span>  |

### <a name="supported-scope-queries-for-accessreviewhistorydefinition"></a><span data-ttu-id="d6b67-152">accessReviewHistoryDefinition 支持的范围查询</span><span class="sxs-lookup"><span data-stu-id="d6b67-152">Supported scope queries for accessReviewHistoryDefinition</span></span>

<span data-ttu-id="d6b67-153">以下是基于[accessreviewqueryscope](../resources/accessreviewqueryscope.md)的[accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md)上支持的查询。</span><span class="sxs-lookup"><span data-stu-id="d6b67-153">The following are queries supported on an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) based on the [accessreviewqueryscope](../resources/accessreviewqueryscope.md).</span></span> <span data-ttu-id="d6b67-154">这些作用域规定创建定义时生成的可下载 CSV 文件中包含哪种类型的审阅历史记录数据。</span><span class="sxs-lookup"><span data-stu-id="d6b67-154">These scopes dictate which type of review history data is included in the downloadable CSV file which is generated when the definition is created.</span></span>

|<span data-ttu-id="d6b67-155">应用场景</span><span class="sxs-lookup"><span data-stu-id="d6b67-155">Scenario</span></span>| <span data-ttu-id="d6b67-156">查询</span><span class="sxs-lookup"><span data-stu-id="d6b67-156">Query</span></span> |
|--|--|
| <span data-ttu-id="d6b67-157">包括单个组上的每个审阅结果 (不包括作用域为具有来宾用户的所有Microsoft 365 `accessReviewScheduleDefinition` 组) </span><span class="sxs-lookup"><span data-stu-id="d6b67-157">Include every `accessReviewScheduleDefinition` review result on individual groups (excludes definitions scoped to all Microsoft 365 groups with guest users)</span></span> | <span data-ttu-id="d6b67-158">/identityGovernance/accessReviews/definitions？$filter=contains (scope/query， '/groups') "</span><span class="sxs-lookup"><span data-stu-id="d6b67-158">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')"</span></span> |
| <span data-ttu-id="d6b67-159">包括特定组上的每个审阅结果 (不包括作用域为具有来宾用户的所有Microsoft 365 `accessReviewScheduleDefinition` 组) </span><span class="sxs-lookup"><span data-stu-id="d6b67-159">Include every `accessReviewScheduleDefinition` review result on a specific group (excludes definitions scoped to all Microsoft 365 groups with guest users)</span></span> | <span data-ttu-id="d6b67-160">/identityGovernance/accessReviews/definitions？$filter=contains (scope/query， '/groups/{group id}') </span><span class="sxs-lookup"><span data-stu-id="d6b67-160">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups/{group id}')</span></span> |
| <span data-ttu-id="d6b67-161">包含范围 `accessReviewScheduleDefinition` 为包含来宾用户的所有Microsoft 365组的所有审阅结果</span><span class="sxs-lookup"><span data-stu-id="d6b67-161">Include every `accessReviewScheduleDefinition` review result scoped to all Microsoft 365 groups with guest users</span></span> | <span data-ttu-id="d6b67-162">/identityGovernance/accessReviews/definitions？$filter=contains (scope/query， './members') </span><span class="sxs-lookup"><span data-stu-id="d6b67-162">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, './members')</span></span> |
| <span data-ttu-id="d6b67-163">包含 `accessReviewScheduleDefinition` 访问包上的每个审阅结果</span><span class="sxs-lookup"><span data-stu-id="d6b67-163">Include every `accessReviewScheduleDefinition` review result on an access package</span></span> | <span data-ttu-id="d6b67-164">/identityGovernance/accessReviews/definitions？$filter=contains (scope/query， 'accessPackageAssignments') </span><span class="sxs-lookup"><span data-stu-id="d6b67-164">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')</span></span> |
| <span data-ttu-id="d6b67-165">包括 `accessReviewScheduleDefinition` 分配给特权角色的服务主体的每次审阅结果</span><span class="sxs-lookup"><span data-stu-id="d6b67-165">Include every `accessReviewScheduleDefinition` review result for service principals assigned to privileged role</span></span> | <span data-ttu-id="d6b67-166">/identityGovernance/accessReviews/definitions？$filter=contains (scope/query， 'roleAssignmentScheduleInstances') </span><span class="sxs-lookup"><span data-stu-id="d6b67-166">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances')</span></span> |
| <span data-ttu-id="d6b67-167">包含 `accessReviewScheduleDefinition` 特定组的每次审阅结果</span><span class="sxs-lookup"><span data-stu-id="d6b67-167">Include every `accessReviewScheduleDefinition` review result for reivews of a specific group</span></span> | <span data-ttu-id="d6b67-168">/identityGovernance/accessReviews/definitions？$filter=scope/query eq '/groups/a1382a9b-8320-4e9c-8f73-dfead37d7723/members'</span><span class="sxs-lookup"><span data-stu-id="d6b67-168">/identityGovernance/accessReviews/definitions?$filter=scope/query eq '/groups/a1382a9b-8320-4e9c-8f73-dfead37d7723/members'</span></span> |

## <a name="response"></a><span data-ttu-id="d6b67-169">响应</span><span class="sxs-lookup"><span data-stu-id="d6b67-169">Response</span></span>

<span data-ttu-id="d6b67-170">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6b67-170">If successful, this method returns a `201 Created` response code and an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6b67-171">示例</span><span class="sxs-lookup"><span data-stu-id="d6b67-171">Examples</span></span>

<span data-ttu-id="d6b67-172">以下示例演示如何创建访问评审历史记录定义，该定义范围为从 01/01/2021 的开始日期到 04/05/2021 的结束日期，以访问访问包和组上的审阅。</span><span class="sxs-lookup"><span data-stu-id="d6b67-172">The following example shows how to create an access review history definition scoped to access reviews on access packages and groups, running between the start date of 01/01/2021 and end date of 04/05/2021.</span></span>

### <a name="request"></a><span data-ttu-id="d6b67-173">请求</span><span class="sxs-lookup"><span data-stu-id="d6b67-173">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d6b67-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6b67-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessreviewhistorydefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions
Content-Type: application/json

{
  "displayName": "Last quarter's group reviews April 2021",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="d6b67-175">C#</span><span class="sxs-lookup"><span data-stu-id="d6b67-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewhistorydefinition-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6b67-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6b67-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewhistorydefinition-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6b67-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6b67-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewhistorydefinition-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6b67-178">Java</span><span class="sxs-lookup"><span data-stu-id="d6b67-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewhistorydefinition-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d6b67-179">响应</span><span class="sxs-lookup"><span data-stu-id="d6b67-179">Response</span></span>
><span data-ttu-id="d6b67-180">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d6b67-180">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
  "displayName": "Last quarter's group reviews April 2021",
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "status": "requested",
  "createdDateTime": "2021-04-14T00:22:48.9392594Z",
  "fulfilledDateTime": null,
  "downloadUri": null,
  "createdBy": {
      "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
      "displayName": "MOD Administrator",
      "userPrincipalName": "admin@contoso.com"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```
