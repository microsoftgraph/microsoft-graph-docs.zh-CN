---
title: 列出 passwordlessMicrosoftAuthenticatorAuthenticationMethods
description: 检索 passwordlessMicrosoftAuthenticatorAuthenticationMethod 对象及其属性的列表。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b13ffdb6ff099eb45c73af66fff5877bfe4e7c9b
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457328"
---
# <a name="list-passwordlessmicrosoftauthenticatorauthenticationmethods"></a><span data-ttu-id="5b982-103">列出 passwordlessMicrosoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="5b982-103">List passwordlessMicrosoftAuthenticatorAuthenticationMethods</span></span>
<span data-ttu-id="5b982-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b982-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b982-105">检索用户的 [Microsoft 身份验证器 Passwordless 电话登录方法](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="5b982-105">Retrieve a list of a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

> [!NOTE]
> <span data-ttu-id="5b982-106">在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。</span><span class="sxs-lookup"><span data-stu-id="5b982-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="5b982-107">由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。</span><span class="sxs-lookup"><span data-stu-id="5b982-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b982-108">权限</span><span class="sxs-lookup"><span data-stu-id="5b982-108">Permissions</span></span>
<span data-ttu-id="5b982-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b982-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b982-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b982-111">Permission type</span></span>|<span data-ttu-id="5b982-112">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="5b982-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="5b982-113">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="5b982-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="5b982-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b982-114">Delegated (work or school account)</span></span>|<span data-ttu-id="5b982-115">UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、All 和 All</span><span class="sxs-lookup"><span data-stu-id="5b982-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="5b982-116">UserAuthenticationMethod、UserAuthenticationMethod 和所有</span><span class="sxs-lookup"><span data-stu-id="5b982-116">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="5b982-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b982-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b982-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b982-118">Not supported.</span></span>|<span data-ttu-id="5b982-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b982-119">Not supported.</span></span>
|<span data-ttu-id="5b982-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b982-120">Application</span></span>|<span data-ttu-id="5b982-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b982-121">Not supported.</span></span>|<span data-ttu-id="5b982-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b982-122">Not supported.</span></span>

<span data-ttu-id="5b982-123">对于在其他用户上执行管理的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="5b982-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="5b982-124">全局管理员</span><span class="sxs-lookup"><span data-stu-id="5b982-124">Global admin</span></span>
* <span data-ttu-id="5b982-125">全局读取者</span><span class="sxs-lookup"><span data-stu-id="5b982-125">Global reader</span></span>
* <span data-ttu-id="5b982-126">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="5b982-126">Privileged authentication admin</span></span>
* <span data-ttu-id="5b982-127">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="5b982-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="5b982-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b982-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b982-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5b982-129">Optional query parameters</span></span>
<span data-ttu-id="5b982-130">此方法不支持用于自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="5b982-130">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b982-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b982-131">Request headers</span></span>
|<span data-ttu-id="5b982-132">名称</span><span class="sxs-lookup"><span data-stu-id="5b982-132">Name</span></span>|<span data-ttu-id="5b982-133">说明</span><span class="sxs-lookup"><span data-stu-id="5b982-133">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5b982-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b982-134">Authorization</span></span>|<span data-ttu-id="5b982-135">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="5b982-135">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b982-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b982-136">Request body</span></span>
<span data-ttu-id="5b982-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5b982-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b982-138">响应</span><span class="sxs-lookup"><span data-stu-id="5b982-138">Response</span></span>

<span data-ttu-id="5b982-139">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5b982-139">If successful, this method returns a `200 OK` response code and a collection of [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b982-140">示例</span><span class="sxs-lookup"><span data-stu-id="5b982-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b982-141">请求</span><span class="sxs-lookup"><span data-stu-id="5b982-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5b982-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b982-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods
```
# <a name="c"></a>[<span data-ttu-id="5b982-143">C#</span><span class="sxs-lookup"><span data-stu-id="5b982-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b982-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b982-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b982-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b982-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5b982-146">响应</span><span class="sxs-lookup"><span data-stu-id="5b982-146">Response</span></span>
<span data-ttu-id="5b982-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5b982-147">The following is an example of the response.</span></span>

<span data-ttu-id="5b982-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5b982-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1",
      "displayName": "My mobile phone",
      "creationDateTime": "2020-09-02T04:16:49Z"
    },
    {
      "id": "J18B378Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJGM1",
      "displayName": "My tablet",
      "creationDateTime": "2020-09-02T03:36:19Z"
    }
  ]
}
```

