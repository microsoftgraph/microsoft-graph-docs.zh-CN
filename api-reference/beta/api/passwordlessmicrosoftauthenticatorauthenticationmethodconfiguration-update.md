---
title: 更新 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: 更新 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 对象的属性。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8536e70f264775a073830aeac77d3fc27810e5f0
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418274"
---
# <a name="update-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="521cb-103">更新 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="521cb-103">Update passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="521cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="521cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="521cb-105">更新 [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) 对象的属性，该对象代表 Azure AD 租户的 Microsoft 身份验证器 Passwordless 电话登录身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="521cb-105">Update the properties of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in authentication method policy for the Azure AD tenant.</span></span>

> [!NOTE]
> <span data-ttu-id="521cb-106">在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。</span><span class="sxs-lookup"><span data-stu-id="521cb-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="521cb-107">由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。</span><span class="sxs-lookup"><span data-stu-id="521cb-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="521cb-108">权限</span><span class="sxs-lookup"><span data-stu-id="521cb-108">Permissions</span></span>
<span data-ttu-id="521cb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="521cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="521cb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="521cb-111">Permission type</span></span>|<span data-ttu-id="521cb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="521cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="521cb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="521cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="521cb-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="521cb-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="521cb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="521cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="521cb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="521cb-116">Not supported.</span></span>|
|<span data-ttu-id="521cb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="521cb-117">Application</span></span>|<span data-ttu-id="521cb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="521cb-118">Not supported.</span></span>|

<span data-ttu-id="521cb-119">对于委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="521cb-119">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="521cb-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="521cb-120">Global admin</span></span>
* <span data-ttu-id="521cb-121">全局读取者</span><span class="sxs-lookup"><span data-stu-id="521cb-121">Global reader</span></span>
* <span data-ttu-id="521cb-122">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="521cb-122">Privileged authentication admin</span></span>
* <span data-ttu-id="521cb-123">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="521cb-123">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="521cb-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="521cb-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="521cb-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="521cb-125">Request headers</span></span>
|<span data-ttu-id="521cb-126">名称</span><span class="sxs-lookup"><span data-stu-id="521cb-126">Name</span></span>|<span data-ttu-id="521cb-127">说明</span><span class="sxs-lookup"><span data-stu-id="521cb-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="521cb-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="521cb-128">Authorization</span></span>|<span data-ttu-id="521cb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="521cb-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="521cb-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="521cb-131">Content-Type</span></span>|<span data-ttu-id="521cb-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="521cb-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="521cb-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="521cb-134">Request body</span></span>
<span data-ttu-id="521cb-135">在请求正文中，提供 [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) 对象的 JSON 表示形式，其中包含应更新的字段的值。</span><span class="sxs-lookup"><span data-stu-id="521cb-135">In the request body, supply a JSON representation of a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="521cb-136">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="521cb-136">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="521cb-137">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="521cb-137">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="521cb-138">有关属性的列表，请参阅 [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="521cb-138">For the list of properties, see [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="521cb-139">**注意：**`@odata.type`值为的属性 `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` 必须包含在正文中。</span><span class="sxs-lookup"><span data-stu-id="521cb-139">**Note:** The `@odata.type` property with a value of `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` must be included in the body.</span></span>


## <a name="response"></a><span data-ttu-id="521cb-140">响应</span><span class="sxs-lookup"><span data-stu-id="521cb-140">Response</span></span>

<span data-ttu-id="521cb-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="521cb-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="521cb-143">示例</span><span class="sxs-lookup"><span data-stu-id="521cb-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="521cb-144">请求</span><span class="sxs-lookup"><span data-stu-id="521cb-144">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="521cb-145">响应</span><span class="sxs-lookup"><span data-stu-id="521cb-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

