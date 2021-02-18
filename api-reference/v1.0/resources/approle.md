---
title: appRole 资源类型
description: 表示客户端应用程序可能请求调用另一个应用程序的应用程序角色，或可能用于将应用程序分配给指定应用程序角色中的用户或组的应用程序角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: ee38168920dee5c836be6801a7f63181df565eb5
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272497"
---
# <a name="approle-resource-type"></a>appRole 资源类型

命名空间：microsoft.graph

表示应用程序角色， (请求并授予) 客户端应用程序，或可用于将应用程序分配给指定角色的用户或组。 

若要添加、更新或删除应用程序的应用程序角色，请 [更新](../api/application-update.md) 应用或服务的应用程序。 应用程序实体上的应用程序角色将在使用该应用程序的所有租户中可用。 若要定义仅适用于租户 (的应用角色，例如，在多租户应用程序) 实例中表示自定义角色的应用角色，还可以更新应用的服务主体，以向 **appRoles** 集合 [](../api/serviceprincipal-update.md)中添加或更新应用角色。

使用 [appRoleAssignments，](approleassignment.md)可以将应用角色分配给用户、组或其他应用程序的服务主体。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|allowedMemberTypes|String collection|通过设置为) ，指定是否可以将此应用程序角色分配给用户和组 (，或者通过设置为 (或同时将 (设置为) 来分配给其他应用程序的 `["User"]` `["Application"]` `["User", "Application"]` (。 支持向其他应用程序的服务主体分配的应用角色也称为 [应用程序权限](/graph/auth/auth-concepts#microsoft-graph-permissions)。 仅应用程序实体上定义的应用程序角色支持 **"Application"** 值。|
|description|String|应用角色的说明。 在分配应用角色时显示此状态，如果应用角色用作应用程序权限，将在同意体验期间显示。|
|displayName|String|在应用名称和许可体验中角色分配名称。|
|id|Guid|**appRoles 集合内的唯一角色** 标识符。 创建新的应用角色时，必须提供新的 Guid 标识符。 |
|isEnabled|Boolean|在创建或更新应用角色时，必须设置为 **true** (这是默认) 。 若要删除角色，必须先将其设置为 **false。**  此时，在后续调用中，可能会删除此角色。|
|origin|String| 指定应用程序角色是在 [应用程序](application.md) 对象上还是 [servicePrincipal 实体](serviceprincipal.md) 上定义。 _不得包含在_ 任何 POST 或 PATCH 请求中。 只读。 |
|value|String|指定要包括在 ID 令牌中的声明和访问令牌（对分配的用户和服务主体进行身份验证） `roles` 中的值。 长度不得超过 120 个字符。 允许的字符 `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` 以及范围中的字符 `0-9` 和 `A-Z` `a-z` 。 不允许任何其他字符（包括空格字符）。  |

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

