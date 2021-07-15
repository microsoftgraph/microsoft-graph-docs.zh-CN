---
title: 列出 userflowidentityproviders
description: 列出 b2xIdentityUserFlow 中所有 identityProviders。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 5403bd03c06322bf91895609db601f2ccda4da9b
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439588"
---
# <a name="list-a-userflowidentityproviders"></a><span data-ttu-id="b01aa-103">列出 userflowidentityproviders</span><span class="sxs-lookup"><span data-stu-id="b01aa-103">List a userflowidentityproviders</span></span>

<span data-ttu-id="b01aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b01aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b01aa-105">获取 [b2xIdentityUserFlow 对象中的标识](../resources/b2xidentityuserflow.md) 提供程序。</span><span class="sxs-lookup"><span data-stu-id="b01aa-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b01aa-106">权限</span><span class="sxs-lookup"><span data-stu-id="b01aa-106">Permissions</span></span>

<span data-ttu-id="b01aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b01aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b01aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b01aa-109">Permission type</span></span>      | <span data-ttu-id="b01aa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b01aa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b01aa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b01aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b01aa-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b01aa-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="b01aa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b01aa-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b01aa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b01aa-114">Not supported.</span></span>|
|<span data-ttu-id="b01aa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b01aa-115">Application</span></span>| <span data-ttu-id="b01aa-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b01aa-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="b01aa-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="b01aa-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="b01aa-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="b01aa-118">Global administrator</span></span>
* <span data-ttu-id="b01aa-119">外部 ID 用户流管理员</span><span class="sxs-lookup"><span data-stu-id="b01aa-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="b01aa-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b01aa-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders
```

## <a name="request-headers"></a><span data-ttu-id="b01aa-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b01aa-121">Request headers</span></span>

|<span data-ttu-id="b01aa-122">名称</span><span class="sxs-lookup"><span data-stu-id="b01aa-122">Name</span></span>|<span data-ttu-id="b01aa-123">说明</span><span class="sxs-lookup"><span data-stu-id="b01aa-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b01aa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b01aa-124">Authorization</span></span>|<span data-ttu-id="b01aa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b01aa-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b01aa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b01aa-127">Request body</span></span>

<span data-ttu-id="b01aa-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b01aa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b01aa-129">响应</span><span class="sxs-lookup"><span data-stu-id="b01aa-129">Response</span></span>

<span data-ttu-id="b01aa-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [identityProviders](../resources/identityproviderbase.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b01aa-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityproviderbase.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b01aa-131">示例</span><span class="sxs-lookup"><span data-stu-id="b01aa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b01aa-132">请求</span><span class="sxs-lookup"><span data-stu-id="b01aa-132">Request</span></span>

<span data-ttu-id="b01aa-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b01aa-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b01aa-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b01aa-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_userflowIdentityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders
```
# <a name="c"></a>[<span data-ttu-id="b01aa-135">C#</span><span class="sxs-lookup"><span data-stu-id="b01aa-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflow-list-userflowidentityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b01aa-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b01aa-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflow-list-userflowidentityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b01aa-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b01aa-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflow-list-userflowidentityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b01aa-138">Java</span><span class="sxs-lookup"><span data-stu-id="b01aa-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflow-list-userflowidentityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b01aa-139">响应</span><span class="sxs-lookup"><span data-stu-id="b01aa-139">Response</span></span>

<span data-ttu-id="b01aa-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b01aa-140">The following is an example of the response.</span></span>

<span data-ttu-id="b01aa-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b01aa-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
            "@odata.type": "#microsoft.graph.builtInIdentityProvider",
            "id": "AADSignup-OAUTH",
            "displayName": "Azure Active Directory Sign up",
            "identityProviderType": "AADSignup"
        },
        {
            "@odata.type": "#microsoft.graph.builtInIdentityProvider",
            "id": "MSASignup-OAUTH",
            "displayName": "Microsoft Account (Preview)",
            "identityProviderType": "MicrosoftAccount"
        },
        {
            "@odata.type": "#microsoft.graph.builtInIdentityProvider",
            "id": "EmailOtpSignup-OAUTH",
            "displayName": "Email one-time passcode (Preview)",
            "identityProviderType": "EmailOTP"
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "Facebook-OAUTH",
            "displayName": "Facebook",
            "identityProviderType": "Facebook",
            "clientId": "clientIdFromFacebook",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "Google-OAuth",
            "type": "Google",
            "name": "Google",
            "clientId": "clientIdFromGoogle",
            "clientSecret": "*****"
        }
    ]
}

```
