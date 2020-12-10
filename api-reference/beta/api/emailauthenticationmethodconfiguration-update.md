---
title: 更新 emailAuthenticationMethodConfiguration
description: 更新 emailAuthenticationMethodConfiguration 对象的属性。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b7fdd3566904c3ee8ad56210be03a8274cc858b
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617112"
---
# <a name="update-emailauthenticationmethodconfiguration"></a><span data-ttu-id="e49d4-103">更新 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="e49d4-103">Update emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="e49d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e49d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e49d4-105">更新 [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) 对象的属性，该对象表示 Azure Active Directory (azure AD) 租户的电子邮件 OTP [身份验证方法策略](../resources/authenticationmethodspolicies-overview.md) 。</span><span class="sxs-lookup"><span data-stu-id="e49d4-105">Update the properties of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e49d4-106">权限</span><span class="sxs-lookup"><span data-stu-id="e49d4-106">Permissions</span></span>
<span data-ttu-id="e49d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e49d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e49d4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e49d4-109">Permission type</span></span>|<span data-ttu-id="e49d4-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e49d4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e49d4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e49d4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e49d4-112">Policy 写的 AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e49d4-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="e49d4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e49d4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e49d4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e49d4-114">Not supported.</span></span>|
|<span data-ttu-id="e49d4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e49d4-115">Application</span></span>|<span data-ttu-id="e49d4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e49d4-116">Not supported.</span></span>|

<span data-ttu-id="e49d4-117">对于委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="e49d4-117">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="e49d4-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="e49d4-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="e49d4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e49d4-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /policies/authenticationMethodsPolicy/email
```

## <a name="request-headers"></a><span data-ttu-id="e49d4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e49d4-120">Request headers</span></span>

|<span data-ttu-id="e49d4-121">名称</span><span class="sxs-lookup"><span data-stu-id="e49d4-121">Name</span></span>|<span data-ttu-id="e49d4-122">说明</span><span class="sxs-lookup"><span data-stu-id="e49d4-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e49d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e49d4-123">Authorization</span></span>|<span data-ttu-id="e49d4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e49d4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e49d4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e49d4-126">Content-Type</span></span>|<span data-ttu-id="e49d4-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e49d4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e49d4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e49d4-129">Request body</span></span>

<span data-ttu-id="e49d4-130">在请求正文中，提供 [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e49d4-130">In the request body, supply a JSON representation of the [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object.</span></span> <span data-ttu-id="e49d4-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="e49d4-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e49d4-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e49d4-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="e49d4-133">有关可更新的属性的列表，请参阅 [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="e49d4-133">For the list of properties that can be updated, see [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="e49d4-134">**注意：**`@odata.type`值为的属性 `#microsoft.graph.emailAuthenticationMethodConfiguration` 必须包含在正文中。</span><span class="sxs-lookup"><span data-stu-id="e49d4-134">**Note:** The `@odata.type` property with a value of `#microsoft.graph.emailAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="e49d4-135">响应</span><span class="sxs-lookup"><span data-stu-id="e49d4-135">Response</span></span>

<span data-ttu-id="e49d4-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e49d4-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e49d4-138">示例</span><span class="sxs-lookup"><span data-stu-id="e49d4-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e49d4-139">请求</span><span class="sxs-lookup"><span data-stu-id="e49d4-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_emailauthenticationmethodconfiguration"
}
-->

```http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfiguration/email
Content-Type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "allowExternalIdToUseEmailOtp": "false",
}
```

### <a name="response"></a><span data-ttu-id="e49d4-140">响应</span><span class="sxs-lookup"><span data-stu-id="e49d4-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 NO CONTENT
```

