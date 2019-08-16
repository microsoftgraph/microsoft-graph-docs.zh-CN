---
title: unifiedRoleDefinition 资源类型
description: 统一角色定义是权限的集合
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: be1b8a0b1a623c6cf322d5cf7997f04b87875c51
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437746"
---
# <a name="unifiedroledefinition-resource-type"></a>unifiedRoleDefinition 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

UnifiedRoleDefinition 是列出可执行的操作 (如读取、写入和删除) 的权限的集合。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 unifiedRoleDefinition](../api/rbacapplication-list-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md)集合 | 读取 unifiedRoleDefinition 对象及其属性的列表。 |
| [获取 unifiedRoleDefinition](../api/unifiedroledefinition-get.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | 读取 unifiedRoleDefinition 对象的属性。 |
| [创建 unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | 创建 unifiedRoleDefinition 对象。 |
| [更新 unifiedRoleDefinition](../api/unifiedroledefinition-update.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | 更新 unifiedRoleDefinition 对象。 |
| [删除 unifiedRoleDefinition](../api/unifiedroledefinition-delete.md) | 无 | 删除 unifiedRoleDefinition 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String| UnifiedRoleDefinition 的说明。 当 isBuiltIn 为 true 时为只读。 |
|displayName|字符串| UnifiedRoleDefinition 的显示名称。 当 isBuiltIn 为 true 时为只读。 必需。|
|id|字符串| UnifiedRoleDefinition 的唯一标识符。 键, 不可为 null, 只读。 |
|isBuiltIn|布尔值| 指示 unifiedRoleDefinition 是否是产品或自定义的默认设置的一部分的标志。 只读。 |
|isEnabled|Boolean| 指示角色是否已启用分配的标志。 如果为 false, 则该角色不可用于分配。 当 isBuiltIn 为 true 时为只读。 |
|resourceScopes|String collection| 由角色定义授予的范围权限列表应用于。 目前仅支持 "/"。 当 isBuiltIn 为 true 时为只读。 |
|rolePermissions|[unifiedRolePermission](unifiedrolepermission.md)集合| 角色中包含的权限的列表。 当 isBuiltIn 为 true 时为只读。 必需。 |
|templateId|String| 当 isBuiltIn 为 false 时可设置的自定义模板标识符。 如果一个要求标识符在不同目录中是相同的, 则通常使用此标识符。 当 isBuiltIn 为 true 时为只读。 |
|version|String| 指示 unifiedRoleDefinition 的版本。 当 isBuiltIn 为 true 时为只读。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isBuiltIn": true,
  "isEnabled": true,
  "resourceScopes": ["String"],
  "rolePermissions": [{"@odata.type": "microsoft.graph.unifiedRolePermission"}],
  "templateId": "String",
  "version": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
