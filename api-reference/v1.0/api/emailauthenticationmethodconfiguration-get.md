---
title: 获取 emailAuthenticationMethodConfiguration
description: 读取 emailAuthenticationMethodConfiguration 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 54bc1d89730590a01bf7787d20313279067eb27a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231995"
---
# <a name="get-emailauthenticationmethodconfiguration"></a><span data-ttu-id="d6821-103">获取 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="d6821-103">Get emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="d6821-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6821-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d6821-105">读取[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)对象的属性和关系，该对象表示 Azure Active Directory (Azure AD 租户的电子邮件[OTP](../resources/authenticationmethodspolicies-overview.md)) 策略。</span><span class="sxs-lookup"><span data-stu-id="d6821-105">Read the properties and relationships of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6821-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6821-106">Permissions</span></span>

<span data-ttu-id="d6821-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6821-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6821-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6821-109">Permission type</span></span>|<span data-ttu-id="d6821-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6821-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6821-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6821-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6821-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d6821-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="d6821-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6821-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6821-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6821-114">Not supported.</span></span>|
|<span data-ttu-id="d6821-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6821-115">Application</span></span>|<span data-ttu-id="d6821-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d6821-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="d6821-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="d6821-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="d6821-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="d6821-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="d6821-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6821-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfiguration/email
```

## <a name="request-headers"></a><span data-ttu-id="d6821-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6821-120">Request headers</span></span>

|<span data-ttu-id="d6821-121">名称</span><span class="sxs-lookup"><span data-stu-id="d6821-121">Name</span></span>|<span data-ttu-id="d6821-122">说明</span><span class="sxs-lookup"><span data-stu-id="d6821-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d6821-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6821-123">Authorization</span></span>|<span data-ttu-id="d6821-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6821-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6821-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6821-126">Request body</span></span>

<span data-ttu-id="d6821-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d6821-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6821-128">响应</span><span class="sxs-lookup"><span data-stu-id="d6821-128">Response</span></span>

<span data-ttu-id="d6821-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6821-129">If successful, this method returns a `200 OK` response code and an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6821-130">示例</span><span class="sxs-lookup"><span data-stu-id="d6821-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6821-131">请求</span><span class="sxs-lookup"><span data-stu-id="d6821-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethodconfiguration"
}
-->

```http
GET /policies/authenticationMethodsPolicy/email
```

### <a name="response"></a><span data-ttu-id="d6821-132">响应</span><span class="sxs-lookup"><span data-stu-id="d6821-132">Response</span></span>

<span data-ttu-id="d6821-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d6821-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethodConfiguration"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 491

{
  "value": {
    "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
    "id": "Email",
    "state": "enabled",
    "allowExternalIdToUseEmailOtp": "enabled"
  }
}
```
