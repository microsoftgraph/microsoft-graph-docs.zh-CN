---
title: 删除 fido2AuthenticationMethod
description: 删除 fido2AuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2ef78f3957f262b59bef7c627ea5450c2c759ab7
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469022"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="cffcc-103">删除 fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cffcc-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="cffcc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cffcc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cffcc-105">删除用户的 [FIDO2 安全密钥身份验证方法](../resources/fido2authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cffcc-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cffcc-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="cffcc-106">Permissions</span></span>

<span data-ttu-id="cffcc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cffcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="cffcc-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="cffcc-109">Permissions acting on self</span></span>

|<span data-ttu-id="cffcc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cffcc-110">Permission type</span></span>      | <span data-ttu-id="cffcc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cffcc-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="cffcc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cffcc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cffcc-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cffcc-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="cffcc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cffcc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cffcc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cffcc-115">Not supported.</span></span> |
| <span data-ttu-id="cffcc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cffcc-116">Application</span></span>                            | <span data-ttu-id="cffcc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cffcc-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="cffcc-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="cffcc-118">Permissions acting on other users</span></span>

|<span data-ttu-id="cffcc-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="cffcc-119">Permission type</span></span>      | <span data-ttu-id="cffcc-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cffcc-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="cffcc-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cffcc-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="cffcc-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cffcc-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="cffcc-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cffcc-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cffcc-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="cffcc-124">Not supported.</span></span> |
| <span data-ttu-id="cffcc-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="cffcc-125">Application</span></span>                            | <span data-ttu-id="cffcc-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cffcc-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="cffcc-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="cffcc-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="cffcc-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="cffcc-128">Global admin</span></span>
* <span data-ttu-id="cffcc-129">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="cffcc-129">Privileged authentication admin</span></span>
* <span data-ttu-id="cffcc-130">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="cffcc-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="cffcc-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cffcc-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cffcc-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="cffcc-132">Request headers</span></span>
|<span data-ttu-id="cffcc-133">名称</span><span class="sxs-lookup"><span data-stu-id="cffcc-133">Name</span></span>|<span data-ttu-id="cffcc-134">说明</span><span class="sxs-lookup"><span data-stu-id="cffcc-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cffcc-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="cffcc-135">Authorization</span></span>|<span data-ttu-id="cffcc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cffcc-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cffcc-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="cffcc-138">Request body</span></span>
<span data-ttu-id="cffcc-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cffcc-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cffcc-140">响应</span><span class="sxs-lookup"><span data-stu-id="cffcc-140">Response</span></span>

<span data-ttu-id="cffcc-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cffcc-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cffcc-143">示例</span><span class="sxs-lookup"><span data-stu-id="cffcc-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cffcc-144">请求</span><span class="sxs-lookup"><span data-stu-id="cffcc-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cffcc-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="cffcc-145">HTTP</span></span>](#tab/http)

# <a name="http"></a>[<span data-ttu-id="cffcc-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="cffcc-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="cffcc-147">C#</span><span class="sxs-lookup"><span data-stu-id="cffcc-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cffcc-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cffcc-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cffcc-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cffcc-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cffcc-150">Java</span><span class="sxs-lookup"><span data-stu-id="cffcc-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cffcc-151">响应</span><span class="sxs-lookup"><span data-stu-id="cffcc-151">Response</span></span>
<span data-ttu-id="cffcc-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cffcc-152">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

