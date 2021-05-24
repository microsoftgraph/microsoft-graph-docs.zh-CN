---
title: 创建 accessReviewHistoryDefinition
description: 创建新的 accessReviewHistoryDefinition 对象。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f266276fae151bd8cc31455c4fd69eab193dd440
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629220"
---
# <a name="create-accessreviewhistorydefinition"></a><span data-ttu-id="e5399-103">创建 accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="e5399-103">Create accessReviewHistoryDefinition</span></span>

<span data-ttu-id="e5399-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5399-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5399-105">创建新的 [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e5399-105">Create a new [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5399-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e5399-106">Permissions</span></span>

<span data-ttu-id="e5399-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5399-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5399-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5399-109">Permission type</span></span>|<span data-ttu-id="e5399-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5399-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5399-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5399-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e5399-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5399-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="e5399-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5399-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5399-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5399-114">Not supported.</span></span>|
|<span data-ttu-id="e5399-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5399-115">Application</span></span>|<span data-ttu-id="e5399-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5399-116">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="e5399-117">登录用户还必须是允许其读取访问评审以检索任何数据的目录角色。</span><span class="sxs-lookup"><span data-stu-id="e5399-117">The signed-in user must also be in a directory role that permits them to read an access review to retrieve any data.</span></span>  <span data-ttu-id="e5399-118">有关详细信息，请参阅访问评审的角色和 [权限要求](../resources/accessreviewsv2-root.md)。</span><span class="sxs-lookup"><span data-stu-id="e5399-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="e5399-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5399-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/historyDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="e5399-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5399-120">Request headers</span></span>

|<span data-ttu-id="e5399-121">名称</span><span class="sxs-lookup"><span data-stu-id="e5399-121">Name</span></span>|<span data-ttu-id="e5399-122">说明</span><span class="sxs-lookup"><span data-stu-id="e5399-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e5399-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5399-123">Authorization</span></span>|<span data-ttu-id="e5399-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5399-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e5399-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5399-126">Content-Type</span></span>|<span data-ttu-id="e5399-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e5399-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5399-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5399-129">Request body</span></span>

<span data-ttu-id="e5399-130">在请求正文中，提供 [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5399-130">In the request body, supply a JSON representation of the [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.</span></span>

<span data-ttu-id="e5399-131">下表显示用于创建 [accessReviewHistoryDefinition 所需的属性](../resources/accessreviewhistorydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="e5399-131">The following table shows the required properties used to create an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md).</span></span>

|<span data-ttu-id="e5399-132">属性</span><span class="sxs-lookup"><span data-stu-id="e5399-132">Property</span></span>|<span data-ttu-id="e5399-133">类型</span><span class="sxs-lookup"><span data-stu-id="e5399-133">Type</span></span>|<span data-ttu-id="e5399-134">说明</span><span class="sxs-lookup"><span data-stu-id="e5399-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5399-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e5399-135">displayName</span></span> | <span data-ttu-id="e5399-136">String</span><span class="sxs-lookup"><span data-stu-id="e5399-136">String</span></span>  | <span data-ttu-id="e5399-137">访问评审历史记录数据收集的名称。</span><span class="sxs-lookup"><span data-stu-id="e5399-137">Name for the access review history data collection.</span></span> <span data-ttu-id="e5399-138">必需。</span><span class="sxs-lookup"><span data-stu-id="e5399-138">Required.</span></span> |
|<span data-ttu-id="e5399-139">reviewHistoryPeriodStartDateTime</span><span class="sxs-lookup"><span data-stu-id="e5399-139">reviewHistoryPeriodStartDateTime</span></span>  | <span data-ttu-id="e5399-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5399-140">DateTimeOffset</span></span>  | <span data-ttu-id="e5399-141">时间戳、在此日期当天或之后开始审阅将包含在提取的历史记录数据中。</span><span class="sxs-lookup"><span data-stu-id="e5399-141">Timestamp, reviews starting on or after this date will be included in the fetched history data.</span></span> <span data-ttu-id="e5399-142">必需。</span><span class="sxs-lookup"><span data-stu-id="e5399-142">Required.</span></span>  |
|<span data-ttu-id="e5399-143">reviewHistoryPeriodEndDateTime</span><span class="sxs-lookup"><span data-stu-id="e5399-143">reviewHistoryPeriodEndDateTime</span></span>  | <span data-ttu-id="e5399-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5399-144">DateTimeOffset</span></span>  | <span data-ttu-id="e5399-145">时间戳、在此日期或之前开始审阅将包含在提取的历史记录数据中。</span><span class="sxs-lookup"><span data-stu-id="e5399-145">Timestamp, reviews starting on or before this date will be included in the fetched history data.</span></span> <span data-ttu-id="e5399-146">必需。</span><span class="sxs-lookup"><span data-stu-id="e5399-146">Required.</span></span>  |
|<span data-ttu-id="e5399-147">scopes</span><span class="sxs-lookup"><span data-stu-id="e5399-147">scopes</span></span>|<span data-ttu-id="e5399-148">[accessReviewQueryScope](../resources/accessreviewqueryscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5399-148">[accessReviewQueryScope](../resources/accessreviewqueryscope.md) collection</span></span>| <span data-ttu-id="e5399-149">用于筛选包含在提取的历史记录数据中的审阅。</span><span class="sxs-lookup"><span data-stu-id="e5399-149">Used to filter which reviews are included in the fetched history data.</span></span> <span data-ttu-id="e5399-150">获取其范围与提供的范围匹配的审阅。</span><span class="sxs-lookup"><span data-stu-id="e5399-150">Fetches reviews whose scope matches with this provided scope.</span></span> <span data-ttu-id="e5399-151">必需。</span><span class="sxs-lookup"><span data-stu-id="e5399-151">Required.</span></span> <br> <span data-ttu-id="e5399-152">有关详细信息，请参阅 [accessReviewHistoryDefinition 支持的作用域查询](#supported-scope-queries-for-accessreviewhistorydefinition)。</span><span class="sxs-lookup"><span data-stu-id="e5399-152">For more, see [Supported scope queries for accessReviewHistoryDefinition](#supported-scope-queries-for-accessreviewhistorydefinition).</span></span> |

### <a name="supported-scope-queries-for-accessreviewhistorydefinition"></a><span data-ttu-id="e5399-153">accessReviewHistoryDefinition 支持的范围查询</span><span class="sxs-lookup"><span data-stu-id="e5399-153">Supported scope queries for accessReviewHistoryDefinition</span></span>

<span data-ttu-id="e5399-154">[accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md)的 **scopes** 属性基于 **accessReviewQueryScope，** 这是一种允许您在查询属性中配置不同 **资源** 的资源。</span><span class="sxs-lookup"><span data-stu-id="e5399-154">The **scopes** property of [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) is based on **accessReviewQueryScope**, a resource that allows you to configure different resources in it's **query** property.</span></span> <span data-ttu-id="e5399-155">这些资源随后表示历史记录定义的范围，并指示创建历史记录定义时生成的可下载 CSV 文件中包含的查看历史记录数据的类型。</span><span class="sxs-lookup"><span data-stu-id="e5399-155">These resources then represent the scope of the history definition and dictate the type of review history data that is included in the downloadable CSV file which is generated when the history definition is created.</span></span>

<span data-ttu-id="e5399-156">对查询 **属性使用以下格式** ：</span><span class="sxs-lookup"><span data-stu-id="e5399-156">Use the following format for the **query** property:</span></span>

```http
/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '{object}')
```

<span data-ttu-id="e5399-157">的值 `{object}` 是可以在 **accessReviewScheduleDefinition 中配置的资源之一**。</span><span class="sxs-lookup"><span data-stu-id="e5399-157">The value of `{object}` is one of the resources that can be configured in an **accessReviewScheduleDefinition**.</span></span> <span data-ttu-id="e5399-158">例如，以下内容包括单个组上的每个 accessReviewScheduleDefinition 审阅结果 (并排除作用域为具有来宾用户的所有 Microsoft 365 组的定义) 。</span><span class="sxs-lookup"><span data-stu-id="e5399-158">For example, the following includes every accessReviewScheduleDefinition review result on individual groups (and excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>

```http
/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')
```

<span data-ttu-id="e5399-159">有关更多支持的值，请参阅在 [accessReviewScheduleDefinition $filter查询参数](accessreviewscheduledefinition-list.md#use-the-filter-query-parameter)。</span><span class="sxs-lookup"><span data-stu-id="e5399-159">For more supported values, see Use the [$filter query parameter on accessReviewScheduleDefinition](accessreviewscheduledefinition-list.md#use-the-filter-query-parameter).</span></span>

## <a name="response"></a><span data-ttu-id="e5399-160">响应</span><span class="sxs-lookup"><span data-stu-id="e5399-160">Response</span></span>

<span data-ttu-id="e5399-161">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e5399-161">If successful, this method returns a `201 Created` response code and an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e5399-162">示例</span><span class="sxs-lookup"><span data-stu-id="e5399-162">Examples</span></span>

<span data-ttu-id="e5399-163">以下示例演示如何创建访问评审历史记录定义，该定义范围为从 01/01/2021 的开始日期到 04/05/2021 的结束日期，以访问访问包和组上的审阅。</span><span class="sxs-lookup"><span data-stu-id="e5399-163">The following example shows how to create an access review history definition scoped to access reviews on access packages and groups, running between the start date of 01/01/2021 and end date of 04/05/2021.</span></span>

### <a name="request"></a><span data-ttu-id="e5399-164">请求</span><span class="sxs-lookup"><span data-stu-id="e5399-164">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e5399-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5399-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e5399-166">C#</span><span class="sxs-lookup"><span data-stu-id="e5399-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewhistorydefinition-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5399-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5399-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewhistorydefinition-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5399-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5399-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewhistorydefinition-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5399-169">Java</span><span class="sxs-lookup"><span data-stu-id="e5399-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewhistorydefinition-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e5399-170">响应</span><span class="sxs-lookup"><span data-stu-id="e5399-170">Response</span></span>
><span data-ttu-id="e5399-171">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e5399-171">**Note:** The response object shown here might be shortened for readability.</span></span>
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
