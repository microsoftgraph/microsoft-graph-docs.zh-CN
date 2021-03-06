---
title: 获取 emailAuthenticationMethodConfiguration
description: 读取 emailAuthenticationMethodConfiguration 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 006fd4ae3bb69157e18235a6dd31d1d090533205
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515875"
---
# <a name="get-emailauthenticationmethodconfiguration"></a><span data-ttu-id="c9c05-103">获取 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="c9c05-103">Get emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="c9c05-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9c05-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9c05-105">读取 [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) 对象的属性和关系，该对象代表 Azure Active Directory (Azure AD) 的电子邮件 [OTP](../resources/authenticationmethodspolicies-overview.md) 身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="c9c05-105">Read the properties and relationships of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9c05-106">权限</span><span class="sxs-lookup"><span data-stu-id="c9c05-106">Permissions</span></span>

<span data-ttu-id="c9c05-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9c05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9c05-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9c05-109">Permission type</span></span>|<span data-ttu-id="c9c05-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c9c05-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9c05-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9c05-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c9c05-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c9c05-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="c9c05-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9c05-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9c05-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9c05-114">Not supported.</span></span>|
|<span data-ttu-id="c9c05-115">Application</span><span class="sxs-lookup"><span data-stu-id="c9c05-115">Application</span></span>|<span data-ttu-id="c9c05-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9c05-116">Not supported.</span></span>|

<span data-ttu-id="c9c05-117">对于委派方案，管理员需要以下角色之 [一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="c9c05-117">For delegated scenarios the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="c9c05-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="c9c05-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="c9c05-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9c05-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="c9c05-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9c05-120">Request headers</span></span>

|<span data-ttu-id="c9c05-121">名称</span><span class="sxs-lookup"><span data-stu-id="c9c05-121">Name</span></span>|<span data-ttu-id="c9c05-122">说明</span><span class="sxs-lookup"><span data-stu-id="c9c05-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c9c05-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9c05-123">Authorization</span></span>|<span data-ttu-id="c9c05-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c9c05-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9c05-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9c05-126">Request body</span></span>

<span data-ttu-id="c9c05-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c9c05-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9c05-128">响应</span><span class="sxs-lookup"><span data-stu-id="c9c05-128">Response</span></span>

<span data-ttu-id="c9c05-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c9c05-129">If successful, this method returns a `200 OK` response code and an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9c05-130">示例</span><span class="sxs-lookup"><span data-stu-id="c9c05-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c9c05-131">请求</span><span class="sxs-lookup"><span data-stu-id="c9c05-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethodconfiguration"
}
-->

```http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

### <a name="response"></a><span data-ttu-id="c9c05-132">响应</span><span class="sxs-lookup"><span data-stu-id="c9c05-132">Response</span></span>

<span data-ttu-id="c9c05-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c9c05-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "allowExternalIdToUseEmailOtp": "True",
    "includeTargets":[
        {
          "targetType":"group",
          "id":"all_users",
          "isRegistrationRequired":false,
        }
    ]
  }
}
```

