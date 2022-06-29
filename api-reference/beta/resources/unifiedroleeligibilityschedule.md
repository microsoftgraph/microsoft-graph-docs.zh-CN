---
title: unifiedRoleEligibilitySchedule 资源类型
description: 表示通过 Azure AD Privileged Identity Management执行符合条件的角色分配操作的计划。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8e581e021df25547b276609d4075c162fcc5fed3
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439919"
---
# <a name="unifiedroleeligibilityschedule-resource-type"></a>unifiedRoleEligibilitySchedule 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户中角色资格的计划，用于实例化 [unifiedRoleEligibilityScheduleInstance](unifiedroleeligibilityscheduleinstance.md)。

继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleEligibilitySchedules](../api/rbacapplication-list-roleeligibilityschedules.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 集合|获取角色资格操作的计划。|
|[获取 unifiedRoleEligibilitySchedule](../api/unifiedroleeligibilityschedule-get.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|检索角色资格操作的计划。|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedule-filterbycurrentuser.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 集合|检索登录用户是其主体的角色可取性的计划。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|分配范围特定于应用时特定于应用的范围的标识符。 分配的范围确定已授予主体访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。 支持`$filter` (`eq`和`ne``null`值) 。|
|createdDateTime|DateTimeOffset|创建计划的时间。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。|
|createdUsing|String|创建此计划的 roleEligibilityScheduleRequest 的标识符。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。 支持`$filter` (`eq`和`ne``null`值) 。|
|directoryScopeId|String|表示分配范围的目录对象的标识符。 分配的范围确定已授予主体访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。 支持`$filter` (`eq`和`ne``null`值) 。|
|id|String|unifiedRoleEligibilitySchedule 的唯一标识符。 键，不可为 null，只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。 支持 `$filter`（`eq`）。|
|memberType|String|符合条件的分配的成员身份类型。 它可以是 `Inherited`， `Direct`或 `Group`. 支持 `$filter`（`eq`）。|
|modifiedDateTime|DateTimeOffset|上次更新计划的时间。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。|
|principalId|String| 要向其授予合格分配的主体的标识符。 可以是组或用户。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。<br> 支持 `$filter`（`eq`）。|
|roleDefinitionId|String|工作分配所用于的 unifiedRoleDefinition 的标识符。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。<br> 支持 `$filter`（`eq`）。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|符合条件的角色分配请求的计划对象。|
|状态|String|`roleEligibilitySchedule`的状态 。 它可以包括状态相关的消息，如 `Provisioned`， `Revoked`， `Pending Provisioning`和 `Pending Approval`。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)。<br> 支持 `$filter`（`eq`）。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|当分配范围特定于应用时，具有特定于应用范围的详细信息的只读属性。 包含实体。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|引用符合条件分配范围的目录对象的属性。 提供此功能，使调用方可以获取与获取符合条件的角色分配同时使用的 `$expand` 目录对象。 只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|主要|[directoryObject](../resources/directoryobject.md)|引用通过请求获取符合条件的角色分配的主体的属性。 提供此功能，使调用方可以在获取符合条件的角色分配的同时获取主体 `$expand` 。 只读。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|指示符合条件分配的 roleDefinition 的属性。 通过提供，调用方可以在获取符合条件的角色分配的同时获取 `$expand` 角色定义。 roleDefinition.Id 将自动展开。 继承自 [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

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

