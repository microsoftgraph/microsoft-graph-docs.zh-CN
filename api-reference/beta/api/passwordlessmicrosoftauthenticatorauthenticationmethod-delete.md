---
title: 删除 passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: 删除一个 passwordlessMicrosoftAuthenticatorAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce55978f153bca32fb2f34a33947d612340f2dc6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968643"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethod"></a><span data-ttu-id="78910-103">删除 passwordlessMicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="78910-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="78910-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78910-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78910-105">删除用户的 [Microsoft 身份验证 Passwordless Phone 登录方法](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78910-105">Deletes a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="78910-106">在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。</span><span class="sxs-lookup"><span data-stu-id="78910-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="78910-107">由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。</span><span class="sxs-lookup"><span data-stu-id="78910-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>


## <a name="permissions"></a><span data-ttu-id="78910-108">权限</span><span class="sxs-lookup"><span data-stu-id="78910-108">Permissions</span></span>
<span data-ttu-id="78910-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78910-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78910-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="78910-111">Permission type</span></span>|<span data-ttu-id="78910-112">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="78910-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="78910-113">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="78910-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="78910-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78910-114">Delegated (work or school account)</span></span>|<span data-ttu-id="78910-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="78910-115">Not supported.</span></span>|<span data-ttu-id="78910-116">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="78910-116">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="78910-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78910-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78910-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="78910-118">Not supported.</span></span>|<span data-ttu-id="78910-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="78910-119">Not supported.</span></span>
|<span data-ttu-id="78910-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="78910-120">Application</span></span>|<span data-ttu-id="78910-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="78910-121">Not supported.</span></span>|<span data-ttu-id="78910-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="78910-122">Not supported.</span></span>

<span data-ttu-id="78910-123">对于在其他用户上执行管理的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="78910-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="78910-124">全局管理员</span><span class="sxs-lookup"><span data-stu-id="78910-124">Global admin</span></span>
* <span data-ttu-id="78910-125">全局读取者</span><span class="sxs-lookup"><span data-stu-id="78910-125">Global reader</span></span>
* <span data-ttu-id="78910-126">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="78910-126">Privileged authentication admin</span></span>
* <span data-ttu-id="78910-127">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="78910-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="78910-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78910-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="78910-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="78910-129">Request headers</span></span>
|<span data-ttu-id="78910-130">名称</span><span class="sxs-lookup"><span data-stu-id="78910-130">Name</span></span>|<span data-ttu-id="78910-131">说明</span><span class="sxs-lookup"><span data-stu-id="78910-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="78910-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="78910-132">Authorization</span></span>|<span data-ttu-id="78910-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78910-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="78910-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="78910-135">Request body</span></span>
<span data-ttu-id="78910-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="78910-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78910-137">响应</span><span class="sxs-lookup"><span data-stu-id="78910-137">Response</span></span>

<span data-ttu-id="78910-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="78910-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="78910-140">示例</span><span class="sxs-lookup"><span data-stu-id="78910-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="78910-141">请求</span><span class="sxs-lookup"><span data-stu-id="78910-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="78910-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="78910-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="78910-143">C#</span><span class="sxs-lookup"><span data-stu-id="78910-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78910-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78910-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78910-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78910-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78910-146">Java</span><span class="sxs-lookup"><span data-stu-id="78910-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="78910-147">响应</span><span class="sxs-lookup"><span data-stu-id="78910-147">Response</span></span>
<span data-ttu-id="78910-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="78910-148">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

