---
title: unifiedRoleDefinition 资源类型
description: 角色定义是Azure Active Directory (Azure AD) 中的权限集合。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f3a54d12ce4c11ee10d106759ccbaa0e32b80978
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246592"
---
# <a name="unifiedroledefinition-resource-type"></a>unifiedRoleDefinition 资源类型

命名空间：microsoft.graph

角色定义是Azure Active Directory (Azure AD) 列出可执行的操作及其可以执行的资源的权限的集合。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 unifiedRoleDefinition](../api/rbacapplication-list-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) 集合 | 读取 unifiedRoleDefinition 对象及其属性的列表。 |
| [获取 unifiedRoleDefinition](../api/unifiedroledefinition-get.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | 读取 unifiedRoleDefinition 对象的属性。 |
| [创建 roleDefinitions](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | 创建 unifiedRoleDefinition 对象。 |
| [更新 unifiedRoleDefinition](../api/unifiedroledefinition-update.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | 更新 unifiedRoleDefinition 对象。 |
| [删除 unifiedRoleDefinition](../api/unifiedroledefinition-delete.md) | 无 | 删除 unifiedRoleDefinition 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String| unifiedRoleDefinition 的说明。 **IsBuiltIn 为** `true`只读。 |
|displayName|String| unifiedRoleDefinition 的显示名称。 **IsBuiltIn 为** `true`只读。 必填。  支持$filter (`eq`、 `in`) 。|
|id|String| 角色定义的唯一标识符。 键，不可为 null，只读。 继承自 [entity](../resources/entity.md)。 支持$filter (`eq`、 `in`) 。 |
|isBuiltIn|Boolean| 指示角色定义是Azure Active Directory (Azure AD) 或自定义定义中包含的默认集的一部分的标志。 只读。 支持$filter (`eq`、 `in`) 。 |
|isEnabled|Boolean| 指示是否为分配启用角色的标志。 如果 `false` 该角色不可用于分配。 如果 **IsBuiltIn** 为 true，则为只读。 |
|resourceScopes|String collection| 角色定义应用于的范围或权限的列表。 目前仅 `/` 支持。 如果 **IsBuiltIn** 为 true，则为只读。 **请勿使用。这将很快被弃用。将范围附加到角色分配。** | 
|rolePermissions|[unifiedRolePermission](unifiedrolepermission.md) 集合| 角色中包含的权限列表。 **IsBuiltIn 为** `true`只读。 必填。 |
|templateId|String| 可在 **isBuiltIn** 时设置的自定义模板标识符， `false` 但在 **IsBuiltIn** 为 `true`时为只读标识符。 如果需要不同目录中的标识符相同，则通常会使用此标识符。 |
|version|String| 指示角色定义的版本。 **IsBuiltIn 为** `true`只读。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|inheritsPermissionsFrom| [unifiedRoleDefinition](unifiedroledefinition.md) 集合| 给定角色定义继承的角色定义的只读集合。 只有 (**isBuiltIn** `true` Azure AD内置角色) 支持此属性。 支持 `$expand`。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.unifiedRoleDefinition",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isBuiltIn": "Boolean",
  "isEnabled": "Boolean",
  "resourceScopes": [
    "String"
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.unifiedRolePermission"
    }
  ],
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

