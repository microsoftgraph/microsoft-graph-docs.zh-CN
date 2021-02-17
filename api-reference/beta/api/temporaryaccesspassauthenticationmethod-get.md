---
title: 获取 temporaryAccessPassAuthenticationMethod
description: 读取 temporaryAccessPassAuthenticationMethod 对象的属性和关系。
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 154afeae29769fb29122f6f35503b919bfad0e7e
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272605"
---
# <a name="get-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="e0dff-103">获取 temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e0dff-103">Get temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="e0dff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0dff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0dff-105">检索用户的单个  [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0dff-105">Retrieve a user's single  [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0dff-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e0dff-106">Permissions</span></span>
<span data-ttu-id="e0dff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0dff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="e0dff-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="e0dff-109">Permissions acting on self</span></span>

|<span data-ttu-id="e0dff-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0dff-110">Permission type</span></span>      | <span data-ttu-id="e0dff-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0dff-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="e0dff-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0dff-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0dff-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0dff-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="e0dff-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0dff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0dff-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0dff-115">Not supported.</span></span> |
| <span data-ttu-id="e0dff-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0dff-116">Application</span></span>                            | <span data-ttu-id="e0dff-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0dff-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="e0dff-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="e0dff-118">Permissions acting on other users</span></span>

|<span data-ttu-id="e0dff-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0dff-119">Permission type</span></span>      | <span data-ttu-id="e0dff-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0dff-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="e0dff-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0dff-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0dff-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0dff-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="e0dff-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0dff-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0dff-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0dff-124">Not supported.</span></span> |
| <span data-ttu-id="e0dff-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0dff-125">Application</span></span>                            | <span data-ttu-id="e0dff-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0dff-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="e0dff-127">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="e0dff-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="e0dff-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="e0dff-128">Global admin</span></span>
* <span data-ttu-id="e0dff-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="e0dff-129">Global reader</span></span>
* <span data-ttu-id="e0dff-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="e0dff-130">Privileged authentication admin</span></span>
* <span data-ttu-id="e0dff-131">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="e0dff-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="e0dff-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0dff-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
```


## <a name="request-headers"></a><span data-ttu-id="e0dff-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0dff-133">Request headers</span></span>
|<span data-ttu-id="e0dff-134">名称</span><span class="sxs-lookup"><span data-stu-id="e0dff-134">Name</span></span>|<span data-ttu-id="e0dff-135">说明</span><span class="sxs-lookup"><span data-stu-id="e0dff-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e0dff-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0dff-136">Authorization</span></span>|<span data-ttu-id="e0dff-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0dff-p102">Bearer {token}. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="e0dff-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0dff-139">Request body</span></span>
<span data-ttu-id="e0dff-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e0dff-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0dff-141">响应</span><span class="sxs-lookup"><span data-stu-id="e0dff-141">Response</span></span>

<span data-ttu-id="e0dff-142">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0dff-142">If successful, this method returns a `200 OK` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0dff-143">示例</span><span class="sxs-lookup"><span data-stu-id="e0dff-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e0dff-144">请求</span><span class="sxs-lookup"><span data-stu-id="e0dff-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30
```


### <a name="response"></a><span data-ttu-id="e0dff-145">响应</span><span class="sxs-lookup"><span data-stu-id="e0dff-145">Response</span></span>
<span data-ttu-id="e0dff-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e0dff-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
    "id": "30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30",
    "temporaryAccessPass": null,
    "createdDateTime": "String (timestamp)",
    "startDateTime": "String (timestamp)",
    "lifetimeInMinutes": "Integer",
    "isUsableOnce": "Boolean",
    "isUsable": "Boolean",
    "methodUsabilityReason": "String"
  }
}
```
