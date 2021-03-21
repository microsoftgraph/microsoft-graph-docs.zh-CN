---
title: 获取 riskyUser
description: 检索 **riskyUser** 对象的属性和关系。
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: 9582066edadf5fb431bec0f7b3c9701fe71ead8c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960770"
---
# <a name="get-riskyuser"></a><span data-ttu-id="282f2-103">获取 riskyUser</span><span class="sxs-lookup"><span data-stu-id="282f2-103">Get riskyUser</span></span>

<span data-ttu-id="282f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="282f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="282f2-105">检索 **riskyUser** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="282f2-105">Retrieve the properties and relationships of a **riskyUser** object.</span></span>

><span data-ttu-id="282f2-106">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="282f2-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="282f2-107">权限</span><span class="sxs-lookup"><span data-stu-id="282f2-107">Permissions</span></span>
<span data-ttu-id="282f2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="282f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="282f2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="282f2-110">Permission type</span></span>      | <span data-ttu-id="282f2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="282f2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="282f2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="282f2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="282f2-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="282f2-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="282f2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="282f2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="282f2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="282f2-115">Not supported.</span></span>    |
|<span data-ttu-id="282f2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="282f2-116">Application</span></span> | <span data-ttu-id="282f2-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="282f2-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="282f2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="282f2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
GET /identityProtection/riskyUsers/{id}
```


## <a name="request-headers"></a><span data-ttu-id="282f2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="282f2-119">Request headers</span></span>
| <span data-ttu-id="282f2-120">名称</span><span class="sxs-lookup"><span data-stu-id="282f2-120">Name</span></span>      |<span data-ttu-id="282f2-121">说明</span><span class="sxs-lookup"><span data-stu-id="282f2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="282f2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="282f2-122">Authorization</span></span>  | <span data-ttu-id="282f2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="282f2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="282f2-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="282f2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="282f2-126">确定是否保留更改的工作簿会话 ID。</span><span class="sxs-lookup"><span data-stu-id="282f2-126">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="282f2-127">可选。</span><span class="sxs-lookup"><span data-stu-id="282f2-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="282f2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="282f2-128">Request body</span></span>
<span data-ttu-id="282f2-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="282f2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="282f2-130">响应</span><span class="sxs-lookup"><span data-stu-id="282f2-130">Response</span></span>

<span data-ttu-id="282f2-131">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [riskyUser](../resources/riskyuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="282f2-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="282f2-132">示例</span><span class="sxs-lookup"><span data-stu-id="282f2-132">Examples</span></span>
### <a name="example-1-get-a-risky-user"></a><span data-ttu-id="282f2-133">示例 1：获取有风险的用户</span><span class="sxs-lookup"><span data-stu-id="282f2-133">Example 1: Get a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="282f2-134">请求</span><span class="sxs-lookup"><span data-stu-id="282f2-134">Request</span></span>
<span data-ttu-id="282f2-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="282f2-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="282f2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="282f2-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_1",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="282f2-137">C#</span><span class="sxs-lookup"><span data-stu-id="282f2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="282f2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="282f2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="282f2-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="282f2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="282f2-140">Java</span><span class="sxs-lookup"><span data-stu-id="282f2-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskyuser-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="282f2-141">响应</span><span class="sxs-lookup"><span data-stu-id="282f2-141">Response</span></span>
<span data-ttu-id="282f2-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="282f2-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
```
### <a name="example-2-get-risky-users"></a><span data-ttu-id="282f2-143">示例 2：获取有风险的用户</span><span class="sxs-lookup"><span data-stu-id="282f2-143">Example 2: Get risky users</span></span>
#### <a name="request"></a><span data-ttu-id="282f2-144">请求</span><span class="sxs-lookup"><span data-stu-id="282f2-144">Request</span></span>
<span data-ttu-id="282f2-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="282f2-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="282f2-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="282f2-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_2",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers
```
# <a name="c"></a>[<span data-ttu-id="282f2-147">C#</span><span class="sxs-lookup"><span data-stu-id="282f2-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="282f2-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="282f2-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="282f2-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="282f2-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="282f2-150">Java</span><span class="sxs-lookup"><span data-stu-id="282f2-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskyuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="282f2-151">响应</span><span class="sxs-lookup"><span data-stu-id="282f2-151">Response</span></span>
<span data-ttu-id="282f2-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="282f2-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->



