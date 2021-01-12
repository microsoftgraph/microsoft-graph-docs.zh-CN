---
title: phoneAuthenticationMethod：enableSmsSignIn
description: 为移动电话启用短信登录。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e2c8087005f65ac74a202ea43d90767172267a46
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796603"
---
# <a name="phoneauthenticationmethod-enablesmssignin"></a><span data-ttu-id="a59e5-103">phoneAuthenticationMethod：enableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="a59e5-103">phoneAuthenticationMethod: enableSmsSignIn</span></span>

<span data-ttu-id="a59e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a59e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a59e5-105">为现有电话号码启用短信 `mobile` 登录。</span><span class="sxs-lookup"><span data-stu-id="a59e5-105">Enable SMS sign-in for an existing `mobile` phone number.</span></span> <span data-ttu-id="a59e5-106">要成功启用：</span><span class="sxs-lookup"><span data-stu-id="a59e5-106">To be successfully enabled:</span></span>

* <span data-ttu-id="a59e5-107">电话必须具有 `"phoneType": "mobile"` 。</span><span class="sxs-lookup"><span data-stu-id="a59e5-107">The phone must have `"phoneType": "mobile"`.</span></span>
* <span data-ttu-id="a59e5-108">电话在短信登录系统中必须是唯一 (其他人也不得使用该号码) 。</span><span class="sxs-lookup"><span data-stu-id="a59e5-108">The phone must be unique in the SMS sign-in system (no one else can also be using that number).</span></span>
* <span data-ttu-id="a59e5-109">必须在身份验证方法策略中为用户启用短信 [登录](/azure/active-directory/authentication/concept-authentication-methods) 。</span><span class="sxs-lookup"><span data-stu-id="a59e5-109">The user must be enabled for SMS sign-in in the [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="a59e5-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="a59e5-110">Permissions</span></span>

<span data-ttu-id="a59e5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a59e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="a59e5-113">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="a59e5-113">Permissions acting on self</span></span>

|<span data-ttu-id="a59e5-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="a59e5-114">Permission type</span></span>      | <span data-ttu-id="a59e5-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a59e5-115">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="a59e5-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a59e5-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="a59e5-117">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a59e5-117">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="a59e5-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a59e5-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a59e5-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a59e5-119">Not supported.</span></span> |
| <span data-ttu-id="a59e5-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="a59e5-120">Application</span></span>                            | <span data-ttu-id="a59e5-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="a59e5-121">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="a59e5-122">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="a59e5-122">Permissions acting on other users</span></span>

|<span data-ttu-id="a59e5-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="a59e5-123">Permission type</span></span>      | <span data-ttu-id="a59e5-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a59e5-124">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="a59e5-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a59e5-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="a59e5-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a59e5-126">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="a59e5-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a59e5-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a59e5-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="a59e5-128">Not supported.</span></span> |
| <span data-ttu-id="a59e5-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="a59e5-129">Application</span></span>                            | <span data-ttu-id="a59e5-130">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a59e5-130">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="a59e5-131">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="a59e5-131">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="a59e5-132">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a59e5-132">Global admin</span></span>
* <span data-ttu-id="a59e5-133">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="a59e5-133">Privileged authentication admin</span></span>
* <span data-ttu-id="a59e5-134">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="a59e5-134">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="a59e5-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a59e5-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/enableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/enableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="a59e5-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="a59e5-136">Request headers</span></span>

| <span data-ttu-id="a59e5-137">名称</span><span class="sxs-lookup"><span data-stu-id="a59e5-137">Name</span></span>          | <span data-ttu-id="a59e5-138">说明</span><span class="sxs-lookup"><span data-stu-id="a59e5-138">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a59e5-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="a59e5-139">Authorization</span></span> | <span data-ttu-id="a59e5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a59e5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a59e5-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="a59e5-142">Request body</span></span>

<span data-ttu-id="a59e5-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a59e5-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a59e5-144">响应</span><span class="sxs-lookup"><span data-stu-id="a59e5-144">Response</span></span>

<span data-ttu-id="a59e5-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a59e5-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a59e5-147">示例</span><span class="sxs-lookup"><span data-stu-id="a59e5-147">Examples</span></span>

<span data-ttu-id="a59e5-148">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a59e5-148">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a59e5-149">请求</span><span class="sxs-lookup"><span data-stu-id="a59e5-149">Request</span></span>

<span data-ttu-id="a59e5-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a59e5-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a59e5-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="a59e5-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_enablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/enableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="a59e5-152">C#</span><span class="sxs-lookup"><span data-stu-id="a59e5-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-enablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a59e5-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a59e5-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-enablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a59e5-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a59e5-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-enablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a59e5-155">Java</span><span class="sxs-lookup"><span data-stu-id="a59e5-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-enablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a59e5-156">响应</span><span class="sxs-lookup"><span data-stu-id="a59e5-156">Response</span></span>

<span data-ttu-id="a59e5-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a59e5-157">The following is an example of the response.</span></span>
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
