---
title: 列出 userflowidentityproviders
description: 列出 b2cIdentityUserFlow 中所有标识提供程序。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 04d45c4fc622b24f3d9a04410ec010e08c45e3ad
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439742"
---
# <a name="list-a-userflowidentityproviders"></a><span data-ttu-id="3fa34-103">列出 userflowidentityproviders</span><span class="sxs-lookup"><span data-stu-id="3fa34-103">List a userflowidentityproviders</span></span>

<span data-ttu-id="3fa34-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fa34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fa34-105">获取 [b2cIdentityUserFlow 对象中的标识](../resources/b2cidentityuserflow.md) 提供程序。</span><span class="sxs-lookup"><span data-stu-id="3fa34-105">Get the identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fa34-106">权限</span><span class="sxs-lookup"><span data-stu-id="3fa34-106">Permissions</span></span>

<span data-ttu-id="3fa34-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3fa34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fa34-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3fa34-109">Permission type</span></span>      | <span data-ttu-id="3fa34-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3fa34-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fa34-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3fa34-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3fa34-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa34-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3fa34-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3fa34-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3fa34-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3fa34-114">Not supported.</span></span>|
|<span data-ttu-id="3fa34-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3fa34-115">Application</span></span>| <span data-ttu-id="3fa34-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa34-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="3fa34-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="3fa34-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="3fa34-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="3fa34-118">Global administrator</span></span>
* <span data-ttu-id="3fa34-119">外部 ID 用户流管理员</span><span class="sxs-lookup"><span data-stu-id="3fa34-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3fa34-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3fa34-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders
```

## <a name="request-headers"></a><span data-ttu-id="3fa34-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3fa34-121">Request headers</span></span>

|<span data-ttu-id="3fa34-122">名称</span><span class="sxs-lookup"><span data-stu-id="3fa34-122">Name</span></span>|<span data-ttu-id="3fa34-123">说明</span><span class="sxs-lookup"><span data-stu-id="3fa34-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3fa34-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fa34-124">Authorization</span></span>|<span data-ttu-id="3fa34-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3fa34-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fa34-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3fa34-127">Request body</span></span>

<span data-ttu-id="3fa34-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3fa34-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fa34-129">响应</span><span class="sxs-lookup"><span data-stu-id="3fa34-129">Response</span></span>

<span data-ttu-id="3fa34-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [identityProviders](../resources/identityproviderbase.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3fa34-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityproviderbase.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fa34-131">示例</span><span class="sxs-lookup"><span data-stu-id="3fa34-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fa34-132">请求</span><span class="sxs-lookup"><span data-stu-id="3fa34-132">Request</span></span>

<span data-ttu-id="3fa34-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3fa34-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3fa34-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3fa34-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlow_list_userflowidentityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders
```
# <a name="c"></a>[<span data-ttu-id="3fa34-135">C#</span><span class="sxs-lookup"><span data-stu-id="3fa34-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cuserflow-list-userflowidentityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3fa34-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3fa34-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cuserflow-list-userflowidentityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3fa34-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3fa34-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cuserflow-list-userflowidentityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3fa34-138">Java</span><span class="sxs-lookup"><span data-stu-id="3fa34-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cuserflow-list-userflowidentityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3fa34-139">响应</span><span class="sxs-lookup"><span data-stu-id="3fa34-139">Response</span></span>

<span data-ttu-id="3fa34-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3fa34-140">The following is an example of the response.</span></span>
><span data-ttu-id="3fa34-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3fa34-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.identityProviderBase)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.openIdConnectIdentityProvider",
            "id": "OIDC-V1-AD_Test-3e393390-ed2d-4794-97f6-5c1a1ccc61f7",
            "displayName": "OIDC AD Test",
            "clientId": "fe1b1576-adca-4bef-b321-076fde19950b",
            "clientSecret": "******",
            "scope": "openid",
            "metadataUrl": "https://login.microsoftonline.com/contoso.com/.well-known/openid-configuration",
            "domainHint": "",
            "responseType": "code",
            "responseMode": "form_post",
            "claimsMapping": {
                "userId": "oid",
                "displayName": "samuel",
                "givenName": "samuel",
                "surname": "emmense",
                "email": "sam.e@contoso.com"
            }
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "Apple-Managed-OIDC",
            "displayName": "Sign in with Apple",
            "identityProviderType": "AppleManaged",
            "clientId": "com.contoso.client",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "MSA-OIDC",
            "displayName": "Microsoft Account",
            "identityProviderType": "Microsoft",
            "clientId": "1e02ac8a-0c37-4046-abe4-35098a840090",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "Facebook-OAUTH",
            "displayName": "Facebook",
            "identityProviderType": "Facebook",
            "clientId": "576628889930009",
            "clientSecret": "******"
        }
    ]
}
```
