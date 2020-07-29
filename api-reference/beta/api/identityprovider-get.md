---
title: 获取 identityProvider
description: 检索 Identityprovider.read.all 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 288c84eef3efc0ca8495b3d579a0e02607faf40d
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509720"
---
# <a name="get-identityprovider"></a><span data-ttu-id="73895-103">获取 identityProvider</span><span class="sxs-lookup"><span data-stu-id="73895-103">Get identityProvider</span></span>

<span data-ttu-id="73895-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73895-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73895-105">检索[identityprovider.read.all](../resources/identityprovider.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="73895-105">Retrieve the properties and relationships of an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="73895-106">权限</span><span class="sxs-lookup"><span data-stu-id="73895-106">Permissions</span></span>

<span data-ttu-id="73895-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73895-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73895-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73895-109">Permission type</span></span>      | <span data-ttu-id="73895-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73895-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73895-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73895-111">Delegated (work or school account)</span></span>|<span data-ttu-id="73895-112">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73895-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="73895-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="73895-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="73895-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73895-114">Not supported.</span></span>|
|<span data-ttu-id="73895-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="73895-115">Application</span></span>|<span data-ttu-id="73895-116">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73895-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="73895-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="73895-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="73895-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="73895-118">Global administrator</span></span>
* <span data-ttu-id="73895-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="73895-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="73895-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73895-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="73895-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="73895-121">Request headers</span></span>

|<span data-ttu-id="73895-122">名称</span><span class="sxs-lookup"><span data-stu-id="73895-122">Name</span></span>|<span data-ttu-id="73895-123">说明</span><span class="sxs-lookup"><span data-stu-id="73895-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="73895-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="73895-124">Authorization</span></span>|<span data-ttu-id="73895-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73895-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73895-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="73895-127">Request body</span></span>

<span data-ttu-id="73895-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73895-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73895-129">响应</span><span class="sxs-lookup"><span data-stu-id="73895-129">Response</span></span>

<span data-ttu-id="73895-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[Identityprovider.read.all](../resources/identityprovider.md)或[openIdConnectProvider](../resources/openidconnectprovider.md) （仅适用于 AZURE AD B2C）的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73895-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73895-131">示例</span><span class="sxs-lookup"><span data-stu-id="73895-131">Examples</span></span>

### <a name="example-1-retrieves-a-specific-identityprovider"></a><span data-ttu-id="73895-132">示例1：检索特定**identityprovider.read.all**</span><span class="sxs-lookup"><span data-stu-id="73895-132">Example 1: Retrieves a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="73895-133">请求</span><span class="sxs-lookup"><span data-stu-id="73895-133">Request</span></span>

<span data-ttu-id="73895-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="73895-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```

#### <a name="response"></a><span data-ttu-id="73895-135">响应</span><span class="sxs-lookup"><span data-stu-id="73895-135">Response</span></span>

<span data-ttu-id="73895-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="73895-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
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
### <a name="example-2-retrieves-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="73895-137">示例2：检索特定**openIDConnectProvider** （仅适用于 AZURE AD B2C）</span><span class="sxs-lookup"><span data-stu-id="73895-137">Example 2: Retrieves a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="73895-138">请求</span><span class="sxs-lookup"><span data-stu-id="73895-138">Request</span></span>

<span data-ttu-id="73895-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="73895-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```

#### <a name="response"></a><span data-ttu-id="73895-140">响应</span><span class="sxs-lookup"><span data-stu-id="73895-140">Response</span></span>

<span data-ttu-id="73895-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="73895-141">The following is an example of the response.</span></span>
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
