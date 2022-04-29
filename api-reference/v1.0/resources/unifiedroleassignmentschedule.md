---
title: unifiedRoleAssignmentSchedule 资源类型
description: 表示租户中活动角色分配的计划。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7294918800c68857ca11ac41a7baf8fab7e4da5e
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133923"
---
# <a name="unifiedroleassignmentschedule-resource-type"></a>unifiedRoleAssignmentSchedule 资源类型

命名空间：microsoft.graph

表示租户中活动角色分配的计划，用于实例化 [unifiedRoleAssignmentScheduleInstance](unifiedroleassignmentscheduleinstance.md)。 活动分配可能是通过 [PIM 分配和激活请求](../api/rbacapplication-post-roleassignmentschedulerequests.md)进行的，也可以是直接通过 [角色分配 API](../resources/unifiedroleassignment.md) 进行的。

继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleAssignmentSchedules](../api/rbacapplication-list-roleassignmentschedules.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 集合|获取活动角色分配操作的计划。|
|[获取 unifiedRoleAssignmentSchedule](../api/unifiedroleassignmentschedule-get.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|检索活动角色分配操作的计划。|
|[filterByCurrentUser](../api/unifiedroleassignmentschedule-filterbycurrentuser.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 集合|检索登录用户是其主体的活动角色分配操作的计划。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|分配作用域为应用时特定于应用的范围的标识符。 分配的范围确定已授予主体访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。 支持`$filter` (`eq`和`ne``null`值) 。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。|
|assignmentType|String|工作分配的类型，可以是 `Assigned` 或 `Activated`。 支持 `$filter`（`eq`、`ne`）。|
|createdDateTime|DateTimeOffset|创建计划时。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。|
|createdUsing|String|通过此计划创建的 **unifiedRoleAssignmentScheduleRequest** 对象的标识符。 可为 NULL。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。 支持`$filter` (`eq`和`ne``null`值) 。|
|directoryScopeId|String|表示分配范围的目录对象的标识符。 分配的范围确定已授予主体访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。 支持`$filter` (`eq`和`ne``null`值) 。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。|
|id|String|**unifiedRoleAssignmentScheduleRequest** 对象的唯一标识符。 支持 `$filter`（`eq`）。 继承自 [entity](../resources/entity.md)。|
|memberType|String|分配的继承方式。 它可以是 `Inherited`， `Direct`或 `Group`. 这进一步意味着 **unifiedRoleAssignmentSchedule** 是否可以由调用方管理。 支持 `$filter`（`eq`、`ne`）。|
|modifiedDateTime|DateTimeOffset|上次修改计划的时间。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。|
|principalId|String|已授予角色分配的主体的标识符。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。 支持 `$filter`（`eq`、`ne`）。|
|roleDefinitionId|String|分配给主体的 [unifiedRoleDefinition](unifiedroledefinition.md) 对象的标识符。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。 支持 `$filter`（`eq`、`ne`）。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|角色分配的周期。 它可以表示单个事件或多次重复。|
|状态|String|**unifiedRoleAssignmentScheduleRequest** 对象的状态。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。 可能的值为：`Canceled`、、`Denied`、`Failed`、`Granted`、`PendingApproval``PendingAdminDecision`、`PendingProvisioning``Revoked``PendingScheduleCreation``Provisioned`、和 。`ScheduleCreated` 不可为 null。 支持 `$filter`（`eq`、`ne`）。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|如果请求来自符合条件的管理员来激活角色，则此参数将显示该激活的相关合格分配。 否则，情况会如此 `null`。 支持 `$expand`。|
|appScope|[appScope](../resources/appscope.md)|当分配范围限定到应用时，具有特定于应用范围的详细信息的只读属性。 可为 NULL。 支持 `$expand`。|
|directoryScope|[directoryObject](../resources/directoryobject.md)|作为分配范围的目录对象。 只读。 支持 `$expand`。|
|主要|[directoryObject](../resources/directoryobject.md)|通过请求获取角色分配的主体。 支持 `$expand`。|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|通过 **roleDefinitionId** 属性引用的 roleDefinition 对象的详细信息。 支持 `$expand`。|

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

