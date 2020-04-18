---
title: 删除 phoneAuthenticationMethod
description: 删除用户的电话身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 05e6b50b04b0b527ad7b37bcadb5405c0e896fe0
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557813"
---
# <a name="delete-phoneauthenticationmethod"></a><span data-ttu-id="f5b24-103">删除 phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f5b24-103">Delete phoneAuthenticationMethod</span></span>

<span data-ttu-id="f5b24-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5b24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5b24-105">删除用户的[电话身份验证方法](../resources/phoneauthenticationmethod.md)。</span><span class="sxs-lookup"><span data-stu-id="f5b24-105">Delete a user's [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> 

><span data-ttu-id="f5b24-106">**注意：** 这将从用户中删除电话号码，并且这些号码将无法再使用身份验证的号码（无论是通过短信还是语音呼叫）。</span><span class="sxs-lookup"><span data-stu-id="f5b24-106">**Note:** This removes the phone number from the user and they will no longer be able to use the number for authentication, whether via SMS or voice calls.</span></span>

<span data-ttu-id="f5b24-107">请注意，用户的`alternateMobile`编号`mobile`不能为数字。</span><span class="sxs-lookup"><span data-stu-id="f5b24-107">Remember that a user cannot have an `alternateMobile` number without a `mobile` number.</span></span> <span data-ttu-id="f5b24-108">如果要从`mobile`也有`alternateMobile`号码的用户中删除号码，请首先将该`mobile` `alternateMobile`号码[更新](phoneauthenticationmethod-update.md)为新号码，然后删除该号码。</span><span class="sxs-lookup"><span data-stu-id="f5b24-108">If you want to remove a `mobile` number from a user that also has an `alternateMobile` number, first [update](phoneauthenticationmethod-update.md) the `mobile` number to the new number, then delete the `alternateMobile` number.</span></span>

<span data-ttu-id="f5b24-109">如果电话号码是用户的默认 Azure 多重身份验证（MFA）身份验证方法，则不能将其删除。</span><span class="sxs-lookup"><span data-stu-id="f5b24-109">If the phone number is the user's default Azure multi-factor authentication (MFA) authentication method, it cannot be deleted.</span></span> <span data-ttu-id="f5b24-110">让用户更改其默认的身份验证方法，然后删除该号码。</span><span class="sxs-lookup"><span data-stu-id="f5b24-110">Have the user change their default authentication method, and then delete the number.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5b24-111">权限</span><span class="sxs-lookup"><span data-stu-id="f5b24-111">Permissions</span></span>

<span data-ttu-id="f5b24-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5b24-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5b24-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5b24-114">Permission type</span></span>                        | <span data-ttu-id="f5b24-115">作用于自助的权限（从最高特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5b24-115">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="f5b24-116">对其他用户的权限（从最低到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5b24-116">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="f5b24-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5b24-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5b24-118">UserAuthenticationMethod，UserAuthenticationMethod。</span><span class="sxs-lookup"><span data-stu-id="f5b24-118">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="f5b24-119">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f5b24-119">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="f5b24-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5b24-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5b24-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5b24-121">Not supported.</span></span> | <span data-ttu-id="f5b24-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5b24-122">Not supported.</span></span> |
| <span data-ttu-id="f5b24-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5b24-123">Application</span></span>                            | <span data-ttu-id="f5b24-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5b24-124">Not supported.</span></span> | <span data-ttu-id="f5b24-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5b24-125">Not supported.</span></span> |

<span data-ttu-id="f5b24-126">对于在其他用户上执行管理的委派方案，管理员需要[以下角色之一](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="f5b24-126">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="f5b24-127">全局管理员</span><span class="sxs-lookup"><span data-stu-id="f5b24-127">Global admin</span></span>
* <span data-ttu-id="f5b24-128">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="f5b24-128">Privileged authentication admin</span></span>
* <span data-ttu-id="f5b24-129">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="f5b24-129">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="f5b24-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5b24-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/authentication/phoneMethods/{id}
DELETE /users/{id}/authentication/phoneMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f5b24-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5b24-131">Request headers</span></span>

| <span data-ttu-id="f5b24-132">名称</span><span class="sxs-lookup"><span data-stu-id="f5b24-132">Name</span></span>          | <span data-ttu-id="f5b24-133">说明</span><span class="sxs-lookup"><span data-stu-id="f5b24-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f5b24-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5b24-134">Authorization</span></span> | <span data-ttu-id="f5b24-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f5b24-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5b24-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5b24-137">Request body</span></span>

<span data-ttu-id="f5b24-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f5b24-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5b24-139">响应</span><span class="sxs-lookup"><span data-stu-id="f5b24-139">Response</span></span>

<span data-ttu-id="f5b24-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f5b24-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5b24-142">示例</span><span class="sxs-lookup"><span data-stu-id="f5b24-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5b24-143">请求</span><span class="sxs-lookup"><span data-stu-id="f5b24-143">Request</span></span>

<span data-ttu-id="f5b24-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f5b24-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_phoneauthenticationmethod"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```

### <a name="response"></a><span data-ttu-id="f5b24-145">响应</span><span class="sxs-lookup"><span data-stu-id="f5b24-145">Response</span></span>

<span data-ttu-id="f5b24-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f5b24-146">The following is an example of the response.</span></span>

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
