---
title: 获取 windowsHelloForBusinessAuthenticationMethod
description: 读取 windowsHelloForBusinessAuthenticationMethod 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e9fdb6b8b48a12f1f618479b2e939944e25288fe
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873309"
---
# <a name="get-windowshelloforbusinessauthenticationmethod"></a><span data-ttu-id="cba72-103">获取 windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cba72-103">Get windowsHelloForBusinessAuthenticationMethod</span></span>
<span data-ttu-id="cba72-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cba72-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cba72-105">读取 [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cba72-105">Read the properties and relationships of a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cba72-106">权限</span><span class="sxs-lookup"><span data-stu-id="cba72-106">Permissions</span></span>

<span data-ttu-id="cba72-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cba72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="cba72-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="cba72-109">Permissions acting on self</span></span>

|<span data-ttu-id="cba72-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cba72-110">Permission type</span></span>      | <span data-ttu-id="cba72-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cba72-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="cba72-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cba72-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cba72-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cba72-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="cba72-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cba72-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cba72-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cba72-115">Not supported.</span></span> |
| <span data-ttu-id="cba72-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cba72-116">Application</span></span>                            | <span data-ttu-id="cba72-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cba72-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="cba72-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="cba72-118">Permissions acting on other users</span></span>

|<span data-ttu-id="cba72-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="cba72-119">Permission type</span></span>      | <span data-ttu-id="cba72-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cba72-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="cba72-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cba72-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="cba72-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cba72-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="cba72-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cba72-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cba72-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="cba72-124">Not supported.</span></span> |
| <span data-ttu-id="cba72-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="cba72-125">Application</span></span>                            | <span data-ttu-id="cba72-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cba72-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="cba72-127">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="cba72-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="cba72-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="cba72-128">Global admin</span></span>
* <span data-ttu-id="cba72-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="cba72-129">Global reader</span></span>
* <span data-ttu-id="cba72-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="cba72-130">Privileged authentication admin</span></span>
* <span data-ttu-id="cba72-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="cba72-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="cba72-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cba72-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cba72-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cba72-133">Optional query parameters</span></span>

<span data-ttu-id="cba72-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="cba72-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cba72-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="cba72-135">Request headers</span></span>
|<span data-ttu-id="cba72-136">名称</span><span class="sxs-lookup"><span data-stu-id="cba72-136">Name</span></span>|<span data-ttu-id="cba72-137">说明</span><span class="sxs-lookup"><span data-stu-id="cba72-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cba72-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="cba72-138">Authorization</span></span>|<span data-ttu-id="cba72-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cba72-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cba72-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="cba72-141">Request body</span></span>
<span data-ttu-id="cba72-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cba72-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cba72-143">响应</span><span class="sxs-lookup"><span data-stu-id="cba72-143">Response</span></span>

<span data-ttu-id="cba72-144">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cba72-144">If successful, this method returns a `200 OK` response code and a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cba72-145">示例</span><span class="sxs-lookup"><span data-stu-id="cba72-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cba72-146">请求</span><span class="sxs-lookup"><span data-stu-id="cba72-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2
```

### <a name="response"></a><span data-ttu-id="cba72-147">响应</span><span class="sxs-lookup"><span data-stu-id="cba72-147">Response</span></span>
<span data-ttu-id="cba72-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cba72-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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

