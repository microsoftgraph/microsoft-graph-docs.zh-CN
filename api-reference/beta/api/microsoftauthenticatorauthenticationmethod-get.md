---
title: 获取 microsoftAuthenticatorAuthenticationMethod
description: 读取 microsoftAuthenticatorAuthenticationMethod 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 76a192e9fd896f65deaba715b32cc8a0a4cad09a
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873442"
---
# <a name="get-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="53f89-103">获取 microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="53f89-103">Get microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="53f89-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53f89-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53f89-105">读取 [microsoftAuthenticatorAuthenticationMethod 对象的属性和](../resources/microsoftauthenticatorauthenticationmethod.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="53f89-105">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53f89-106">权限</span><span class="sxs-lookup"><span data-stu-id="53f89-106">Permissions</span></span>

<span data-ttu-id="53f89-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53f89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="53f89-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="53f89-109">Permissions acting on self</span></span>

|<span data-ttu-id="53f89-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="53f89-110">Permission type</span></span>      | <span data-ttu-id="53f89-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53f89-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="53f89-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53f89-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="53f89-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53f89-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="53f89-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53f89-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53f89-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="53f89-115">Not supported.</span></span> |
| <span data-ttu-id="53f89-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="53f89-116">Application</span></span>                            | <span data-ttu-id="53f89-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="53f89-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="53f89-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="53f89-118">Permissions acting on other users</span></span>

|<span data-ttu-id="53f89-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="53f89-119">Permission type</span></span>      | <span data-ttu-id="53f89-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53f89-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="53f89-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53f89-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="53f89-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53f89-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="53f89-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53f89-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53f89-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="53f89-124">Not supported.</span></span> |
| <span data-ttu-id="53f89-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="53f89-125">Application</span></span>                            | <span data-ttu-id="53f89-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53f89-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="53f89-127">对于管理员正在操作其他用户的委派方案，管理员需要以下角色 [之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="53f89-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="53f89-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="53f89-128">Global admin</span></span>
* <span data-ttu-id="53f89-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="53f89-129">Global reader</span></span>
* <span data-ttu-id="53f89-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="53f89-130">Privileged authentication admin</span></span>
* <span data-ttu-id="53f89-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="53f89-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="53f89-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53f89-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53f89-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="53f89-133">Optional query parameters</span></span>
<span data-ttu-id="53f89-134">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="53f89-134">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="53f89-135">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="53f89-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="53f89-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="53f89-136">Request headers</span></span>
|<span data-ttu-id="53f89-137">名称</span><span class="sxs-lookup"><span data-stu-id="53f89-137">Name</span></span>|<span data-ttu-id="53f89-138">说明</span><span class="sxs-lookup"><span data-stu-id="53f89-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="53f89-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="53f89-139">Authorization</span></span>|<span data-ttu-id="53f89-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53f89-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53f89-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="53f89-142">Request body</span></span>
<span data-ttu-id="53f89-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53f89-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53f89-144">响应</span><span class="sxs-lookup"><span data-stu-id="53f89-144">Response</span></span>

<span data-ttu-id="53f89-145">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53f89-145">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53f89-146">示例</span><span class="sxs-lookup"><span data-stu-id="53f89-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53f89-147">请求</span><span class="sxs-lookup"><span data-stu-id="53f89-147">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a><span data-ttu-id="53f89-148">响应</span><span class="sxs-lookup"><span data-stu-id="53f89-148">Response</span></span>
<span data-ttu-id="53f89-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="53f89-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
    "id": "6803c096-c096-6803-96c0-036896c00368",
    "displayName": "Sandeep's iPhone",
    "deviceTag": "",
    "phoneAppVersion": "6.5.4",
    "createdDateTime": "2020-12-03T23:16:12Z"
  }
}
```
