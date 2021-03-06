---
title: phoneAuthenticationMethod：enableSmsSignIn
description: 为移动电话启用短信登录。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8377d1d2806bb5ec86f14911c60a6569bd1054e3
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516568"
---
# <a name="phoneauthenticationmethod-enablesmssignin"></a><span data-ttu-id="96e53-103">phoneAuthenticationMethod：enableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="96e53-103">phoneAuthenticationMethod: enableSmsSignIn</span></span>

<span data-ttu-id="96e53-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96e53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96e53-105">为现有电话号码启用短信 `mobile` 登录。</span><span class="sxs-lookup"><span data-stu-id="96e53-105">Enable SMS sign-in for an existing `mobile` phone number.</span></span> <span data-ttu-id="96e53-106">要成功启用：</span><span class="sxs-lookup"><span data-stu-id="96e53-106">To be successfully enabled:</span></span>

* <span data-ttu-id="96e53-107">电话必须具有 `"phoneType": "mobile"` 。</span><span class="sxs-lookup"><span data-stu-id="96e53-107">The phone must have `"phoneType": "mobile"`.</span></span>
* <span data-ttu-id="96e53-108">电话在短信登录系统中必须是唯一 (其他人也不得使用该号码) 。</span><span class="sxs-lookup"><span data-stu-id="96e53-108">The phone must be unique in the SMS sign-in system (no one else can also be using that number).</span></span>
* <span data-ttu-id="96e53-109">必须在身份验证方法策略中为用户启用短信 [登录](/azure/active-directory/authentication/concept-authentication-methods) 。</span><span class="sxs-lookup"><span data-stu-id="96e53-109">The user must be enabled for SMS sign-in in the [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="96e53-110">权限</span><span class="sxs-lookup"><span data-stu-id="96e53-110">Permissions</span></span>

<span data-ttu-id="96e53-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96e53-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="96e53-113">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="96e53-113">Permissions acting on self</span></span>

|<span data-ttu-id="96e53-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="96e53-114">Permission type</span></span>      | <span data-ttu-id="96e53-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96e53-115">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="96e53-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96e53-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="96e53-117">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96e53-117">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="96e53-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96e53-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96e53-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="96e53-119">Not supported.</span></span> |
| <span data-ttu-id="96e53-120">Application</span><span class="sxs-lookup"><span data-stu-id="96e53-120">Application</span></span>                            | <span data-ttu-id="96e53-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="96e53-121">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="96e53-122">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="96e53-122">Permissions acting on other users</span></span>

|<span data-ttu-id="96e53-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="96e53-123">Permission type</span></span>      | <span data-ttu-id="96e53-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96e53-124">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="96e53-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96e53-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="96e53-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e53-126">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="96e53-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96e53-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96e53-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="96e53-128">Not supported.</span></span> |
| <span data-ttu-id="96e53-129">Application</span><span class="sxs-lookup"><span data-stu-id="96e53-129">Application</span></span>                            | <span data-ttu-id="96e53-130">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e53-130">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="96e53-131">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="96e53-131">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="96e53-132">全局管理员</span><span class="sxs-lookup"><span data-stu-id="96e53-132">Global admin</span></span>
* <span data-ttu-id="96e53-133">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="96e53-133">Privileged authentication admin</span></span>
* <span data-ttu-id="96e53-134">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="96e53-134">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="96e53-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96e53-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/enableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/enableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="96e53-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="96e53-136">Request headers</span></span>

| <span data-ttu-id="96e53-137">名称</span><span class="sxs-lookup"><span data-stu-id="96e53-137">Name</span></span>          | <span data-ttu-id="96e53-138">说明</span><span class="sxs-lookup"><span data-stu-id="96e53-138">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="96e53-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="96e53-139">Authorization</span></span> | <span data-ttu-id="96e53-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96e53-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96e53-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="96e53-142">Request body</span></span>

<span data-ttu-id="96e53-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96e53-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96e53-144">响应</span><span class="sxs-lookup"><span data-stu-id="96e53-144">Response</span></span>

<span data-ttu-id="96e53-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="96e53-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96e53-147">示例</span><span class="sxs-lookup"><span data-stu-id="96e53-147">Examples</span></span>

<span data-ttu-id="96e53-148">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="96e53-148">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="96e53-149">请求</span><span class="sxs-lookup"><span data-stu-id="96e53-149">Request</span></span>

<span data-ttu-id="96e53-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="96e53-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="96e53-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="96e53-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_enablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/enableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="96e53-152">C#</span><span class="sxs-lookup"><span data-stu-id="96e53-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-enablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96e53-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96e53-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-enablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96e53-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96e53-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-enablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96e53-155">Java</span><span class="sxs-lookup"><span data-stu-id="96e53-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-enablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="96e53-156">响应</span><span class="sxs-lookup"><span data-stu-id="96e53-156">Response</span></span>

<span data-ttu-id="96e53-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="96e53-157">The following is an example of the response.</span></span>
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
  "description": "phoneAuthenticationMethod: enableSmsSignIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
