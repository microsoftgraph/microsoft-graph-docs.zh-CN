---
title: unifiedRoleDefinition 资源类型
description: 统一的角色定义是权限的集合
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 93bc01ac19e0f976463821342524b060141e6182
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247229"
---
# <a name="unifiedroledefinition-resource-type"></a>unifiedRoleDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个权限集合，其中列出了可由 RBAC 提供程序执行的操作（如读取、写入和删除）作为 Microsoft 365 RBAC [角色管理](rolemanagement.md)的一部分。

目前支持以下 RBAC 提供程序：
- 云电脑 
- 设备管理 (Intune) 
- 目录 (Azure AD)  
- 权利管理 (Azure AD) 


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
|说明|String| unifiedRoleDefinition 的说明。 如果 **IsBuiltIn** 为 true，则为只读。 |
|displayName|String| unifiedRoleDefinition 的显示名称。 如果 **IsBuiltIn** 为 true，则为只读。 必填。  仅支持 `$filter` (`eq` 和 `startsWith` 运算符) 。|
|id|String| unifiedRoleDefinition 的唯一标识符。 键，不可为 null，只读。  仅支持 `$filter` (运算 `eq` 符) 。 |
|isBuiltIn|Boolean| 指示 unifiedRoleDefinition 是否是产品或自定义中包含的默认集的一部分的标志。 只读。  仅支持 `$filter` (运算 `eq` 符) 。|
|isEnabled|Boolean| 指示是否为分配启用角色的标志。 如果为 false，则该角色不可用于分配。 如果 **IsBuiltIn** 为 true，则为只读。 |
|resourceScopes|String collection| 角色定义授予的范围权限列表适用。 目前仅 `/` 支持。 如果 IsBuiltIn 为 true，则为只读。 **请勿使用。这将很快被弃用。将范围附加到角色分配** | 
|rolePermissions|[unifiedRolePermission](unifiedrolepermission.md) 集合| 角色中包含的权限列表。 如果 **IsBuiltIn** 为 true，则为只读。 必填。 |
|templateId|String| 可在 isBuiltIn 为 false 时设置的自定义模板标识符。 如果需要不同目录中的标识符相同，则通常会使用此标识符。 如果 **IsBuiltIn** 为 true，则为只读。 |
|version|String| 指示 unifiedRoleDefinition 的版本。 如果 **IsBuiltIn** 为 true，则为只读。|

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|inheritsPermissionsFrom| [unifiedRoleDefinition](unifiedroledefinition.md) 集合| 给定角色定义继承的角色定义的只读集合。 只有Azure AD内置角色支持此属性。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
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
  "inheritsPermissionsFrom": [{"@odata.type": "microsoft.graph.unifiedRoleDefinition"}],
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


