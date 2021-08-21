---
title: unifiedRoleAssignmentScheduleInstance 资源类型
description: 表示通过 Azure AD 角色分配活动应用程序操作的计划Privileged Identity Management。
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 64ccc65b7daf312ee79bbc5bed032ceaafd956f8
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453182"
---
# <a name="unifiedroleassignmentscheduleinstance-resource-type"></a>unifiedRoleAssignmentScheduleInstance 资源类型

命名空间：microsoft.graph 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通过 Azure AD 角色分配活动Privileged Identity Management。 **unifiedRoleAssignmentScheduleInstance** 由 [unifiedRoleAssignmentSchedule](unifiedroleassignmentschedule.md)创建，表示通过 角色分配 创建的实际Privileged Identity Management。 此资源支持 List 和 Get 操作，以便查看当前和将来的工作分配。

继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleAssignmentScheduleInstances](../api/unifiedroleassignmentscheduleinstance-list.md)|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) 集合|获取 [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) 对象及其属性的列表。|
|[获取 unifiedRoleAssignmentScheduleInstance](../api/unifiedroleassignmentscheduleinstance-get.md)|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|读取 [unifiedRoleAssignmentScheduleInstance 对象的属性和](../resources/unifiedroleassignmentscheduleinstance.md) 关系。|
|[filterByCurrentUser](../api/unifiedroleassignmentscheduleinstance-filterbycurrentuser.md)|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) 集合|获取 [unifiedRoleAssignmentScheduleInstance](../resources/unifiedRoleAssignmentScheduleInstance.md) 对象的列表，以及授予特定用户的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 应用程序作用域是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将作用域限制为特定目录对象，例如管理单元。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。|
|assignmentType|String|工作分配类型。 它可以是 或 `Assigned` `Activated` 。|
|createdDateTime|DateTimeOffset|创建计划的时间。|
|directoryScopeId|String|表示工作分配范围的目录对象的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 目录范围是存储在目录中的多个应用程序可以理解的共享范围。 用于 `/` 租户范围范围。 使用 **appScopeId** 将作用域限制为仅应用程序。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|endDateTime|DateTimeOffset|roleAssignmentInstance 到期的时间|
|id|String|unifiedRoleAssignmentScheduleInstance 的唯一标识符。 键，不可为 null，只读。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|memberType|字符串|工作分配的成员身份类型。 它可以是 `Inherited` `Direct` 、、 或 `Group` 。|
|principalId|String|要向其中授予工作分配的主体的标识符。 可以是组或用户。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleAssignmentOriginId|字符串|目录中 roleAssignment 的 ID|
|roleAssignmentScheduleId|字符串|此实例的父 roleAssignmentSchedule 的 ID|
|roleDefinitionId|String|分配所针对的 unifiedRoleDefinition 的标识符。 只读。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。  <br> 支持 `$filter`（`eq`）。|
|startDateTime|DateTimeOffset|roleAssignmentInstance 将启动的时间|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|如果 roleAssignmentScheduleInstance 由 roleEligibilityScheduleRequest 激活，则这是指向相关计划实例的链接。|
|appScope|[appScope](../resources/appscope.md)|只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。 包含实体。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|引用作为工作分配范围的目录对象的属性。 提供，以便调用方可以在获取目录对象的同时获取 `$expand` 角色分配。 只读。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|principal|[directoryObject](../resources/directoryobject.md)|引用通过请求获取角色分配主体的属性。 提供此权限，以便调用方可以使用 与获取权限相同的 `$expand` 角色分配。 只读。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|指示分配所针对的 roleDefinition 的属性。 提供，以便调用方可以在获取角色定义的同时使用 `$expand` 角色分配。 roleDefinition.Id 自动展开。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|

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

