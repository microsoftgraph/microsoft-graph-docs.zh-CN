---
title: 获取 identityProvider
description: 检索 identityProvider 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 37b7a16f815c62909716a14c5644fe201a49f853
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491089"
---
# <a name="get-identityprovider"></a><span data-ttu-id="97bce-103">获取 identityProvider</span><span class="sxs-lookup"><span data-stu-id="97bce-103">Get identityProvider</span></span>

<span data-ttu-id="97bce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97bce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97bce-105">在 Azure AD 中检索 [socialIdentityProvider](../resources/socialidentityprovider.md) 或 [builtinIdentityProvider](../resources/builtinidentityprovider.md) 的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="97bce-105">Retrieve the properties and relationships of a [socialIdentityProvider](../resources/socialidentityprovider.md) or a [builtinIdentityProvider](../resources/builtinidentityprovider.md) in Azure AD.</span></span>

<span data-ttu-id="97bce-106">对于 Azure AD B2C，它可以检索 [socialIdentityProvider](../resources/socialidentityprovider.md) [、openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) 或 [appleIdentityProvider 的属性和关系](../resources/appleidentityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="97bce-106">For Azure AD B2C, it can retrieve properties and relationships of a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="97bce-107">权限</span><span class="sxs-lookup"><span data-stu-id="97bce-107">Permissions</span></span>

<span data-ttu-id="97bce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97bce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97bce-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="97bce-110">Permission type</span></span>      | <span data-ttu-id="97bce-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97bce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97bce-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97bce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97bce-113">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97bce-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="97bce-114">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="97bce-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="97bce-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="97bce-115">Not supported.</span></span>|
|<span data-ttu-id="97bce-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="97bce-116">Application</span></span>|<span data-ttu-id="97bce-117">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97bce-117">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="97bce-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="97bce-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="97bce-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="97bce-119">Global Administrator</span></span>
* <span data-ttu-id="97bce-120">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="97bce-120">External Identity Provider Administrator</span></span>
* <span data-ttu-id="97bce-121">外部 ID 用户流管理员</span><span class="sxs-lookup"><span data-stu-id="97bce-121">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="97bce-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97bce-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="97bce-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="97bce-123">Request headers</span></span>

|<span data-ttu-id="97bce-124">名称</span><span class="sxs-lookup"><span data-stu-id="97bce-124">Name</span></span>|<span data-ttu-id="97bce-125">说明</span><span class="sxs-lookup"><span data-stu-id="97bce-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="97bce-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="97bce-126">Authorization</span></span>|<span data-ttu-id="97bce-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97bce-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97bce-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="97bce-129">Request body</span></span>

<span data-ttu-id="97bce-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="97bce-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97bce-131">响应</span><span class="sxs-lookup"><span data-stu-id="97bce-131">Response</span></span>

<span data-ttu-id="97bce-132">如果成功，此方法在 Azure AD 租户的响应正文中返回 `200 OK` [socialIdentityProvider](../resources/socialidentityprovider.md) 或 [builtinIdentityProvider](../resources/builtinidentityprovider.md) 的响应代码和 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97bce-132">If successful, this method returns a `200 OK` response code and a JSON representation of a [socialIdentityProvider](../resources/socialidentityprovider.md) or a [builtinIdentityProvider](../resources/builtinidentityprovider.md) in the response body for an Azure AD tenant.</span></span>

<span data-ttu-id="97bce-133">对于 Azure AD B2C 租户，此方法在响应正文中返回 响应代码和 `200 OK` [socialIdentityProvider](../resources/socialidentityprovider.md) [、openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) 或 [appleIdentityProvider](../resources/appleidentityprovider.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97bce-133">For an Azure AD B2C tenant, this method returns a `200 OK` response code and a JSON representation of a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="97bce-134">示例</span><span class="sxs-lookup"><span data-stu-id="97bce-134">Examples</span></span>

### <a name="example-1-retrieve-a-specific-social-identity-provider-azure-ad-or-azure-ad-b2c"></a><span data-ttu-id="97bce-135">示例 1：在Azure AD 或 Azure AD B2C (检索特定社会标识) </span><span class="sxs-lookup"><span data-stu-id="97bce-135">Example 1: Retrieve a specific **social identity provider** (Azure AD or Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="97bce-136">请求</span><span class="sxs-lookup"><span data-stu-id="97bce-136">Request</span></span>

<span data-ttu-id="97bce-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="97bce-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_socialidentityprovider_from_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/Amazon-OAUTH
```

---

#### <a name="response"></a><span data-ttu-id="97bce-138">响应</span><span class="sxs-lookup"><span data-stu-id="97bce-138">Response</span></span>

<span data-ttu-id="97bce-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="97bce-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.socialIdentityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "displayName": "Amazon",
    "identityProviderType": "Amazon",
    "clientId": "09876545678908765978678",
    "clientSecret": "******"
}
```

### <a name="example-2-retrieve-a-specific-built-in-identity-provider-only-for-azure-ad"></a><span data-ttu-id="97bce-140">示例 2：仅为Azure AD (检索特定的内置标识) </span><span class="sxs-lookup"><span data-stu-id="97bce-140">Example 2: Retrieve a specific **built-in identity provider** (only for Azure AD)</span></span>

#### <a name="request"></a><span data-ttu-id="97bce-141">请求</span><span class="sxs-lookup"><span data-stu-id="97bce-141">Request</span></span>

<span data-ttu-id="97bce-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="97bce-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_builtinidentityprovider_from_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/MSASignup-OAUTH
```

---

#### <a name="response"></a><span data-ttu-id="97bce-143">响应</span><span class="sxs-lookup"><span data-stu-id="97bce-143">Response</span></span>

<span data-ttu-id="97bce-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="97bce-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.builtInIdentityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "MSASignup-OAUTH",
    "identityProviderType": "MicrosoftAccount",
    "displayName": "MicrosoftAccount"
}
```

### <a name="example-3-retrieve-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="97bce-145">示例 3：仅为 Azure AD B2C (检索特定的 **OpenID Connect** 标识) </span><span class="sxs-lookup"><span data-stu-id="97bce-145">Example 3: Retrieve a specific **OpenID Connect identity provider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="97bce-146">请求</span><span class="sxs-lookup"><span data-stu-id="97bce-146">Request</span></span>

<span data-ttu-id="97bce-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="97bce-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_openidconnectidentityprovider_from_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/OIDC-V1-test-icm-4470de58-86c2-4a3f-a22c-63c9366cd000
```

---

#### <a name="response"></a><span data-ttu-id="97bce-148">响应</span><span class="sxs-lookup"><span data-stu-id="97bce-148">Response</span></span>

<span data-ttu-id="97bce-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="97bce-149">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
  "id": "OIDC-V1-test-icm-4470de58-86c2-4a3f-a22c-63c9366cd000",
  "displayName": "Login with the Contoso identity provider",
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

### <a name="example-4-retrieves-apple-identity-provideronly-for-azure-ad-b2c"></a><span data-ttu-id="97bce-150">示例 4：仅为 Azure AD B2C (检索 Apple 标识) </span><span class="sxs-lookup"><span data-stu-id="97bce-150">Example 4: Retrieves Apple identity provider(only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="97bce-151">请求</span><span class="sxs-lookup"><span data-stu-id="97bce-151">Request</span></span>

<span data-ttu-id="97bce-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="97bce-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_applemanagedidentityprovider_from_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/Apple-Managed-OIDC
```

---

#### <a name="response"></a><span data-ttu-id="97bce-153">响应</span><span class="sxs-lookup"><span data-stu-id="97bce-153">Response</span></span>

<span data-ttu-id="97bce-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="97bce-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Apple-Managed-OIDC",
    "displayName": "Sign in with Apple",
    "developerId": "UBF8T346G9",
    "serviceId": "com.microsoft.rts.b2c.test.client",
    "keyId": "99P6D879C4",
    "certificateData": "******"
}
```
