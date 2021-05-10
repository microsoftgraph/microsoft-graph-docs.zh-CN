---
title: unifiedRoleEligibilitySchedule 资源类型
description: 表示通过 Azure AD 角色分配符合条件的操作Privileged Identity Management。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1593e819b3c57ee24dae0480aadcb7f532d2fbf4
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299197"
---
# <a name="unifiedroleeligibilityschedule-resource-type"></a>unifiedRoleEligibilitySchedule 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通过 Azure AD 角色分配符合条件的用户Privileged Identity Management。 `roleEligibilitySchedule`由 创建 `roleEligibilityScheduleRequest` ，用于实例化 `roleEligibilityInstance` 。 我们支持列出和获取用于检索计划的操作，以便查看当前和未来符合条件的分配。

继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleEligibilitySchedules](../api/unifiedroleeligibilityschedule-list.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 集合|获取 [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 对象及其属性的列表。|
|[获取 unifiedRoleEligibilitySchedule](../api/unifiedroleeligibilityschedule-get.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|读取 [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 对象的属性和关系。|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedule-filterbycurrentuser.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 集合|获取 [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 对象的列表，以及授予特定用户的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 对租户范围范围使用"/"。 应用程序作用域是仅由此应用程序定义和理解的范围。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|createdDateTime|DateTimeOffset|创建计划的时间。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|createdUsing|String|创建此计划的 RoleEligibilityScheduleRequest 的 ID。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScopeId|String|表示工作分配范围的目录对象的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 应用程序作用域是仅由此应用程序定义和理解的范围。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|id|String|unifiedRoleEligibilitySchedule 的唯一标识符。 键，不可为 null，只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|memberType|String|符合条件的分配的成员身份类型。 它可以是 `Inherited` `Direct` 、、 或 `Group` 。|
|modifiedDateTime|DateTimeOffset|上次更新计划的时间。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principalId|String| 要授予符合条件的工作分配的主体的 Objectid。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinitionId|String|符合条件的分配所针对的 unifiedRoleDefinition 的 ID。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|符合条件的请求的计划角色分配对象。|
|状态|String|的状态 `roleEligibilitySchedule` 。 它可以包含与状态相关的消息，如 `Provisioned` `Revoked` `Pending Provisioning` 、、 和 `Pending Approval` 。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|将弃用。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|appScope|[appScope](../resources/appscope.md)|只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。 包含实体。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|引用作为合格分配范围的目录对象的属性。 提供，以便调用方可以在获取符合条件的对象的同时获取 `$expand` 角色分配。 只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principal|[directoryObject](../resources/directoryobject.md)|引用通过请求获取符合条件的角色分配的属性。 提供此权限，以便调用方可以使用 与获取符合条件 `$expand` 角色分配。 只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|指示符合条件的分配所针对的 roleDefinition 的属性。 提供，以便调用方可以在获取符合条件的角色定义的同时获取角色 `$expand` 角色分配。 roleDefinition.Id 自动展开。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleEligibilitySchedule",
  "baseType": "microsoft.graph.unifiedRoleScheduleBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleEligibilitySchedule",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "createdUsing": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "status": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "memberType": "String"
}
```

