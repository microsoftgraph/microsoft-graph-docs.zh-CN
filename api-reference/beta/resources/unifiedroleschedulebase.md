---
title: unifiedRoleScheduleBase 资源类型
description: 将统一的角色分配计划与统一的角色资格计划相结合的统一角色计划的基属性
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dbe8b597286bacd9c6f8d0a7dc17cf82296fadb9
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398831"
---
# <a name="unifiedroleschedulebase-resource-type"></a>unifiedRoleScheduleBase 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将统一的角色分配计划与统一的角色资格计划相结合的统一角色计划的基属性

## <a name="properties"></a>属性

| 属性         | 类型           | 说明               |
| :--------------- | :------------- | :------------------------ |
| appScopeId       | String         | 分配范围特定于应用时特定于应用的范围的标识符。 分配的范围确定已授予主体访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元或所有用户。 |
| createdDateTime  | DateTimeOffset | 创建计划的时间。 |
| createdUsing     | String         | 创建此计划的角色AssignmentScheduleRequest 的标识符。 |
| directoryScopeId | String         | 表示分配范围的目录对象的标识符。 分配的范围确定已授予主体访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。 |
| id               | String         | unifiedRoleAssignmentSchedule 的唯一标识符。 键，不可为 null，只读。 |
| modifiedDateTime | DateTimeOffset | 上次更新计划的时间。 |
| principalId      | String         | 要向其授予分配的主体的标识符。 支持 `$filter`（`eq`）。 |
| roleDefinitionId | 字符串         | 工作分配所用于的 unifiedRoleDefinition 的标识符。 只读。 支持 `$filter`（`eq`）。 |
| status           | String         | `roleAssignmentSchedule`的状态 。 它可以包括状态相关的消息，如 `Provisioned`， `Revoked`， `Pending Provisioning`和 `Pending Approval`。 支持 `$filter`（`eq`）。  |

## <a name="relationships"></a>关系

| 关系   | 类型                                                                               | 说明               |
| :------------- | :--------------------------------------------------------------------------------- | :------------------------ |
| activeInstance (已弃用)  | [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) | 已弃用。 |
| appScope       | [appScope](../resources/appscope.md)                                               | 当分配范围特定于应用时，具有特定于应用范围的详细信息的只读属性。 包含实体。 |
| directoryScope | [directoryObject](../resources/directoryobject.md)                                 | 引用分配范围的目录对象的属性。 通过提供，调用方可以在获取角色分配的同时获取使用 `$expand` 目录对象。 只读。 |
| 主要      | [directoryObject](../resources/directoryobject.md)                                 | 引用通过请求获取角色分配的主体的属性。 提供此功能，使调用方可以在获取角色分配的同时获取主体 `$expand` 。 只读。 |
| roleDefinition | [unifiedRoleDefinition](../resources/unifiedroledefinition.md)                     | 指示分配所用于的 roleDefinition 的属性。 提供此功能，使调用方可以在获取角色分配的同时获取 `$expand` 角色定义。 roleDefinition.Id 将自动展开。 |

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
