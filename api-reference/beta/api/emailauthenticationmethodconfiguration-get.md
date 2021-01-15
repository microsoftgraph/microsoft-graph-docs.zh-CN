---
title: 获取 emailAuthenticationMethodConfiguration
description: 读取 emailAuthenticationMethodConfiguration 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 82f1653e5fdf091bd92638b4596bacd4b8194817
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873323"
---
# <a name="get-emailauthenticationmethodconfiguration"></a><span data-ttu-id="6e479-103">获取 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e479-103">Get emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="6e479-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e479-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e479-105">读取 [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) 对象的属性和关系，该对象代表 Azure Active Directory (Azure AD) 的电子邮件 [OTP](../resources/authenticationmethodspolicies-overview.md) 身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="6e479-105">Read the properties and relationships of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e479-106">权限</span><span class="sxs-lookup"><span data-stu-id="6e479-106">Permissions</span></span>

<span data-ttu-id="6e479-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e479-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e479-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e479-109">Permission type</span></span>|<span data-ttu-id="6e479-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e479-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e479-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e479-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6e479-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6e479-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="6e479-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e479-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e479-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e479-114">Not supported.</span></span>|
|<span data-ttu-id="6e479-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e479-115">Application</span></span>|<span data-ttu-id="6e479-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e479-116">Not supported.</span></span>|

<span data-ttu-id="6e479-117">对于委派方案，管理员需要以下角色之 [一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="6e479-117">For delegated scenarios the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="6e479-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="6e479-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="6e479-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e479-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfiguration/email
```

## <a name="request-headers"></a><span data-ttu-id="6e479-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e479-120">Request headers</span></span>

|<span data-ttu-id="6e479-121">名称</span><span class="sxs-lookup"><span data-stu-id="6e479-121">Name</span></span>|<span data-ttu-id="6e479-122">说明</span><span class="sxs-lookup"><span data-stu-id="6e479-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6e479-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e479-123">Authorization</span></span>|<span data-ttu-id="6e479-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e479-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e479-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e479-126">Request body</span></span>

<span data-ttu-id="6e479-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e479-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e479-128">响应</span><span class="sxs-lookup"><span data-stu-id="6e479-128">Response</span></span>

<span data-ttu-id="6e479-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6e479-129">If successful, this method returns a `200 OK` response code and an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e479-130">示例</span><span class="sxs-lookup"><span data-stu-id="6e479-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e479-131">请求</span><span class="sxs-lookup"><span data-stu-id="6e479-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethodconfiguration"
}
-->

```http
GET /policies/authenticationMethodsPolicy/email
```

### <a name="response"></a><span data-ttu-id="6e479-132">响应</span><span class="sxs-lookup"><span data-stu-id="6e479-132">Response</span></span>

<span data-ttu-id="6e479-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6e479-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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

