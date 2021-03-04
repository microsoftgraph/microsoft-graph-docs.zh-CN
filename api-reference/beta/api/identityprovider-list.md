---
title: 列出 identityProvider
description: 检索 identityProvider 对象的列表。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 80f44a6fd00d6bc9720911e96f45e68950177ab7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435432"
---
# <a name="list-identityproviders"></a><span data-ttu-id="f37ca-103">列出 identityProvider</span><span class="sxs-lookup"><span data-stu-id="f37ca-103">List identityProviders</span></span>

<span data-ttu-id="f37ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f37ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f37ca-105">检索 [identityProviders 对象](../resources/identityprovider.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="f37ca-105">Retrieve a list of [identityProviders](../resources/identityprovider.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f37ca-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f37ca-106">Permissions</span></span>

<span data-ttu-id="f37ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f37ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f37ca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f37ca-109">Permission type</span></span>      | <span data-ttu-id="f37ca-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f37ca-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f37ca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f37ca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f37ca-112">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f37ca-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="f37ca-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="f37ca-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f37ca-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f37ca-114">Not supported.</span></span>|
|<span data-ttu-id="f37ca-115">Application</span><span class="sxs-lookup"><span data-stu-id="f37ca-115">Application</span></span>|<span data-ttu-id="f37ca-116">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f37ca-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="f37ca-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="f37ca-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="f37ca-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="f37ca-118">Global administrator</span></span>
* <span data-ttu-id="f37ca-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="f37ca-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f37ca-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f37ca-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="f37ca-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f37ca-121">Request headers</span></span>

|<span data-ttu-id="f37ca-122">名称</span><span class="sxs-lookup"><span data-stu-id="f37ca-122">Name</span></span>|<span data-ttu-id="f37ca-123">说明</span><span class="sxs-lookup"><span data-stu-id="f37ca-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f37ca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f37ca-124">Authorization</span></span>|<span data-ttu-id="f37ca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f37ca-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f37ca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f37ca-127">Request body</span></span>

<span data-ttu-id="f37ca-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f37ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f37ca-129">响应</span><span class="sxs-lookup"><span data-stu-id="f37ca-129">Response</span></span>

<span data-ttu-id="f37ca-130">如果成功，此方法返回响应代码和 `200 OK` [identityProvider](../resources/identityprovider.md) 和 [openIdConnectProvider](../resources/openIdConnectProvider.md) (仅针对响应正文中的 Azure AD B2C) 对象。</span><span class="sxs-lookup"><span data-stu-id="f37ca-130">If successful, this method returns a `200 OK` response code and a collection of [identityProvider](../resources/identityprovider.md) and [openIdConnectProvider](../resources/openIdConnectProvider.md) (only for Azure AD B2C) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f37ca-131">示例</span><span class="sxs-lookup"><span data-stu-id="f37ca-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f37ca-132">请求</span><span class="sxs-lookup"><span data-stu-id="f37ca-132">Request</span></span>

<span data-ttu-id="f37ca-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f37ca-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f37ca-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f37ca-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="f37ca-135">C#</span><span class="sxs-lookup"><span data-stu-id="f37ca-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f37ca-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f37ca-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f37ca-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f37ca-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f37ca-138">Java</span><span class="sxs-lookup"><span data-stu-id="f37ca-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f37ca-139">响应</span><span class="sxs-lookup"><span data-stu-id="f37ca-139">Response</span></span>

<span data-ttu-id="f37ca-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f37ca-140">The following is an example of the response.</span></span>

<span data-ttu-id="f37ca-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f37ca-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityProviders",
    "value": [
      {
          "@odata.type": "microsoft.graph.identityProvider",
          "id": "Amazon-OAUTH",
          "name": "Login with Amazon",
          "type": "Amazon",
          "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
          "clientSecret": "*****"
      },
      {
          "@odata.type": "microsoft.graph.openIdConnectProvider",
          "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
          "name": "Login with the Contoso identity provider",
          "type": "OpenIDConnect",
          "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
          "clientSecret": "*****",
          "claimsMapping": {
              "userId": "myUserId",
              "givenName": "myGivenName",
              "surname": "mySurname",
              "email": "myEmail",
              "displayName": "myDisplayName"
          },
          "domainHint": "contoso",
          "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
          "responseMode": "form_post",
          "responseType": "code",
          "scope": "openid"
      },
    ]
}
```


