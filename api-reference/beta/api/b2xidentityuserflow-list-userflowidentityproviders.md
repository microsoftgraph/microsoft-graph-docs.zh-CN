---
title: 列出 userflowidentityproviders
description: 列出 b2xIdentityUserFlow 中所有 identityProviders。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 63bf686abbe51a9abd132e71d1e4472fc45c0849
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401071"
---
# <a name="list-a-userflowidentityproviders"></a><span data-ttu-id="bd660-103">列出 userflowidentityproviders</span><span class="sxs-lookup"><span data-stu-id="bd660-103">List a userflowidentityproviders</span></span>

<span data-ttu-id="bd660-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd660-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd660-105">获取 [b2xIdentityUserFlow 对象中的标识](../resources/b2xidentityuserflow.md) 提供程序。</span><span class="sxs-lookup"><span data-stu-id="bd660-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd660-106">权限</span><span class="sxs-lookup"><span data-stu-id="bd660-106">Permissions</span></span>

<span data-ttu-id="bd660-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd660-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd660-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd660-109">Permission type</span></span>      | <span data-ttu-id="bd660-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd660-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd660-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd660-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bd660-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd660-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="bd660-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd660-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="bd660-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd660-114">Not supported.</span></span>|
|<span data-ttu-id="bd660-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd660-115">Application</span></span>| <span data-ttu-id="bd660-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd660-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="bd660-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="bd660-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="bd660-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="bd660-118">Global administrator</span></span>
* <span data-ttu-id="bd660-119">外部 ID 用户流管理员</span><span class="sxs-lookup"><span data-stu-id="bd660-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="bd660-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd660-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders
```

## <a name="request-headers"></a><span data-ttu-id="bd660-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd660-121">Request headers</span></span>

|<span data-ttu-id="bd660-122">名称</span><span class="sxs-lookup"><span data-stu-id="bd660-122">Name</span></span>|<span data-ttu-id="bd660-123">说明</span><span class="sxs-lookup"><span data-stu-id="bd660-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="bd660-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd660-124">Authorization</span></span>|<span data-ttu-id="bd660-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bd660-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd660-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd660-127">Request body</span></span>

<span data-ttu-id="bd660-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd660-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd660-129">响应</span><span class="sxs-lookup"><span data-stu-id="bd660-129">Response</span></span>

<span data-ttu-id="bd660-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [identityProviders](../resources/identityproviderbase.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd660-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityproviderbase.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd660-131">示例</span><span class="sxs-lookup"><span data-stu-id="bd660-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd660-132">请求</span><span class="sxs-lookup"><span data-stu-id="bd660-132">Request</span></span>

<span data-ttu-id="bd660-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bd660-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_userflowIdentityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders
```

### <a name="response"></a><span data-ttu-id="bd660-134">响应</span><span class="sxs-lookup"><span data-stu-id="bd660-134">Response</span></span>

<span data-ttu-id="bd660-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bd660-135">The following is an example of the response.</span></span>

<span data-ttu-id="bd660-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bd660-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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
