---
title: 'phoneAuthenticationMethod: enableSmsSignIn'
description: 为移动电话启用 SMS 登录。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: de09f7c2dccc5f2822ec2c69646774cda722c643
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557788"
---
# <a name="phoneauthenticationmethod-enablesmssignin"></a><span data-ttu-id="0d9c1-103">phoneAuthenticationMethod: enableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="0d9c1-103">phoneAuthenticationMethod: enableSmsSignIn</span></span>

<span data-ttu-id="0d9c1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d9c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d9c1-105">为现有`mobile`的电话号码启用 SMS 登录。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-105">Enable SMS sign-in for an existing `mobile` phone number.</span></span> <span data-ttu-id="0d9c1-106">若要成功启用，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="0d9c1-106">To be successfully enabled:</span></span>

* <span data-ttu-id="0d9c1-107">电话必须具有`"phoneType": "mobile"`。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-107">The phone must have `"phoneType": "mobile"`.</span></span>
* <span data-ttu-id="0d9c1-108">电话在 SMS 登录系统中必须是唯一的（其他任何人也都不能使用该号码）。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-108">The phone must be unique in the SMS sign-in system (no one else can also be using that number).</span></span>
* <span data-ttu-id="0d9c1-109">必须为用户启用[身份验证方法](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods)策略中的 SMS 登录。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-109">The user must be enabled for SMS sign-in in the [authentication methods](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d9c1-110">权限</span><span class="sxs-lookup"><span data-stu-id="0d9c1-110">Permissions</span></span>

<span data-ttu-id="0d9c1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d9c1-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d9c1-113">Permission type</span></span>                        | <span data-ttu-id="0d9c1-114">作用于自助的权限（从最高特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d9c1-114">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="0d9c1-115">对其他用户的权限（从最低到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d9c1-115">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="0d9c1-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d9c1-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d9c1-117">UserAuthenticationMethod，UserAuthenticationMethod。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-117">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="0d9c1-118">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0d9c1-118">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="0d9c1-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d9c1-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d9c1-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-120">Not supported.</span></span> | <span data-ttu-id="0d9c1-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-121">Not supported.</span></span> |
| <span data-ttu-id="0d9c1-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d9c1-122">Application</span></span>                            | <span data-ttu-id="0d9c1-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-123">Not supported.</span></span> | <span data-ttu-id="0d9c1-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-124">Not supported.</span></span> |

<span data-ttu-id="0d9c1-125">对于在其他用户上执行管理的委派方案，管理员需要[以下角色之一](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="0d9c1-125">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="0d9c1-126">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0d9c1-126">Global admin</span></span>
* <span data-ttu-id="0d9c1-127">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="0d9c1-127">Privileged authentication admin</span></span>
* <span data-ttu-id="0d9c1-128">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="0d9c1-128">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="0d9c1-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d9c1-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/enableSmsSignIn
POST /users/{id}/authentication/phoneMethods/{id}/enableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="0d9c1-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d9c1-130">Request headers</span></span>

| <span data-ttu-id="0d9c1-131">名称</span><span class="sxs-lookup"><span data-stu-id="0d9c1-131">Name</span></span>          | <span data-ttu-id="0d9c1-132">说明</span><span class="sxs-lookup"><span data-stu-id="0d9c1-132">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0d9c1-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d9c1-133">Authorization</span></span> | <span data-ttu-id="0d9c1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d9c1-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d9c1-136">Request body</span></span>

<span data-ttu-id="0d9c1-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d9c1-138">响应</span><span class="sxs-lookup"><span data-stu-id="0d9c1-138">Response</span></span>

<span data-ttu-id="0d9c1-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d9c1-141">示例</span><span class="sxs-lookup"><span data-stu-id="0d9c1-141">Examples</span></span>

<span data-ttu-id="0d9c1-142">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-142">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0d9c1-143">请求</span><span class="sxs-lookup"><span data-stu-id="0d9c1-143">Request</span></span>

<span data-ttu-id="0d9c1-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_enablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/enableSmsSignIn
```

### <a name="response"></a><span data-ttu-id="0d9c1-145">响应</span><span class="sxs-lookup"><span data-stu-id="0d9c1-145">Response</span></span>

<span data-ttu-id="0d9c1-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0d9c1-146">The following is an example of the response.</span></span>
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
