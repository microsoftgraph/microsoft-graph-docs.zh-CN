---
title: 更新 x509CertificateAuthenticationMethodConfiguration
description: 更新 x509CertificateAuthenticationMethodConfiguration 对象的属性。
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 798a994648de5f94d92a7f7b831fdb94135d8516
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437226"
---
# <a name="update-x509certificateauthenticationmethodconfiguration"></a>更新 x509CertificateAuthenticationMethodConfiguration
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [X.509 证书身份验证方法](../resources/x509certificateauthenticationmethodconfiguration.md)的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.ReadWrite.AuthenticationMethod|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|不支持。|

对于委派方案，管理员需要以下 [Azure AD 角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：

* 身份验证策略管理员
* 全局管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/x509Certificate
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]
可更新以下属性。

|属性|类型|说明|
|:---|:---|:---|
|state|authenticationMethodState|可能的值为： `enabled`. `disabled` 继承自 [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)。|
|certificateUserBindings|[x509CertificateUserBinding](../resources/x509certificateuserbinding.md) 集合|定义 X.509 证书中的字段，这些字段映射到 Azure AD 用户对象的属性，以便将证书绑定到用户。 对象的 **优先级** 确定执行绑定的顺序。将使用匹配的第一个绑定，其余绑定将被忽略。 |
|authenticationModeConfiguration|[x509CertificateAuthenticationModeConfiguration](../resources/x509certificateauthenticationmodeconfiguration.md)|定义强身份验证配置。 此配置包括默认身份验证模式和强身份验证绑定的不同规则。 |

>**注意：**`@odata.type`具有值的`#microsoft.graph.x509CertificateAuthenticationMethodConfiguration`属性必须包含在正文中。


## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `204 No Content` 响应代码和更新后的 [x509CertificateAuthenticationMethodConfiguration](../resources/x509certificateauthenticationmethodconfiguration.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面是具有以下设置的更新请求的示例：

+ 在租户中启用 x509 证书身份验证方法。
+ 在证书 **PrincipalName** 和 Azure AD **onPremisesUserPrincipalName** 属性之间仅配置一个用户绑定。
+ 将多重身份验证定义为要求。
+ 针对规则类型配置强身份验证方法的绑定规则。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_x509certificateauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/x509Certificate
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.x509CertificateAuthenticationMethodConfiguration",
    "id": "X509Certificate",
    "state": "enabled",
    "certificateUserBindings": [
        {
            "x509CertificateField": "PrincipalName",
            "userProperty": "onPremisesUserPrincipalName",
            "priority": 1
        }
    ],
    "authenticationModeConfiguration": {
        "x509CertificateAuthenticationDefaultMode": "x509CertificateMultiFactor",
        "rules": [
            {
                "x509CertificateRuleType": "issuerSubject",
                "identifier": "CN=ContosoCA,DC=Contoso,DC=org ",
                "x509CertificateAuthenticationMode": "x509CertificateMultiFactor"
            },
            {
                "x509CertificateRuleType": "policyOID",
                "identifier": "1.2.3.4",
                "x509CertificateAuthenticationMode": "x509CertificateMultiFactor"
            }
        ]
    },
    "includeTargets": [
        {
            "targetType": "group",
            "id": "all_users",
            "isRegistrationRequired": false
        }
    ]
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-x509certificateauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-x509certificateauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-x509certificateauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-x509certificateauthenticationmethodconfiguration-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-x509certificateauthenticationmethodconfiguration-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- {
  "blockType": "response"
}
-->
``` http
HTTP/1.1 204 No Content
```

