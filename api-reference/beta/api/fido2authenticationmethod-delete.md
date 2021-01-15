---
title: 删除 fido2AuthenticationMethod
description: 删除 fido2AuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0230b693528f0ba481bd99c385f43445e7b9ccd9
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872063"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="e0ff4-103">删除 fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e0ff4-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="e0ff4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0ff4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0ff4-105">删除用户的 [FIDO2 安全密钥身份验证方法](../resources/fido2authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0ff4-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0ff4-106">权限</span><span class="sxs-lookup"><span data-stu-id="e0ff4-106">Permissions</span></span>
<span data-ttu-id="e0ff4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0ff4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0ff4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0ff4-109">Permission type</span></span>|<span data-ttu-id="e0ff4-110">对自身执行 (权限从最低特权到最多特权) </span><span class="sxs-lookup"><span data-stu-id="e0ff4-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="e0ff4-111">对他人的操作权限 (权限从最低特权级别) </span><span class="sxs-lookup"><span data-stu-id="e0ff4-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="e0ff4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0ff4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0ff4-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0ff4-113">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="e0ff4-114">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0ff4-114">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="e0ff4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0ff4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0ff4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0ff4-116">Not supported.</span></span> | <span data-ttu-id="e0ff4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0ff4-117">Not supported.</span></span> |
| <span data-ttu-id="e0ff4-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0ff4-118">Application</span></span>                            | <span data-ttu-id="e0ff4-119">不适用。</span><span class="sxs-lookup"><span data-stu-id="e0ff4-119">Not applicable.</span></span> | <span data-ttu-id="e0ff4-120">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0ff4-120">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="e0ff4-121">对于管理员正在操作其他用户的委派方案，管理员需要以下角色之 [一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="e0ff4-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="e0ff4-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="e0ff4-122">Global admin</span></span>
* <span data-ttu-id="e0ff4-123">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="e0ff4-123">Privileged authentication admin</span></span>
* <span data-ttu-id="e0ff4-124">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="e0ff4-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="e0ff4-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0ff4-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e0ff4-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0ff4-126">Request headers</span></span>
|<span data-ttu-id="e0ff4-127">名称</span><span class="sxs-lookup"><span data-stu-id="e0ff4-127">Name</span></span>|<span data-ttu-id="e0ff4-128">说明</span><span class="sxs-lookup"><span data-stu-id="e0ff4-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e0ff4-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0ff4-129">Authorization</span></span>|<span data-ttu-id="e0ff4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0ff4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0ff4-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0ff4-132">Request body</span></span>
<span data-ttu-id="e0ff4-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e0ff4-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0ff4-134">响应</span><span class="sxs-lookup"><span data-stu-id="e0ff4-134">Response</span></span>

<span data-ttu-id="e0ff4-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e0ff4-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0ff4-137">示例</span><span class="sxs-lookup"><span data-stu-id="e0ff4-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e0ff4-138">请求</span><span class="sxs-lookup"><span data-stu-id="e0ff4-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e0ff4-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0ff4-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="e0ff4-140">C#</span><span class="sxs-lookup"><span data-stu-id="e0ff4-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0ff4-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0ff4-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0ff4-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0ff4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0ff4-143">Java</span><span class="sxs-lookup"><span data-stu-id="e0ff4-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e0ff4-144">响应</span><span class="sxs-lookup"><span data-stu-id="e0ff4-144">Response</span></span>
<span data-ttu-id="e0ff4-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e0ff4-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

