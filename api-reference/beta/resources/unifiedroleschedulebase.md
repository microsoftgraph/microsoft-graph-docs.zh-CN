---
title: unifiedRoleScheduleBase 资源类型
description: 将统一角色计划与统一角色资格计划角色分配统一角色计划的基础属性
author: shauliu1
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b65d7d41feccfa8336ea347936433da2437f0f6b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59050878"
---
# <a name="unifiedroleschedulebase-resource-type"></a>unifiedRoleScheduleBase 资源类型

命名空间：microsoft.graph

将统一角色计划与统一角色资格计划角色分配统一角色计划的基础属性

## <a name="properties"></a>属性

| 属性         | 类型           | 说明               |
| :--------------- | :------------- | :------------------------ |
| appScopeId       | String         | 当分配范围特定于应用时，特定于应用的范围的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 应用程序作用域是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将作用域限制为特定的目录对象，例如管理单元或所有用户。 |
| createdDateTime  | DateTimeOffset | 创建计划的时间。 |
| createdUsing     | String         | 创建此计划的 roleAssignmentScheduleRequest 的标识符。 |
| directoryScopeId | String         | 表示工作分配范围的目录对象的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 目录范围是存储在目录中的多个应用程序可以理解的共享范围。 用于 `/` 租户范围范围。 使用 **appScopeId** 将作用域限制为仅应用程序。 |
| id               | String         | unifiedRoleAssignmentSchedule 的唯一标识符。 键，不可为 null，只读。 |
| modifiedDateTime | DateTimeOffset | 上次更新计划的时间。 |
| principalId      | String         | 要向其中授予工作分配的主体的标识符。 支持 `$filter`（`eq`）。 |
| roleDefinitionId | String         | 分配所针对的 unifiedRoleDefinition 的标识符。 只读。 支持 `$filter`（`eq`）。 |
| status           | String         | 的状态 `roleAssignmentSchedule` 。 它可以包含与状态相关的消息，如 `Provisioned` `Revoked` `Pending Provisioning` 、、 和 `Pending Approval` 。 支持 `$filter`（`eq`）。  |

## <a name="relationships"></a>关系

| 关系   | 类型                                                                               | 说明               |
| :------------- | :--------------------------------------------------------------------------------- | :------------------------ |
| activeInstance (已弃)  | [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) | 已弃用。 |
| appScope       | [appScope](../resources/appscope.md)                                               | 只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。 包含实体。 |
| directoryScope | [directoryObject](../resources/directoryobject.md)                                 | 引用作为工作分配范围的目录对象的属性。 提供，以便调用方可以在获取目录对象的同时获取 `$expand` 角色分配。 只读。 |
| principal      | [directoryObject](../resources/directoryobject.md)                                 | 引用通过请求获取角色分配的属性。 提供此权限，以便调用方可以使用 与获取权限 `$expand` 角色分配。 只读。 |
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
