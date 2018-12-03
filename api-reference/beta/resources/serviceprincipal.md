---
title: servicePrincipal 资源类型
description: 表示一个目录中的应用程序的实例。 继承自 directoryObject。
ms.openlocfilehash: c3a08efb1dea1109bd32d59a479260e14089783d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046843"
---
# <a name="serviceprincipal-resource-type"></a>servicePrincipal 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示一个目录中的应用程序的实例。 继承自 [directoryObject](directoryobject.md)。

该资源支持：

- 通过提供 [delta](../api/serviceprincipal-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

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
  "@odata.type": "microsoft.graph.serviceprincipal"
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
  "tags": ["string"]
}

```
## <a name="properties"></a>属性
| 属性     | 类型 |说明|
|:---------------|:--------|:----------|
|accountEnabled|布尔| **true**如果已启用的服务主体帐户;否则为**false**。            |
|appDisplayName|字符串|通过关联的应用程序公开的显示名称。|
|appId|String|关联的应用程序 （其**appId**属性） 的唯一标识符。|
|appRoleAssignmentRequired|布尔值|指定 Azure AD 将问题的用户或访问令牌对应用程序之前是否需要向用户或组**appRoleAssignment** 。 不可为 null。 |
|appRoles|[appRole](approle.md)集合|由关联的应用程序公开应用程序角色。 有关详细信息请参阅[应用程序](application.md)在实体上的**appRoles**属性定义。 不可为 null。 |
|displayName|字符串|服务主体的显示名。|
|errorUrl|字符串|            |
|主页|字符串|关联的应用程序的主页的 URL。|
|keyCredentials|[keyCredential](keycredential.md)集合|关键凭据与主体服务相关联的集合。 不可为 null。            |
|logoutUrl|字符串| 指定将由 Microsoft 的授权服务的用户使用[前信道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[后通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议的注销 URL。  |
|oauth2Permissions|[oAuth2Permission](oauth2permission.md)集合|由关联的应用程序公开 OAuth 2.0 权限。 有关详细信息请参阅[应用程序](application.md)在实体上的**oauth2Permissions**属性定义。 不可为 null。            |
|id|字符串|服务主体的唯一标识符。 继承自 [directoryObject](directoryobject.md)。 键。 不可为 null。 只读。|
|passwordCredentials|[passwordCredential](passwordcredential.md)集合|密码凭据的服务主体相关联的集合。 不可为 null。 |
|preferredTokenSigningKeyThumbprint|字符串|保留以仅供内部使用。 不要编写或否则依赖于此属性。 可能会在将来版本中删除。 |
|publisherName|String|在其中指定关联的应用程序租户的显示名称。|
|replyUrls|String 集合|用户令牌发送到的登录关联的应用程序或重定向 Uri 的 OAuth 2.0 授权代码和访问令牌发送到关联的应用程序的 Url。 不可为 null。 |
|samlMetadataUrl|字符串| |
|servicePrincipalNames|String 集合|标识关联的应用程序的 Uri。 有关详细信息，请参阅[应用程序对象和服务主体对象](https://msdn.microsoft.com/library/azure/dn132633.aspx)。**Any**运算符，则需要为多值属性的筛选器表达式。  不可为 null。 |
|标记前添加的标记|String collection| 不可为 null。 |

## <a name="relationships"></a>Relationships
| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|主体 （用户、 组和服务主体） 分配给此服务主体。 只读。|
|appRoleAssignments|[appRoleAssignment](approleassignment.md)集合|使用分配给的服务主体的应用程序。 只读。 可为 Null。|
|createdObjects|[directoryObject](directoryobject.md) 集合|创建的此服务主体的目录对象。 只读。 可为 Null。|
|memberOf|[directoryObject](directoryobject.md) 集合|此服务主体所在的角色。 HTTP 方法： 获取只读的。 可为 Null。|
|oauth2PermissionGrants|[oAuth2PermissionGrant](oauth2permissiongrant.md)集合|用户模拟授予与此服务主体关联。 只读。 可为 Null。|
|ownedObjects|[directoryObject](directoryobject.md) 集合|通过此服务主体拥有的目录对象。 只读。 可为 Null。|
|owners|[directoryObject](directoryobject.md) 集合|将此服务主体的所有者的目录对象。 所有者是一组的非管理员用户有权修改此对象。 只读。 可为 Null。|
|策略|[策略](policy.md)集合|分配给此服务主体的策略。|

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |读取属性和 servicePrincipal 对象的关系。|
|[列表 servicePrincipals](../api/serviceprincipal-list.md) | [servicePrincipal](serviceprincipal.md)集合 | 检索 servicePrincipal 对象的列表。 |
|[创建 appRoleAssignment](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| 通过发布到 appRoleAssignments 集合中创建新 appRoleAssignment。|
|[列表 appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |[appRoleAssignment](approleassignment.md)集合| 获取 appRoleAssignment 对象集合。|
|[List createdObjects](../api/serviceprincipal-list-createdobjects.md) |[directoryObject](directoryobject.md) collection| 获取 createdObject 对象集合。|
|[List memberOf](../api/serviceprincipal-list-memberof.md) |[directoryObject](directoryobject.md) 集合| 获取主体此服务是从 memberOf 导航属性的直接成员的组。|
|[列表可传递 memberOf](../api/serviceprincipal-list-transitivememberof.md) |[directoryObject](directoryobject.md) 集合| 列出此服务主体的成员的组。 此操作可传递，包括此服务主体的嵌套的成员的组。 |
|[列表分配策略](../api/policy-list-assigned.md)| [策略](policy.md)集合| 获取所有策略分配给此对象。|
|[列表 oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |[oAuth2PermissionGrant](oauth2permissiongrant.md)集合| 获取 oAuth2PermissionGrant 对象集合。|
|[List ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |[directoryObject](directoryobject.md) collection| 获取 ownedObject 对象集合。|
|[添加所有者](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| 通过发布到所有者集合中创建一个新的所有者。|
|[列出所有者](../api/serviceprincipal-list-owners.md) |[directoryObject](directoryobject.md) 集合| 获取一个所有者对象集合。|
|[Update](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |更新 servicePrincipal 对象。 |
|[删除](../api/serviceprincipal-delete.md) | 无 |删除 servicePrincipal 对象。 |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|String collection||
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|String collection||
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|String collection||
|[delta](../api/serviceprincipal-delta.md)|servicePrincipal 集合| 获得的服务主体的增量更改。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
