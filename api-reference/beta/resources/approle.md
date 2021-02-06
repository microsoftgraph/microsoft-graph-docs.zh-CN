---
title: appRole 资源类型
description: 表示应用程序角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: ff659cb8e149d952b1a27fdcbc1154b0fda49841
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136288"
---
# <a name="approle-resource-type"></a>appRole 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示应用程序角色， (并授予) 客户端应用程序，或可用于将应用程序分配给指定角色中的用户或组的应用程序角色。 

应用程序和 [servicePrincipal](serviceprincipal.md)实体的 **appRoles** 属性是 **appRole 的集合**。 [](application.md) 

使用 [appRoleAssignments，](approleassignment.md)可以将应用角色分配给用户、组或其他应用程序的服务主体。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|allowedMemberTypes|字符串集合|指定是否可以通过将此应用程序角色设置为 (来分配给用户和组) ，通过设置为 (或将两者设置为 (来分配给应用程序的 `["User"]` `["Application"]` `["User", "Application"]`) 。 支持向其他应用程序的服务主体分配的应用程序角色也称为 [应用程序权限](/graph/auth/auth-concepts#microsoft-graph-permissions)。 "Application"值仅支持在应用程序实体上 **定义的应用** 角色。 |
|说明|字符串|应用角色的说明。 在分配应用角色时显示此状态，如果应用角色用作应用程序权限，将在同意体验期间显示。|
|displayName|字符串|应用和许可体验中显示的权限角色分配名称。|
|id|Guid|**appRoles 集合内的唯一角色** 标识符。 创建新的应用角色时，必须提供新的 Guid 标识符。 |
|isEnabled|Boolean|在创建或更新应用角色时，必须设置为 **true** (默认角色) 。 若要删除角色，必须先将其设置为 **false。**  此时，在后续调用中，可能会删除此角色。|
|origin|字符串| 指定应用程序角色是在 [应用程序](application.md) 对象上还是 [servicePrincipal 实体上](serviceprincipal.md) 定义。 _不得包含在_ 任何 POST 或 PATCH 请求中。 只读。 |
|value|String|指定要包括在 ID 令牌和访问令牌中的声明中的值，对分配的用户和服务主体 `roles` 进行身份验证。 长度不得超过 120 个字符。 允许的字符 `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` 以及范围中的字符 `0-9` 和 `A-Z` `a-z` 。 不允许任何其他字符，包括空格字符。  |

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


