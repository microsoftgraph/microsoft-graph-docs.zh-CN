---
title: unifiedRoleDefinition 资源类型
description: 角色定义是 Azure AD Azure Active Directory (中的权限) 。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2307b6fd429e8cc4942a5a50e04316ee77332671
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148500"
---
# <a name="unifiedroledefinition-resource-type"></a>unifiedRoleDefinition 资源类型

命名空间：microsoft.graph

角色定义是 Azure AD Azure Active Directory (权限) 列出可以执行的操作以及可针对这些操作执行的资源。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 unifiedRoleDefinition](../api/rbacapplication-list-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) 集合 | 读取 unifiedRoleDefinition 对象及其属性的列表。 |
| [获取 unifiedRoleDefinition](../api/unifiedroledefinition-get.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | 读取 unifiedRoleDefinition 对象的属性。 |
| [创建 unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | 创建 unifiedRoleDefinition 对象。 |
| [更新 unifiedRoleDefinition](../api/unifiedroledefinition-update.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | 更新 unifiedRoleDefinition 对象。 |
| [删除 unifiedRoleDefinition](../api/unifiedroledefinition-delete.md) | 无 | 删除 unifiedRoleDefinition 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String| unifiedRoleDefinition 的说明。 **isBuiltIn** 为 时为只读 `true` 。 |
|displayName|String| unifiedRoleDefinition 的 显示名称。 **isBuiltIn** 为 时为只读 `true` 。 必需。  支持 $filter (`eq` `in` 、) 。|
|id|String| 角色定义的唯一标识符。 键，不可为 null，只读。 继承自 [实体](../resources/entity.md)。 支持 $filter (`eq` `in` 、) 。 |
|isBuiltIn|Boolean| 指示角色定义是包含在 Azure AD Azure Active Directory (或自定义定义) 集的一部分的标志。 只读。 支持 $filter (`eq` `in` 、) 。 |
|isEnabled|Boolean| 指示角色是否已启用分配的标志。 如果 `false` 角色不能用于分配。 **isBuiltIn** 为 true 时为只读。 |
|resourceScopes|String collection| 角色定义适用的范围或权限的列表。 当前仅 `/` 受支持。 **isBuiltIn** 为 true 时为只读。 **请勿使用。这将很快被弃用。将作用域附加到角色分配。** | 
|rolePermissions|[unifiedRolePermission](unifiedrolepermission.md) 集合| 角色中包含的权限列表。 **isBuiltIn** 为 时为只读 `true` 。 必需。 |
|templateId|String| 可在 **isBuiltIn** 为 时设置的自定义模板标识符，但在 `false` **isBuiltIn** 为 时为只读 `true` 。 如果一个标识符在不同目录之间需要相同，则通常使用此标识符。 |
|version|String| 指示角色定义的版本。 **isBuiltIn** 为 时为只读 `true` 。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|inheritsPermissionsFrom| [unifiedRoleDefinition](unifiedroledefinition.md) 集合| 给定角色定义从其继承的角色定义的只读集合。 只有 **isBuiltIn** (Azure AD 内置角色 `true`) 此属性。 支持 `$expand`。 |

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

