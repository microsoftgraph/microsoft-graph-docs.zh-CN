---
title: 'phoneAuthenticationMethod: disableSmsSignIn'
description: 禁用移动电话的 SMS 登录
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dfb16775b2c4a452b3218e7fc4e19620e4174f16
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557778"
---
# <a name="phoneauthenticationmethod-disablesmssignin"></a><span data-ttu-id="ea129-103">phoneAuthenticationMethod: disableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="ea129-103">phoneAuthenticationMethod: disableSmsSignIn</span></span>

<span data-ttu-id="ea129-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea129-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea129-105">禁用现有`mobile`电话号码的 SMS 登录。</span><span class="sxs-lookup"><span data-stu-id="ea129-105">Disable SMS sign-in for an existing `mobile` phone number.</span></span> 

><span data-ttu-id="ea129-106">**注意：** 该号码将不再可用于 SMS 登录，这可能会阻止用户登录。</span><span class="sxs-lookup"><span data-stu-id="ea129-106">**Note:** The number will no longer be available for SMS sign-in, which can prevent your user from signing in.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea129-107">权限</span><span class="sxs-lookup"><span data-stu-id="ea129-107">Permissions</span></span>

<span data-ttu-id="ea129-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea129-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea129-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea129-110">Permission type</span></span>                        | <span data-ttu-id="ea129-111">作用于自助的权限（从最高特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea129-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="ea129-112">对其他用户的权限（从最低到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea129-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="ea129-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea129-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea129-114">UserAuthenticationMethod，UserAuthenticationMethod。</span><span class="sxs-lookup"><span data-stu-id="ea129-114">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="ea129-115">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ea129-115">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="ea129-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea129-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea129-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea129-117">Not supported.</span></span> | <span data-ttu-id="ea129-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea129-118">Not supported.</span></span> |
| <span data-ttu-id="ea129-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea129-119">Application</span></span>                            | <span data-ttu-id="ea129-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea129-120">Not supported.</span></span> | <span data-ttu-id="ea129-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea129-121">Not supported.</span></span> |

<span data-ttu-id="ea129-122">对于在其他用户上执行管理的委派方案，管理员需要[以下角色之一](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="ea129-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="ea129-123">全局管理员</span><span class="sxs-lookup"><span data-stu-id="ea129-123">Global admin</span></span>
* <span data-ttu-id="ea129-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="ea129-124">Privileged authentication admin</span></span>
* <span data-ttu-id="ea129-125">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="ea129-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="ea129-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea129-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/disableSmsSignIn
POST /users/{id}/authentication/phoneMethods/{id}/disableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="ea129-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea129-127">Request headers</span></span>

| <span data-ttu-id="ea129-128">名称</span><span class="sxs-lookup"><span data-stu-id="ea129-128">Name</span></span>          | <span data-ttu-id="ea129-129">说明</span><span class="sxs-lookup"><span data-stu-id="ea129-129">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ea129-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea129-130">Authorization</span></span> | <span data-ttu-id="ea129-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ea129-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea129-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea129-133">Request body</span></span>

<span data-ttu-id="ea129-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ea129-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea129-135">响应</span><span class="sxs-lookup"><span data-stu-id="ea129-135">Response</span></span>

<span data-ttu-id="ea129-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ea129-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ea129-138">示例</span><span class="sxs-lookup"><span data-stu-id="ea129-138">Examples</span></span>

<span data-ttu-id="ea129-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="ea129-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ea129-140">请求</span><span class="sxs-lookup"><span data-stu-id="ea129-140">Request</span></span>

<span data-ttu-id="ea129-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ea129-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_disablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn
```

### <a name="response"></a><span data-ttu-id="ea129-142">响应</span><span class="sxs-lookup"><span data-stu-id="ea129-142">Response</span></span>

<span data-ttu-id="ea129-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ea129-143">The following is an example of the response.</span></span>
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
