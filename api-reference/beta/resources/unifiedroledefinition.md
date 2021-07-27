---
title: unifiedRoleDefinition 资源类型
description: 统一角色定义是权限的集合
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: be8c37fcc5014abedaeb63ff061d4ac4cca68add
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53533876"
---
# <a name="unifiedroledefinition-resource-type"></a>unifiedRoleDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示列出操作（如读取、写入和删除）的权限集合，这些操作可在 RBAC 角色管理中由 RBAC Microsoft 365[执行](rolemanagement.md)。

目前支持以下 RBAC 提供程序：
- 云电脑 
- Intune (设备) 
- Azure AD (目录)  
- Azure AD (授权) 

> [!NOTE]
> 云电脑和权利管理 RBAC 提供程序当前仅支持[列表和](../api/rbacapplication-list-roledefinitions.md)[获取](../api/unifiedroledefinition-get.md)操作。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

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
|说明|String| unifiedRoleDefinition 的说明。 **isBuiltIn** 为 true 时为只读。 |
|displayName|String| unifiedRoleDefinition 的 显示名称。 **isBuiltIn** 为 true 时为只读。 必填。  仅 `$filter` (`eq` `startsWith` 和运算符) 。|
|id|String| unifiedRoleDefinition 的唯一标识符。 键，不可为 null，只读。  仅 `$filter` (`eq` 运算符) 。 |
|isBuiltIn|Boolean| 指示 unifiedRoleDefinition 是否属于产品或自定义中包含的默认集的标志。 只读。  仅 `$filter` (`eq` 运算符) 。|
|isEnabled|Boolean| 指示角色是否已启用分配的标志。 如果为 false，则角色不能用于分配。 **isBuiltIn** 为 true 时为只读。 |
|resourceScopes|String collection| 角色定义授予的作用域权限列表适用。 当前仅 `/` 受支持。 isBuiltIn 为 true 时为只读。 **请勿使用。这将很快被弃用。将作用域附加到角色分配** | 
|rolePermissions|[unifiedRolePermission](unifiedrolepermission.md) 集合| 角色中包含的权限列表。 **isBuiltIn** 为 true 时为只读。 必填。 |
|templateId|String| 可以在 isBuiltIn 为 false 时设置的自定义模板标识符。 如果一个标识符在不同目录之间需要相同，则通常使用此标识符。 **isBuiltIn** 为 true 时为只读。 |
|version|String| 指示 unifiedRoleDefinition 的版本。 **isBuiltIn** 为 true 时为只读。|

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|inheritsPermissionsFrom| [unifiedRoleDefinition](unifiedroledefinition.md) 集合| 给定角色定义从其继承的角色定义的只读集合。 仅 Azure AD 内置角色支持此属性。 |

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


