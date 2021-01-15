---
title: 更新 microsoftAuthenticatorAuthenticationMethodConfiguration
description: 更新 microsoftAuthenticatorAuthenticationMethodConfiguration 对象的属性。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b6d715e32d2e42a81cf042884ab38d4f06097a3f
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874479"
---
# <a name="update-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="05894-103">更新 microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="05894-103">Update microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="05894-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05894-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05894-105">更新 [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) 对象的属性，该对象表示 Azure AD 租户的 Microsoft Authenticator 身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="05894-105">Update the properties of a [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator authentication method policy for the Azure AD tenant.</span></span>


## <a name="permissions"></a><span data-ttu-id="05894-106">权限</span><span class="sxs-lookup"><span data-stu-id="05894-106">Permissions</span></span>
<span data-ttu-id="05894-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05894-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05894-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="05894-109">Permission type</span></span>|<span data-ttu-id="05894-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05894-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05894-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05894-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05894-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="05894-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="05894-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05894-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05894-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="05894-114">Not supported.</span></span>|
|<span data-ttu-id="05894-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="05894-115">Application</span></span>|<span data-ttu-id="05894-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="05894-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="05894-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="05894-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="05894-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="05894-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="05894-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05894-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="05894-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="05894-120">Request headers</span></span>
|<span data-ttu-id="05894-121">名称</span><span class="sxs-lookup"><span data-stu-id="05894-121">Name</span></span>|<span data-ttu-id="05894-122">说明</span><span class="sxs-lookup"><span data-stu-id="05894-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="05894-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05894-123">Authorization</span></span>|<span data-ttu-id="05894-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05894-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="05894-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05894-126">Content-Type</span></span>|<span data-ttu-id="05894-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="05894-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="05894-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="05894-129">Request body</span></span>
<span data-ttu-id="05894-130">在请求正文中，提供 [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) 对象的 JSON 表示形式以及应更新的字段的值。</span><span class="sxs-lookup"><span data-stu-id="05894-130">In the request body, supply a JSON representation of the [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="05894-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="05894-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="05894-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="05894-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="05894-133">有关属性的列表，请参阅[microsoftAuthenticatorAuthenticationMethodConfiguration。](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05894-133">For the list of properties, see [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="05894-134">**注意：**`@odata.type`正文中必须包含属性值为 `#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration` 1 的属性。</span><span class="sxs-lookup"><span data-stu-id="05894-134">**Note:** The `@odata.type` property with a value of `#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="05894-135">响应</span><span class="sxs-lookup"><span data-stu-id="05894-135">Response</span></span>

<span data-ttu-id="05894-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="05894-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05894-138">示例</span><span class="sxs-lookup"><span data-stu-id="05894-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="05894-139">请求</span><span class="sxs-lookup"><span data-stu-id="05894-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
Content-Type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "state": "String"
}
```


### <a name="response"></a><span data-ttu-id="05894-140">响应</span><span class="sxs-lookup"><span data-stu-id="05894-140">Response</span></span>
<span data-ttu-id="05894-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="05894-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "129ae788-e788-129a-88e7-9a1288e79a12",
  "state": "String"
}
```

