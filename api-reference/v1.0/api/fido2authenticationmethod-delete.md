---
title: 删除 fido2AuthenticationMethod
description: 删除 fido2AuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8ffbb31e7c8c5fd992a2a8942c91566269e8f218
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201252"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="cf069-103">删除 fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cf069-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="cf069-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf069-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cf069-105">删除用户的 [FIDO2 安全密钥身份验证方法](../resources/fido2authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cf069-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf069-106">权限</span><span class="sxs-lookup"><span data-stu-id="cf069-106">Permissions</span></span>

<span data-ttu-id="cf069-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf069-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="cf069-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="cf069-109">Permissions acting on self</span></span>

|<span data-ttu-id="cf069-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf069-110">Permission type</span></span>      | <span data-ttu-id="cf069-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf069-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="cf069-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf069-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf069-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf069-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="cf069-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf069-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf069-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf069-115">Not supported.</span></span> |
| <span data-ttu-id="cf069-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf069-116">Application</span></span>                            | <span data-ttu-id="cf069-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf069-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="cf069-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="cf069-118">Permissions acting on other users</span></span>

|<span data-ttu-id="cf069-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf069-119">Permission type</span></span>      | <span data-ttu-id="cf069-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf069-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="cf069-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf069-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf069-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf069-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="cf069-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf069-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf069-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf069-124">Not supported.</span></span> |
| <span data-ttu-id="cf069-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf069-125">Application</span></span>                            | <span data-ttu-id="cf069-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf069-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="cf069-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="cf069-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="cf069-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="cf069-128">Global admin</span></span>
* <span data-ttu-id="cf069-129">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="cf069-129">Privileged authentication admin</span></span>
* <span data-ttu-id="cf069-130">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="cf069-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="cf069-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf069-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cf069-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf069-132">Request headers</span></span>
|<span data-ttu-id="cf069-133">名称</span><span class="sxs-lookup"><span data-stu-id="cf069-133">Name</span></span>|<span data-ttu-id="cf069-134">说明</span><span class="sxs-lookup"><span data-stu-id="cf069-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cf069-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf069-135">Authorization</span></span>|<span data-ttu-id="cf069-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf069-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf069-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf069-138">Request body</span></span>
<span data-ttu-id="cf069-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf069-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf069-140">响应</span><span class="sxs-lookup"><span data-stu-id="cf069-140">Response</span></span>

<span data-ttu-id="cf069-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cf069-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cf069-143">示例</span><span class="sxs-lookup"><span data-stu-id="cf069-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cf069-144">请求</span><span class="sxs-lookup"><span data-stu-id="cf069-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cf069-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf069-145">HTTP</span></span>](#tab/http)

# <a name="http"></a>[<span data-ttu-id="cf069-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf069-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="cf069-147">C#</span><span class="sxs-lookup"><span data-stu-id="cf069-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf069-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf069-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf069-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf069-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf069-150">Java</span><span class="sxs-lookup"><span data-stu-id="cf069-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cf069-151">响应</span><span class="sxs-lookup"><span data-stu-id="cf069-151">Response</span></span>
<span data-ttu-id="cf069-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cf069-152">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

