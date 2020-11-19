---
title: 删除 fido2AuthenticationMethod
description: 删除一个 fido2AuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3c3089214c6100b945c504448ee07120d479b58a
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352160"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="677aa-103">删除 fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="677aa-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="677aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="677aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="677aa-105">删除用户的 [FIDO2 安全密钥身份验证方法](../resources/fido2authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="677aa-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="677aa-106">权限</span><span class="sxs-lookup"><span data-stu-id="677aa-106">Permissions</span></span>
<span data-ttu-id="677aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="677aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="677aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="677aa-109">Permission type</span></span>|<span data-ttu-id="677aa-110">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="677aa-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="677aa-111">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="677aa-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="677aa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="677aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="677aa-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="677aa-113">Not supported.</span></span>|<span data-ttu-id="677aa-114">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="677aa-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="677aa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="677aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="677aa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="677aa-116">Not supported.</span></span>|<span data-ttu-id="677aa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="677aa-117">Not supported.</span></span>
|<span data-ttu-id="677aa-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="677aa-118">Application</span></span>|<span data-ttu-id="677aa-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="677aa-119">Not supported.</span></span>|<span data-ttu-id="677aa-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="677aa-120">Not supported.</span></span>

<span data-ttu-id="677aa-121">对于在其他用户上执行管理的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="677aa-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="677aa-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="677aa-122">Global admin</span></span>
* <span data-ttu-id="677aa-123">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="677aa-123">Privileged authentication admin</span></span>
* <span data-ttu-id="677aa-124">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="677aa-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="677aa-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="677aa-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="677aa-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="677aa-126">Request headers</span></span>
|<span data-ttu-id="677aa-127">名称</span><span class="sxs-lookup"><span data-stu-id="677aa-127">Name</span></span>|<span data-ttu-id="677aa-128">说明</span><span class="sxs-lookup"><span data-stu-id="677aa-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="677aa-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="677aa-129">Authorization</span></span>|<span data-ttu-id="677aa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="677aa-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="677aa-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="677aa-132">Request body</span></span>
<span data-ttu-id="677aa-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="677aa-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="677aa-134">响应</span><span class="sxs-lookup"><span data-stu-id="677aa-134">Response</span></span>

<span data-ttu-id="677aa-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="677aa-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="677aa-137">示例</span><span class="sxs-lookup"><span data-stu-id="677aa-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="677aa-138">请求</span><span class="sxs-lookup"><span data-stu-id="677aa-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="677aa-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="677aa-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="677aa-140">C#</span><span class="sxs-lookup"><span data-stu-id="677aa-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="677aa-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="677aa-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="677aa-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="677aa-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="677aa-143">Java</span><span class="sxs-lookup"><span data-stu-id="677aa-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="677aa-144">响应</span><span class="sxs-lookup"><span data-stu-id="677aa-144">Response</span></span>
<span data-ttu-id="677aa-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="677aa-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

