---
title: 更新 serviceprincipal
description: 更新 serviceprincipal 对象的属性。
author: sureshja
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4a80b28cb42a3c23902fed139f7ccc7ec92ea794
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896131"
---
# <a name="update-serviceprincipal"></a>更新 servicePrincipal

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新[servicePrincipal](../resources/serviceprincipal.md)对象的属性。

> [!IMPORTANT]
> 不支持使用修补程序设置[**passwordCredential**](../resources/passwordcredential.md) 。 使用[addPassword](./serviceprincipal-addpassword.md)和[RemovePassword](./serviceprincipal-removepassword.md)方法更新 servicePrincipal 的密码。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 所有的 Directory.accessasuser.all，all，all，All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.readwrite.ownedby、所有的 readwrite、全部、读写。 |

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
|accountEnabled|布尔| 如果服务主体帐户已启用，则为 **true**；否则，为 **false**。|
| addIns | [addIn](../resources/addin.md) | 定义使用服务可用于调用特定上下文中的应用的自定义行为。 例如，呈现文件流的应用程序可能会为其“FileHandler”功能[设置 addIns 属性](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online)。 这将使 Microsoft 365 等服务能够在用户正在使用的文档的上下文中调用应用程序。|
|alternativeNames|String collection| 用于按订阅检索服务主体，标识[托管标识](https://aka.ms/azuremanagedidentity)的资源组和完整资源 id。|
|appRoleAssignmentRequired|Boolean|指定在 Azure AD 在向应用程序签发用户或访问令牌之前用户或组是否需要 **appRoleAssignment**。 不可为 null。 |
|appRoles|[appRole](../resources/approle.md) 集合|关联应用程序公开的应用程序角色。 有关详细信息，请参阅[应用程序](../resources/application.md)资源上的**appRoles**属性定义。 不可为空。 |
|displayName|String|服务主体的显示名称。|
|homepage|String|应用程序的主页或登录页。|
|keyCredentials|[keyCredential](../resources/keycredential.md) 集合|与服务帐户关联的密钥凭据集合。 不可为 null。            |
|loginUrl|String|指定服务提供程序将用户重定向到 Azure AD 以进行身份验证的 URL。 Azure AD 使用 URL 从 Microsoft 365 或 Azure AD My 应用启动应用程序。 当为空时，Azure AD 将针对使用[基于 SAML 的单一登录](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso)配置的应用程序执行 IdP 启动的登录。 用户从 Microsoft 365、Azure AD My 应用或 Azure AD SSO URL 启动应用程序。|
|logoutUrl|String| 指定 Microsoft 授权服务使用[正向通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[反向通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户时所使用的 URL。|
|notificationEmailAddresses|String collection|指定当活动证书接近到期日期时，Azure AD 发送通知的电子邮件地址的列表。 这仅适用于用于对 Azure AD 库应用程序颁发的 SAML 令牌进行签名的证书。|
|publishedPermissionScopes|[permissionScope](../resources/permissionScope.md)集合|关联应用程序的 OAuth 2.0 权限。 有关详细信息，请参阅[应用程序](../resources/application.md)资源上的**oauth2PermissionScopes**属性定义。 不可为 null。            |
|preferredSingleSignOnMode|string|指定为此应用程序配置的单一登录模式。 Azure AD 使用首选的单一登录模式，从 Microsoft 365 或 Azure AD My 应用启动应用程序。 受支持的值为 password、saml、external 和 oidc。|
|preferredTokenSigningKeyEndDateTime|DateTimeOffset|指定用于令牌签名的 keyCredential 的到期日期，由**preferredTokenSigningKeyThumbprint**标记。|
|preferredTokenSigningKeyThumbprint|String|仅供内部使用。 请勿写入属性，否则将依赖该属性。 可能会在未来版本中删除。 |
|publisherName|String|在其中指定关联应用程序的租户的显示名称。|
|replyUrls|String 集合|向其发送用户令牌以使用关联应用程序登录的 URL，或者为关联应用程序向其发送 OAuth 2.0 authorization 代码和访问令牌的重定向 URL。 不可为空。 |
|samlSingleSignOnSettings|[samlSingleSignOnSettings](../resources/samlsinglesignonsettings.md)|与 saml 单一登录相关的设置的集合。|
|servicePrincipalNames|String 集合|包含从关联的[应用程序](../resources/application.md)复制的**identifiersUris**的列表。 可以向混合应用程序中添加其他值。 这些值可用于标识此应用在 Azure AD 中公开的权限。 For example,<ul><li>请求对此资源的权限的客户端应用程序可以使用这些 Uri 在其应用程序清单的**requiredResourceAccess**属性中，或在应用程序注册体验中的 "API 权限" 中指定所需的权限。</li><li>客户端应用可以指定基于此属性的值获取访问令牌的资源 URI，这是在 "aud" 声明中返回的 URI。</li></ul><br>需要多值属性筛选器表达式的 any 运算符。 不可为 null。|
|标记|String collection| 不可为空。 |
|tokenEncryptionKeyId|String|指定 keyCredentials 集合中的公共密钥的 keyId。 配置后，Azure AD 将使用此属性指定的密钥为此应用程序颁发令牌。 接收加密令牌的应用程序代码必须先使用匹配的私钥来解密该令牌，然后才能将该令牌用于登录用户。|

## <a name="response"></a>响应

如果成功，此方法 `204 No Content` 在响应正文中返回响应代码和更新的[servicePrincipal](../resources/serviceprincipal.md)对象。
## <a name="examples"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->

```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

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

---


### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
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
