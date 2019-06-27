---
title: 列出 riskyUsers
description: 检索**riskyUser**对象集合的属性和关系。
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b91237a5957875256adf3a03d97054e05696894
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264972"
---
# <a name="list-riskyusers"></a><span data-ttu-id="5a7ed-103">列出 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="5a7ed-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a7ed-104">检索**riskyUser**对象集合的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-104">Retrieve the properties and relationships of a collection of **riskyUser** objects.</span></span>

><span data-ttu-id="5a7ed-105">**注意:** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a7ed-106">权限</span><span class="sxs-lookup"><span data-stu-id="5a7ed-106">Permissions</span></span>
<span data-ttu-id="5a7ed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a7ed-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a7ed-109">Permission type</span></span>      | <span data-ttu-id="5a7ed-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a7ed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a7ed-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a7ed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5a7ed-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a7ed-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="5a7ed-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a7ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a7ed-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-114">Not supported.</span></span>    |
|<span data-ttu-id="5a7ed-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a7ed-115">Application</span></span> | <span data-ttu-id="5a7ed-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a7ed-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a7ed-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a7ed-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5a7ed-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5a7ed-118">Optional query parameters</span></span>
<span data-ttu-id="5a7ed-119">此方法支持`$filter`自定义查询响应。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="5a7ed-120">请参阅本主题后面的示例。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="5a7ed-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a7ed-121">Request headers</span></span>
| <span data-ttu-id="5a7ed-122">名称</span><span class="sxs-lookup"><span data-stu-id="5a7ed-122">Name</span></span>      |<span data-ttu-id="5a7ed-123">说明</span><span class="sxs-lookup"><span data-stu-id="5a7ed-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5a7ed-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a7ed-124">Authorization</span></span>  | <span data-ttu-id="5a7ed-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5a7ed-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5a7ed-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="5a7ed-128">用于确定是否保留更改的工作簿会话 ID。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-128">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="5a7ed-129">可选。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a7ed-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a7ed-130">Request body</span></span>
<span data-ttu-id="5a7ed-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a7ed-132">响应</span><span class="sxs-lookup"><span data-stu-id="5a7ed-132">Response</span></span>
<span data-ttu-id="5a7ed-133">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[riskyUser](../resources/riskyuser.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-133">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5a7ed-134">示例</span><span class="sxs-lookup"><span data-stu-id="5a7ed-134">Examples</span></span>
### <a name="example-1-list-risky-users"></a><span data-ttu-id="5a7ed-135">示例 1: 列出有风险的用户</span><span class="sxs-lookup"><span data-stu-id="5a7ed-135">Example 1: List risky users</span></span>
#### <a name="request"></a><span data-ttu-id="5a7ed-136">请求</span><span class="sxs-lookup"><span data-stu-id="5a7ed-136">Request</span></span>
<span data-ttu-id="5a7ed-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
#### <a name="response"></a><span data-ttu-id="5a7ed-138">响应</span><span class="sxs-lookup"><span data-stu-id="5a7ed-138">Response</span></span>
<span data-ttu-id="5a7ed-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
            "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
            "isGuest": true,
            "isProcessing": true,
            "isDeleted": true,
            "riskDetail": "adminConfirmedSigninCompromised",
            "riskLevel": "high",
            "riskState": "atRisk",
            "userDisplayName": "Alex Wilbur",
            "userPrincipalName": "alexw@contoso.com"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5a7ed-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5a7ed-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5a7ed-141">C#</span><span class="sxs-lookup"><span data-stu-id="5a7ed-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list_riskyusers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a7ed-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="5a7ed-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list_riskyusers-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5a7ed-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="5a7ed-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/list_riskyusers-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="5a7ed-144">示例 2: 列出有风险的用户并筛选结果</span><span class="sxs-lookup"><span data-stu-id="5a7ed-144">Example 2: List risky users and filter the results</span></span>
#### <a name="request"></a><span data-ttu-id="5a7ed-145">请求</span><span class="sxs-lookup"><span data-stu-id="5a7ed-145">Request</span></span>
<span data-ttu-id="5a7ed-146">下面的示例演示如何使用`$filter`来获取其聚合风险级别为中的 riskyUser 的集合。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-146">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```

#### <a name="response"></a><span data-ttu-id="5a7ed-147">响应</span><span class="sxs-lookup"><span data-stu-id="5a7ed-147">Response</span></span>
<span data-ttu-id="5a7ed-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5a7ed-148">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
            "riskLastUpdatedDateTime": "2018-09-22T00:04:49.1195968Z",
            "isGuest": false,
            "isProcessing": true,
            "isDeleted": false,
            "riskDetail": "none",
            "riskLevel": "medium",
            "riskState": "atRisk",
            "userDisplayName": "Alex Wilbur",
            "userPrincipalName": "alexw@contoso.com",
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5a7ed-149">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5a7ed-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5a7ed-150">C#</span><span class="sxs-lookup"><span data-stu-id="5a7ed-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list_filter_riskyusers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a7ed-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="5a7ed-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list_filter_riskyusers-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5a7ed-152">目标-C</span><span class="sxs-lookup"><span data-stu-id="5a7ed-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/list_filter_riskyusers-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
