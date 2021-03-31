---
title: 更新 emailAuthenticationMethodConfiguration
description: 更新 emailAuthenticationMethodConfiguration 对象的属性。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ce5d52d99f2f80b4ff285a5ebfc1971db1932383
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469274"
---
# <a name="update-emailauthenticationmethodconfiguration"></a><span data-ttu-id="73225-103">更新 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="73225-103">Update emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="73225-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73225-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73225-105">更新 [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) 对象的属性，该对象表示 Azure Active Directory (Azure AD 租户的电子邮件 [OTP](../resources/authenticationmethodspolicies-overview.md)) 策略。</span><span class="sxs-lookup"><span data-stu-id="73225-105">Update the properties of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="73225-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="73225-106">Permissions</span></span>
<span data-ttu-id="73225-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73225-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73225-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73225-109">Permission type</span></span>|<span data-ttu-id="73225-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73225-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73225-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73225-111">Delegated (work or school account)</span></span>|<span data-ttu-id="73225-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73225-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="73225-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73225-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73225-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73225-114">Not supported.</span></span>|
|<span data-ttu-id="73225-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="73225-115">Application</span></span>|<span data-ttu-id="73225-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73225-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="73225-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="73225-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="73225-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="73225-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="73225-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73225-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /policies/authenticationMethodsPolicy/email
```

## <a name="request-headers"></a><span data-ttu-id="73225-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="73225-120">Request headers</span></span>

|<span data-ttu-id="73225-121">名称</span><span class="sxs-lookup"><span data-stu-id="73225-121">Name</span></span>|<span data-ttu-id="73225-122">说明</span><span class="sxs-lookup"><span data-stu-id="73225-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="73225-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="73225-123">Authorization</span></span>|<span data-ttu-id="73225-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73225-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="73225-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73225-126">Content-Type</span></span>|<span data-ttu-id="73225-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="73225-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73225-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="73225-129">Request body</span></span>

<span data-ttu-id="73225-130">在请求正文中，提供 [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73225-130">In the request body, supply a JSON representation of the [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object.</span></span> <span data-ttu-id="73225-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="73225-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="73225-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="73225-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="73225-133">有关可更新的属性的列表，请参阅 [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="73225-133">For the list of properties that can be updated, see [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="73225-134">**注意：**`@odata.type`属性值为 的 `#microsoft.graph.emailAuthenticationMethodConfiguration` 属性必须包含在正文中。</span><span class="sxs-lookup"><span data-stu-id="73225-134">**Note:** The `@odata.type` property with a value of `#microsoft.graph.emailAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="73225-135">响应</span><span class="sxs-lookup"><span data-stu-id="73225-135">Response</span></span>

<span data-ttu-id="73225-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="73225-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73225-138">示例</span><span class="sxs-lookup"><span data-stu-id="73225-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73225-139">请求</span><span class="sxs-lookup"><span data-stu-id="73225-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_emailauthenticationmethodconfiguration"
}
-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfiguration/email
Content-Type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "allowExternalIdToUseEmailOtp": "false",
}
```

### <a name="response"></a><span data-ttu-id="73225-140">响应</span><span class="sxs-lookup"><span data-stu-id="73225-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 NO CONTENT
```

