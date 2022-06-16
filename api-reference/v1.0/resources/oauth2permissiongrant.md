---
title: oAuth2PermissionGrant 资源类型
description: 表示已授予应用程序 (OAuth 2.0 范围) 委派权限，通常是用户或管理员同意过程的结果。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 300c44691aab3cc8f09bf621dd39bd89825dee2a
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118450"
---
# <a name="oauth2permissiongrant-resource-type"></a>oAuth2PermissionGrant 资源类型

命名空间：microsoft.graph

表示已授予应用程序服务主体的委派权限。

由于用户同意应用程序访问 API 或直接创建的请求，可以创建委托的权限授予。

委派的权限有时称为“OAuth 2.0 范围”或“范围”。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
| [列出 oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) 集合 | 检索委派权限授予的列表。 |
| [获取 oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md)  | 读取单个委派权限授予。|
| [创建 oAuth2PermissionGrant](../api/oauth2permissiongrant-post.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) | 创建委托的权限授予。 |
| [更新 oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | 无 | 更新 oAuth2PermissionGrant 对象。 |
| [Delete oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | 无  | 删除委托的权限授予。 |
|[Get delta](../api/oauth2permissiongrant-delta.md)|[oAuth2PermissionGrant](oauth2permissiongrant.md)|获取新创建、更新或删除的 **oauth2permissiongrant** 对象，而无需对整个资源集合执行完整读取。|

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| id | String | **oAuth2PermissionGrant** 的唯一标识符。 只读。|
| clientId | 字符串 | 应用程序的客户端 [服务主体](serviceprincipal.md)**的 ID**，该应用程序有权在访问 API 时代表已登录用户执行操作。 必需项。 支持 `$filter`（仅 `eq`）。 |
| consentType | String | 指示是否授予客户端应用程序模拟所有用户或仅特定用户的授权。 *AllPrincipals* 指示授权模拟所有用户。 *主体* 指示授权模拟特定用户。 管理员可以代表所有用户授予同意。 在某些情况下，对于某些委派的权限，非管理员用户可能有权代表自己同意。 必需项。 支持 `$filter`（仅 `eq`）。 |
| principalId | String | 当 **consentType** 为 *主体* 时，客户端有权访问资源的 [用户](user.md) **ID**。 如果 **consentType** 为 *AllPrincipals* ，则此值为 null。 如果 **consentType** 是主体，则为必需 *。* 支持 `$filter`（仅 `eq`）。|
| resourceId | String | 有权访问权限的资源 [服务主体](serviceprincipal.md)的 **ID**。 这将标识客户端有权代表已登录用户尝试调用的 API。 支持 `$filter`（仅 `eq`）。 |
| scope | String | 委托权限的声明值的空格分隔列表，应包含在资源应用程序的访问令牌中， (API) 。 例如，`openid User.Read GroupMember.Read.All`。 每个声明值应与 API 定义的委托权限之一的 **值** 字段匹配，该权限在资源 [服务主体](serviceprincipal.md)的 **oauth2PermissionScopes** 属性中列出。 |

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

