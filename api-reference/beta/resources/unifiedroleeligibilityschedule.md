---
title: unifiedRoleEligibilitySchedule 资源类型
description: 表示通过项目执行符合条件的角色分配计划Azure AD Privileged Identity Management。
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e9cf19622cb707688711361b3ef71e405bbaf665
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695242"
---
# <a name="unifiedroleeligibilityschedule-resource-type"></a>unifiedRoleEligibilitySchedule 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示符合条件的项目到角色分配Azure AD Privileged Identity Management。 **unifiedRoleEligibilitySchedule** 由 [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md)创建，用于实例化 [unifiedRoleEligibilityScheduleInstance](unifiedroleeligibilityscheduleinstance.md)。 此资源支持 List 和 Get 操作以检索计划，以便查看当前和未来符合条件的工作分配。

继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleEligibilitySchedules](../api/unifiedroleeligibilityschedule-list.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 集合|获取 [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 对象及其属性的列表。|
|[获取 unifiedRoleEligibilitySchedule](../api/unifiedroleeligibilityschedule-get.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|读取 [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 对象的属性和关系。|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedule-filterbycurrentuser.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 集合|获取 [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 对象的列表，以及授予特定用户的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 应用程序作用域是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将作用域限制为特定的目录对象，例如管理单元。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。|
|createdDateTime|DateTimeOffset|创建计划的时间。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。|
|createdUsing|String|创建此计划的 roleEligibilityScheduleRequest 的标识符。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。|
|directoryScopeId|String|表示工作分配范围的目录对象的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 用于 `/` 租户范围范围。 使用 **appScopeId** 将作用域限制为仅应用程序。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。|
|id|String|unifiedRoleEligibilitySchedule 的唯一标识符。 键，不可为 null，只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。|
|memberType|String|符合条件的分配的成员身份类型。 它可以是 `Inherited` `Direct` 、、 或 `Group` 。|
|modifiedDateTime|DateTimeOffset|上次更新计划的时间。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。|
|principalId|字符串| 要授予合格工作分配的主体的标识符。 可以是组或用户。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。<br> 支持 `$filter`（`eq`）。|
|roleDefinitionId|字符串|分配所针对的 unifiedRoleDefinition 的标识符。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。<br> 支持 `$filter`（`eq`）。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|符合条件的请求的计划角色分配对象。|
|status|字符串|的状态 `roleEligibilitySchedule` 。 它可以包含与状态相关的消息，如 `Provisioned` `Revoked` `Pending Provisioning` 、、 和 `Pending Approval` 。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。<br> 支持 `$filter`（`eq`）。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|将弃用。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|appScope|[appScope](../resources/appscope.md)|只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。 包含实体。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|引用作为合格分配范围的目录对象的属性。 提供，以便调用方可以使用 同时获取符合条件 `$expand` 角色分配。 只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principal|[directoryObject](../resources/directoryobject.md)|引用通过请求获取符合条件的角色分配的属性。 提供此权限，以便调用方可以在获取符合条件的服务的同时使用 `$expand` 角色分配。 只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
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

