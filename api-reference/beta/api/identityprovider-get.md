---
title: 获取 identityProvider
description: 检索 Identityprovider.read.all 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2203296635f40707673a2a8d5c621bf5c9ff8726
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319546"
---
# <a name="get-identityprovider"></a><span data-ttu-id="cfdae-103">获取 identityProvider</span><span class="sxs-lookup"><span data-stu-id="cfdae-103">Get identityProvider</span></span>

<span data-ttu-id="cfdae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfdae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfdae-105">检索 [identityprovider.read.all](../resources/identityprovider.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cfdae-105">Retrieve the properties and relationships of an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cfdae-106">权限</span><span class="sxs-lookup"><span data-stu-id="cfdae-106">Permissions</span></span>

<span data-ttu-id="cfdae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfdae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfdae-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfdae-109">Permission type</span></span>      | <span data-ttu-id="cfdae-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cfdae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfdae-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfdae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cfdae-112">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfdae-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="cfdae-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="cfdae-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="cfdae-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfdae-114">Not supported.</span></span>|
|<span data-ttu-id="cfdae-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfdae-115">Application</span></span>|<span data-ttu-id="cfdae-116">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfdae-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="cfdae-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="cfdae-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="cfdae-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="cfdae-118">Global administrator</span></span>
* <span data-ttu-id="cfdae-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="cfdae-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="cfdae-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfdae-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cfdae-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfdae-121">Request headers</span></span>

|<span data-ttu-id="cfdae-122">名称</span><span class="sxs-lookup"><span data-stu-id="cfdae-122">Name</span></span>|<span data-ttu-id="cfdae-123">说明</span><span class="sxs-lookup"><span data-stu-id="cfdae-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="cfdae-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfdae-124">Authorization</span></span>|<span data-ttu-id="cfdae-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cfdae-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfdae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfdae-127">Request body</span></span>

<span data-ttu-id="cfdae-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cfdae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfdae-129">响应</span><span class="sxs-lookup"><span data-stu-id="cfdae-129">Response</span></span>

<span data-ttu-id="cfdae-130">如果成功，此方法 `200 OK` 仅在响应正文中返回响应代码和 [Identityprovider.read.all](../resources/identityprovider.md) 或 [openIdConnectProvider](../resources/openidconnectprovider.md) (的 JSON 表示形式（仅适用于 Azure AD B2C) ）。</span><span class="sxs-lookup"><span data-stu-id="cfdae-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cfdae-131">示例</span><span class="sxs-lookup"><span data-stu-id="cfdae-131">Examples</span></span>

### <a name="example-1-retrieve-a-specific-identityprovider"></a><span data-ttu-id="cfdae-132">示例1：检索特定的 Identityprovider.read.all</span><span class="sxs-lookup"><span data-stu-id="cfdae-132">Example 1: Retrieve a specific identityProvider</span></span>

#### <a name="request"></a><span data-ttu-id="cfdae-133">请求</span><span class="sxs-lookup"><span data-stu-id="cfdae-133">Request</span></span>

<span data-ttu-id="cfdae-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cfdae-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cfdae-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfdae-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="cfdae-136">C#</span><span class="sxs-lookup"><span data-stu-id="cfdae-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfdae-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfdae-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfdae-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfdae-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cfdae-139">响应</span><span class="sxs-lookup"><span data-stu-id="cfdae-139">Response</span></span>

<span data-ttu-id="cfdae-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cfdae-140">The following is an example of the response.</span></span>

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
### <a name="example-2-retrieve-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="cfdae-141">示例2：仅检索 Azure AD B2C) 的特定 openIDConnectProvider (</span><span class="sxs-lookup"><span data-stu-id="cfdae-141">Example 2: Retrieve a specific openIDConnectProvider (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="cfdae-142">请求</span><span class="sxs-lookup"><span data-stu-id="cfdae-142">Request</span></span>

<span data-ttu-id="cfdae-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cfdae-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```

#### <a name="response"></a><span data-ttu-id="cfdae-144">响应</span><span class="sxs-lookup"><span data-stu-id="cfdae-144">Response</span></span>

<span data-ttu-id="cfdae-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cfdae-145">The following is an example of the response.</span></span>
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
