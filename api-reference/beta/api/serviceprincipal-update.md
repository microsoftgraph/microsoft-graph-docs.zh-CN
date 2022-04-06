---
title: 更新 serviceprincipal
description: 更新 serviceprincipal 对象的属性。
author: sureshja
ms.localizationpriority: high
doc_type: apiPageType
ms.prod: applications
ms.openlocfilehash: 344ef0ff4fcea8dd8032f4d7a53d6fc940369fc0
ms.sourcegitcommit: 0249c86925c9b4797908394c952073b5d9137911
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2022
ms.locfileid: "64477879"
---
# <a name="update-serviceprincipal"></a>更新 servicePrincipal

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [servicePrincipal](../resources/serviceprincipal.md) 对象的属性。

> [!IMPORTANT]
> 不支持使用 PATCH 设置 [**passwordCredential**](../resources/passwordcredential.md)。 使用 [addPassword](./serviceprincipal-addpassword.md) 和 [removePassword](./serviceprincipal-removepassword.md) 方法更新 servicePrincipal 的密码或密钥。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Application.ReadWrite.All、Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:-----------|:----------|
| Authorization | Bearer {token}。必需。  |
| Content-Type | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性     | 类型 |说明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| 如果服务主体帐户已启用，则为 **true**；否则，为 **false**。|
| addIns | [addIn](../resources/addin.md) | 定义使用服务可用于调用特定上下文中的应用的自定义行为。 例如，呈现文件流的应用程序可能会为其“FileHandler”功能[设置 addIns 属性](/onedrive/developer/file-handlers/)。 这将使 Microsoft 365 之类的服务在用户正在处理的文档上下文中调用应用程序。|
|alternativeNames|字符串集合| 用于按订阅、标识资源组和[托管标识](/azure/active-directory/managed-identities-azure-resources/overview)的完整资源 ID 检索服务主体。|
|appRoleAssignmentRequired|Boolean|指定在 Azure AD 在向应用程序签发用户或访问令牌之前用户或组是否需要 **appRoleAssignment**。不可为 null。 |
|appRoles|[appRole](../resources/approle.md) 集合|关联应用程序公开的应用程序角色。 有关详细信息，请参阅 [应用程序](../resources/application.md)资源上的 **appRoles** 属性定义。 不可为空。 |
|customSecurityAttributes|[customSecurityAttributeValue](../resources/customsecurityattributevalue.md)|保留分配给目录对象的自定义安全属性的值的开放式复杂类型。<br/><br/>若要更新此属性，必须为调用主体分配"属性分配管理员"角色，并且必须向其授予 *CustomSecAttributeAssignment.ReadWrite.All* 权限。|
|displayName|String|服务主体的显示名称。|
|homepage|String|应用程序的主页或登录页面。|
|keyCredentials|[keyCredential](../resources/keycredential.md) 集合|与服务主题关联的密钥凭据集合。不可为 null。            |
|loginUrl|String|指定服务提供商将用户重定向到 Azure AD 进行身份验证的 URL。 Azure AD 使用 URL 从 Microsoft 365 或Azure AD My Apps 启动应用程序。 该选项为空时，Azure AD 将对使用“[基于 SAML 的单一登录](/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso)”配置的应用程序执行 IdP 启动的登录。 用户从 Microsoft 365、Azure AD My Apps 或Azure AD SSO URL 启动应用程序。|
|logoutUrl|String| 指定 Microsoft 授权服务使用[正向通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[反向通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户时所使用的 URL。|
|notificationEmailAddresses|字符串集合|指定在活动证书临近到期日期时，Azure AD 在其中发送通知的电子邮件地址列表。 这仅适用于用于签署为 Azure AD 库应用程序发行的 SAML 令牌的证书。|
|publishedPermissionScopes|[permissionScope](../resources/permissionScope.md) 集合|关联应用程序的 OAuth 2.0 权限。 有关详细信息，请参阅 [应用程序](../resources/application.md)资源上的 **oauth2PermissionScopes** 属性定义。 不可为空。            |
|preferredSingleSignOnMode|string|指定为此应用程序配置的单一登录模式。 Azure AD 使用首选单一登录模式从 Microsoft 365 或Azure AD My Apps 启动应用程序。 支持的值有 password、saml、external 和 oidc。|
|preferredTokenSigningKeyEndDateTime|DateTimeOffset|指定用于令牌签名的 keyCredential 的到期日期，由 **preferredTokenSigningKeyThumbprint** 标记。|
|preferredTokenSigningKeyThumbprint|String|仅供内部使用。 请勿写入属性，否则将依赖该属性。 可能会在未来版本中删除。 |
|publisherName|String|在其中指定关联应用程序的租户的显示名称。|
|replyUrls|String 集合|向其发送用户令牌以使用关联应用程序登录的 URL，或者为关联应用程序向其发送 OAuth 2.0 authorization 代码和访问令牌的重定向 URL。不可为 NULL。 |
|samlSingleSignOnSettings|[samlSingleSignOnSettings](../resources/samlsinglesignonsettings.md)|有关 saml 单一登录的设置的集合。|
|servicePrincipalNames|字符串集合|包含从关联的 [应用程序](../resources/application.md)中复制的 **identifiersUris** 列表。 可以将其他值添加到混合应用程序。 这些值可用于标识此应用程序在 Azure AD 中公开的权限。 例如，<ul><li>请求对此资源的权限的客户端应用可以使用这些 URI 在其应用程序清单的 **requiredResourceAccess** 属性中或在应用注册体验的“API 权限”边栏选项卡中指定所需的权限。</li><li>客户端应用可以指定基于此属性的值的资源 URI（即“aud”声明中返回的 URI），以获取访问令牌。</li></ul><br>多值属性上的筛选器表达式需要 any 运算符。不可为 NULL。|
|tags|String collection| 不可为空。 |
|tokenEncryptionKeyId|String|指定 keyCredentials 集合中的公共密钥的 keyId。 配置后，Azure AD 为此应用程序发布使用此属性指定的密钥加密的令牌。 接收加密令牌的应用程序代码必须先使用匹配的私钥来解密该令牌，然后才能将该令牌用于登录用户。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `204 No Content` 响应代码和更新的 [servicePrincipal](../resources/serviceprincipal.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-update-properties-of-the-specified-service-principal"></a>示例 1：更新指定服务主体的属性

#### <a name="request"></a>请求
下面是一个请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->

```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json

{
  "appRoleAssignmentRequired": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-serviceprincipal-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-serviceprincipal-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


### <a name="example-2-assign-a-custom-security-attribute-with-a-string-value-to-a-service-principal"></a>示例 2：将具有字符串值的自定义安全属性分配给服务主体

下面的示例演示如何将具有字符串值的自定义安全属性分配给服务主体。

+ 属性集： `Engineering`
+ 属性：`ProjectDate`
+ 属性数据类型：字符串
+ 属性值： `"2022-10-01"`

若要分配自定义安全属性，必须为调用主体分配"属性分配管理员"角色，并且必须授予 *CustomSecAttributeAssignment.ReadWrite.All* 权限。

有关用户的其他类似示例，请参阅[使用 Microsoft Graph API 分配、更新或删除自定义安全属性](/graph/custom-security-attributes-examples)。

#### <a name="request"></a>请求



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "assign_serviceprincipal_customsecurityattribute_string"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":"2022-10-01"
        }
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/assign-serviceprincipal-customsecurityattribute-string-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/assign-serviceprincipal-customsecurityattribute-string-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/assign-serviceprincipal-customsecurityattribute-string-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/assign-serviceprincipal-customsecurityattribute-string-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
