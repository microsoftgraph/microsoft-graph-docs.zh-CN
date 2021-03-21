---
title: 删除 phoneAuthenticationMethod
description: 删除用户的电话身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bbd08b9da7a75c471e90b9846e3aaa2c1a503879
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957484"
---
# <a name="delete-phoneauthenticationmethod"></a><span data-ttu-id="921f8-103">删除 phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="921f8-103">Delete phoneAuthenticationMethod</span></span>

<span data-ttu-id="921f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="921f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="921f8-105">删除用户的电话 [身份验证方法](../resources/phoneauthenticationmethod.md)。</span><span class="sxs-lookup"><span data-stu-id="921f8-105">Delete a user's [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> 

><span data-ttu-id="921f8-106">**注意：** 这将删除用户的电话号码，他们将不再能够使用该号码进行身份验证，无论是通过短信还是语音呼叫。</span><span class="sxs-lookup"><span data-stu-id="921f8-106">**Note:** This removes the phone number from the user and they will no longer be able to use the number for authentication, whether via SMS or voice calls.</span></span>

<span data-ttu-id="921f8-107">请记住，用户不能有 `alternateMobile` 没有数字 `mobile` 的号码。</span><span class="sxs-lookup"><span data-stu-id="921f8-107">Remember that a user cannot have an `alternateMobile` number without a `mobile` number.</span></span> <span data-ttu-id="921f8-108">如果要从也具有号码的用户中删除号码，请首先将号码更新为新号码，然后 `mobile` `alternateMobile` [](phoneauthenticationmethod-update.md) `mobile` 删除该 `alternateMobile` 号码。</span><span class="sxs-lookup"><span data-stu-id="921f8-108">If you want to remove a `mobile` number from a user that also has an `alternateMobile` number, first [update](phoneauthenticationmethod-update.md) the `mobile` number to the new number, then delete the `alternateMobile` number.</span></span>

<span data-ttu-id="921f8-109">如果电话号码是用户的默认 Azure 多重身份验证 (MFA) 身份验证方法，则不能删除该号码。</span><span class="sxs-lookup"><span data-stu-id="921f8-109">If the phone number is the user's default Azure multi-factor authentication (MFA) authentication method, it cannot be deleted.</span></span> <span data-ttu-id="921f8-110">让用户更改其默认身份验证方法，然后删除该号码。</span><span class="sxs-lookup"><span data-stu-id="921f8-110">Have the user change their default authentication method, and then delete the number.</span></span>

## <a name="permissions"></a><span data-ttu-id="921f8-111">权限</span><span class="sxs-lookup"><span data-stu-id="921f8-111">Permissions</span></span>

<span data-ttu-id="921f8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="921f8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="921f8-114">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="921f8-114">Permissions acting on self</span></span>

|<span data-ttu-id="921f8-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="921f8-115">Permission type</span></span>      | <span data-ttu-id="921f8-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="921f8-116">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="921f8-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="921f8-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="921f8-118">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="921f8-118">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="921f8-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="921f8-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="921f8-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="921f8-120">Not supported.</span></span> |
| <span data-ttu-id="921f8-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="921f8-121">Application</span></span>                            | <span data-ttu-id="921f8-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="921f8-122">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="921f8-123">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="921f8-123">Permissions acting on other users</span></span>

|<span data-ttu-id="921f8-124">权限类型</span><span class="sxs-lookup"><span data-stu-id="921f8-124">Permission type</span></span>      | <span data-ttu-id="921f8-125">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="921f8-125">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="921f8-126">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="921f8-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="921f8-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="921f8-127">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="921f8-128">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="921f8-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="921f8-129">不支持。</span><span class="sxs-lookup"><span data-stu-id="921f8-129">Not supported.</span></span> |
| <span data-ttu-id="921f8-130">应用程序</span><span class="sxs-lookup"><span data-stu-id="921f8-130">Application</span></span>                            | <span data-ttu-id="921f8-131">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="921f8-131">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="921f8-132">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="921f8-132">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="921f8-133">全局管理员</span><span class="sxs-lookup"><span data-stu-id="921f8-133">Global admin</span></span>
* <span data-ttu-id="921f8-134">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="921f8-134">Privileged authentication admin</span></span>
* <span data-ttu-id="921f8-135">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="921f8-135">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="921f8-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="921f8-136">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/authentication/phoneMethods/{id}
DELETE /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
<span data-ttu-id="921f8-137">与要 `id` 删除的 phoneType 对应的值是下列值之一：</span><span class="sxs-lookup"><span data-stu-id="921f8-137">The value of `id` corresponding to the phoneType to delete is one of the following:</span></span>
+ <span data-ttu-id="921f8-138">`b6332ec1-7057-4abe-9331-3d72feddfe41` 删除 `alternateMobile` **phoneType**。</span><span class="sxs-lookup"><span data-stu-id="921f8-138">`b6332ec1-7057-4abe-9331-3d72feddfe41` to delete the `alternateMobile` **phoneType**.</span></span>
+ <span data-ttu-id="921f8-139">`e37fc753-ff3b-4958-9484-eaa9425c82bc` 删除 `office` **phoneType**。</span><span class="sxs-lookup"><span data-stu-id="921f8-139">`e37fc753-ff3b-4958-9484-eaa9425c82bc` to delete the `office` **phoneType**.</span></span>
+ <span data-ttu-id="921f8-140">`3179e48a-750b-4051-897c-87b9720928f7` 删除 `mobile` **phoneType**。</span><span class="sxs-lookup"><span data-stu-id="921f8-140">`3179e48a-750b-4051-897c-87b9720928f7` to delete the `mobile` **phoneType**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="921f8-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="921f8-141">Request headers</span></span>

| <span data-ttu-id="921f8-142">名称</span><span class="sxs-lookup"><span data-stu-id="921f8-142">Name</span></span>          | <span data-ttu-id="921f8-143">说明</span><span class="sxs-lookup"><span data-stu-id="921f8-143">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="921f8-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="921f8-144">Authorization</span></span> | <span data-ttu-id="921f8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="921f8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="921f8-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="921f8-147">Request body</span></span>

<span data-ttu-id="921f8-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="921f8-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="921f8-149">响应</span><span class="sxs-lookup"><span data-stu-id="921f8-149">Response</span></span>

<span data-ttu-id="921f8-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="921f8-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="921f8-152">示例</span><span class="sxs-lookup"><span data-stu-id="921f8-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="921f8-153">请求</span><span class="sxs-lookup"><span data-stu-id="921f8-153">Request</span></span>

<span data-ttu-id="921f8-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="921f8-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="921f8-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="921f8-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_phoneauthenticationmethod"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="921f8-156">C#</span><span class="sxs-lookup"><span data-stu-id="921f8-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="921f8-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="921f8-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="921f8-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="921f8-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="921f8-159">Java</span><span class="sxs-lookup"><span data-stu-id="921f8-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="921f8-160">响应</span><span class="sxs-lookup"><span data-stu-id="921f8-160">Response</span></span>

<span data-ttu-id="921f8-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="921f8-161">The following is an example of the response.</span></span>

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
