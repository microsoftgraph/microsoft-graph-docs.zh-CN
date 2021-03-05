---
title: oAuth2PermissionGrant 资源类型
description: 表示已授予 (OAuth 2.0) （通常是由于用户或管理员同意过程）的委派权限。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: d0c9e78d22a882998c0e17ba521cc76a611697af
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50432842"
---
# <a name="oauth2permissiongrant-resource-type"></a>oAuth2PermissionGrant 资源类型

命名空间：microsoft.graph

表示已授予应用程序的服务主体的委派权限。

委派的权限授予可以是用户同意应用程序访问 API 请求的结果，也可以直接创建。

委派的权限有时称为"OAuth 2.0 范围"或"作用域"。

## <a name="methods"></a>Methods

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
| [列出 oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) 集合 | 检索委派权限授予的列表。 |
| [获取 oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md)  | 读取单个委派权限授予。|
| [创建 oAuth2PermissionGrant](../api/oauth2permissiongrant-post.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) | 创建委派权限授予。 |
| [更新 oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | 无 | 更新 oAuth2PermissionGrant 对象。 |
| [删除 oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | 无  | 删除委派权限授予。 |
|[获取 delta](../api/oauth2permissiongrant-delta.md)|[oAuth2PermissionGrant](oauth2permissiongrant.md)|获取新创建、更新或删除的 **oauth2permissiongrant** 对象，而无需执行整个资源集合的完全读取。|

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| id | String | **oAuth2PermissionGrant 的唯一标识符**。 只读。|
| clientId | 字符串 | **应用程序** 客户端 [服务](serviceprincipal.md)主体的 ID，授权在访问 API 时代表登录用户操作。 必填。 支持 `$filter`（仅 `eq`）。 |
| consentType | String | 指示是否向客户端应用程序授予了模拟所有用户或仅模拟特定用户的授权。 *AllPrincipals* 指示对模拟所有用户的授权。 *主体* 指示对模拟特定用户的授权。 管理员可以代表所有用户授予同意。 在某些情况下，对于某些委派权限，非管理员用户可能有权代表自己同意。 必填。 支持 `$filter`（仅 `eq`）。 |
| principalId | String | **consentType** 为 [Principal](user.md)时，客户端有权访问资源的用户的 *ID。* 如果 **consentType** *为 AllPrincipals，* 则此值为 null。 consentType 为 **主体** 时 *必需*。 |
| resourceId | String | **有权访问** 的资源 [服务](serviceprincipal.md)主体的 ID。 这标识了客户端有权尝试代表登录用户调用的 API。 |
| scope | String | 委派权限声明值的列表（以空格分隔）应包含在 API (访问令牌) 。 例如，`openid User.Read GroupMember.Read.All`。 每个声明值应匹配由API 定义的委派权限之一的值字段，在资源服务主体的 **publishedPermissionScopes** 属性 [中列出](serviceprincipal.md)。 |

## <a name="relationships"></a>关系

无。

该资源支持通过提供 [delta](../api/oauth2permissiongrant-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

