---
title: 获取 temporaryAccessPassAuthenticationMethodConfiguration
description: 读取 temporaryAccessPassAuthenticationMethodConfiguration 对象的属性和关系。
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 52ea16ad502a24ac0eb75de94c2cad4c9fbe93d5
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272610"
---
# <a name="get-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="4323c-103">获取 temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="4323c-103">Get temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="4323c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4323c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4323c-105">读取[临时AccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)对象的属性和关系，该对象代表 Azure Active Directory (Azure AD) 租户的临时访问传递身份验证方法策略。 [](../resources/authenticationmethodspolicies-overview.md)</span><span class="sxs-lookup"><span data-stu-id="4323c-105">Read the properties and relationships of a [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object, which represents the Temporary Access Pass [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4323c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4323c-106">Permissions</span></span>
<span data-ttu-id="4323c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4323c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4323c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4323c-109">Permission type</span></span>|<span data-ttu-id="4323c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4323c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4323c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4323c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4323c-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4323c-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="4323c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4323c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4323c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4323c-114">Not supported.</span></span>|
|<span data-ttu-id="4323c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4323c-115">Application</span></span>|<span data-ttu-id="4323c-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4323c-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="4323c-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="4323c-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="4323c-118">有关详细信息，请参阅[角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="4323c-118">For more information, see[roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="4323c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4323c-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```
## <a name="request-headers"></a><span data-ttu-id="4323c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4323c-120">Request headers</span></span>
|<span data-ttu-id="4323c-121">名称</span><span class="sxs-lookup"><span data-stu-id="4323c-121">Name</span></span>|<span data-ttu-id="4323c-122">说明</span><span class="sxs-lookup"><span data-stu-id="4323c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4323c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4323c-123">Authorization</span></span>|<span data-ttu-id="4323c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4323c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4323c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4323c-126">Request body</span></span>
<span data-ttu-id="4323c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4323c-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="4323c-128">响应</span><span class="sxs-lookup"><span data-stu-id="4323c-128">Response</span></span>
<span data-ttu-id="4323c-129">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4323c-129">The following is an example of the response.</span></span>

<span data-ttu-id="4323c-130">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4323c-130">**Note:** The response object shown here might be shortened for readability.</span></span>
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