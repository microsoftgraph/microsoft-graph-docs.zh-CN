---
title: 删除 emailAuthenticationMethod
description: 删除一个 emailAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 281d20e1903e05c4d131f3b2a087d5c1d2043793
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418258"
---
# <a name="delete-emailauthenticationmethod"></a><span data-ttu-id="7f11f-103">删除 emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7f11f-103">Delete emailAuthenticationMethod</span></span>
<span data-ttu-id="7f11f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f11f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f11f-105">删除用户的 [电子邮件身份验证方法](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f11f-105">Deletes a user's [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f11f-106">权限</span><span class="sxs-lookup"><span data-stu-id="7f11f-106">Permissions</span></span>
<span data-ttu-id="7f11f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f11f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f11f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f11f-109">Permission type</span></span>|<span data-ttu-id="7f11f-110">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="7f11f-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="7f11f-111">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="7f11f-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="7f11f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f11f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f11f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f11f-113">Not supported.</span></span>|<span data-ttu-id="7f11f-114">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7f11f-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="7f11f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f11f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f11f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f11f-116">Not supported.</span></span>|<span data-ttu-id="7f11f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f11f-117">Not supported.</span></span>
|<span data-ttu-id="7f11f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f11f-118">Application</span></span>|<span data-ttu-id="7f11f-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f11f-119">Not supported.</span></span>|<span data-ttu-id="7f11f-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f11f-120">Not supported.</span></span>

<span data-ttu-id="7f11f-121">对于在其他用户上执行管理的委派方案，管理员需要 [以下角色之一](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="7f11f-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="7f11f-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="7f11f-122">Global admin</span></span>
* <span data-ttu-id="7f11f-123">全局读取者</span><span class="sxs-lookup"><span data-stu-id="7f11f-123">Global reader</span></span>
* <span data-ttu-id="7f11f-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="7f11f-124">Privileged authentication admin</span></span>
* <span data-ttu-id="7f11f-125">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="7f11f-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="7f11f-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f11f-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7f11f-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f11f-127">Request headers</span></span>
|<span data-ttu-id="7f11f-128">名称</span><span class="sxs-lookup"><span data-stu-id="7f11f-128">Name</span></span>|<span data-ttu-id="7f11f-129">说明</span><span class="sxs-lookup"><span data-stu-id="7f11f-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7f11f-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f11f-130">Authorization</span></span>|<span data-ttu-id="7f11f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f11f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f11f-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f11f-133">Request body</span></span>
<span data-ttu-id="7f11f-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f11f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f11f-135">响应</span><span class="sxs-lookup"><span data-stu-id="7f11f-135">Response</span></span>

<span data-ttu-id="7f11f-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7f11f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7f11f-138">示例</span><span class="sxs-lookup"><span data-stu-id="7f11f-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7f11f-139">请求</span><span class="sxs-lookup"><span data-stu-id="7f11f-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```


### <a name="response"></a><span data-ttu-id="7f11f-140">响应</span><span class="sxs-lookup"><span data-stu-id="7f11f-140">Response</span></span>
<span data-ttu-id="7f11f-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7f11f-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

