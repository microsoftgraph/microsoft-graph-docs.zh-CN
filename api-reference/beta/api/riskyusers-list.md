---
title: 列出 riskyUsers
description: 检索**riskyUser**对象集合的属性和关系。
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9c9543321e8fcf0c86d5a8be6948dcafe5eee68
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336355"
---
# <a name="list-riskyusers"></a><span data-ttu-id="ebba7-103">列出 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="ebba7-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebba7-104">检索**riskyUser**对象集合的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ebba7-104">Retrieve the properties and relationships of a collection of **riskyUser** objects.</span></span>

><span data-ttu-id="ebba7-105">**注意:** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="ebba7-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebba7-106">权限</span><span class="sxs-lookup"><span data-stu-id="ebba7-106">Permissions</span></span>
<span data-ttu-id="ebba7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebba7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebba7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebba7-109">Permission type</span></span>      | <span data-ttu-id="ebba7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ebba7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebba7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebba7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ebba7-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebba7-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="ebba7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebba7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebba7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebba7-114">Not supported.</span></span>    |
|<span data-ttu-id="ebba7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ebba7-115">Application</span></span> | <span data-ttu-id="ebba7-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebba7-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebba7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebba7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ebba7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ebba7-118">Optional query parameters</span></span>
<span data-ttu-id="ebba7-119">此方法支持`$filter`自定义查询响应。</span><span class="sxs-lookup"><span data-stu-id="ebba7-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="ebba7-120">请参阅本主题后面的示例。</span><span class="sxs-lookup"><span data-stu-id="ebba7-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="ebba7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebba7-121">Request headers</span></span>
| <span data-ttu-id="ebba7-122">名称</span><span class="sxs-lookup"><span data-stu-id="ebba7-122">Name</span></span>      |<span data-ttu-id="ebba7-123">说明</span><span class="sxs-lookup"><span data-stu-id="ebba7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ebba7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebba7-124">Authorization</span></span>  | <span data-ttu-id="ebba7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebba7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ebba7-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ebba7-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="ebba7-128">用于确定是否保留更改的工作簿会话 ID。</span><span class="sxs-lookup"><span data-stu-id="ebba7-128">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="ebba7-129">可选。</span><span class="sxs-lookup"><span data-stu-id="ebba7-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebba7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebba7-130">Request body</span></span>
<span data-ttu-id="ebba7-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ebba7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebba7-132">响应</span><span class="sxs-lookup"><span data-stu-id="ebba7-132">Response</span></span>
<span data-ttu-id="ebba7-133">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[riskyUser](../resources/riskyUser.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ebba7-133">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyUser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ebba7-134">示例</span><span class="sxs-lookup"><span data-stu-id="ebba7-134">Examples</span></span>
### <a name="example-1-list-risky-users"></a><span data-ttu-id="ebba7-135">示例 1: 列出有风险的用户</span><span class="sxs-lookup"><span data-stu-id="ebba7-135">Example 1: List risky users</span></span>
#### <a name="request"></a><span data-ttu-id="ebba7-136">请求</span><span class="sxs-lookup"><span data-stu-id="ebba7-136">Request</span></span>
<span data-ttu-id="ebba7-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ebba7-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
#### <a name="response"></a><span data-ttu-id="ebba7-138">响应</span><span class="sxs-lookup"><span data-stu-id="ebba7-138">Response</span></span>
<span data-ttu-id="ebba7-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ebba7-139">Here is an example of the response.</span></span>
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

### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="ebba7-140">示例 2: 列出有风险的用户并筛选结果</span><span class="sxs-lookup"><span data-stu-id="ebba7-140">Example 2: List risky users and filter the results</span></span>
#### <a name="request"></a><span data-ttu-id="ebba7-141">请求</span><span class="sxs-lookup"><span data-stu-id="ebba7-141">Request</span></span>
<span data-ttu-id="ebba7-142">下面的示例演示如何使用`$filter`来获取其聚合风险级别为中的 riskyUser 的集合。</span><span class="sxs-lookup"><span data-stu-id="ebba7-142">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```

#### <a name="response"></a><span data-ttu-id="ebba7-143">响应</span><span class="sxs-lookup"><span data-stu-id="ebba7-143">Response</span></span>
<span data-ttu-id="ebba7-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ebba7-144">Here is an example of the response.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
