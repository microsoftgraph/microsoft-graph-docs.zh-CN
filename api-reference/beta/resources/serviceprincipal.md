---
title: servicePrincipal 资源类型
description: 表示目录中的一个应用程序实例。 继承自 directoryObject。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 37a4311fe59498a8d210b3ccf6d7184e1263bfb5
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234024"
---
# <a name="serviceprincipal-resource-type"></a>servicePrincipal 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示目录中的一个应用程序实例。 继承自 [directoryObject](directoryobject.md)。

该资源支持通过提供 [delta](../api/serviceprincipal-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[Get servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |读取 servicePrincipal 对象的属性和关系。|
|[列出 servicePrincipals](../api/serviceprincipal-list.md) | [servicePrincipal](serviceprincipal.md) 集合 | 检索 servicePrincipal 对象列表。 |
|[创建 appRoleAssignment](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| 通过发布至 appRoleAssignments 集合创建新的 appRoleAssignment。|
|[列出 appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |[appRoleAssignment](approleassignment.md) 集合| 获取 appRoleAssignment 对象集合。|
|[列出 createdObjects](../api/serviceprincipal-list-createdobjects.md) |[directoryObject](directoryobject.md) 集合| 获取 createdObject 对象集合。|
|[列出 memberOf](../api/serviceprincipal-list-memberof.md) |[directoryObject](directoryobject.md) 集合| 从 memberOf 导航属性中获取此服务主体是其直接成员的组。|
|[列出 transitive memberOf](../api/serviceprincipal-list-transitivememberof.md) |[directoryObject](directoryobject.md) 集合| 列出此服务主体所属的组。 此操作是可传递的，并包括此服务主体以嵌套方式所属的组。 |
|[分配 claimsMappingPolicy](../api/serviceprincipal-post-claimsmappingpolicies.md)| [claimsMappingPolicy](claimsmappingpolicy.md) 集合| 向此对象分配 claimsMappingPolicy。|
|[列出 claimsMappingPolicies](../api/serviceprincipal-list-claimsmappingpolicies.md)| [claimsMappingPolicy](claimsmappingpolicy.md) 集合| 为此对象分配的 claimsMappingPolicies。|
|[删除 claimsMappingPolicy](../api/serviceprincipal-delete-claimsmappingpolicies.md)| [claimsMappingPolicy](claimsmappingpolicy.md) 集合| 从此对象中删除 tokenLifetimePolicy。|
|[分配 homeRealmDiscoveryPolicy](../api/serviceprincipal-post-homerealmdiscoverypolicies.md)| [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) 集合| 向此对象分配 homeRealmDiscoveryPolicy。|
|[列出 homeRealmDiscoveryPolicy](../api/serviceprincipal-list-homerealmdiscoverypolicies.md)| [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) 集合| 为此对象分配的 homeRealmDiscoveryPolicies。|
|[删除 homeRealmDiscoveryPolicy](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md)| [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) 集合| 从此对象中删除 homeRealmDiscoveryPolicy。|
|[分配 tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md)| [tokenLifetimePolicy](tokenlifetimepolicy.md) 集合| 向此对象分配 tokenLifetimePolicy。|
|[列出 tokenLifetimePolicies](../api/application-list-tokenlifetimepolicies.md)| [tokenLifetimePolicy](tokenlifetimepolicy.md) 集合| 获取已分配至此对象的所有 tokenLifetimePolicies。|
|[删除 tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md)| [tokenLifetimePolicy](tokenlifetimepolicy.md) 集合| 从此对象中删除 tokenLifetimePolicy。|
|[List oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合| 获取 oAuth2PermissionGrant 对象集合。|
|[列出 ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |[directoryObject](directoryobject.md) 集合| 获取 ownedObject 对象集合。|
|[添加所有者](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| 通过发布到所有者集合创建新的所有者。|
|[列出所有者](../api/serviceprincipal-list-owners.md) |[directoryObject](directoryobject.md) 集合| 获取所有者对象集合。|
|[更新](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |更新 servicePrincipal 对象。 |
|[删除](../api/serviceprincipal-delete.md) | 无 |删除 servicePrincipal 对象。 |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|String 集合|检查指定组列表中的成员身份。|
|[checkMemberObjects](../api/serviceprincipal-checkmemberobjects.md)|String 集合|检查组、目录角色或管理单元对象指定列表中的成员身份。|
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|String 集合|获取此服务主体所属的组列表。|
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|String 集合|获取此服务主体所属的组和目录角色列表。|
|[delta](../api/serviceprincipal-delta.md)|servicePrincipal 集合| 获取服务主体的增量更改。 |
|[createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)|[passwordSingleSignOnCredentialSet](passwordsinglesignoncredentialset.md)|为正文中指定的用户或组创建凭据集。|
|[deletePasswordSingleSignOnCredentials](../api/serviceprincipal-deletepasswordsinglesignoncredentials.md)|无|删除正文中指定的用户或组的凭据集。|
|[getPasswordSingleSignOnCredentials](../api/serviceprincipal-getpasswordsinglesignoncredentials.md)|[passwordSingleSignOnCredentialSet](passwordsinglesignoncredentialset.md)|为正文中指定的用户或组获取凭据集。|
|[updatePasswordSingleSignOnCredentials](../api/serviceprincipal-updatepasswordsinglesignoncredentials.md)|无|为正文中指定的用户或组更新凭据集。|

## <a name="properties"></a>属性
| 属性     | 类型 |说明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| 如果服务主体帐户已启用，则为 **true**；否则，为 **false**。            |
|appDisplayName|String|关联应用程序公开的显示名称。|
|appId|String|关联应用程序的唯一标识符（其 **appId** 属性）。|
|appRoleAssignmentRequired|Boolean|指定在 Azure AD 在向应用程序签发用户或访问令牌之前用户或组是否需要 **appRoleAssignment**。 不可为空。 |
|appRoles|[appRole](approle.md) 集合|关联应用程序公开的应用程序角色。 有关详细信息，请参阅[应用程序](application.md)实体上的 **appRoles** 属性定义。 不可为空。 |
|displayName|String|服务主体的显示名称。|
|errorUrl|String|            |
|homepage|String|关联应用程序的主页的 URL。|
|keyCredentials|[keyCredential](keycredential.md) 集合|与服务帐户关联的密钥凭据集合。 不可为空。            |
|logoutUrl|String| 指定 Microsoft 授权服务使用[正向通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[反向通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户时所使用的 URL。  |
|oauth2Permissions|[oAuth2Permission](oauth2permission.md) 集合|关联应用程序的 OAuth 2.0 权限。 有关详细信息，请参阅[应用程序](application.md)实体上的 **oauth2Permissions** 属性定义。 不可为空。            |
|id|String|服务主体的唯一标识符。 继承自 [directoryObject](directoryobject.md)。 键。 不可为 null。 只读。|
|passwordCredentials|[passwordCredential](passwordcredential.md) 集合|与服务帐户关联的密码凭据集合。 不可为空。 |
|preferredTokenSigningKeyThumbprint|String|仅供内部使用。 请勿写入属性，否则将依赖该属性。 可能会在未来版本中删除。 |
|publisherName|String|在其中指定关联应用程序的租户的显示名称。|
|replyUrls|String 集合|向其发送用户令牌以使用关联应用程序登录的 URL，或者为关联应用程序向其发送 OAuth 2.0 authorization 代码和访问令牌的重定向 URL。 不可为空。 |
|samlMetadataUrl|String| |
|servicePrincipalNames|String 集合|标识关联应用程序的 URL。 有关详细信息，请参阅[应用程序对象和服务主体对象](https://msdn.microsoft.com/library/azure/dn132633.aspx)。多值属性的筛选表达器需要 **any** 运算符。  不可为空。 |
|标记|String 集合| 不可为空。 |

## <a name="relationships"></a>关系
| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|为此服务主体分配的主体（用户、组和服务主体）。 只读。|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) 集合|为服务主体分配的应用程序。 只读。 可为 Null。|
|claimsMappingPolicies|[claimsMappingPolicy](claimsmappingpolicy.md) 集合|为此服务主体分配的 claimsMappingPolicies。|
|createdObjects|[directoryObject](directoryobject.md) 集合|此服务主体所创建的目录对象。 只读。 可为 Null。|
|homeRealmDiscoveryPolicies|[homeRealmDiscoveryPolicy](homeRealmDiscoveryPolicy.md) 集合|为此服务主体分配的 homeRealmDiscoveryPolicies。|
|memberOf|[directoryObject](directoryobject.md) 集合|此服务主体所属的角色。 HTTP 方法：GET 只读。 可为空。|
|oauth2PermissionGrants|[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合|与此服务主体关联的用户模拟授权。 只读。 可为 Null。|
|ownedObjects|[directoryObject](directoryobject.md) 集合|此服务主体所拥有的目录对象。 只读。 可为空。|
|所有者|[directoryObject](directoryobject.md) 集合|拥有此服务主体的目录对象。 所有者是一组允许修改此对象的非管理员用户。 只读。 可为 Null。|
|tokenLifetimePolicies|[tokenLifetimePolicy](tokenLifetimePolicy.md) 集合|为此服务主体分配的 tokenLifetimePolicies。|

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignedTo",
    "appRoleAssignments",
    "createdObjects",
    "createdOnBehalfOf",
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
  "appDisplayName": "string",
  "appId": "string",
  "appOwnerOrganizationId": "guid",
  "appRoleAssignmentRequired": true,
  "displayName": "string",
  "errorUrl": "string",
  "homepage": "string",
  "id": "string (identifier)",
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logoutUrl": "string",
  "oauth2Permissions": [{"@odata.type": "microsoft.graph.oAuth2Permission"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "preferredTokenSigningKeyThumbprint": "string",
  "publisherName": "string",
  "replyUrls": ["string"],
  "samlMetadataUrl": "string",
  "servicePrincipalNames": ["string"],
  "tags": ["string"],
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}]
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
  "suppressions": []
}
-->
