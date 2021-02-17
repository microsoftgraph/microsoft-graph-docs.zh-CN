---
title: 列出 temporaryAccessPassAuthenticationMethods
description: 获取 temporaryAccessPassAuthenticationMethod 对象及其属性的列表。
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b44daae82d401da223d7012c662c9b3c9a97bec
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272646"
---
# <a name="list-temporaryaccesspassauthenticationmethods"></a><span data-ttu-id="0269c-103">列出 temporaryAccessPassAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="0269c-103">List temporaryAccessPassAuthenticationMethods</span></span>
<span data-ttu-id="0269c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0269c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0269c-105">检索用户的临时 [AccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)  对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="0269c-105">Retrieve a list of a user's [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)  objects and their properties.</span></span> <span data-ttu-id="0269c-106">此调用将仅返回单个对象，因为只能为用户设置一个临时访问传递方法。</span><span class="sxs-lookup"><span data-stu-id="0269c-106">This call will only return a single object as only one Temporary Access Pass method can be set on users.</span></span>

## <a name="permissions"></a><span data-ttu-id="0269c-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="0269c-107">Permissions</span></span>
<span data-ttu-id="0269c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0269c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="0269c-110">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="0269c-110">Permissions acting on self</span></span>

|<span data-ttu-id="0269c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0269c-111">Permission type</span></span>      | <span data-ttu-id="0269c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0269c-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="0269c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0269c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0269c-114">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0269c-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="0269c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0269c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0269c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0269c-116">Not supported.</span></span> |
| <span data-ttu-id="0269c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0269c-117">Application</span></span>                            | <span data-ttu-id="0269c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0269c-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="0269c-119">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="0269c-119">Permissions acting on other users</span></span>

|<span data-ttu-id="0269c-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="0269c-120">Permission type</span></span>      | <span data-ttu-id="0269c-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0269c-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="0269c-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0269c-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="0269c-123">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0269c-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="0269c-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0269c-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0269c-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="0269c-125">Not supported.</span></span> |
| <span data-ttu-id="0269c-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="0269c-126">Application</span></span>                            | <span data-ttu-id="0269c-127">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0269c-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |


<span data-ttu-id="0269c-128">对于管理员正在操作其他用户的委派方案，管理员需要以下角色之 [一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="0269c-128">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="0269c-129">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0269c-129">Global admin</span></span>
* <span data-ttu-id="0269c-130">全局读取者</span><span class="sxs-lookup"><span data-stu-id="0269c-130">Global reader</span></span>
* <span data-ttu-id="0269c-131">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="0269c-131">Privileged authentication admin</span></span>
* <span data-ttu-id="0269c-132">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="0269c-132">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="0269c-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0269c-133">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0269c-134">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0269c-134">Optional query parameters</span></span>
<span data-ttu-id="0269c-135">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="0269c-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0269c-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="0269c-136">Request headers</span></span>
|<span data-ttu-id="0269c-137">名称</span><span class="sxs-lookup"><span data-stu-id="0269c-137">Name</span></span>|<span data-ttu-id="0269c-138">说明</span><span class="sxs-lookup"><span data-stu-id="0269c-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0269c-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="0269c-139">Authorization</span></span>|<span data-ttu-id="0269c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0269c-p103">Bearer {token}. Required.</span></span>|

## <a name="request"></a><span data-ttu-id="0269c-142">请求</span><span class="sxs-lookup"><span data-stu-id="0269c-142">Request</span></span> 
<span data-ttu-id="0269c-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0269c-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0269c-144">响应</span><span class="sxs-lookup"><span data-stu-id="0269c-144">Response</span></span>

<span data-ttu-id="0269c-145">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0269c-145">If successful, this method returns a `200 OK` response code and a collection of [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) objects in the response body.</span></span>  <span data-ttu-id="0269c-146">此调用将仅返回单个对象，因为只能为用户设置一个 **temporaryAccessPassAuthenticationMethod。**</span><span class="sxs-lookup"><span data-stu-id="0269c-146">This call will only return a single object because only one **temporaryAccessPassAuthenticationMethod** can be set on users.</span></span>

## <a name="examples"></a><span data-ttu-id="0269c-147">示例</span><span class="sxs-lookup"><span data-stu-id="0269c-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0269c-148">请求</span><span class="sxs-lookup"><span data-stu-id="0269c-148">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/temporaryAccessPassMethods
```


### <a name="response"></a><span data-ttu-id="0269c-149">响应</span><span class="sxs-lookup"><span data-stu-id="0269c-149">Response</span></span>
<span data-ttu-id="0269c-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0269c-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.temporaryAccessPassAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
      "id": "String",
      "temporaryAccessPass": "String",
      "createdDateTime": "String (timestamp)",
      "startDateTime": "String (timestamp)",
      "lifetimeInMinutes": "Integer",
      "isUsableOnce": "Boolean",
      "isUsable": "Boolean",
      "methodUsabilityReason": "String"
    }
  ]
}
```
