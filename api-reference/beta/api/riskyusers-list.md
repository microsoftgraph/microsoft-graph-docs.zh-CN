---
title: 列出 riskyUsers
description: 检索 **riskyUser** 对象集合的属性和关系。
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: d0ab9e55f6274f048d6fe25dd9f731c91dd182ad
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440773"
---
# <a name="list-riskyusers"></a><span data-ttu-id="1a3da-103">列出 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="1a3da-103">List riskyUsers</span></span>

<span data-ttu-id="1a3da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a3da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a3da-105">检索 **riskyUser** 对象集合的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a3da-105">Retrieve the properties and relationships of a collection of **riskyUser** objects.</span></span>

><span data-ttu-id="1a3da-106">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="1a3da-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a3da-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="1a3da-107">Permissions</span></span>
<span data-ttu-id="1a3da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a3da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a3da-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a3da-110">Permission type</span></span>      | <span data-ttu-id="1a3da-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a3da-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a3da-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a3da-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1a3da-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a3da-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="1a3da-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a3da-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a3da-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a3da-115">Not supported.</span></span>    |
|<span data-ttu-id="1a3da-116">Application</span><span class="sxs-lookup"><span data-stu-id="1a3da-116">Application</span></span> | <span data-ttu-id="1a3da-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a3da-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a3da-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a3da-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
GET /identityProtection/riskyUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a3da-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1a3da-119">Optional query parameters</span></span>
<span data-ttu-id="1a3da-120">此方法支持 `$filter` 自定义查询响应。</span><span class="sxs-lookup"><span data-stu-id="1a3da-120">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="1a3da-121">请参阅本主题稍后介绍的示例。</span><span class="sxs-lookup"><span data-stu-id="1a3da-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="1a3da-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a3da-122">Request headers</span></span>
| <span data-ttu-id="1a3da-123">名称</span><span class="sxs-lookup"><span data-stu-id="1a3da-123">Name</span></span>      |<span data-ttu-id="1a3da-124">说明</span><span class="sxs-lookup"><span data-stu-id="1a3da-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a3da-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a3da-125">Authorization</span></span>  | <span data-ttu-id="1a3da-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a3da-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a3da-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1a3da-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="1a3da-129">确定是否保留更改的工作簿会话 ID。</span><span class="sxs-lookup"><span data-stu-id="1a3da-129">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="1a3da-130">可选。</span><span class="sxs-lookup"><span data-stu-id="1a3da-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a3da-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a3da-131">Request body</span></span>
<span data-ttu-id="1a3da-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a3da-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a3da-133">响应</span><span class="sxs-lookup"><span data-stu-id="1a3da-133">Response</span></span>
<span data-ttu-id="1a3da-134">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [riskyUser](../resources/riskyuser.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1a3da-134">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a3da-135">示例</span><span class="sxs-lookup"><span data-stu-id="1a3da-135">Examples</span></span>
### <a name="example-1-list-risky-users"></a><span data-ttu-id="1a3da-136">示例 1：列出有风险的用户</span><span class="sxs-lookup"><span data-stu-id="1a3da-136">Example 1: List risky users</span></span>
#### <a name="request"></a><span data-ttu-id="1a3da-137">请求</span><span class="sxs-lookup"><span data-stu-id="1a3da-137">Request</span></span>
<span data-ttu-id="1a3da-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a3da-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a3da-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a3da-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers
```
# <a name="c"></a>[<span data-ttu-id="1a3da-140">C#</span><span class="sxs-lookup"><span data-stu-id="1a3da-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a3da-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a3da-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a3da-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a3da-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a3da-143">Java</span><span class="sxs-lookup"><span data-stu-id="1a3da-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskyusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1a3da-144">响应</span><span class="sxs-lookup"><span data-stu-id="1a3da-144">Response</span></span>
<span data-ttu-id="1a3da-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1a3da-145">Here is an example of the response.</span></span>
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

### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="1a3da-146">示例 2：列出有风险的用户并筛选结果</span><span class="sxs-lookup"><span data-stu-id="1a3da-146">Example 2: List risky users and filter the results</span></span>
#### <a name="request"></a><span data-ttu-id="1a3da-147">请求</span><span class="sxs-lookup"><span data-stu-id="1a3da-147">Request</span></span>
<span data-ttu-id="1a3da-148">以下示例演示如何用于获取聚合风险级别为"中等" `$filter` 的 riskyUser 集合。</span><span class="sxs-lookup"><span data-stu-id="1a3da-148">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>


# <a name="http"></a>[<span data-ttu-id="1a3da-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a3da-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
# <a name="c"></a>[<span data-ttu-id="1a3da-150">C#</span><span class="sxs-lookup"><span data-stu-id="1a3da-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a3da-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a3da-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a3da-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a3da-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a3da-153">Java</span><span class="sxs-lookup"><span data-stu-id="1a3da-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-filter-riskyusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1a3da-154">响应</span><span class="sxs-lookup"><span data-stu-id="1a3da-154">Response</span></span>
<span data-ttu-id="1a3da-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1a3da-155">Here is an example of the response.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


