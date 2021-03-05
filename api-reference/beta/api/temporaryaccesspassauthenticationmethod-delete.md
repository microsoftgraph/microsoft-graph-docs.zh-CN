---
title: 删除 temporaryAccessPassAuthenticationMethod
description: 删除临时AccessPassAuthenticationMethod 对象。
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 31879dfc0d572f1914b15582ec515b0f8a44c85a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475088"
---
# <a name="delete-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="9658d-103">删除 temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9658d-103">Delete temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="9658d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9658d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9658d-105">删除 [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9658d-105">Delete a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

<span data-ttu-id="9658d-106">虽然当前用户的临时访问传递有效，但需要在用户上创建一个新的临时访问传递之前将其删除。</span><span class="sxs-lookup"><span data-stu-id="9658d-106">While the current Temporary Access Pass on the user is valid, it needs to be deleted before a new Temporary Access Pass can be created on the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="9658d-107">权限</span><span class="sxs-lookup"><span data-stu-id="9658d-107">Permissions</span></span>
<span data-ttu-id="9658d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9658d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="9658d-110">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="9658d-110">Permissions acting on self</span></span>

|<span data-ttu-id="9658d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9658d-111">Permission type</span></span>      | <span data-ttu-id="9658d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9658d-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="9658d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9658d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9658d-114">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9658d-114">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="9658d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9658d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9658d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9658d-116">Not supported.</span></span> |
| <span data-ttu-id="9658d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9658d-117">Application</span></span>                            | <span data-ttu-id="9658d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9658d-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="9658d-119">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="9658d-119">Permissions acting on other users</span></span>

|<span data-ttu-id="9658d-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="9658d-120">Permission type</span></span>      | <span data-ttu-id="9658d-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9658d-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="9658d-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9658d-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="9658d-123">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9658d-123">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="9658d-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9658d-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9658d-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="9658d-125">Not supported.</span></span> |
| <span data-ttu-id="9658d-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="9658d-126">Application</span></span>                            | <span data-ttu-id="9658d-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9658d-127">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="9658d-128">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="9658d-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="9658d-129">全局管理员</span><span class="sxs-lookup"><span data-stu-id="9658d-129">Global admin</span></span>
* <span data-ttu-id="9658d-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="9658d-130">Privileged authentication admin</span></span>
* <span data-ttu-id="9658d-131">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="9658d-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="9658d-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9658d-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{id}
DELETE /me/authentication/temporaryAccessPassMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9658d-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="9658d-133">Request headers</span></span>
|<span data-ttu-id="9658d-134">名称</span><span class="sxs-lookup"><span data-stu-id="9658d-134">Name</span></span>|<span data-ttu-id="9658d-135">说明</span><span class="sxs-lookup"><span data-stu-id="9658d-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9658d-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="9658d-136">Authorization</span></span>|<span data-ttu-id="9658d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9658d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9658d-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="9658d-139">Request body</span></span>
<span data-ttu-id="9658d-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9658d-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9658d-141">响应</span><span class="sxs-lookup"><span data-stu-id="9658d-141">Response</span></span>

<span data-ttu-id="9658d-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9658d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9658d-144">示例</span><span class="sxs-lookup"><span data-stu-id="9658d-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9658d-145">请求</span><span class="sxs-lookup"><span data-stu-id="9658d-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9658d-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="9658d-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_temporaryaccesspassauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="9658d-147">C#</span><span class="sxs-lookup"><span data-stu-id="9658d-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-temporaryaccesspassauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9658d-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9658d-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-temporaryaccesspassauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9658d-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9658d-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-temporaryaccesspassauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9658d-150">Java</span><span class="sxs-lookup"><span data-stu-id="9658d-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-temporaryaccesspassauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9658d-151">响应</span><span class="sxs-lookup"><span data-stu-id="9658d-151">Response</span></span>
<span data-ttu-id="9658d-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9658d-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
