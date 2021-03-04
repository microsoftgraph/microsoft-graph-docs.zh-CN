---
title: 删除 microsoftAuthenticatorAuthenticationMethod
description: 删除 microsoftAuthenticatorAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ebbbe634869c0cfcb04fe1e641e9c789af3d2741
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443708"
---
# <a name="delete-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="630db-103">删除 microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="630db-103">Delete microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="630db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="630db-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="630db-105">删除 [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="630db-105">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="630db-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="630db-106">Permissions</span></span>

<span data-ttu-id="630db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="630db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="630db-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="630db-109">Permissions acting on self</span></span>

|<span data-ttu-id="630db-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="630db-110">Permission type</span></span>      | <span data-ttu-id="630db-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="630db-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="630db-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="630db-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="630db-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="630db-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="630db-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="630db-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="630db-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="630db-115">Not supported.</span></span> |
| <span data-ttu-id="630db-116">Application</span><span class="sxs-lookup"><span data-stu-id="630db-116">Application</span></span>                            | <span data-ttu-id="630db-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="630db-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="630db-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="630db-118">Permissions acting on other users</span></span>

|<span data-ttu-id="630db-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="630db-119">Permission type</span></span>      | <span data-ttu-id="630db-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="630db-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="630db-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="630db-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="630db-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="630db-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="630db-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="630db-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="630db-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="630db-124">Not supported.</span></span> |
| <span data-ttu-id="630db-125">Application</span><span class="sxs-lookup"><span data-stu-id="630db-125">Application</span></span>                            | <span data-ttu-id="630db-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="630db-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="630db-127">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="630db-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="630db-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="630db-128">Global admin</span></span>
* <span data-ttu-id="630db-129">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="630db-129">Privileged authentication admin</span></span>
* <span data-ttu-id="630db-130">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="630db-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="630db-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="630db-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
DELETE /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="request-headers"></a><span data-ttu-id="630db-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="630db-132">Request headers</span></span>
|<span data-ttu-id="630db-133">名称</span><span class="sxs-lookup"><span data-stu-id="630db-133">Name</span></span>|<span data-ttu-id="630db-134">说明</span><span class="sxs-lookup"><span data-stu-id="630db-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="630db-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="630db-135">Authorization</span></span>|<span data-ttu-id="630db-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="630db-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="630db-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="630db-138">Request body</span></span>
<span data-ttu-id="630db-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="630db-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="630db-140">响应</span><span class="sxs-lookup"><span data-stu-id="630db-140">Response</span></span>

<span data-ttu-id="630db-141">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="630db-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="630db-142">示例</span><span class="sxs-lookup"><span data-stu-id="630db-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="630db-143">请求</span><span class="sxs-lookup"><span data-stu-id="630db-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="630db-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="630db-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="630db-145">C#</span><span class="sxs-lookup"><span data-stu-id="630db-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-microsoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="630db-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="630db-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-microsoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="630db-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="630db-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-microsoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="630db-148">Java</span><span class="sxs-lookup"><span data-stu-id="630db-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-microsoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="630db-149">响应</span><span class="sxs-lookup"><span data-stu-id="630db-149">Response</span></span>
<span data-ttu-id="630db-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="630db-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

