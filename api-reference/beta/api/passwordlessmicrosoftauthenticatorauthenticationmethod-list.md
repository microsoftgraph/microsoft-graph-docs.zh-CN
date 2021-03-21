---
title: 列出 passwordlessMicrosoftAuthenticatorAuthenticationMethods
description: 检索无密码MicrosoftAuthenticatorAuthenticationMethod 对象及其属性的列表。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 162ef913cbc69431e40365a447440f77a711dac1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962975"
---
# <a name="list-passwordlessmicrosoftauthenticatorauthenticationmethods-deprecated"></a><span data-ttu-id="72bb9-103">列出 passwordlessMicrosoftAuthenticatorAuthenticationMethods (弃) </span><span class="sxs-lookup"><span data-stu-id="72bb9-103">List passwordlessMicrosoftAuthenticatorAuthenticationMethods (deprecated)</span></span>
<span data-ttu-id="72bb9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72bb9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72bb9-105">检索用户的 Microsoft Authenticator 无密码 [电话登录方法](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="72bb9-105">Retrieve a list of a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

> [!CAUTION]
> <span data-ttu-id="72bb9-106">Microsoft Authenticator 无密码电话登录方法 API 已弃用，并且将于 2020 年 12 月 31 日停止返回结果。</span><span class="sxs-lookup"><span data-stu-id="72bb9-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="72bb9-107">请使用新的 [Microsoft Authenticator 身份验证方法](../resources/microsoftAuthenticatorAuthenticationMethod.md)。</span><span class="sxs-lookup"><span data-stu-id="72bb9-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="72bb9-108">权限</span><span class="sxs-lookup"><span data-stu-id="72bb9-108">Permissions</span></span>

<span data-ttu-id="72bb9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72bb9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="72bb9-111">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="72bb9-111">Permissions acting on self</span></span>

|<span data-ttu-id="72bb9-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="72bb9-112">Permission type</span></span>      | <span data-ttu-id="72bb9-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72bb9-113">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="72bb9-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72bb9-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="72bb9-115">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72bb9-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="72bb9-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72bb9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72bb9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="72bb9-117">Not supported.</span></span> |
| <span data-ttu-id="72bb9-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="72bb9-118">Application</span></span>                            | <span data-ttu-id="72bb9-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="72bb9-119">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="72bb9-120">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="72bb9-120">Permissions acting on other users</span></span>

|<span data-ttu-id="72bb9-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="72bb9-121">Permission type</span></span>      | <span data-ttu-id="72bb9-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72bb9-122">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="72bb9-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72bb9-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="72bb9-124">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72bb9-124">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="72bb9-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72bb9-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72bb9-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="72bb9-126">Not supported.</span></span> |
| <span data-ttu-id="72bb9-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="72bb9-127">Application</span></span>                            | <span data-ttu-id="72bb9-128">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72bb9-128">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="72bb9-129">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="72bb9-129">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="72bb9-130">全局管理员</span><span class="sxs-lookup"><span data-stu-id="72bb9-130">Global admin</span></span>
* <span data-ttu-id="72bb9-131">全局读取者</span><span class="sxs-lookup"><span data-stu-id="72bb9-131">Global reader</span></span>
* <span data-ttu-id="72bb9-132">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="72bb9-132">Privileged authentication admin</span></span>
* <span data-ttu-id="72bb9-133">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="72bb9-133">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="72bb9-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72bb9-134">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72bb9-135">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="72bb9-135">Optional query parameters</span></span>
<span data-ttu-id="72bb9-136">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="72bb9-136">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72bb9-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="72bb9-137">Request headers</span></span>
|<span data-ttu-id="72bb9-138">名称</span><span class="sxs-lookup"><span data-stu-id="72bb9-138">Name</span></span>|<span data-ttu-id="72bb9-139">说明</span><span class="sxs-lookup"><span data-stu-id="72bb9-139">Description</span></span>|
|:---|:---|
|<span data-ttu-id="72bb9-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="72bb9-140">Authorization</span></span>|<span data-ttu-id="72bb9-141">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="72bb9-141">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="72bb9-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="72bb9-142">Request body</span></span>
<span data-ttu-id="72bb9-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="72bb9-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72bb9-144">响应</span><span class="sxs-lookup"><span data-stu-id="72bb9-144">Response</span></span>

<span data-ttu-id="72bb9-145">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="72bb9-145">If successful, this method returns a `200 OK` response code and a collection of [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72bb9-146">示例</span><span class="sxs-lookup"><span data-stu-id="72bb9-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72bb9-147">请求</span><span class="sxs-lookup"><span data-stu-id="72bb9-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="72bb9-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="72bb9-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods
```
# <a name="c"></a>[<span data-ttu-id="72bb9-149">C#</span><span class="sxs-lookup"><span data-stu-id="72bb9-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72bb9-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72bb9-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72bb9-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72bb9-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72bb9-152">Java</span><span class="sxs-lookup"><span data-stu-id="72bb9-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordlessmicrosoftauthenticatorauthenticationmethod-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="72bb9-153">响应</span><span class="sxs-lookup"><span data-stu-id="72bb9-153">Response</span></span>
<span data-ttu-id="72bb9-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="72bb9-154">The following is an example of the response.</span></span>

<span data-ttu-id="72bb9-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="72bb9-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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

