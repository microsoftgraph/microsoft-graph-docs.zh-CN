---
title: 列出 identityProvider
description: 检索 identityProviderbase 对象的列表。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 47e136bc63cd7b95bdcf3778047eb77db58c8de0
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921380"
---
# <a name="list-identityproviders"></a><span data-ttu-id="30a50-103">列出 identityProvider</span><span class="sxs-lookup"><span data-stu-id="30a50-103">List identityProviders</span></span>
<span data-ttu-id="30a50-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30a50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30a50-105">检索继承自  [identityProviderBase](../resources/identityproviderbase.md)的对象集合的列表。</span><span class="sxs-lookup"><span data-stu-id="30a50-105">Retrieve a list of collection of object inherited from  [identityProviderBase](../resources/identityproviderbase.md).</span></span>

<span data-ttu-id="30a50-106">对于 Azure AD 租户，它可以是 [socialIdentityProviders](../resources/socialidentityprovider.md) 和/或 [builtinIdentityProviders](../resources/builtinidentityprovider.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="30a50-106">For an Azure AD tenant it can be [socialIdentityProviders](../resources/socialidentityprovider.md) and/or [builtinIdentityProviders](../resources/builtinidentityprovider.md) objects.</span></span>

<span data-ttu-id="30a50-107">对于 Azure AD B2C 租户，它可以是 socialIdentityProviders、openIdConnectIdentityProviders 和/或[appleIdentityProvider](../resources/appleidentityprovider.md)对象。 [](../resources/socialidentityprovider.md) [](../resources/openidconnectidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="30a50-107">For an Azure AD B2C tenant it can be [socialIdentityProviders](../resources/socialidentityprovider.md), [openIdConnectIdentityProviders](../resources/openidconnectidentityprovider.md) and/or [appleIdentityProvider](../resources/appleidentityprovider.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="30a50-108">权限</span><span class="sxs-lookup"><span data-stu-id="30a50-108">Permissions</span></span>

<span data-ttu-id="30a50-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30a50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30a50-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="30a50-111">Permission type</span></span>      | <span data-ttu-id="30a50-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30a50-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30a50-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30a50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30a50-114">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30a50-114">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="30a50-115">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="30a50-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="30a50-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="30a50-116">Not supported.</span></span>|
|<span data-ttu-id="30a50-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="30a50-117">Application</span></span>|<span data-ttu-id="30a50-118">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30a50-118">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="30a50-119">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="30a50-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="30a50-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="30a50-120">Global Administrator</span></span>
* <span data-ttu-id="30a50-121">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="30a50-121">External Identity Provider Administrator</span></span>
* <span data-ttu-id="30a50-122">外部 ID 用户流管理员</span><span class="sxs-lookup"><span data-stu-id="30a50-122">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="30a50-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30a50-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="30a50-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="30a50-124">Request headers</span></span>

|<span data-ttu-id="30a50-125">名称</span><span class="sxs-lookup"><span data-stu-id="30a50-125">Name</span></span>|<span data-ttu-id="30a50-126">说明</span><span class="sxs-lookup"><span data-stu-id="30a50-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="30a50-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="30a50-127">Authorization</span></span>|<span data-ttu-id="30a50-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="30a50-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30a50-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="30a50-130">Request body</span></span>

<span data-ttu-id="30a50-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="30a50-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30a50-132">响应</span><span class="sxs-lookup"><span data-stu-id="30a50-132">Response</span></span>

<span data-ttu-id="30a50-133">如果成功，此方法在 Azure AD 租户的响应正文中返回 响应代码和 `200 OK` [socialIdentityProvider](../resources/socialidentityprovider.md) 和/或 [builtinIdentityProvider](../resources/builtinidentityprovider.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="30a50-133">If successful, this method returns a `200 OK` response code and a collection of [socialIdentityProvider](../resources/socialidentityprovider.md) and/or [builtinIdentityProvider](../resources/builtinidentityprovider.md) objects in the response body for an Azure AD tenant.</span></span>

<span data-ttu-id="30a50-134">对于 Azure AD B2C 租户，此方法在响应正文中返回 响应代码和 `200 OK` socialIdentityProvider、openIdConnectIdentityProvider 和/或[appleIdentityProvider](../resources/appleidentityprovider.md)对象的集合[](../resources/socialidentityprovider.md)[](../resources/openidconnectidentityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="30a50-134">For an Azure AD B2C tenant this method returns a `200 OK` response code and a collection of [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) and/or [appleIdentityProvider](../resources/appleidentityprovider.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30a50-135">示例</span><span class="sxs-lookup"><span data-stu-id="30a50-135">Example</span></span>

### <a name="example-1-list-all-identityprovider-configured-in-an-azure-ad-tenant"></a><span data-ttu-id="30a50-136">示例 1：列出在 Azure AD 租户中配置的所有 **identityProvider**</span><span class="sxs-lookup"><span data-stu-id="30a50-136">Example 1: List all **identityProvider** configured in an Azure AD tenant</span></span>

### <a name="request"></a><span data-ttu-id="30a50-137">请求</span><span class="sxs-lookup"><span data-stu-id="30a50-137">Request</span></span>
<span data-ttu-id="30a50-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="30a50-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="30a50-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="30a50-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="30a50-140">C#</span><span class="sxs-lookup"><span data-stu-id="30a50-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30a50-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30a50-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30a50-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30a50-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30a50-143">Java</span><span class="sxs-lookup"><span data-stu-id="30a50-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="30a50-144">响应</span><span class="sxs-lookup"><span data-stu-id="30a50-144">Response</span></span>
<span data-ttu-id="30a50-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="30a50-145">The following is an example of the response.</span></span>

<span data-ttu-id="30a50-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="30a50-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase",
  "isCollection": true
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/identityProviders",
   "value":[
      {
         "@odata.type": "microsoft.graph.builtInIdentityProvider",
         "id": "MSASignup-OAUTH",
         "identityProviderType": "MicrosoftAccount",
         "displayName": "MicrosoftAccount"
      },
      {
         "@odata.type": "#microsoft.graph.socialIdentityProvider",
         "id": "Facebook-OAUTH",
         "displayName": "Facebook",
         "identityProviderType": "Facebook",
         "clientId": "test",
         "clientSecret": "******"
      }
   ]
}
```

### <a name="example-2-list-all-identityprovider-configured-in-an-azure-ad-b2c-tenant"></a><span data-ttu-id="30a50-147">示例 2：列出在 Azure AD B2C 租户中配置的所有 **identityProvider**</span><span class="sxs-lookup"><span data-stu-id="30a50-147">Example 2: List all **identityProvider** configured in an Azure AD B2C tenant</span></span>

### <a name="request"></a><span data-ttu-id="30a50-148">请求</span><span class="sxs-lookup"><span data-stu-id="30a50-148">Request</span></span>
<span data-ttu-id="30a50-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="30a50-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders
```

### <a name="response"></a><span data-ttu-id="30a50-150">响应</span><span class="sxs-lookup"><span data-stu-id="30a50-150">Response</span></span>
<span data-ttu-id="30a50-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="30a50-151">The following is an example of the response.</span></span>

<span data-ttu-id="30a50-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="30a50-152">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/identityProviders",
    "value": [
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "LinkedIn-OAUTH",
            "displayName": "linkedin",
            "identityProviderType": "LinkedIn",
            "clientId": "866xc0qtyy00ih",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.openIdConnectIdentityProvider",
            "id": "OIDC-V1-rtt_AD_Test-3e393390-ed2d-4794-97f6-5c1a1ccc61f7",
            "displayName": "OIDC AD Test",
            "clientId": "fe1b3476-rdca-4bef-b321-076fde19750b",
            "clientSecret": "******",
            "scope": "openid",
            "metadataUrl": "https://login.microsoftonline.com/sashawho.onmicrosoft.com/.well-known/openid-configuration",
            "domainHint": "",
            "responseType": "code",
            "responseMode": "form_post",
            "claimsMapping": {
                "userId": "oid",
                "displayName": "name",
                "givenName": "given_name",
                "surname": "family_name",
                "email": "unique_email"
            }
        },
        {
            "@odata.type": "#microsoft.graph.appleManagedIdentityProvider",
            "id": "Apple-Managed-OIDC",
            "displayName": "Sign in with Apple",
            "developerId": "UBF8T346G9",
            "serviceId": "com.microsoft.aad.b2c.iuyt.client",
            "keyId": "99P6DD87C4",
            "certificateData": "******"
        }
    ]
}

```
