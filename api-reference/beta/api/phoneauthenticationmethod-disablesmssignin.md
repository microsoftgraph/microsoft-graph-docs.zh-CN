---
title: 'phoneAuthenticationMethod: disableSmsSignIn'
description: 禁用移动电话的 SMS 登录
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8073ecee3fc17462186f7a9fd7d668677395a73c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010612"
---
# <a name="phoneauthenticationmethod-disablesmssignin"></a><span data-ttu-id="b59af-103">phoneAuthenticationMethod: disableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="b59af-103">phoneAuthenticationMethod: disableSmsSignIn</span></span>

<span data-ttu-id="b59af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b59af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b59af-105">禁用现有电话号码的 SMS 登录 `mobile` 。</span><span class="sxs-lookup"><span data-stu-id="b59af-105">Disable SMS sign-in for an existing `mobile` phone number.</span></span> 

><span data-ttu-id="b59af-106">**注意：** 该号码将不再可用于 SMS 登录，这可能会阻止用户登录。</span><span class="sxs-lookup"><span data-stu-id="b59af-106">**Note:** The number will no longer be available for SMS sign-in, which can prevent your user from signing in.</span></span>

## <a name="permissions"></a><span data-ttu-id="b59af-107">权限</span><span class="sxs-lookup"><span data-stu-id="b59af-107">Permissions</span></span>

<span data-ttu-id="b59af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b59af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b59af-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b59af-110">Permission type</span></span>                        | <span data-ttu-id="b59af-111">从最高特权到最高特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="b59af-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="b59af-112">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="b59af-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="b59af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b59af-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b59af-114">UserAuthenticationMethod，UserAuthenticationMethod。</span><span class="sxs-lookup"><span data-stu-id="b59af-114">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="b59af-115">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b59af-115">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b59af-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b59af-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b59af-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b59af-117">Not supported.</span></span> | <span data-ttu-id="b59af-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b59af-118">Not supported.</span></span> |
| <span data-ttu-id="b59af-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="b59af-119">Application</span></span>                            | <span data-ttu-id="b59af-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="b59af-120">Not supported.</span></span> | <span data-ttu-id="b59af-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="b59af-121">Not supported.</span></span> |

<span data-ttu-id="b59af-122">对于在其他用户上执行管理的委派方案，管理员需要 [以下角色之一](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="b59af-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b59af-123">全局管理员</span><span class="sxs-lookup"><span data-stu-id="b59af-123">Global admin</span></span>
* <span data-ttu-id="b59af-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="b59af-124">Privileged authentication admin</span></span>
* <span data-ttu-id="b59af-125">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="b59af-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b59af-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b59af-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/disableSmsSignIn
POST /users/{id}/authentication/phoneMethods/{id}/disableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="b59af-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="b59af-127">Request headers</span></span>

| <span data-ttu-id="b59af-128">名称</span><span class="sxs-lookup"><span data-stu-id="b59af-128">Name</span></span>          | <span data-ttu-id="b59af-129">说明</span><span class="sxs-lookup"><span data-stu-id="b59af-129">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b59af-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="b59af-130">Authorization</span></span> | <span data-ttu-id="b59af-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b59af-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b59af-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="b59af-133">Request body</span></span>

<span data-ttu-id="b59af-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b59af-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b59af-135">响应</span><span class="sxs-lookup"><span data-stu-id="b59af-135">Response</span></span>

<span data-ttu-id="b59af-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b59af-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b59af-138">示例</span><span class="sxs-lookup"><span data-stu-id="b59af-138">Examples</span></span>

<span data-ttu-id="b59af-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b59af-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b59af-140">请求</span><span class="sxs-lookup"><span data-stu-id="b59af-140">Request</span></span>

<span data-ttu-id="b59af-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b59af-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b59af-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="b59af-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_disablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="b59af-143">C#</span><span class="sxs-lookup"><span data-stu-id="b59af-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-disablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b59af-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b59af-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-disablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b59af-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b59af-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-disablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b59af-146">响应</span><span class="sxs-lookup"><span data-stu-id="b59af-146">Response</span></span>

<span data-ttu-id="b59af-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b59af-147">The following is an example of the response.</span></span>
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


