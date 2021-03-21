---
title: 获取 identityProvider
description: 检索 identityProvider 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 8a91b4d52dcb3eb9cd889d8406349bd057948208
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961042"
---
# <a name="get-identityprovider"></a><span data-ttu-id="ce962-103">获取 identityProvider</span><span class="sxs-lookup"><span data-stu-id="ce962-103">Get identityProvider</span></span>

<span data-ttu-id="ce962-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce962-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce962-105">检索 [identityProvider 的属性和关系](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="ce962-105">Retrieve the properties and relationships of an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ce962-106">权限</span><span class="sxs-lookup"><span data-stu-id="ce962-106">Permissions</span></span>

<span data-ttu-id="ce962-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce962-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce962-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce962-109">Permission type</span></span>      | <span data-ttu-id="ce962-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce962-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce962-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce962-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ce962-112">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce962-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="ce962-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="ce962-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ce962-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce962-114">Not supported.</span></span>|
|<span data-ttu-id="ce962-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce962-115">Application</span></span>|<span data-ttu-id="ce962-116">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce962-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="ce962-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="ce962-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="ce962-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="ce962-118">Global administrator</span></span>
* <span data-ttu-id="ce962-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="ce962-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ce962-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce962-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ce962-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce962-121">Request headers</span></span>

|<span data-ttu-id="ce962-122">名称</span><span class="sxs-lookup"><span data-stu-id="ce962-122">Name</span></span>|<span data-ttu-id="ce962-123">说明</span><span class="sxs-lookup"><span data-stu-id="ce962-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ce962-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce962-124">Authorization</span></span>|<span data-ttu-id="ce962-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ce962-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce962-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce962-127">Request body</span></span>

<span data-ttu-id="ce962-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ce962-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce962-129">响应</span><span class="sxs-lookup"><span data-stu-id="ce962-129">Response</span></span>

<span data-ttu-id="ce962-130">如果成功，此方法返回响应代码和 `200 OK` [identityProvider](../resources/identityprovider.md) 或 [openIdConnectProvider](../resources/openidconnectprovider.md) (仅在响应正文中为 Azure AD B2C) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce962-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce962-131">示例</span><span class="sxs-lookup"><span data-stu-id="ce962-131">Examples</span></span>

### <a name="example-1-retrieve-a-specific-identityprovider"></a><span data-ttu-id="ce962-132">示例 1：检索特定 identityProvider</span><span class="sxs-lookup"><span data-stu-id="ce962-132">Example 1: Retrieve a specific identityProvider</span></span>

#### <a name="request"></a><span data-ttu-id="ce962-133">请求</span><span class="sxs-lookup"><span data-stu-id="ce962-133">Request</span></span>

<span data-ttu-id="ce962-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ce962-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ce962-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce962-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="ce962-136">C#</span><span class="sxs-lookup"><span data-stu-id="ce962-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce962-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce962-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce962-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce962-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce962-139">Java</span><span class="sxs-lookup"><span data-stu-id="ce962-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ce962-140">响应</span><span class="sxs-lookup"><span data-stu-id="ce962-140">Response</span></span>

<span data-ttu-id="ce962-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ce962-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
### <a name="example-2-retrieve-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="ce962-142">示例 2：仅为 Azure AD B2C (检索特定的 openIDConnectProvider) </span><span class="sxs-lookup"><span data-stu-id="ce962-142">Example 2: Retrieve a specific openIDConnectProvider (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="ce962-143">请求</span><span class="sxs-lookup"><span data-stu-id="ce962-143">Request</span></span>

<span data-ttu-id="ce962-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ce962-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ce962-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce962-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="ce962-146">C#</span><span class="sxs-lookup"><span data-stu-id="ce962-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce962-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce962-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce962-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce962-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce962-149">Java</span><span class="sxs-lookup"><span data-stu-id="ce962-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ce962-150">响应</span><span class="sxs-lookup"><span data-stu-id="ce962-150">Response</span></span>

<span data-ttu-id="ce962-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ce962-151">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
  "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
  "name": "Login with the Contoso identity provider",
  "type": "OpenIDConnect",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "12345",
  "claimsMapping": {
      "userId": "myUserId",
      "givenName": "myGivenName",
      "surname": "mySurname",
      "email": "myEmail",
      "displayName": "myDisplayName"
  },
  "domainHint": "mycustomoidc",
  "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
  "responseMode": "form_post",
  "responseType": "code",
  "scope": "openid"
}
```


