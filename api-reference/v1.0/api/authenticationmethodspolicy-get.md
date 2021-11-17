---
title: 获取 authenticationMethodsPolicy
description: 读取 authenticationMethodsPolicy 对象的属性和关系。
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c53a49da33debac12798775d8f62858b06907de3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988649"
---
# <a name="get-authenticationmethodspolicy"></a>获取 authenticationMethodsPolicy
命名空间：microsoft.graph

读取 [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) 对象的属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.ReadWrite.AuthenticationMethod|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|Policy.ReadWrite.AuthenticationMethod|

对于委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：

* 全局读取者
* 身份验证策略管理员
* 全局管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法不支持任何可选的查询参数。

## <a name="request-headers"></a>请求头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethodspolicy"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-authenticationmethodspolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethodsPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#authenticationMethodsPolicy",
    "id": "authenticationMethodsPolicy",
    "displayName": "Authentication Methods Policy",
    "description": "The tenant-wide policy that controls which authentication methods are allowed in the tenant, authentication method registration requirements, and self-service password reset settings",
    "lastModifiedDateTime": "2021-07-02T13:34:13.1991781Z",
    "policyVersion": "1.4",
    "registrationEnforcement": {
        "authenticationMethodsRegistrationCampaign": {
            "snoozeDurationInDays": 2,
            "state": "enabled",
            "excludeTargets": [],
            "includeTargets": [
                {
                    "id": "3ee3a9de-0a86-4e12-a287-9769accf1ba2",
                    "targetType": "group",
                    "targetedAuthenticationMethod": "microsoftAuthenticator"
                }
            ]
        }
    },
    "authenticationMethodConfigurations@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/authenticationMethodsPolicy/authenticationMethodConfigurations",
    "authenticationMethodConfigurations": [
        {
            "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
            "id": "Fido2",
            "state": "enabled",
            "isSelfServiceRegistrationAllowed": true,
            "isAttestationEnforced": true,
            "keyRestrictions": {
                "isEnforced": false,
                "enforcementType": "block",
                "aaGuids": []
            },
            "includeTargets@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/authenticationMethodsPolicy/authenticationMethodConfigurations('Fido2')/microsoft.graph.fido2AuthenticationMethodConfiguration/includeTargets",
            "includeTargets": [
                {
                    "targetType": "group",
                    "id": "all_users",
                    "isRegistrationRequired": false
                }
            ]
        },
        {
            "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
            "id": "MicrosoftAuthenticator",
            "state": "disabled",
            "includeTargets@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/authenticationMethodsPolicy/authenticationMethodConfigurations('MicrosoftAuthenticator')/microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration/includeTargets",
            "includeTargets": [
                {
                    "targetType": "group",
                    "id": "all_users",
                    "isRegistrationRequired": false,
                    "authenticationMode": "any",
                    "featureSettings": null
                }
            ]
        },
        {
            "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
            "id": "Email",
            "state": "enabled",
            "allowExternalIdToUseEmailOtp": "default",
            "includeTargets@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/authenticationMethodsPolicy/authenticationMethodConfigurations('Email')/microsoft.graph.emailAuthenticationMethodConfiguration/includeTargets",
            "includeTargets": []
        }
    ]
}
```
