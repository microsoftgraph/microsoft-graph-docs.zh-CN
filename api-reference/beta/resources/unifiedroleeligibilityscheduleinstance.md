---
title: unifiedRoleEligibilityScheduleInstance 资源类型
description: 表示通过 Azure AD 角色分配符合条件的应用程序操作的计划Privileged Identity Management。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 024f00486898f6af0955fe2ecda93fdb024758d3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682122"
---
# <a name="unifiedroleeligibilityscheduleinstance-resource-type"></a>unifiedRoleEligibilityScheduleInstance 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通过 Azure AD 角色分配符合条件的用户Privileged Identity Management。 由 `roleEligibilityInstance` 和 `roleEligibilitySchedule` 创建，表示通过角色分配创建的实际合格Privileged Identity Management。 我们支持列出和获取 roleEligibilityInstance 上的操作，以便查看当前和将来的分配。

继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleEligibilityScheduleInstances](../api/unifiedroleeligibilityscheduleinstance-list.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 集合|获取 [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 对象及其属性的列表。|
|[获取 unifiedRoleEligibilityScheduleInstance](../api/unifiedroleeligibilityscheduleinstance-get.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|读取 [unifiedRoleEligibilityScheduleInstance 对象的属性和](../resources/unifiedroleeligibilityscheduleinstance.md) 关系。|
|[filterByCurrentUser](../api/unifiedroleeligibilityscheduleinstance-filterbycurrentuser.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 集合|获取 [unifiedRoleEligibilityInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 对象的列表，以及授予特定用户的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 对租户范围范围使用"/"。 应用程序作用域是仅由此应用程序定义和理解的范围。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|directoryScopeId|String|表示工作分配范围的目录对象的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 应用程序作用域是仅由此应用程序定义和理解的范围。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|endDateTime|DateTimeOffset|roleEligibilityScheduleInstance 到期的时间|
|id|String|roleEligibilityScheduleInstance 的唯一标识符。 Key，不可为 null，只读。继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|memberType|String|工作分配的成员身份类型。 它可以是 `Inherited` `Direct` 、、 或 `Group` 。|
|principalId|String|要授予分配的主体的 Objectid。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleDefinitionId|String|分配所针对的 unifiedRoleDefinition 的 ID。 只读。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleEligibilityScheduleId|String|此实例的父 roleEligibilitySchedule 的 ID|
|startDateTime|DateTimeOffset|roleEligibilityScheduleInstance 启动的时间|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。 包含实体。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|引用作为工作分配范围的目录对象的属性。 提供，以便调用方可以在获取符合条件的角色分配的同时获取 `$expand` 目录对象。 只读。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|principal|[directoryObject](../resources/directoryobject.md)|引用通过请求获取符合条件的角色分配的属性。 提供，以便调用方可以在获取符合条件的角色分配的同时 `$expand` 获取主体。 只读。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|指示分配所针对的 roleDefinition 的属性。 提供，以便调用方可以在获取符合条件的角色分配的同时获取 `$expand` 角色定义。 roleDefinition.Id 自动展开。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleInstance",
  "baseType": "microsoft.graph.unifiedRoleScheduleInstanceBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleEligibilityScheduleInstance",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "memberType": "String",
  "roleEligibilityScheduleId": "String"
}
```

