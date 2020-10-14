---
title: 获取 passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: 读取 passwordlessMicrosoftAuthenticatorAuthenticationMethod 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1a92e7669df96efe69d8e793fc327a8c578ffcde
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457497"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethod"></a><span data-ttu-id="bf121-103">获取 passwordlessMicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bf121-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="bf121-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf121-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf121-105">检索用户的单一 [Microsoft 身份验证器 Passwordless 电话登录方法](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bf121-105">Retrieve a user's single [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="bf121-106">在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。</span><span class="sxs-lookup"><span data-stu-id="bf121-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="bf121-107">由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。</span><span class="sxs-lookup"><span data-stu-id="bf121-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf121-108">权限</span><span class="sxs-lookup"><span data-stu-id="bf121-108">Permissions</span></span>
<span data-ttu-id="bf121-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf121-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf121-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf121-111">Permission type</span></span>|<span data-ttu-id="bf121-112">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="bf121-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="bf121-113">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="bf121-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="bf121-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf121-114">Delegated (work or school account)</span></span>|<span data-ttu-id="bf121-115">UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、All 和 All</span><span class="sxs-lookup"><span data-stu-id="bf121-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="bf121-116">UserAuthenticationMethod、UserAuthenticationMethod 和所有</span><span class="sxs-lookup"><span data-stu-id="bf121-116">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="bf121-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf121-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf121-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf121-118">Not supported.</span></span>|<span data-ttu-id="bf121-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf121-119">Not supported.</span></span>
|<span data-ttu-id="bf121-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf121-120">Application</span></span>|<span data-ttu-id="bf121-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf121-121">Not supported.</span></span>|<span data-ttu-id="bf121-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf121-122">Not supported.</span></span>

<span data-ttu-id="bf121-123">对于在其他用户上执行管理的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="bf121-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="bf121-124">全局管理员</span><span class="sxs-lookup"><span data-stu-id="bf121-124">Global admin</span></span>
* <span data-ttu-id="bf121-125">全局读取者</span><span class="sxs-lookup"><span data-stu-id="bf121-125">Global reader</span></span>
* <span data-ttu-id="bf121-126">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="bf121-126">Privileged authentication admin</span></span>
* <span data-ttu-id="bf121-127">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="bf121-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="bf121-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf121-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bf121-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf121-129">Request headers</span></span>
|<span data-ttu-id="bf121-130">名称</span><span class="sxs-lookup"><span data-stu-id="bf121-130">Name</span></span>|<span data-ttu-id="bf121-131">说明</span><span class="sxs-lookup"><span data-stu-id="bf121-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bf121-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf121-132">Authorization</span></span>|<span data-ttu-id="bf121-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bf121-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf121-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf121-135">Request body</span></span>
<span data-ttu-id="bf121-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bf121-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf121-137">响应</span><span class="sxs-lookup"><span data-stu-id="bf121-137">Response</span></span>

<span data-ttu-id="bf121-138">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bf121-138">If successful, this method returns a `200 OK` response code and the requested [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bf121-139">示例</span><span class="sxs-lookup"><span data-stu-id="bf121-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bf121-140">请求</span><span class="sxs-lookup"><span data-stu-id="bf121-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bf121-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf121-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="bf121-142">C#</span><span class="sxs-lookup"><span data-stu-id="bf121-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf121-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf121-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf121-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf121-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="bf121-145">响应</span><span class="sxs-lookup"><span data-stu-id="bf121-145">Response</span></span>
<span data-ttu-id="bf121-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bf121-146">The following is an example of the response.</span></span>

<span data-ttu-id="bf121-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bf121-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1",
      "displayName": "My mobile phone",
      "creationDateTime": "2020-09-02T04:16:49Z"
  }
}
```

