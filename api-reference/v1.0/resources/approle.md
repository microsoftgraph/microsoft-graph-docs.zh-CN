---
title: appRole 资源类型
description: 表示客户端应用程序可能请求调用另一个应用程序的应用程序角色，或可能用于将应用程序分配给具有指定应用程序角色的用户或组的应用程序角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 7bff67b287c12a984299045b7ac0297b253974d5
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638849"
---
# <a name="approle-resource-type"></a>appRole 资源类型

命名空间：microsoft.graph

表示应用程序角色， (请求并授予) 客户端应用程序，或可用于将应用程序分配给指定角色中的用户或组。 

若要添加、更新或删除应用程序的应用程序角色，请 [更新](../api/application-update.md) 应用程序或服务的应用程序。 应用程序实体上的应用程序角色将在使用应用程序的所有租户中可用。 若要定义仅适用于租户 (例如，代表多租户应用程序) 实例中的自定义角色的应用角色，还可以更新应用的服务主体，以向 **appRoles** 集合添加或更新应用 [](../api/serviceprincipal-update.md)角色。

使用 [appRoleAssignments，](approleassignment.md)可以将应用角色分配给用户、组或其他应用程序的服务主体。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|allowedMemberTypes|String 集合|通过设置为) ，指定此应用角色是否可分配给用户和组 (，或者通过设置为) 将此应用程序角色设置为 或同时将两 (分配给应用程序的 `["User"]` `["Application"]` `["User", "Application"]` (。 支持向其他应用程序的服务主体分配的应用程序角色也称为应用程序 [权限](/graph/auth/auth-concepts#microsoft-graph-permissions)。 "Application"值仅受应用程序实体上定义的 **应用角色** 支持。|
|说明|String|应用角色的说明。 在分配应用角色时显示，如果应用角色在同意体验期间用作应用程序权限，则显示此状态。|
|displayName|String|应用和许可体验中显示的权限角色分配名称。|
|id|Guid|**appRoles 集合内的唯一角色** 标识符。 创建新的应用角色时，必须提供新的 Guid 标识符。 |
|isEnabled|Boolean|在创建或更新应用角色时，必须设置为 **true** (这是默认角色) 。 若要删除角色，必须先将其设置为 **false**。  此时，在后续调用中，可能会删除此角色。|
|origin|String| 指定应用程序角色是在 [application](application.md) 对象上还是 [servicePrincipal](serviceprincipal.md) 实体上定义。 _不得_ 包含在任何 POST 或 PATCH 请求中。 只读。 |
|value|String|指定要包括在 ID 令牌和访问令牌中的声明中的值，对分配的用户和服务主体 `roles` 进行身份验证。 长度不得超过 120 个字符。 允许的字符 `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` 包括 、 和 范围 `0-9` `A-Z` 中的字符 `a-z` 。 不允许任何其他字符，包括空格字符。 不得以 开头 `.` 。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRole"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

