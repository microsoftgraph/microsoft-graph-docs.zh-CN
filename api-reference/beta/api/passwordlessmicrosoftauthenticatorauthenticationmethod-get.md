---
title: 获取 passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: 读取 passwordlessMicrosoftAuthenticatorAuthenticationMethod 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3462fca79b04fa19f0a0d7302760f9a5267ea339
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968635"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethod"></a><span data-ttu-id="b1300-103">获取 passwordlessMicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b1300-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="b1300-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1300-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1300-105">检索用户的单一 [Microsoft 身份验证器 Passwordless 电话登录方法](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1300-105">Retrieve a user's single [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="b1300-106">在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。</span><span class="sxs-lookup"><span data-stu-id="b1300-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="b1300-107">由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。</span><span class="sxs-lookup"><span data-stu-id="b1300-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1300-108">权限</span><span class="sxs-lookup"><span data-stu-id="b1300-108">Permissions</span></span>
<span data-ttu-id="b1300-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1300-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1300-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1300-111">Permission type</span></span>|<span data-ttu-id="b1300-112">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="b1300-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="b1300-113">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="b1300-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="b1300-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1300-114">Delegated (work or school account)</span></span>|<span data-ttu-id="b1300-115">UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、All 和 All</span><span class="sxs-lookup"><span data-stu-id="b1300-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="b1300-116">UserAuthenticationMethod、UserAuthenticationMethod 和所有</span><span class="sxs-lookup"><span data-stu-id="b1300-116">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="b1300-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1300-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1300-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1300-118">Not supported.</span></span>|<span data-ttu-id="b1300-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1300-119">Not supported.</span></span>
|<span data-ttu-id="b1300-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1300-120">Application</span></span>|<span data-ttu-id="b1300-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1300-121">Not supported.</span></span>|<span data-ttu-id="b1300-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1300-122">Not supported.</span></span>

<span data-ttu-id="b1300-123">对于在其他用户上执行管理的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="b1300-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b1300-124">全局管理员</span><span class="sxs-lookup"><span data-stu-id="b1300-124">Global admin</span></span>
* <span data-ttu-id="b1300-125">全局读取者</span><span class="sxs-lookup"><span data-stu-id="b1300-125">Global reader</span></span>
* <span data-ttu-id="b1300-126">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="b1300-126">Privileged authentication admin</span></span>
* <span data-ttu-id="b1300-127">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="b1300-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b1300-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1300-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b1300-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1300-129">Request headers</span></span>
|<span data-ttu-id="b1300-130">名称</span><span class="sxs-lookup"><span data-stu-id="b1300-130">Name</span></span>|<span data-ttu-id="b1300-131">说明</span><span class="sxs-lookup"><span data-stu-id="b1300-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b1300-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1300-132">Authorization</span></span>|<span data-ttu-id="b1300-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b1300-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1300-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1300-135">Request body</span></span>
<span data-ttu-id="b1300-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b1300-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1300-137">响应</span><span class="sxs-lookup"><span data-stu-id="b1300-137">Response</span></span>

<span data-ttu-id="b1300-138">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1300-138">If successful, this method returns a `200 OK` response code and the requested [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b1300-139">示例</span><span class="sxs-lookup"><span data-stu-id="b1300-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1300-140">请求</span><span class="sxs-lookup"><span data-stu-id="b1300-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b1300-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1300-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="b1300-142">C#</span><span class="sxs-lookup"><span data-stu-id="b1300-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1300-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1300-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1300-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1300-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1300-145">Java</span><span class="sxs-lookup"><span data-stu-id="b1300-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b1300-146">响应</span><span class="sxs-lookup"><span data-stu-id="b1300-146">Response</span></span>
<span data-ttu-id="b1300-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b1300-147">The following is an example of the response.</span></span>

<span data-ttu-id="b1300-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b1300-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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

