---
title: 列出 windowsHelloForBusinessAuthenticationMethods
description: 获取 windowsHelloForBusinessAuthenticationMethod 对象及其属性的列表。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: df1f8979ef506eaddd4cf68bb3f60f8da9656d86
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964641"
---
# <a name="list-windowshelloforbusinessauthenticationmethods"></a><span data-ttu-id="b6d16-103">列出 windowsHelloForBusinessAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="b6d16-103">List windowsHelloForBusinessAuthenticationMethods</span></span>
<span data-ttu-id="b6d16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6d16-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6d16-105">获取 [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="b6d16-105">Get a list of the [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6d16-106">权限</span><span class="sxs-lookup"><span data-stu-id="b6d16-106">Permissions</span></span>

<span data-ttu-id="b6d16-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6d16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="b6d16-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="b6d16-109">Permissions acting on self</span></span>

|<span data-ttu-id="b6d16-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6d16-110">Permission type</span></span>      | <span data-ttu-id="b6d16-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b6d16-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="b6d16-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6d16-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6d16-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6d16-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="b6d16-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6d16-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6d16-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6d16-115">Not supported.</span></span> |
| <span data-ttu-id="b6d16-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6d16-116">Application</span></span>                            | <span data-ttu-id="b6d16-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6d16-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="b6d16-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="b6d16-118">Permissions acting on other users</span></span>

|<span data-ttu-id="b6d16-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6d16-119">Permission type</span></span>      | <span data-ttu-id="b6d16-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b6d16-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="b6d16-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6d16-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6d16-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6d16-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b6d16-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6d16-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6d16-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6d16-124">Not supported.</span></span> |
| <span data-ttu-id="b6d16-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6d16-125">Application</span></span>                            | <span data-ttu-id="b6d16-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6d16-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="b6d16-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="b6d16-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="b6d16-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="b6d16-128">Global admin</span></span>
* <span data-ttu-id="b6d16-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="b6d16-129">Global reader</span></span>
* <span data-ttu-id="b6d16-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="b6d16-130">Privileged authentication admin</span></span>
* <span data-ttu-id="b6d16-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="b6d16-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="b6d16-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6d16-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/windowsHelloForBusinessMethods
GET /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6d16-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b6d16-133">Optional query parameters</span></span>

<span data-ttu-id="b6d16-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6d16-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6d16-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6d16-135">Request headers</span></span>
|<span data-ttu-id="b6d16-136">名称</span><span class="sxs-lookup"><span data-stu-id="b6d16-136">Name</span></span>|<span data-ttu-id="b6d16-137">说明</span><span class="sxs-lookup"><span data-stu-id="b6d16-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b6d16-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6d16-138">Authorization</span></span>|<span data-ttu-id="b6d16-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b6d16-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6d16-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6d16-141">Request body</span></span>
<span data-ttu-id="b6d16-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b6d16-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6d16-143">响应</span><span class="sxs-lookup"><span data-stu-id="b6d16-143">Response</span></span>

<span data-ttu-id="b6d16-144">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b6d16-144">If successful, this method returns a `200 OK` response code and a collection of [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b6d16-145">示例</span><span class="sxs-lookup"><span data-stu-id="b6d16-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b6d16-146">请求</span><span class="sxs-lookup"><span data-stu-id="b6d16-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods
```


### <a name="response"></a><span data-ttu-id="b6d16-147">响应</span><span class="sxs-lookup"><span data-stu-id="b6d16-147">Response</span></span>
<span data-ttu-id="b6d16-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b6d16-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsHelloForBusinessAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
      "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
      "displayName": "Jordan's Surface Book",
      "createdDateTime": "2020-11-27T23:12:49Z",
      "keyStrength": "normal"
    },
    {
      "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
      "id": "e6dab818-e68d-433e-89d5-547357870cb2",
      "displayName": "New Surface Duo",
      "createdDateTime": "2020-12-25T02:20:13Z",
      "keyStrength": "normal"
    }
  ]
}
```

