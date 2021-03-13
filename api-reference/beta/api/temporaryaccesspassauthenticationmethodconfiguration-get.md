---
title: 获取 temporaryAccessPassAuthenticationMethodConfiguration
description: 读取 temporaryAccessPassAuthenticationMethodConfiguration 对象的属性和关系。
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 08a20da2f4c14a3d3a6d3581765eb5e168e8b721
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759508"
---
# <a name="get-temporaryaccesspassauthenticationmethodconfiguration"></a>获取 temporaryAccessPassAuthenticationMethodConfiguration
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取[临时AccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)对象的属性和关系，该对象表示 Azure Active Directory (Azure AD) 租户的临时访问传递身份验证方法策略。 [](../resources/authenticationmethodspolicies-overview.md)

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.ReadWrite.AuthenticationMethod|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|Policy.ReadWrite.AuthenticationMethod|

 对于委派方案，管理员需要全局管理员角色。 有关详细信息，请参阅[角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```
## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

### <a name="response"></a>响应
下面展示了示例响应。

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
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