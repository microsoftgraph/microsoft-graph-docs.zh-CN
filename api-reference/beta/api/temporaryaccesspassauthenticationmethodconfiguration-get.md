---
title: 获取 temporaryAccessPassAuthenticationMethodConfiguration
description: 读取 temporaryAccessPassAuthenticationMethodConfiguration 对象的属性和关系。
author: inbarckms
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b0874968f9cce1b60a3b0f85a68ac4ccbf9a887e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049644"
---
# <a name="get-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="9f7c0-103">获取 temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="9f7c0-103">Get temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="9f7c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f7c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f7c0-105">读取[临时AccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)对象的属性和关系，该对象表示 Azure Active Directory (Azure AD 租户的临时访问) 策略。 [](../resources/authenticationmethodspolicies-overview.md)</span><span class="sxs-lookup"><span data-stu-id="9f7c0-105">Read the properties and relationships of a [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object, which represents the Temporary Access Pass [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f7c0-106">权限</span><span class="sxs-lookup"><span data-stu-id="9f7c0-106">Permissions</span></span>
<span data-ttu-id="9f7c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f7c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f7c0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f7c0-109">Permission type</span></span>|<span data-ttu-id="9f7c0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f7c0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f7c0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f7c0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f7c0-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9f7c0-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="9f7c0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f7c0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f7c0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f7c0-114">Not supported.</span></span>|
|<span data-ttu-id="9f7c0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f7c0-115">Application</span></span>|<span data-ttu-id="9f7c0-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9f7c0-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="9f7c0-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="9f7c0-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="9f7c0-118">有关详细信息，请参阅[角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="9f7c0-118">For more information, see[roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="9f7c0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f7c0-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```
## <a name="request-headers"></a><span data-ttu-id="9f7c0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f7c0-120">Request headers</span></span>
|<span data-ttu-id="9f7c0-121">名称</span><span class="sxs-lookup"><span data-stu-id="9f7c0-121">Name</span></span>|<span data-ttu-id="9f7c0-122">说明</span><span class="sxs-lookup"><span data-stu-id="9f7c0-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9f7c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f7c0-123">Authorization</span></span>|<span data-ttu-id="9f7c0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9f7c0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f7c0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f7c0-126">Request body</span></span>
<span data-ttu-id="9f7c0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9f7c0-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="9f7c0-128">响应</span><span class="sxs-lookup"><span data-stu-id="9f7c0-128">Response</span></span>
<span data-ttu-id="9f7c0-129">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9f7c0-129">The following is an example of the response.</span></span>

<span data-ttu-id="9f7c0-130">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9f7c0-130">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fido2AuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#authenticationMethodConfigurations/$entity",
    "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
    "id": "TemporaryAccessPass",
    "state": "enabled",
    "defaultLifetimeInMinutes": 60,
    "defaultLength": 12,
    "minimumLifetimeInMinutes": 60,
    "maximumLifetimeInMinutes": 1440,
    "isUsableOnce": false,
    "includeTargets@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authenticationMethodsPolicy/authenticationMethodConfigurations('TemporaryAccessPass')/microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration/includeTargets",
    "includeTargets": [
        {
            "targetType": "group",
            "id": "all_users",
            "isRegistrationRequired": false
        }
    ]
}
```