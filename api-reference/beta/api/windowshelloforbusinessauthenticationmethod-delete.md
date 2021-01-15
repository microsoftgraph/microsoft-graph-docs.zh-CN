---
title: 删除 windowsHelloForBusinessAuthenticationMethod
description: 删除 windowsHelloForBusinessAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d0412cc7bdc1ed20ddba80d70b992d3859ca507c
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873316"
---
# <a name="delete-windowshelloforbusinessauthenticationmethod"></a><span data-ttu-id="4ac68-103">删除 windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4ac68-103">Delete windowsHelloForBusinessAuthenticationMethod</span></span>
<span data-ttu-id="4ac68-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ac68-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ac68-105">删除 [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ac68-105">Deletes a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ac68-106">权限</span><span class="sxs-lookup"><span data-stu-id="4ac68-106">Permissions</span></span>

<span data-ttu-id="4ac68-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ac68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="4ac68-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="4ac68-109">Permissions acting on self</span></span>

|<span data-ttu-id="4ac68-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ac68-110">Permission type</span></span>      | <span data-ttu-id="4ac68-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ac68-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="4ac68-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ac68-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ac68-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ac68-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="4ac68-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ac68-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ac68-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ac68-115">Not supported.</span></span> |
| <span data-ttu-id="4ac68-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ac68-116">Application</span></span>                            | <span data-ttu-id="4ac68-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ac68-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="4ac68-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="4ac68-118">Permissions acting on other users</span></span>

|<span data-ttu-id="4ac68-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ac68-119">Permission type</span></span>      | <span data-ttu-id="4ac68-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ac68-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="4ac68-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ac68-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ac68-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ac68-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="4ac68-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ac68-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ac68-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ac68-124">Not supported.</span></span> |
| <span data-ttu-id="4ac68-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ac68-125">Application</span></span>                            | <span data-ttu-id="4ac68-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ac68-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="4ac68-127">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="4ac68-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="4ac68-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4ac68-128">Global admin</span></span>
* <span data-ttu-id="4ac68-129">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="4ac68-129">Privileged authentication admin</span></span>
* <span data-ttu-id="4ac68-130">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="4ac68-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="4ac68-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ac68-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
DELETE /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
```

## <a name="request-headers"></a><span data-ttu-id="4ac68-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ac68-132">Request headers</span></span>
|<span data-ttu-id="4ac68-133">名称</span><span class="sxs-lookup"><span data-stu-id="4ac68-133">Name</span></span>|<span data-ttu-id="4ac68-134">说明</span><span class="sxs-lookup"><span data-stu-id="4ac68-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4ac68-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ac68-135">Authorization</span></span>|<span data-ttu-id="4ac68-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ac68-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ac68-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ac68-138">Request body</span></span>
<span data-ttu-id="4ac68-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ac68-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ac68-140">响应</span><span class="sxs-lookup"><span data-stu-id="4ac68-140">Response</span></span>

<span data-ttu-id="4ac68-141">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4ac68-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4ac68-142">示例</span><span class="sxs-lookup"><span data-stu-id="4ac68-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4ac68-143">请求</span><span class="sxs-lookup"><span data-stu-id="4ac68-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a><span data-ttu-id="4ac68-144">响应</span><span class="sxs-lookup"><span data-stu-id="4ac68-144">Response</span></span>
<span data-ttu-id="4ac68-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4ac68-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

