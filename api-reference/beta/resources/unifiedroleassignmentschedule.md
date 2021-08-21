---
title: unifiedRoleAssignmentSchedule 资源类型
description: 表示通过 Azure AD 角色分配活动应用程序操作Privileged Identity Management。
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8e528fe7fd6508d8cc5c3eac23f1796731c50d5f
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453210"
---
# <a name="unifiedroleassignmentschedule-resource-type"></a>unifiedRoleAssignmentSchedule 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通过 Azure AD 角色分配活动Privileged Identity Management。 **unifiedRoleAssignmentSchedule** 由 [unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md)创建，用于实例化 [unifiedRoleAssignmentScheduleInstance](unifiedroleassignmentscheduleinstance.md)。 此资源支持列表和获取操作以检索计划，以便查看当前和将来的工作分配。

继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleAssignmentSchedules](../api/unifiedroleassignmentschedule-list.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 集合|获取 [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 对象及其属性的列表。|
|[获取 unifiedRoleAssignmentSchedule](../api/unifiedroleassignmentschedule-get.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|读取 [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 对象的属性和关系。|
|[filterByCurrentUser](../api/unifiedroleassignmentschedule-filterbycurrentuser.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 集合|获取向特定用户 [授予 unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 对象及其属性的列表。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 应用程序作用域是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将作用域限制为特定目录对象，例如管理单元。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|assignmentType|String|工作分配类型。 它可以是 或 `Assigned` `Activated` 。|
|createdDateTime|DateTimeOffset|创建计划的时间。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|createdUsing|String|创建此计划的 roleAssignmentScheduleRequest 的 ID。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScopeId|String|表示工作分配范围的目录对象的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 目录范围是存储在目录中的多个应用程序可以理解的共享范围。 用于 `/` 租户范围范围。 使用 **appScopeId** 将作用域限制为仅应用程序。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|id|String|unifiedRoleAssignmentSchedule 的唯一标识符。 键，不可为 null，只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|memberType|字符串|工作分配的成员身份类型。 它可以是 `Inherited` `Direct` 、、 或 `Group` 。|
|modifiedDateTime|DateTimeOffset|上次更新计划的时间。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principalId|String| 要授予分配的主体的 Objectid。 可以是组或用户。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。 <br> 支持 `$filter`（`eq`）。|
|roleDefinitionId|字符串|分配所针对的 unifiedRoleDefinition 的 ID。 只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。 <br> 支持 `$filter`（`eq`）。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|请求的计划角色分配对象。|
|状态|String|的状态 `roleAssignmentSchedule` 。 它可以包含与状态相关的消息，如 `Provisioned` `Revoked` `Pending Provisioning` 、、 和 `Pending Approval` 。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。<br> 支持 `$filter`（`eq`）。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|如果 roleAssignmentSchedule 由 roleEligibilitySchedule 激活，则这是指向该计划的链接。|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|将弃用。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|appScope|[appScope](../resources/appscope.md)|只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。 包含实体。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|引用作为工作分配范围的目录对象的属性。 提供，以便调用方可以在获取目录对象的同时获取 `$expand` 角色分配。 只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principal|[directoryObject](../resources/directoryobject.md)|引用通过请求获取角色分配主体的属性。 提供此权限，以便调用方可以在获取安全主体的同时获取 `$expand` 角色分配。 只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|指示分配所针对的 roleDefinition 的属性。 提供，以便调用方可以在获取角色定义的同时使用 `$expand` 角色分配。 roleDefinition.Id 自动展开。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentSchedule",
  "baseType": "microsoft.graph.unifiedRoleScheduleBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentSchedule",
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
  "assignmentType": "String",
  "memberType": "String"
}
```

