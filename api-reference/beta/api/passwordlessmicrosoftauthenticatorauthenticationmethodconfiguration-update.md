---
title: 更新 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: 更新无密码MicrosoftAuthenticatorAuthenticationMethodConfiguration 对象的属性。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a05df00deaf73d8aad7f98023b56405c2b618025
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472421"
---
# <a name="update-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-deprecated"></a><span data-ttu-id="febde-103">更新 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (弃) </span><span class="sxs-lookup"><span data-stu-id="febde-103">Update passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span></span>
<span data-ttu-id="febde-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="febde-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="febde-105">更新无 [密码MicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) 对象的属性，该对象表示 Azure AD 租户的 Microsoft Authenticator 无密码电话登录身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="febde-105">Update the properties of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in authentication method policy for the Azure AD tenant.</span></span>

> [!CAUTION]
> <span data-ttu-id="febde-106">Microsoft Authenticator 无密码电话登录身份验证方法策略 API 已弃用，并停止在 2020 年 12 月 31 日返回结果。</span><span class="sxs-lookup"><span data-stu-id="febde-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="febde-107">请使用新的 [Microsoft Authenticator 身份验证方法策略](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="febde-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="febde-108">权限</span><span class="sxs-lookup"><span data-stu-id="febde-108">Permissions</span></span>
<span data-ttu-id="febde-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="febde-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="febde-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="febde-111">Permission type</span></span>|<span data-ttu-id="febde-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="febde-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="febde-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="febde-113">Delegated (work or school account)</span></span>|<span data-ttu-id="febde-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="febde-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="febde-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="febde-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="febde-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="febde-116">Not supported.</span></span>|
|<span data-ttu-id="febde-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="febde-117">Application</span></span>|<span data-ttu-id="febde-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="febde-118">Not supported.</span></span>|

<span data-ttu-id="febde-119">对于委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="febde-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="febde-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="febde-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="febde-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="febde-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="febde-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="febde-122">Request headers</span></span>
|<span data-ttu-id="febde-123">名称</span><span class="sxs-lookup"><span data-stu-id="febde-123">Name</span></span>|<span data-ttu-id="febde-124">说明</span><span class="sxs-lookup"><span data-stu-id="febde-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="febde-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="febde-125">Authorization</span></span>|<span data-ttu-id="febde-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="febde-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="febde-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="febde-128">Content-Type</span></span>|<span data-ttu-id="febde-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="febde-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="febde-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="febde-131">Request body</span></span>
<span data-ttu-id="febde-132">在请求正文中，提供无 [密码MicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) 对象的 JSON 表示形式以及应更新的字段的值。</span><span class="sxs-lookup"><span data-stu-id="febde-132">In the request body, supply a JSON representation of a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="febde-133">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="febde-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="febde-134">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="febde-134">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="febde-135">有关属性的列表，请参阅 [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="febde-135">For the list of properties, see [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="febde-136">**注意：**`@odata.type`属性值必须为 `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` 1 的属性必须包含在正文中。</span><span class="sxs-lookup"><span data-stu-id="febde-136">**Note:** The `@odata.type` property with a value of `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` must be included in the body.</span></span>


## <a name="response"></a><span data-ttu-id="febde-137">响应</span><span class="sxs-lookup"><span data-stu-id="febde-137">Response</span></span>

<span data-ttu-id="febde-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="febde-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="febde-140">示例</span><span class="sxs-lookup"><span data-stu-id="febde-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="febde-141">请求</span><span class="sxs-lookup"><span data-stu-id="febde-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="febde-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="febde-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
    "state": "enabled"
}
```
# <a name="c"></a>[<span data-ttu-id="febde-143">C#</span><span class="sxs-lookup"><span data-stu-id="febde-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="febde-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="febde-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="febde-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="febde-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="febde-146">Java</span><span class="sxs-lookup"><span data-stu-id="febde-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="febde-147">响应</span><span class="sxs-lookup"><span data-stu-id="febde-147">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

