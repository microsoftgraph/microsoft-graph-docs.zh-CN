---
title: unifiedRoleEligibilityScheduleInstance 资源类型
description: 表示一个计划实例，该实例用于角色分配一个Azure AD Privileged Identity Management。
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 514c731693cf0f04037d5ee413ef4a66f17397e3
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695235"
---
# <a name="unifiedroleeligibilityscheduleinstance-resource-type"></a>unifiedRoleEligibilityScheduleInstance 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示符合条件的应用程序实例角色分配Azure AD Privileged Identity Management。 **unifiedRoleEligibilityScheduleInstance** 由 [unifiedRoleEligibilitySchedule](unifiedroleeligibilityschedule.md)创建，表示通过 Privileged Identity Management 创建的实际合格角色分配。 此资源支持"列表"和"获取"操作，以便查看当前和将来的工作分配。

继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleEligibilityScheduleInstances](../api/unifiedroleeligibilityscheduleinstance-list.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 集合|获取 [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 对象及其属性的列表。|
|[获取 unifiedRoleEligibilityScheduleInstance](../api/unifiedroleeligibilityscheduleinstance-get.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|读取 [unifiedRoleEligibilityScheduleInstance 对象的属性和](../resources/unifiedroleeligibilityscheduleinstance.md) 关系。|
|[filterByCurrentUser](../api/unifiedroleeligibilityscheduleinstance-filterbycurrentuser.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 集合|获取 [unifiedRoleEligibilityInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 对象的列表，以及授予特定用户的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 应用程序作用域是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将作用域限制为特定的目录对象，例如管理单元。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。|
|directoryScopeId|String|表示工作分配范围的目录对象的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 用于 `/` 租户范围范围。 使用 **appScopeId** 将作用域限制为仅应用程序。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。|
|endDateTime|DateTimeOffset|roleEligibilityScheduleInstance 到期的时间。|
|id|String|roleEligibilityScheduleInstance 的唯一标识符。 键，不可为 null，只读。继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。|
|memberType|String|工作分配的成员身份类型。 它可以是 `Inherited` `Direct` 、、 或 `Group` 。|
|principalId|String|要向其中授予工作分配的主体的标识符。 可以是组或用户。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。|
|roleDefinitionId|字符串|分配所针对的 unifiedRoleDefinition 的标识符。 只读。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。<br> 支持 `$filter`（`eq`）。|
|roleEligibilityScheduleId|字符串|此实例的父 roleEligibilitySchedule 的标识符。|
|startDateTime|DateTimeOffset|roleEligibilityScheduleInstance 将启动的时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。 包含实体。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|引用作为工作分配范围的目录对象的属性。 提供，以便调用方可以在获取符合条件的角色分配的同时获取 `$expand` 目录对象。 只读。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|principal|[directoryObject](../resources/directoryobject.md)|引用通过请求获取符合条件的角色分配的属性。 提供，以便调用方可以在获取符合条件的角色分配的同时获取 `$expand` 主体。 只读。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
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

