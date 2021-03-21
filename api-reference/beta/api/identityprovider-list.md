---
title: 列出 identityProvider
description: 检索 identityProvider 对象的列表。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 2b988fa0aab5e59e165defc9f953cc267606dd84
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960977"
---
# <a name="list-identityproviders"></a><span data-ttu-id="671de-103">列出 identityProvider</span><span class="sxs-lookup"><span data-stu-id="671de-103">List identityProviders</span></span>

<span data-ttu-id="671de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="671de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="671de-105">检索 [identityProviders 对象](../resources/identityprovider.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="671de-105">Retrieve a list of [identityProviders](../resources/identityprovider.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="671de-106">权限</span><span class="sxs-lookup"><span data-stu-id="671de-106">Permissions</span></span>

<span data-ttu-id="671de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="671de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="671de-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="671de-109">Permission type</span></span>      | <span data-ttu-id="671de-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="671de-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="671de-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="671de-111">Delegated (work or school account)</span></span>|<span data-ttu-id="671de-112">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="671de-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="671de-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="671de-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="671de-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="671de-114">Not supported.</span></span>|
|<span data-ttu-id="671de-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="671de-115">Application</span></span>|<span data-ttu-id="671de-116">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="671de-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="671de-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="671de-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="671de-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="671de-118">Global administrator</span></span>
* <span data-ttu-id="671de-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="671de-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="671de-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="671de-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="671de-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="671de-121">Request headers</span></span>

|<span data-ttu-id="671de-122">名称</span><span class="sxs-lookup"><span data-stu-id="671de-122">Name</span></span>|<span data-ttu-id="671de-123">说明</span><span class="sxs-lookup"><span data-stu-id="671de-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="671de-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="671de-124">Authorization</span></span>|<span data-ttu-id="671de-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="671de-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="671de-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="671de-127">Request body</span></span>

<span data-ttu-id="671de-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="671de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="671de-129">响应</span><span class="sxs-lookup"><span data-stu-id="671de-129">Response</span></span>

<span data-ttu-id="671de-130">如果成功，此方法返回 响应代码和 `200 OK` [identityProvider](../resources/identityprovider.md) 和 [openIdConnectProvider](../resources/openIdConnectProvider.md) (仅适用于响应正文中的 Azure AD B2C) 对象。</span><span class="sxs-lookup"><span data-stu-id="671de-130">If successful, this method returns a `200 OK` response code and a collection of [identityProvider](../resources/identityprovider.md) and [openIdConnectProvider](../resources/openIdConnectProvider.md) (only for Azure AD B2C) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="671de-131">示例</span><span class="sxs-lookup"><span data-stu-id="671de-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="671de-132">请求</span><span class="sxs-lookup"><span data-stu-id="671de-132">Request</span></span>

<span data-ttu-id="671de-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="671de-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="671de-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="671de-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="671de-135">C#</span><span class="sxs-lookup"><span data-stu-id="671de-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="671de-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="671de-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="671de-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="671de-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="671de-138">Java</span><span class="sxs-lookup"><span data-stu-id="671de-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="671de-139">响应</span><span class="sxs-lookup"><span data-stu-id="671de-139">Response</span></span>

<span data-ttu-id="671de-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="671de-140">The following is an example of the response.</span></span>

<span data-ttu-id="671de-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="671de-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


