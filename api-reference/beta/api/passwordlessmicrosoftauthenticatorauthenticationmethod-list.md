---
title: 列出 passwordlessMicrosoftAuthenticatorAuthenticationMethods
description: 检索无密码MicrosoftAuthenticatorAuthenticationMethod 对象及其属性的列表。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 340eea7eab990f1164b7b19bcb6bb2f9643b1d66
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515945"
---
# <a name="list-passwordlessmicrosoftauthenticatorauthenticationmethods-deprecated"></a><span data-ttu-id="e8577-103">列出已弃 (passwordlessMicrosoftAuthenticatorAuthenticationMethods) </span><span class="sxs-lookup"><span data-stu-id="e8577-103">List passwordlessMicrosoftAuthenticatorAuthenticationMethods (deprecated)</span></span>
<span data-ttu-id="e8577-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8577-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8577-105">检索用户的 [Microsoft Authenticator Passwordless Phone Sign-in 方法](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="e8577-105">Retrieve a list of a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

> [!CAUTION]
> <span data-ttu-id="e8577-106">Microsoft Authenticator 无密码电话登录方法 API 已弃用，将于 2020 年 12 月 31 日停止返回结果。</span><span class="sxs-lookup"><span data-stu-id="e8577-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="e8577-107">请使用新的 [Microsoft Authenticator 身份验证方法](../resources/microsoftAuthenticatorAuthenticationMethod.md)。</span><span class="sxs-lookup"><span data-stu-id="e8577-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e8577-108">权限</span><span class="sxs-lookup"><span data-stu-id="e8577-108">Permissions</span></span>

<span data-ttu-id="e8577-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8577-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="e8577-111">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="e8577-111">Permissions acting on self</span></span>

|<span data-ttu-id="e8577-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8577-112">Permission type</span></span>      | <span data-ttu-id="e8577-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8577-113">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="e8577-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8577-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8577-115">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8577-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="e8577-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8577-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8577-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8577-117">Not supported.</span></span> |
| <span data-ttu-id="e8577-118">Application</span><span class="sxs-lookup"><span data-stu-id="e8577-118">Application</span></span>                            | <span data-ttu-id="e8577-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8577-119">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="e8577-120">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="e8577-120">Permissions acting on other users</span></span>

|<span data-ttu-id="e8577-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8577-121">Permission type</span></span>      | <span data-ttu-id="e8577-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8577-122">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="e8577-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8577-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8577-124">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8577-124">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="e8577-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8577-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8577-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8577-126">Not supported.</span></span> |
| <span data-ttu-id="e8577-127">Application</span><span class="sxs-lookup"><span data-stu-id="e8577-127">Application</span></span>                            | <span data-ttu-id="e8577-128">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8577-128">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="e8577-129">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="e8577-129">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="e8577-130">全局管理员</span><span class="sxs-lookup"><span data-stu-id="e8577-130">Global admin</span></span>
* <span data-ttu-id="e8577-131">全局读取者</span><span class="sxs-lookup"><span data-stu-id="e8577-131">Global reader</span></span>
* <span data-ttu-id="e8577-132">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="e8577-132">Privileged authentication admin</span></span>
* <span data-ttu-id="e8577-133">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="e8577-133">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="e8577-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8577-134">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8577-135">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e8577-135">Optional query parameters</span></span>
<span data-ttu-id="e8577-136">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="e8577-136">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8577-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8577-137">Request headers</span></span>
|<span data-ttu-id="e8577-138">名称</span><span class="sxs-lookup"><span data-stu-id="e8577-138">Name</span></span>|<span data-ttu-id="e8577-139">说明</span><span class="sxs-lookup"><span data-stu-id="e8577-139">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e8577-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8577-140">Authorization</span></span>|<span data-ttu-id="e8577-141">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="e8577-141">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8577-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8577-142">Request body</span></span>
<span data-ttu-id="e8577-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8577-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8577-144">响应</span><span class="sxs-lookup"><span data-stu-id="e8577-144">Response</span></span>

<span data-ttu-id="e8577-145">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [无密码MicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e8577-145">If successful, this method returns a `200 OK` response code and a collection of [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8577-146">示例</span><span class="sxs-lookup"><span data-stu-id="e8577-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8577-147">请求</span><span class="sxs-lookup"><span data-stu-id="e8577-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e8577-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8577-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods
```
# <a name="c"></a>[<span data-ttu-id="e8577-149">C#</span><span class="sxs-lookup"><span data-stu-id="e8577-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8577-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8577-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8577-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8577-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8577-152">Java</span><span class="sxs-lookup"><span data-stu-id="e8577-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e8577-153">响应</span><span class="sxs-lookup"><span data-stu-id="e8577-153">Response</span></span>
<span data-ttu-id="e8577-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e8577-154">The following is an example of the response.</span></span>

<span data-ttu-id="e8577-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e8577-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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

