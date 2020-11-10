---
title: 'phoneAuthenticationMethod: disableSmsSignIn'
description: 禁用移动电话的 SMS 登录
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6743c2e57b4d6f4f1499cc1e68711996912914fd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971213"
---
# <a name="phoneauthenticationmethod-disablesmssignin"></a><span data-ttu-id="2ce89-103">phoneAuthenticationMethod: disableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="2ce89-103">phoneAuthenticationMethod: disableSmsSignIn</span></span>

<span data-ttu-id="2ce89-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ce89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ce89-105">禁用现有电话号码的 SMS 登录 `mobile` 。</span><span class="sxs-lookup"><span data-stu-id="2ce89-105">Disable SMS sign-in for an existing `mobile` phone number.</span></span> 

><span data-ttu-id="2ce89-106">**注意：** 该号码将不再可用于 SMS 登录，这可能会阻止用户登录。</span><span class="sxs-lookup"><span data-stu-id="2ce89-106">**Note:** The number will no longer be available for SMS sign-in, which can prevent your user from signing in.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ce89-107">权限</span><span class="sxs-lookup"><span data-stu-id="2ce89-107">Permissions</span></span>

<span data-ttu-id="2ce89-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ce89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ce89-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ce89-110">Permission type</span></span>                        | <span data-ttu-id="2ce89-111">从最高特权到最高特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="2ce89-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="2ce89-112">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="2ce89-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="2ce89-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ce89-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ce89-114">UserAuthenticationMethod，UserAuthenticationMethod。</span><span class="sxs-lookup"><span data-stu-id="2ce89-114">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="2ce89-115">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2ce89-115">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="2ce89-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ce89-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ce89-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ce89-117">Not supported.</span></span> | <span data-ttu-id="2ce89-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ce89-118">Not supported.</span></span> |
| <span data-ttu-id="2ce89-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ce89-119">Application</span></span>                            | <span data-ttu-id="2ce89-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ce89-120">Not supported.</span></span> | <span data-ttu-id="2ce89-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ce89-121">Not supported.</span></span> |

<span data-ttu-id="2ce89-122">对于在其他用户上执行管理的委派方案，管理员需要 [以下角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="2ce89-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="2ce89-123">全局管理员</span><span class="sxs-lookup"><span data-stu-id="2ce89-123">Global admin</span></span>
* <span data-ttu-id="2ce89-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="2ce89-124">Privileged authentication admin</span></span>
* <span data-ttu-id="2ce89-125">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="2ce89-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="2ce89-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ce89-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/disableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/disableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="2ce89-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ce89-127">Request headers</span></span>

| <span data-ttu-id="2ce89-128">名称</span><span class="sxs-lookup"><span data-stu-id="2ce89-128">Name</span></span>          | <span data-ttu-id="2ce89-129">说明</span><span class="sxs-lookup"><span data-stu-id="2ce89-129">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2ce89-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ce89-130">Authorization</span></span> | <span data-ttu-id="2ce89-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ce89-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ce89-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ce89-133">Request body</span></span>

<span data-ttu-id="2ce89-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ce89-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ce89-135">响应</span><span class="sxs-lookup"><span data-stu-id="2ce89-135">Response</span></span>

<span data-ttu-id="2ce89-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2ce89-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ce89-138">示例</span><span class="sxs-lookup"><span data-stu-id="2ce89-138">Examples</span></span>

<span data-ttu-id="2ce89-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="2ce89-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2ce89-140">请求</span><span class="sxs-lookup"><span data-stu-id="2ce89-140">Request</span></span>

<span data-ttu-id="2ce89-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2ce89-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ce89-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ce89-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_disablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="2ce89-143">C#</span><span class="sxs-lookup"><span data-stu-id="2ce89-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-disablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ce89-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ce89-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-disablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ce89-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ce89-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-disablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ce89-146">Java</span><span class="sxs-lookup"><span data-stu-id="2ce89-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-disablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ce89-147">响应</span><span class="sxs-lookup"><span data-stu-id="2ce89-147">Response</span></span>

<span data-ttu-id="2ce89-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2ce89-148">The following is an example of the response.</span></span>
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
