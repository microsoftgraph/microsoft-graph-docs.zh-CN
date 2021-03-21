---
title: 删除 windowsHelloForBusinessAuthenticationMethod
description: 删除 windowsHelloForBusinessAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e07acd532a20c54a9ac503a53024aeb40df40380
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964643"
---
# <a name="delete-windowshelloforbusinessauthenticationmethod"></a><span data-ttu-id="766c9-103">删除 windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="766c9-103">Delete windowsHelloForBusinessAuthenticationMethod</span></span>
<span data-ttu-id="766c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="766c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="766c9-105">删除 [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="766c9-105">Deletes a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="766c9-106">权限</span><span class="sxs-lookup"><span data-stu-id="766c9-106">Permissions</span></span>

<span data-ttu-id="766c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="766c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="766c9-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="766c9-109">Permissions acting on self</span></span>

|<span data-ttu-id="766c9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="766c9-110">Permission type</span></span>      | <span data-ttu-id="766c9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="766c9-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="766c9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="766c9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="766c9-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="766c9-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="766c9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="766c9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="766c9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="766c9-115">Not supported.</span></span> |
| <span data-ttu-id="766c9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="766c9-116">Application</span></span>                            | <span data-ttu-id="766c9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="766c9-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="766c9-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="766c9-118">Permissions acting on other users</span></span>

|<span data-ttu-id="766c9-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="766c9-119">Permission type</span></span>      | <span data-ttu-id="766c9-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="766c9-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="766c9-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="766c9-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="766c9-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="766c9-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="766c9-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="766c9-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="766c9-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="766c9-124">Not supported.</span></span> |
| <span data-ttu-id="766c9-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="766c9-125">Application</span></span>                            | <span data-ttu-id="766c9-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="766c9-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="766c9-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="766c9-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="766c9-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="766c9-128">Global admin</span></span>
* <span data-ttu-id="766c9-129">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="766c9-129">Privileged authentication admin</span></span>
* <span data-ttu-id="766c9-130">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="766c9-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="766c9-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="766c9-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
DELETE /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
```

## <a name="request-headers"></a><span data-ttu-id="766c9-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="766c9-132">Request headers</span></span>
|<span data-ttu-id="766c9-133">名称</span><span class="sxs-lookup"><span data-stu-id="766c9-133">Name</span></span>|<span data-ttu-id="766c9-134">说明</span><span class="sxs-lookup"><span data-stu-id="766c9-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="766c9-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="766c9-135">Authorization</span></span>|<span data-ttu-id="766c9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="766c9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="766c9-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="766c9-138">Request body</span></span>
<span data-ttu-id="766c9-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="766c9-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="766c9-140">响应</span><span class="sxs-lookup"><span data-stu-id="766c9-140">Response</span></span>

<span data-ttu-id="766c9-141">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="766c9-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="766c9-142">示例</span><span class="sxs-lookup"><span data-stu-id="766c9-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="766c9-143">请求</span><span class="sxs-lookup"><span data-stu-id="766c9-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/users/kim@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a><span data-ttu-id="766c9-144">响应</span><span class="sxs-lookup"><span data-stu-id="766c9-144">Response</span></span>
<span data-ttu-id="766c9-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="766c9-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

