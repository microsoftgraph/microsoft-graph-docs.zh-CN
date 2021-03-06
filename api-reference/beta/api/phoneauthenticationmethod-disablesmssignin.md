---
title: phoneAuthenticationMethod： disableSmsSignIn
description: 禁用移动电话的短信登录
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: eb8933a141dcd343ab26a5d5809844ee79c39697
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516491"
---
# <a name="phoneauthenticationmethod-disablesmssignin"></a><span data-ttu-id="4b589-103">phoneAuthenticationMethod： disableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="4b589-103">phoneAuthenticationMethod: disableSmsSignIn</span></span>

<span data-ttu-id="4b589-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b589-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b589-105">禁用现有电话号码的短信 `mobile` 登录。</span><span class="sxs-lookup"><span data-stu-id="4b589-105">Disable SMS sign-in for an existing `mobile` phone number.</span></span> 

><span data-ttu-id="4b589-106">**注意：** 该号码将不再可用于短信登录，这将阻止用户登录。</span><span class="sxs-lookup"><span data-stu-id="4b589-106">**Note:** The number will no longer be available for SMS sign-in, which can prevent your user from signing in.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b589-107">权限</span><span class="sxs-lookup"><span data-stu-id="4b589-107">Permissions</span></span>

<span data-ttu-id="4b589-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b589-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="4b589-110">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="4b589-110">Permissions acting on self</span></span>

|<span data-ttu-id="4b589-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b589-111">Permission type</span></span>      | <span data-ttu-id="4b589-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b589-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="4b589-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b589-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b589-114">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b589-114">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="4b589-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b589-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b589-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b589-116">Not supported.</span></span> |
| <span data-ttu-id="4b589-117">Application</span><span class="sxs-lookup"><span data-stu-id="4b589-117">Application</span></span>                            | <span data-ttu-id="4b589-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b589-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="4b589-119">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="4b589-119">Permissions acting on other users</span></span>

|<span data-ttu-id="4b589-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b589-120">Permission type</span></span>      | <span data-ttu-id="4b589-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b589-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="4b589-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b589-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b589-123">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b589-123">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="4b589-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b589-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b589-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b589-125">Not supported.</span></span> |
| <span data-ttu-id="4b589-126">Application</span><span class="sxs-lookup"><span data-stu-id="4b589-126">Application</span></span>                            | <span data-ttu-id="4b589-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b589-127">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="4b589-128">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="4b589-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="4b589-129">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4b589-129">Global admin</span></span>
* <span data-ttu-id="4b589-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="4b589-130">Privileged authentication admin</span></span>
* <span data-ttu-id="4b589-131">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="4b589-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="4b589-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b589-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/disableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/disableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="4b589-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b589-133">Request headers</span></span>

| <span data-ttu-id="4b589-134">名称</span><span class="sxs-lookup"><span data-stu-id="4b589-134">Name</span></span>          | <span data-ttu-id="4b589-135">说明</span><span class="sxs-lookup"><span data-stu-id="4b589-135">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4b589-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b589-136">Authorization</span></span> | <span data-ttu-id="4b589-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b589-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b589-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b589-139">Request body</span></span>

<span data-ttu-id="4b589-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b589-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b589-141">响应</span><span class="sxs-lookup"><span data-stu-id="4b589-141">Response</span></span>

<span data-ttu-id="4b589-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4b589-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b589-144">示例</span><span class="sxs-lookup"><span data-stu-id="4b589-144">Examples</span></span>

<span data-ttu-id="4b589-145">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="4b589-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4b589-146">请求</span><span class="sxs-lookup"><span data-stu-id="4b589-146">Request</span></span>

<span data-ttu-id="4b589-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4b589-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b589-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b589-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_disablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="4b589-149">C#</span><span class="sxs-lookup"><span data-stu-id="4b589-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-disablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b589-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b589-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-disablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b589-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b589-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-disablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b589-152">Java</span><span class="sxs-lookup"><span data-stu-id="4b589-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-disablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4b589-153">响应</span><span class="sxs-lookup"><span data-stu-id="4b589-153">Response</span></span>

<span data-ttu-id="4b589-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4b589-154">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phoneAuthenticationMethod: disableSmsSignIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
