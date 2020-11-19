---
title: 删除 passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: 删除一个 passwordlessMicrosoftAuthenticatorAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 42d7ffe92488a7166356b0e43688a17f2935b503
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352387"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethod"></a><span data-ttu-id="518ec-103">删除 passwordlessMicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="518ec-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="518ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="518ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="518ec-105">删除用户的 [Microsoft 身份验证 Passwordless Phone 登录方法](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="518ec-105">Deletes a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="518ec-106">在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。</span><span class="sxs-lookup"><span data-stu-id="518ec-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="518ec-107">由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。</span><span class="sxs-lookup"><span data-stu-id="518ec-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>


## <a name="permissions"></a><span data-ttu-id="518ec-108">权限</span><span class="sxs-lookup"><span data-stu-id="518ec-108">Permissions</span></span>
<span data-ttu-id="518ec-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="518ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="518ec-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="518ec-111">Permission type</span></span>|<span data-ttu-id="518ec-112">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="518ec-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="518ec-113">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="518ec-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="518ec-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="518ec-114">Delegated (work or school account)</span></span>|<span data-ttu-id="518ec-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="518ec-115">Not supported.</span></span>|<span data-ttu-id="518ec-116">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="518ec-116">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="518ec-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="518ec-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="518ec-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="518ec-118">Not supported.</span></span>|<span data-ttu-id="518ec-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="518ec-119">Not supported.</span></span>
|<span data-ttu-id="518ec-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="518ec-120">Application</span></span>|<span data-ttu-id="518ec-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="518ec-121">Not supported.</span></span>|<span data-ttu-id="518ec-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="518ec-122">Not supported.</span></span>

<span data-ttu-id="518ec-123">对于在其他用户上执行管理的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="518ec-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="518ec-124">全局管理员</span><span class="sxs-lookup"><span data-stu-id="518ec-124">Global admin</span></span>
* <span data-ttu-id="518ec-125">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="518ec-125">Privileged authentication admin</span></span>
* <span data-ttu-id="518ec-126">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="518ec-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="518ec-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="518ec-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="518ec-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="518ec-128">Request headers</span></span>
|<span data-ttu-id="518ec-129">名称</span><span class="sxs-lookup"><span data-stu-id="518ec-129">Name</span></span>|<span data-ttu-id="518ec-130">说明</span><span class="sxs-lookup"><span data-stu-id="518ec-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="518ec-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="518ec-131">Authorization</span></span>|<span data-ttu-id="518ec-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="518ec-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="518ec-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="518ec-134">Request body</span></span>
<span data-ttu-id="518ec-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="518ec-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="518ec-136">响应</span><span class="sxs-lookup"><span data-stu-id="518ec-136">Response</span></span>

<span data-ttu-id="518ec-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="518ec-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="518ec-139">示例</span><span class="sxs-lookup"><span data-stu-id="518ec-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="518ec-140">请求</span><span class="sxs-lookup"><span data-stu-id="518ec-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="518ec-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="518ec-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="518ec-142">C#</span><span class="sxs-lookup"><span data-stu-id="518ec-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="518ec-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="518ec-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="518ec-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="518ec-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="518ec-145">Java</span><span class="sxs-lookup"><span data-stu-id="518ec-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="518ec-146">响应</span><span class="sxs-lookup"><span data-stu-id="518ec-146">Response</span></span>
<span data-ttu-id="518ec-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="518ec-147">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

