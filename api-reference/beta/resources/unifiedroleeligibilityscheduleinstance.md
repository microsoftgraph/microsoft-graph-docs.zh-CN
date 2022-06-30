---
title: unifiedRoleEligibilityScheduleInstance 资源类型
description: 表示通过 Azure AD Privileged Identity Management执行符合条件的角色分配操作的计划实例。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 14345412d06d1a36210f1cb2c5cfd5c2cf18c5a1
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439360"
---
# <a name="unifiedroleeligibilityscheduleinstance-resource-type"></a>unifiedRoleEligibilityScheduleInstance 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户中角色资格的实例。

继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleEligibilityScheduleInstances](../api/rbacapplication-list-roleeligibilityscheduleinstances.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 集合|GGet 角色突出显示的实例。|
|[获取 unifiedRoleEligibilityScheduleInstance](../api/unifiedroleeligibilityscheduleinstance-get.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|获取角色资格的实例。|
|[filterByCurrentUser](../api/unifiedroleeligibilityscheduleinstance-filterbycurrentuser.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 集合|获取调用主体的合格角色实例。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|分配范围特定于应用时特定于应用的范围的标识符。 分配的范围确定已授予主体访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持`$filter` (`eq`和`ne``null`值) 。|
|directoryScopeId|String|表示分配范围的目录对象的标识符。 分配的范围确定已授予主体访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持`$filter` (`eq`和`ne``null`值) 。|
|endDateTime|DateTimeOffset|roleEligibilityScheduleInstance 到期的时间。|
|id|String|roleEligibilityScheduleInstance 的唯一标识符。 键（不可为 null）只读。继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。|
|memberType|String|分配的成员身份类型。 它可以是 `Inherited`， `Direct`或 `Group`.|
|principalId|String|要向其授予分配的主体的标识符。 可以是组或用户。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。|
|roleDefinitionId|String|工作分配所用于的 unifiedRoleDefinition 的标识符。 只读。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。<br> 支持 `$filter`（`eq`）。|
|roleEligibilityScheduleId|String|此实例的父角色EligibilitySchedule 的标识符。|
|startDateTime|DateTimeOffset|角色EligibilityScheduleInstance 的开始时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|当分配范围特定于应用时，具有特定于应用范围的详细信息的只读属性。 包含实体。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持 `$expand`。|
|directoryScope|[directoryObject](../resources/directoryobject.md)|引用分配范围的目录对象的属性。 提供此功能，使调用方可以获取与获取符合条件的角色分配同时使用的 `$expand` 目录对象。 只读。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持 `$expand`。|
|主要|[directoryObject](../resources/directoryobject.md)|引用通过请求获取符合条件的角色分配的主体的属性。 提供此功能，使调用方可以在获取符合条件的角色分配的同时获取主体 `$expand` 。 只读。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持 `$expand`。|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|指示分配所用于的 roleDefinition 的属性。 提供此功能，使调用方可以在获取符合条件的角色分配的同时获取 `$expand` 角色定义。 roleDefinition.Id 将自动展开。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持 `$expand`。|

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

