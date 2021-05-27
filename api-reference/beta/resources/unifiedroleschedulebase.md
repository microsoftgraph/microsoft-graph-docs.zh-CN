---
title: unifiedRoleScheduleBase 资源类型
description: 将统一角色计划与统一角色资格计划角色分配统一角色计划的基础属性
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ac0738d7ebc8ddc9a507b0911a3abc2016d78d33
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682217"
---
# <a name="unifiedroleschedulebase-resource-type"></a>unifiedRoleScheduleBase 资源类型

命名空间：microsoft.graph

将统一角色计划与统一角色资格计划角色分配统一角色计划的基础属性

## <a name="properties"></a>属性

| 属性         | 类型           | 说明               |
| :--------------- | :------------- | :------------------------ |
| appScopeId       | String         | 当分配范围特定于应用时，特定于应用的范围的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 对租户范围范围使用"/"。 应用程序作用域是仅由此应用程序定义和理解的范围。 |
| createdDateTime  | DateTimeOffset | 创建计划的时间。 |
| createdUsing     | String         | 创建此计划的 roleAssignmentScheduleRequest 的 ID。 |
| directoryScopeId | String         | 表示工作分配范围的目录对象的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 应用程序作用域是仅由此应用程序定义和理解的范围。 |
| id               | String         | unifiedRoleAssignmentSchedule 的唯一标识符。 键，不可为 null，只读。 |
| modifiedDateTime | DateTimeOffset | 上次更新计划的时间。 |
| principalId      | String         | 要授予分配的主体的 Objectid。 |
| roleDefinitionId | String         | 分配所针对的 unifiedRoleDefinition 的 ID。 只读。 |
| 状态           | String         | 的状态 `roleAssignmentSchedule` 。 它可以包含与状态相关的消息，如 `Provisioned` `Revoked` `Pending Provisioning` 、、 和 `Pending Approval` 。 |

## <a name="relationships"></a>关系

| 关系   | 类型                                                                               | 说明               |
| :------------- | :--------------------------------------------------------------------------------- | :------------------------ |
| activeInstance | [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) | 将弃用。 |
| appScope       | [appScope](../resources/appscope.md)                                               | 只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。 包含实体。 |
| directoryScope | [directoryObject](../resources/directoryobject.md)                                 | 引用作为工作分配范围的目录对象的属性。 提供，以便调用方可以在获取目录对象的同时使用 `$expand` 角色分配。 只读。 |
| principal      | [directoryObject](../resources/directoryobject.md)                                 | 引用通过请求获取角色分配主体的属性。 提供此权限，以便调用方可以使用 与获取 角色分配 同时 `$expand` 使用。 只读。 |
| roleDefinition | [unifiedRoleDefinition](../resources/unifiedroledefinition.md)                     | 指示分配所针对的 roleDefinition 的属性。 提供，以便调用方可以在获取角色定义的同时使用 `$expand` 角色分配。 roleDefinition.Id 自动展开。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleBase",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.unifiedRoleScheduleBase",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "createdUsing": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "status": "String"
}
```
