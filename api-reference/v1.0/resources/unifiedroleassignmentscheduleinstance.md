---
title: unifiedRoleAssignmentScheduleInstance 资源类型
description: 表示租户中活动角色分配的实例。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 004a4af4b84712d824787e7d45d7b4f083d9fd6b
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549342"
---
# <a name="unifiedroleassignmentscheduleinstance-resource-type"></a>unifiedRoleAssignmentScheduleInstance 资源类型

命名空间：microsoft.graph

表示租户中活动角色分配的实例。 活动分配可能是通过 [PIM 分配和激活请求](../api/rbacapplication-post-roleassignmentschedulerequests.md)进行的，也可以是直接通过 [角色分配 API](../resources/unifiedroleassignment.md) 进行的。

继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleAssignmentScheduleInstances](../api/rbacapplication-list-roleassignmentscheduleinstances.md)|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) 集合|获取活动角色分配的实例。|
|[获取 unifiedRoleAssignmentScheduleInstance](../api/unifiedroleassignmentscheduleinstance-get.md)|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|获取活动角色分配的实例。|
|[filterByCurrentUser](../api/unifiedroleassignmentscheduleinstance-filterbycurrentuser.md)|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) 集合|获取调用主体的活动角色分配实例。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|分配作用域为应用时特定于应用的范围的标识符。 分配的范围确定已授予主体访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。 支持`$filter` (`eq`和`ne``null`值) 。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。|
|assignmentType|字符串|工作分配的类型，可以是 `Assigned` 或 `Activated`。 支持 `$filter`（`eq`、`ne`）。|
|directoryScopeId|String|表示分配范围的目录对象的标识符。 分配的范围确定已授予主体访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。 支持`$filter` (`eq`和`ne``null`值) 。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。|
|endDateTime|DateTimeOffset| 计划实例的结束日期。|
|id|String|**unifiedRoleAssignmentScheduleInstance** 对象的唯一标识符。 继承自 [entity](../resources/entity.md)。|
|memberType|字符串|分配的继承方式。 它可以是 `Inherited`， `Direct`或 `Group`. 这进一步意味着 **unifiedRoleAssignmentSchedule** 是否可以由调用方管理。 支持 `$filter`（`eq`、`ne`）。|
|principalId|String|已授予角色分配的主体的标识符。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持 `$filter`（`eq`、`ne`）。 |
|roleAssignmentOriginId|String|Azure AD 中角色分配的标识符。 支持 `$filter`（`eq`、`ne`）。|
|roleAssignmentScheduleId|String|从中创建此实例的 **unifiedRoleAssignmentSchedule** 对象的标识符。 支持 `$filter`（`eq`、`ne`）。|
|roleDefinitionId|String|分配给主体的 [unifiedRoleDefinition](unifiedroledefinition.md) 对象的标识符。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持 `$filter`（`eq`、`ne`）。|
|startDateTime|DateTimeOffset|当此实例启动时。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|如果请求来自符合条件的管理员来激活角色，则此参数将显示该激活的相关合格分配。 否则，情况会如此 `null`。 支持 `$expand`。|
|appScope|[appScope](../resources/appscope.md)|当分配范围限定到应用时，具有特定于应用范围的详细信息的只读属性。 可为 NULL。 支持 `$expand`。|
|directoryScope|[directoryObject](../resources/directoryobject.md)|作为分配范围的目录对象。 只读。 支持 `$expand`。|
|主要|[directoryObject](../resources/directoryobject.md)|通过请求获取角色分配的主体。 支持 `$expand`。|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|通过 **roleDefinitionId** 属性引用的 roleDefinition 对象的详细信息。 支持 `$expand`。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleInstance",
  "baseType": "microsoft.graph.unifiedRoleScheduleInstanceBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleInstance",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentType": "String",
  "memberType": "String",
  "roleAssignmentOriginId": "String",
  "roleAssignmentScheduleId": "String"
}
```

