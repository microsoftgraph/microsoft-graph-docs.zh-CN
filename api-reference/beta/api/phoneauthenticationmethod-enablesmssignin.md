---
title: 'phoneAuthenticationMethod: enableSmsSignIn'
description: 为移动电话启用 SMS 登录。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f3a7b61e8463d2c4c8a71dcf75885658f465504e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971184"
---
# <a name="phoneauthenticationmethod-enablesmssignin"></a><span data-ttu-id="c6fb8-103">phoneAuthenticationMethod: enableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="c6fb8-103">phoneAuthenticationMethod: enableSmsSignIn</span></span>

<span data-ttu-id="c6fb8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6fb8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6fb8-105">为现有的电话号码启用 SMS 登录 `mobile` 。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-105">Enable SMS sign-in for an existing `mobile` phone number.</span></span> <span data-ttu-id="c6fb8-106">若要成功启用，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="c6fb8-106">To be successfully enabled:</span></span>

* <span data-ttu-id="c6fb8-107">电话必须具有 `"phoneType": "mobile"` 。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-107">The phone must have `"phoneType": "mobile"`.</span></span>
* <span data-ttu-id="c6fb8-108">电话在 SMS 登录系统中必须是唯一的 (任何其他人也不能使用该号码) 。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-108">The phone must be unique in the SMS sign-in system (no one else can also be using that number).</span></span>
* <span data-ttu-id="c6fb8-109">必须为用户启用 [身份验证方法](/azure/active-directory/authentication/concept-authentication-methods) 策略中的 SMS 登录。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-109">The user must be enabled for SMS sign-in in the [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6fb8-110">权限</span><span class="sxs-lookup"><span data-stu-id="c6fb8-110">Permissions</span></span>

<span data-ttu-id="c6fb8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c6fb8-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6fb8-113">Permission type</span></span>                        | <span data-ttu-id="c6fb8-114">从最高特权到最高特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="c6fb8-114">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="c6fb8-115">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="c6fb8-115">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="c6fb8-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6fb8-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6fb8-117">UserAuthenticationMethod，UserAuthenticationMethod。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-117">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="c6fb8-118">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c6fb8-118">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="c6fb8-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6fb8-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6fb8-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-120">Not supported.</span></span> | <span data-ttu-id="c6fb8-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-121">Not supported.</span></span> |
| <span data-ttu-id="c6fb8-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6fb8-122">Application</span></span>                            | <span data-ttu-id="c6fb8-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-123">Not supported.</span></span> | <span data-ttu-id="c6fb8-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-124">Not supported.</span></span> |

<span data-ttu-id="c6fb8-125">对于在其他用户上执行管理的委派方案，管理员需要 [以下角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="c6fb8-125">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="c6fb8-126">全局管理员</span><span class="sxs-lookup"><span data-stu-id="c6fb8-126">Global admin</span></span>
* <span data-ttu-id="c6fb8-127">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="c6fb8-127">Privileged authentication admin</span></span>
* <span data-ttu-id="c6fb8-128">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="c6fb8-128">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="c6fb8-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6fb8-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/enableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/enableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="c6fb8-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6fb8-130">Request headers</span></span>

| <span data-ttu-id="c6fb8-131">名称</span><span class="sxs-lookup"><span data-stu-id="c6fb8-131">Name</span></span>          | <span data-ttu-id="c6fb8-132">说明</span><span class="sxs-lookup"><span data-stu-id="c6fb8-132">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c6fb8-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6fb8-133">Authorization</span></span> | <span data-ttu-id="c6fb8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6fb8-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6fb8-136">Request body</span></span>

<span data-ttu-id="c6fb8-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6fb8-138">响应</span><span class="sxs-lookup"><span data-stu-id="c6fb8-138">Response</span></span>

<span data-ttu-id="c6fb8-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c6fb8-141">示例</span><span class="sxs-lookup"><span data-stu-id="c6fb8-141">Examples</span></span>

<span data-ttu-id="c6fb8-142">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-142">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c6fb8-143">请求</span><span class="sxs-lookup"><span data-stu-id="c6fb8-143">Request</span></span>

<span data-ttu-id="c6fb8-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c6fb8-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6fb8-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_enablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/enableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="c6fb8-146">C#</span><span class="sxs-lookup"><span data-stu-id="c6fb8-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-enablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6fb8-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6fb8-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-enablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6fb8-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6fb8-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-enablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6fb8-149">Java</span><span class="sxs-lookup"><span data-stu-id="c6fb8-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-enablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c6fb8-150">响应</span><span class="sxs-lookup"><span data-stu-id="c6fb8-150">Response</span></span>

<span data-ttu-id="c6fb8-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c6fb8-151">The following is an example of the response.</span></span>
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
