---
title: unifiedRoleAssignmentSchedule 资源类型
description: 表示通过 Azure AD Privileged Identity Management执行活动角色分配操作的计划。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ab32cf141bf16b8b763c5b2d54700df7d3f3d8a9
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461623"
---
# <a name="unifiedroleassignmentschedule-resource-type"></a>unifiedRoleAssignmentSchedule 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通过 Azure AD Privileged Identity Management进行活动角色分配的计划。 **unifiedRoleAssignmentSchedule** 由 [unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) 创建，用于实例化 [unifiedRoleAssignmentScheduleInstance](unifiedroleassignmentscheduleinstance.md)。 此资源支持列表并获取用于检索计划以查看当前和将来分配的操作。

继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleAssignmentSchedules](../api/rbacapplication-list-roleassignmentschedules.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 集合|获取 [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 对象及其属性的列表。|
|[获取 unifiedRoleAssignmentSchedule](../api/unifiedroleassignmentschedule-get.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|读取 [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 对象的属性和关系。|
|[filterByCurrentUser](../api/unifiedroleassignmentschedule-filterbycurrentuser.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 集合|获取向特定用户授予的 [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 对象及其属性的列表。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|分配范围特定于应用时特定于应用的范围的标识符。 分配的范围确定已授予主体访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|assignmentType|String|工作分配类型。 它可以是 `Assigned` 或 `Activated`.|
|createdDateTime|DateTimeOffset|创建计划的时间。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|createdUsing|字符串|创建此计划的角色AssignmentScheduleRequest 的 ID。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScopeId|String|表示分配范围的目录对象的标识符。 分配的范围确定已授予主体访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|id|字符串|unifiedRoleAssignmentSchedule 的唯一标识符。 键，不可为 null，只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|memberType|String|分配的成员身份类型。 它可以是 `Inherited`， `Direct`或 `Group`.|
|modifiedDateTime|DateTimeOffset|上次更新计划的时间。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principalId|字符串| 要向其授予分配的主体的 Objectid。 可以是组或用户。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。 <br> 支持 `$filter`（`eq`）。|
|roleDefinitionId|字符串|工作分配所针对的 unifiedRoleDefinition 的 ID。 只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。 <br> 支持 `$filter`（`eq`）。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|角色分配请求的计划对象。|
|status|String|`roleAssignmentSchedule`的状态 。 它可以包括状态相关的消息，如 `Provisioned`， `Revoked`， `Pending Provisioning`和 `Pending Approval`。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。<br> 支持 `$filter`（`eq`）。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|如果 roleEligibilitySchedule 激活了 roleAssignmentSchedule，则这是指向该计划的链接。|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|将被弃用。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|appScope|[appScope](../resources/appscope.md)|当分配范围特定于应用时，具有特定于应用范围的详细信息的只读属性。 包含实体。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|引用分配范围的目录对象的属性。 通过提供，调用方可以在获取角色分配的同时获取使用 `$expand` 目录对象。 只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|主要|[directoryObject](../resources/directoryobject.md)|引用通过请求获取角色分配的主体的属性。 提供此功能，使调用方可以在获取角色分配的同时获取主体 `$expand` 。 只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|指示分配所用于的 roleDefinition 的属性。 提供此功能，使调用方可以在获取角色分配的同时获取 `$expand` 角色定义。 roleDefinition.Id 将自动展开。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

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

