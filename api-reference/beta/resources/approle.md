---
title: appRole 资源类型
description: 表示可能由调用其他应用程序的客户端应用程序请求的应用程序角色, 或可用于向指定的应用程序角色中的用户或组分配应用程序的应用程序角色。 ServicePrincipal 实体和 application 实体的**appRoles**属性是**appRole**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 35c26e52c5d7eb9529474d08a43b68fceddfc954
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013316"
---
# <a name="approle-resource-type"></a>appRole 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可能由调用其他应用程序的客户端应用程序请求的应用程序角色, 或可用于向指定的应用程序角色中的用户或组分配应用程序的应用程序角色。 [ServicePrincipal](serviceprincipal.md)实体和[Application](application.md)实体的**appRoles**属性是**appRole**的集合。

> 重要说明: 当前版本中禁用了此功能。

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
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowedMemberTypes|String collection|指定是否可以通过设置为 "用户" 或将此应用程序角色定义分配给用户和组, 或通过设置为 "应用程序" 或同时设置为 "应用程序" 来将此应用程序角色定义分配给用户和组。|
|说明|String|在管理员应用分配和同意体验中显示的权限帮助文本。|
|displayName|字符串|管理员同意和应用工作分配体验中显示的权限的显示名称。|
|id|Guid|**AppRoles**集合中的唯一角色标识符。 创建新的应用程序角色时, 必须提供新的 Guid 标识符。 |
|isEnabled|Boolean|在创建或更新应用程序角色时, 必须将其设置为**true** (默认值为)。 若要删除角色, 必须首先将此设置为**false**。  此时, 在后续调用中, 可能会删除此角色。|
|格式|String| 只读。 指定是在 Application 对象上还是在 ServicePrincipal 对象上定义应用程序角色。 不得__ 包含在任何 POST 或 PATCH 请求中。 |
|value|String|指定将包含在 authentication 和 access 令牌中`roles`的声明中的值。 长度不得超过120个字符。 允许的字符`:` `!` `#` `$` `%`为`&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `0-9`中`A-Z`的字符`a-z`和。 `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` 不允许使用任何其他字符, 包括空格字符。  |


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
