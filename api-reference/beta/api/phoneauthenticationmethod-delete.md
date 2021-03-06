---
title: 删除 phoneAuthenticationMethod
description: 删除用户的电话身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1abea19acd14c53d75e51783f8bd01fa8ed74d81
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516495"
---
# <a name="delete-phoneauthenticationmethod"></a><span data-ttu-id="f229b-103">删除 phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f229b-103">Delete phoneAuthenticationMethod</span></span>

<span data-ttu-id="f229b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f229b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f229b-105">删除用户 [的电话身份验证方法](../resources/phoneauthenticationmethod.md)。</span><span class="sxs-lookup"><span data-stu-id="f229b-105">Delete a user's [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> 

><span data-ttu-id="f229b-106">**注意：** 这将从用户中删除电话号码，他们将不再能够使用该号码进行身份验证，无论是通过短信还是语音呼叫。</span><span class="sxs-lookup"><span data-stu-id="f229b-106">**Note:** This removes the phone number from the user and they will no longer be able to use the number for authentication, whether via SMS or voice calls.</span></span>

<span data-ttu-id="f229b-107">请记住，用户不能有 `alternateMobile` 没有数字 `mobile` 的号码。</span><span class="sxs-lookup"><span data-stu-id="f229b-107">Remember that a user cannot have an `alternateMobile` number without a `mobile` number.</span></span> <span data-ttu-id="f229b-108">如果要从同样具有号码的用户中删除号码，请首先将号码更新为新号码，然后 `mobile` `alternateMobile` [](phoneauthenticationmethod-update.md) `mobile` 删除该 `alternateMobile` 号码。</span><span class="sxs-lookup"><span data-stu-id="f229b-108">If you want to remove a `mobile` number from a user that also has an `alternateMobile` number, first [update](phoneauthenticationmethod-update.md) the `mobile` number to the new number, then delete the `alternateMobile` number.</span></span>

<span data-ttu-id="f229b-109">如果电话号码是用户的默认 Azure 多重身份验证 (MFA) 方法，则不能将其删除。</span><span class="sxs-lookup"><span data-stu-id="f229b-109">If the phone number is the user's default Azure multi-factor authentication (MFA) authentication method, it cannot be deleted.</span></span> <span data-ttu-id="f229b-110">让用户更改其默认身份验证方法，然后删除该号码。</span><span class="sxs-lookup"><span data-stu-id="f229b-110">Have the user change their default authentication method, and then delete the number.</span></span>

## <a name="permissions"></a><span data-ttu-id="f229b-111">权限</span><span class="sxs-lookup"><span data-stu-id="f229b-111">Permissions</span></span>

<span data-ttu-id="f229b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f229b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="f229b-114">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="f229b-114">Permissions acting on self</span></span>

|<span data-ttu-id="f229b-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="f229b-115">Permission type</span></span>      | <span data-ttu-id="f229b-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f229b-116">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="f229b-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f229b-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="f229b-118">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f229b-118">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="f229b-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f229b-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f229b-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="f229b-120">Not supported.</span></span> |
| <span data-ttu-id="f229b-121">Application</span><span class="sxs-lookup"><span data-stu-id="f229b-121">Application</span></span>                            | <span data-ttu-id="f229b-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="f229b-122">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="f229b-123">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="f229b-123">Permissions acting on other users</span></span>

|<span data-ttu-id="f229b-124">权限类型</span><span class="sxs-lookup"><span data-stu-id="f229b-124">Permission type</span></span>      | <span data-ttu-id="f229b-125">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f229b-125">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="f229b-126">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f229b-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="f229b-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f229b-127">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="f229b-128">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f229b-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f229b-129">不支持。</span><span class="sxs-lookup"><span data-stu-id="f229b-129">Not supported.</span></span> |
| <span data-ttu-id="f229b-130">Application</span><span class="sxs-lookup"><span data-stu-id="f229b-130">Application</span></span>                            | <span data-ttu-id="f229b-131">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f229b-131">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="f229b-132">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="f229b-132">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="f229b-133">全局管理员</span><span class="sxs-lookup"><span data-stu-id="f229b-133">Global admin</span></span>
* <span data-ttu-id="f229b-134">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="f229b-134">Privileged authentication admin</span></span>
* <span data-ttu-id="f229b-135">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="f229b-135">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="f229b-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f229b-136">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/authentication/phoneMethods/{id}
DELETE /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f229b-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="f229b-137">Request headers</span></span>

| <span data-ttu-id="f229b-138">名称</span><span class="sxs-lookup"><span data-stu-id="f229b-138">Name</span></span>          | <span data-ttu-id="f229b-139">说明</span><span class="sxs-lookup"><span data-stu-id="f229b-139">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f229b-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="f229b-140">Authorization</span></span> | <span data-ttu-id="f229b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f229b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f229b-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="f229b-143">Request body</span></span>

<span data-ttu-id="f229b-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f229b-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f229b-145">响应</span><span class="sxs-lookup"><span data-stu-id="f229b-145">Response</span></span>

<span data-ttu-id="f229b-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f229b-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f229b-148">示例</span><span class="sxs-lookup"><span data-stu-id="f229b-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f229b-149">请求</span><span class="sxs-lookup"><span data-stu-id="f229b-149">Request</span></span>

<span data-ttu-id="f229b-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f229b-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f229b-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="f229b-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_phoneauthenticationmethod"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="f229b-152">C#</span><span class="sxs-lookup"><span data-stu-id="f229b-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f229b-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f229b-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f229b-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f229b-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f229b-155">Java</span><span class="sxs-lookup"><span data-stu-id="f229b-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f229b-156">响应</span><span class="sxs-lookup"><span data-stu-id="f229b-156">Response</span></span>

<span data-ttu-id="f229b-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f229b-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
