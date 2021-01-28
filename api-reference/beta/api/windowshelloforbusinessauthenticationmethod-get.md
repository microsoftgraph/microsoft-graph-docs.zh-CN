---
title: 获取 windowsHelloForBusinessAuthenticationMethod
description: 读取 windowsHelloForBusinessAuthenticationMethod 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 74181a0af8f2c6da8fde310ce70899522bb3b27b
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033881"
---
# <a name="get-windowshelloforbusinessauthenticationmethod"></a><span data-ttu-id="636f5-103">获取 windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="636f5-103">Get windowsHelloForBusinessAuthenticationMethod</span></span>
<span data-ttu-id="636f5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="636f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="636f5-105">读取 [windowsHelloForBusinessAuthenticationMethod 对象的属性和](../resources/windowshelloforbusinessauthenticationmethod.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="636f5-105">Read the properties and relationships of a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="636f5-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="636f5-106">Permissions</span></span>

<span data-ttu-id="636f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="636f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="636f5-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="636f5-109">Permissions acting on self</span></span>

|<span data-ttu-id="636f5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="636f5-110">Permission type</span></span>      | <span data-ttu-id="636f5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="636f5-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="636f5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="636f5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="636f5-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="636f5-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="636f5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="636f5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="636f5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="636f5-115">Not supported.</span></span> |
| <span data-ttu-id="636f5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="636f5-116">Application</span></span>                            | <span data-ttu-id="636f5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="636f5-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="636f5-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="636f5-118">Permissions acting on other users</span></span>

|<span data-ttu-id="636f5-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="636f5-119">Permission type</span></span>      | <span data-ttu-id="636f5-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="636f5-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="636f5-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="636f5-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="636f5-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="636f5-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="636f5-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="636f5-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="636f5-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="636f5-124">Not supported.</span></span> |
| <span data-ttu-id="636f5-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="636f5-125">Application</span></span>                            | <span data-ttu-id="636f5-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="636f5-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="636f5-127">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="636f5-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="636f5-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="636f5-128">Global admin</span></span>
* <span data-ttu-id="636f5-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="636f5-129">Global reader</span></span>
* <span data-ttu-id="636f5-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="636f5-130">Privileged authentication admin</span></span>
* <span data-ttu-id="636f5-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="636f5-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="636f5-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="636f5-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="636f5-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="636f5-133">Optional query parameters</span></span>

<span data-ttu-id="636f5-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="636f5-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="636f5-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="636f5-135">Request headers</span></span>
|<span data-ttu-id="636f5-136">名称</span><span class="sxs-lookup"><span data-stu-id="636f5-136">Name</span></span>|<span data-ttu-id="636f5-137">说明</span><span class="sxs-lookup"><span data-stu-id="636f5-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="636f5-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="636f5-138">Authorization</span></span>|<span data-ttu-id="636f5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="636f5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="636f5-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="636f5-141">Request body</span></span>
<span data-ttu-id="636f5-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="636f5-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="636f5-143">响应</span><span class="sxs-lookup"><span data-stu-id="636f5-143">Response</span></span>

<span data-ttu-id="636f5-144">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="636f5-144">If successful, this method returns a `200 OK` response code and a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="636f5-145">示例</span><span class="sxs-lookup"><span data-stu-id="636f5-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="636f5-146">请求</span><span class="sxs-lookup"><span data-stu-id="636f5-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2
```

### <a name="response"></a><span data-ttu-id="636f5-147">响应</span><span class="sxs-lookup"><span data-stu-id="636f5-147">Response</span></span>
<span data-ttu-id="636f5-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="636f5-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsHelloForBusinessAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
    "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
    "displayName": "Jordan's Surface Book",
    "createdDateTime": "2020-11-27T23:12:49Z",
    "keyStrength": "normal"
  }
}
```

