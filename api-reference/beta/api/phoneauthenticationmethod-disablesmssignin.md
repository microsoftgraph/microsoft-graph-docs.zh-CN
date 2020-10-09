---
title: 'phoneAuthenticationMethod: disableSmsSignIn'
description: 禁用移动电话的 SMS 登录
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 953c417b53dd21d294dd00607e9adaf0ed22babd
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402665"
---
# <a name="phoneauthenticationmethod-disablesmssignin"></a><span data-ttu-id="176a5-103">phoneAuthenticationMethod: disableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="176a5-103">phoneAuthenticationMethod: disableSmsSignIn</span></span>

<span data-ttu-id="176a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="176a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="176a5-105">禁用现有电话号码的 SMS 登录 `mobile` 。</span><span class="sxs-lookup"><span data-stu-id="176a5-105">Disable SMS sign-in for an existing `mobile` phone number.</span></span> 

><span data-ttu-id="176a5-106">**注意：** 该号码将不再可用于 SMS 登录，这可能会阻止用户登录。</span><span class="sxs-lookup"><span data-stu-id="176a5-106">**Note:** The number will no longer be available for SMS sign-in, which can prevent your user from signing in.</span></span>

## <a name="permissions"></a><span data-ttu-id="176a5-107">权限</span><span class="sxs-lookup"><span data-stu-id="176a5-107">Permissions</span></span>

<span data-ttu-id="176a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="176a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="176a5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="176a5-110">Permission type</span></span>                        | <span data-ttu-id="176a5-111">从最高特权到最高特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="176a5-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="176a5-112">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="176a5-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="176a5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="176a5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="176a5-114">UserAuthenticationMethod，UserAuthenticationMethod。</span><span class="sxs-lookup"><span data-stu-id="176a5-114">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="176a5-115">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="176a5-115">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="176a5-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="176a5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="176a5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="176a5-117">Not supported.</span></span> | <span data-ttu-id="176a5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="176a5-118">Not supported.</span></span> |
| <span data-ttu-id="176a5-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="176a5-119">Application</span></span>                            | <span data-ttu-id="176a5-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="176a5-120">Not supported.</span></span> | <span data-ttu-id="176a5-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="176a5-121">Not supported.</span></span> |

<span data-ttu-id="176a5-122">对于在其他用户上执行管理的委派方案，管理员需要 [以下角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="176a5-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="176a5-123">全局管理员</span><span class="sxs-lookup"><span data-stu-id="176a5-123">Global admin</span></span>
* <span data-ttu-id="176a5-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="176a5-124">Privileged authentication admin</span></span>
* <span data-ttu-id="176a5-125">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="176a5-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="176a5-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="176a5-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/disableSmsSignIn
POST /users/{id}/authentication/phoneMethods/{id}/disableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="176a5-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="176a5-127">Request headers</span></span>

| <span data-ttu-id="176a5-128">名称</span><span class="sxs-lookup"><span data-stu-id="176a5-128">Name</span></span>          | <span data-ttu-id="176a5-129">说明</span><span class="sxs-lookup"><span data-stu-id="176a5-129">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="176a5-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="176a5-130">Authorization</span></span> | <span data-ttu-id="176a5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="176a5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="176a5-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="176a5-133">Request body</span></span>

<span data-ttu-id="176a5-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="176a5-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="176a5-135">响应</span><span class="sxs-lookup"><span data-stu-id="176a5-135">Response</span></span>

<span data-ttu-id="176a5-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="176a5-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="176a5-138">示例</span><span class="sxs-lookup"><span data-stu-id="176a5-138">Examples</span></span>

<span data-ttu-id="176a5-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="176a5-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="176a5-140">请求</span><span class="sxs-lookup"><span data-stu-id="176a5-140">Request</span></span>

<span data-ttu-id="176a5-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="176a5-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="176a5-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="176a5-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_disablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="176a5-143">C#</span><span class="sxs-lookup"><span data-stu-id="176a5-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-disablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="176a5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="176a5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-disablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="176a5-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="176a5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-disablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="176a5-146">响应</span><span class="sxs-lookup"><span data-stu-id="176a5-146">Response</span></span>

<span data-ttu-id="176a5-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="176a5-147">The following is an example of the response.</span></span>
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