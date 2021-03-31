---
title: 删除 microsoftAuthenticatorAuthenticationMethod
description: 删除 microsoftAuthenticatorAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7b77c27db8f1fd26503e9f45da179b42425af504
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469204"
---
# <a name="delete-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="eec07-103">删除 microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="eec07-103">Delete microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="eec07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eec07-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eec07-105">删除 [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eec07-105">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eec07-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="eec07-106">Permissions</span></span>

<span data-ttu-id="eec07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eec07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="eec07-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="eec07-109">Permissions acting on self</span></span>

|<span data-ttu-id="eec07-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eec07-110">Permission type</span></span>      | <span data-ttu-id="eec07-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eec07-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="eec07-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eec07-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="eec07-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eec07-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="eec07-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eec07-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eec07-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eec07-115">Not supported.</span></span> |
| <span data-ttu-id="eec07-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="eec07-116">Application</span></span>                            | <span data-ttu-id="eec07-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="eec07-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="eec07-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="eec07-118">Permissions acting on other users</span></span>

|<span data-ttu-id="eec07-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="eec07-119">Permission type</span></span>      | <span data-ttu-id="eec07-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eec07-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="eec07-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eec07-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="eec07-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eec07-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="eec07-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eec07-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eec07-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="eec07-124">Not supported.</span></span> |
| <span data-ttu-id="eec07-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="eec07-125">Application</span></span>                            | <span data-ttu-id="eec07-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eec07-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="eec07-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="eec07-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="eec07-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="eec07-128">Global admin</span></span>
* <span data-ttu-id="eec07-129">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="eec07-129">Privileged authentication admin</span></span>
* <span data-ttu-id="eec07-130">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="eec07-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="eec07-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eec07-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
DELETE /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="request-headers"></a><span data-ttu-id="eec07-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="eec07-132">Request headers</span></span>
|<span data-ttu-id="eec07-133">名称</span><span class="sxs-lookup"><span data-stu-id="eec07-133">Name</span></span>|<span data-ttu-id="eec07-134">说明</span><span class="sxs-lookup"><span data-stu-id="eec07-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eec07-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="eec07-135">Authorization</span></span>|<span data-ttu-id="eec07-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eec07-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eec07-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="eec07-138">Request body</span></span>
<span data-ttu-id="eec07-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eec07-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eec07-140">响应</span><span class="sxs-lookup"><span data-stu-id="eec07-140">Response</span></span>

<span data-ttu-id="eec07-141">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="eec07-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="eec07-142">示例</span><span class="sxs-lookup"><span data-stu-id="eec07-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eec07-143">请求</span><span class="sxs-lookup"><span data-stu-id="eec07-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eec07-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="eec07-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/users/kim@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="eec07-145">C#</span><span class="sxs-lookup"><span data-stu-id="eec07-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-microsoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eec07-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eec07-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-microsoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eec07-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eec07-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-microsoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eec07-148">Java</span><span class="sxs-lookup"><span data-stu-id="eec07-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-microsoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="eec07-149">响应</span><span class="sxs-lookup"><span data-stu-id="eec07-149">Response</span></span>
<span data-ttu-id="eec07-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="eec07-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

