---
title: servicePrincipal 资源类型
description: 表示目录中的一个应用程序实例。 继承自 directoryObject。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 94a651a613d64ee5cefeed6a7e8f3f0b4656a916
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332318"
---
# <a name="serviceprincipal-resource-type"></a>servicePrincipal 资源类型

命名空间：microsoft.graph

表示目录中的一个应用程序实例。 继承自 [directoryObject](directoryobject.md)。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[列出 servicePrincipals](../api/serviceprincipal-list.md) | [servicePrincipal](serviceprincipal.md) 集合 | 检索 servicePrincipal 对象列表。 |
|[创建 servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md)| [servicePrincipal](serviceprincipal.md) | 创建一个新的 servicePrincipal 对象。 |
|[Get servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |读取 servicePrincipal 对象的属性和关系。|
|[更新 servicePrincipal](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |更新 servicePrincipal 对象。 |
|[删除 servicePrincipal](../api/serviceprincipal-delete.md) | 无 |删除 servicePrincipal 对象。|
|[列出 createdObjects](../api/serviceprincipal-list-createdobjects.md) |[directoryObject](directoryobject.md) collection| 获取 createdObject 对象集合。|
|[列出 ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |[directoryObject](directoryobject.md) 集合| 获取 ownedObject 对象集合。|
|**应用程序角色分配**| | |
|[列出 appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |[appRoleAssignment](approleassignment.md) 集合| 获取已分配此服务主体的应用程序角色。|
|[添加 appRoleAssignment](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| 将应用程序角色分配给此服务主体。|
|[删除 appRoleAssignment](../api/serviceprincipal-delete-approleassignments.md) | 无 | 从此服务主体中删除应用程序角色分配。|
|[列出 appRoleAssignedTo](../api/serviceprincipal-list-approleassignedto.md) |[appRoleAssignment](approleassignment.md) 集合| 获取为此服务主体分配的应用程序角色的用户、组和服务主体。|
|[添加 appRoleAssignedTo](../api/serviceprincipal-post-approleassignedto.md) |[appRoleAssignment](approleassignment.md)| 将此服务主体的应用程序角色分配给用户、组或服务主体。|
|[删除 appRoleAssignedTo](../api/serviceprincipal-delete-approleassignedto.md) | 无 | 从用户、组或服务主体中删除此服务主体的应用程序角色分配。|
|**证书和密码**| | |
|[添加密码](../api/serviceprincipal-addpassword.md)|[passwordCredential](passwordcredential.md)|将强密码添加到 servicePrincipal。|
|[删除密码](../api/serviceprincipal-removepassword.md)|[passwordCredential](passwordcredential.md)|从 servicePrincipal 中删除密码。|
|[添加密钥](../api/serviceprincipal-addkey.md)|[keyCredential](keycredential.md)|将密钥凭据添加到 servicePrincipal。|
|[Remove 键](../api/serviceprincipal-removekey.md)|无|从 servicePrincipal 中删除密钥凭据。|
|**委派权限授予**| | |
|[List oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合| 获取授权此服务主体的委派权限，以代表登录用户访问 API。|
|**成员身份**| | |
|[List memberOf](../api/serviceprincipal-list-memberof.md) |[directoryObject](directoryobject.md) 集合| 从 memberOf 导航属性中获取此服务主体是其直接成员的组。|
|[列出 transitive memberOf](../api/serviceprincipal-list-transitivememberof.md) |[directoryObject](directoryobject.md) collection| 列出此服务主体所属的组。 此操作是可传递的，并包括此服务主体以嵌套方式所属的组。 |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|String 集合|检查指定组列表中的成员身份。|
|[checkMemberObjects](../api/serviceprincipal-checkmemberobjects.md)|String 集合|检查组、目录角色或管理单元对象指定列表中的成员身份。|
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|String 集合|获取此服务主体所属的组列表。|
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|String 集合|获取此服务主体所属的组和目录角色列表。|
|**Owners**| | |
|[List owners](../api/serviceprincipal-list-owners.md) |[directoryObject](directoryobject.md) 集合| 获取所有者对象集合。|
|[Add owner](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| 通过发布到所有者集合创建新的所有者。|
|[Remove owner](../api/serviceprincipal-delete-owners.md) |无| 从 serviceprincipal 中删除所有者。|

## <a name="properties"></a>属性
| 属性     | 类型 |说明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| 如果服务主体帐户已启用，则为 **true**；否则，为 **false**。|
| addIns | [addIn](addin.md)集合 | 定义使用服务可用于调用特定上下文中的应用的自定义行为。 例如，呈现文件流的应用程序可能会为其“FileHandler”功能[设置 addIns 属性](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online)。 这将使 Office 365 之类的服务在用户正在处理的文档上下文中调用应用程序。|
|alternativeNames|String collection| 用于按订阅检索服务主体，标识[托管标识](https://aka.ms/azuremanagedidentity)的资源组和完整资源 id。|
|appDisplayName|String|关联应用程序公开的显示名称。|
|appId|String|关联应用程序的唯一标识符（其 **appId** 属性）。|
|applicationTemplateId|String|创建 servicePrincipal 的 applicationTemplate 的唯一标识符。 只读。|
|appOwnerOrganizationId|String|包含注册应用程序的租户 id。 这仅适用于由应用程序支持的服务主体。|
|appRoleAssignmentRequired|Boolean|指定在用户可以登录或应用可以获取令牌之前，是否需要为此服务主体授予用户或其他服务主体的应用程序角色分配。 默认值为 **false**。 不可为 null。 |
|appRoles|[appRole](approle.md) 集合|由该服务主体代表的应用程序公开的角色。 有关详细信息，请参阅[应用程序](application.md)实体上的 **appRoles** 属性定义。 不可为 null。 |
| deletedDateTime | DateTimeOffset | 删除服务主体的日期和时间。 只读。 |
|displayName|字符串|服务主体的显示名称。|
|homepage|String|应用程序的主页或登录页。|
|id|String|服务主体的唯一标识符。 继承自 [directoryObject](directoryobject.md)。 键。 不可为 null。 只读。|
| info | [informationalUrl](informationalurl.md) | 获取的应用程序的基本配置文件信息，如应用程序的营销、支持、服务条款和隐私声明 Url。 服务条款和隐私声明通过用户同意体验展示给用户。 有关详细信息，请参阅[如何：为已注册的 Azure AD 应用添加服务条款和隐私声明](https://docs.microsoft.com/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement)。 |
|keyCredentials|[keyCredential](keycredential.md) 集合|与服务帐户关联的密钥凭据集合。 不可为 null。            |
|loginUrl|String|指定服务提供程序将用户重定向到 Azure AD 以进行身份验证的 URL。 Azure AD 使用 URL 从 Office 365 或 Azure AD My 应用程序启动应用程序。 当为空时，Azure AD 将针对使用[基于 SAML 的单一登录](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso)配置的应用程序执行 IdP 启动的登录。 用户从 Office 365、Azure AD My Apps 或 Azure AD SSO URL 启动应用程序。|
|logoutUrl|String| 指定将由 Microsoft 的授权服务用来使用 OpenId Connect[前通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[后信道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户的 URL。|
|oauth2PermissionScopes|[permissionScope](permissionScope.md)集合|由应用程序公开的委派权限。 有关详细信息，请参阅[application](application.md) entity **api**属性上的**oauth2PermissionScopes**属性。 不可为 null。|
|notificationEmailAddresses|String collection|指定当活动证书接近到期日期时，Azure AD 发送通知的电子邮件地址的列表。 这仅适用于用于对 Azure AD 库应用程序颁发的 SAML 令牌进行签名的证书。|
|passwordCredentials|[passwordCredential](passwordcredential.md) 集合|与服务帐户关联的密码凭据集合。 不可为 null。 |
|preferredSingleSignOnMode|string|指定为此应用程序配置的单一登录模式。 Azure AD 使用首选的单一登录模式，从 Office 365 或 Azure AD My Apps 启动应用程序。 受支持的值为 password、saml、external 和 oidc。|
|replyUrls|String 集合|向其发送用户令牌以使用关联应用程序登录的 URL，或者为关联应用程序向其发送 OAuth 2.0 authorization 代码和访问令牌的重定向 URL。 不可为空。 |
|samlSingleSignOnSettings|[samlSingleSignOnSettings](samlsinglesignonsettings.md)|与 saml 单一登录相关的设置的集合。|
|servicePrincipalNames|String 集合|包含从关联的[应用程序](application.md)复制的**identifiersUris**的列表。 可以向混合应用程序中添加其他值。 这些值可用于标识此应用在 Azure AD 中公开的权限。 For example,<ul><li>客户端应用可以指定基于此属性的值获取访问令牌的资源 URI，这是在 "aud" 声明中返回的 URI。</li></ul><br>需要多值属性筛选器表达式的 any 运算符。 不可为 null。|
|servicePrincipalType|String|标识服务主体表示的是应用程序还是托管标识。 这由 Azure AD 在内部进行设置。 对于表示[应用程序](./application.md)的服务主体，将其设置为__应用程序__。 对于表示[托管标识](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)的服务主体，将其设置为__ManagedIdentity__。|
|tags|String collection| 可用于对服务主体进行分类和标识的自定义字符串。 不可为空。 |
| tokenEncryptionKeyId |String|指定 keyCredentials 集合中的公共密钥的 keyId。 配置后，Azure AD 将使用此属性指定的密钥为此应用程序颁发令牌。 接收加密令牌的应用程序代码必须先使用匹配的私钥来解密该令牌，然后才能将该令牌用于登录用户。|

## <a name="relationships"></a>关系
| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|为此服务主体分配的主体（用户、组和服务主体）。 只读。|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) 集合|将此服务主体分配到的应用程序。 此为只读属性。 可为 NULL。|
|createdObjects|[directoryObject](directoryobject.md) 集合|此服务主体所创建的目录对象。 此为只读属性。 可为 NULL。|
|endpoints|[endpoint](endpoint.md) 集合|可用于发现的终结点。 Sharepoint 等服务使用特定于租户的 SharePoint 终结点填充此属性，其他应用程序可以在他们的体验中发现和使用这些终结点。|
|memberOf|[directoryObject](directoryobject.md) collection|此服务主体所属的角色。 HTTP 方法：GET 只读。 可为 NULL。|
|oauth2PermissionGrants|[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合|授权此服务主体的委派权限授予代表登录用户访问 API 的权限。 此为只读属性。 可为 Null。|
|ownedObjects|[directoryObject](directoryobject.md) 集合|此服务主体所拥有的目录对象。 只读。 可为空。|
|所有者|[directoryObject](directoryobject.md) 集合|作为此 servicePrincipal 的所有者的 Directory 对象。 所有者是允许修改此对象的一组非管理员用户或 servicePrincipals。 此为只读属性。 可为 NULL。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignedTo",
    "appRoleAssignments",
    "createdObjects",
    "createdOnBehalfOf",
    "endpoints",
    "memberOf",
    "oauth2PermissionGrants",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.servicePrincipal"
}-->

```json
{
  "accountEnabled": true,
  "addIns": [{"@odata.type": "microsoft.graph.addIn"}],
  "alternativeNames": ["string"] ,
  "appDisplayName": "string",
  "appId": "string",
  "appOwnerOrganizationId": "guid",
  "appRoleAssignmentRequired": true,
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "displayName": "string",
  "homepage": "string",
  "id": "string (identifier)",
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logoutUrl": "string",
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "replyUrls": ["string"],
  "servicePrincipalNames": ["string"],
  "servicePrincipalType": "string",
  "tags": ["string"],
  "tokenEncryptionKeyId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    ]
}
-->
