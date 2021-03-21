---
title: 删除 fido2AuthenticationMethod
description: 删除 fido2AuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 26dc814b92a987d8868cf89d7802a601ef165dd9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964655"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="0c631-103">删除 fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0c631-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="0c631-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c631-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0c631-105">删除用户的 [FIDO2 安全密钥身份验证方法](../resources/fido2authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c631-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c631-106">权限</span><span class="sxs-lookup"><span data-stu-id="0c631-106">Permissions</span></span>

<span data-ttu-id="0c631-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c631-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="0c631-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="0c631-109">Permissions acting on self</span></span>

|<span data-ttu-id="0c631-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c631-110">Permission type</span></span>      | <span data-ttu-id="0c631-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c631-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="0c631-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c631-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c631-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c631-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="0c631-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c631-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c631-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c631-115">Not supported.</span></span> |
| <span data-ttu-id="0c631-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c631-116">Application</span></span>                            | <span data-ttu-id="0c631-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c631-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="0c631-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="0c631-118">Permissions acting on other users</span></span>

|<span data-ttu-id="0c631-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c631-119">Permission type</span></span>      | <span data-ttu-id="0c631-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c631-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="0c631-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c631-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c631-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c631-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="0c631-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c631-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c631-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c631-124">Not supported.</span></span> |
| <span data-ttu-id="0c631-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c631-125">Application</span></span>                            | <span data-ttu-id="0c631-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c631-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="0c631-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="0c631-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="0c631-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0c631-128">Global admin</span></span>
* <span data-ttu-id="0c631-129">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="0c631-129">Privileged authentication admin</span></span>
* <span data-ttu-id="0c631-130">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="0c631-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="0c631-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c631-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0c631-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c631-132">Request headers</span></span>
|<span data-ttu-id="0c631-133">名称</span><span class="sxs-lookup"><span data-stu-id="0c631-133">Name</span></span>|<span data-ttu-id="0c631-134">说明</span><span class="sxs-lookup"><span data-stu-id="0c631-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0c631-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c631-135">Authorization</span></span>|<span data-ttu-id="0c631-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c631-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c631-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c631-138">Request body</span></span>
<span data-ttu-id="0c631-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0c631-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c631-140">响应</span><span class="sxs-lookup"><span data-stu-id="0c631-140">Response</span></span>

<span data-ttu-id="0c631-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0c631-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0c631-143">示例</span><span class="sxs-lookup"><span data-stu-id="0c631-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0c631-144">请求</span><span class="sxs-lookup"><span data-stu-id="0c631-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0c631-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c631-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```

### <a name="response"></a><span data-ttu-id="0c631-146">响应</span><span class="sxs-lookup"><span data-stu-id="0c631-146">Response</span></span>
<span data-ttu-id="0c631-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0c631-147">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

