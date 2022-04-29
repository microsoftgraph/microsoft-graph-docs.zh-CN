---
title: unifiedRoleEligibilityScheduleInstance 资源类型
description: 表示租户中角色资格的实例。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 91ed173a26262fd6285df4d60518a80aded68b60
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134052"
---
# <a name="unifiedroleeligibilityscheduleinstance-resource-type"></a>unifiedRoleEligibilityScheduleInstance 资源类型

命名空间：microsoft.graph

表示租户中角色资格的实例。

继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleEligibilityScheduleInstances](../api/rbacapplication-list-roleeligibilityscheduleinstances.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 集合|获取角色可变性实例。|
|[获取 unifiedRoleEligibilityScheduleInstance](../api/unifiedroleeligibilityscheduleinstance-get.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|获取角色资格的实例。|
|[filterByCurrentUser](../api/unifiedroleeligibilityscheduleinstance-filterbycurrentuser.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 集合|获取调用主体的合格角色实例。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|当角色资格限定到应用时，特定于应用的范围的标识符。 角色资格的范围决定了向主体授予访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持`$filter` (`eq`和`ne``null`值) 。|
|directoryScopeId|String|表示角色资格范围的目录对象的标识符。 角色资格的范围决定了向主体授予访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持`$filter` (`eq`和`ne``null`值) 。|
|endDateTime|DateTimeOffset|计划实例的结束日期。|
|id|String|计划对象的唯一标识符。 继承自 [entity](../resources/entity.md)。|
|memberType|String|角色资格的继承方式。 它可以是 `Inherited`， `Direct`或 `Group`. 这进一步意味着 **unifiedRoleEligibilitySchedule** 是否可由调用方管理。 支持 `$filter`（`eq`、`ne`）。|
|principalId|String|符合角色条件的主体的标识符。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持 `$filter`（`eq`、`ne`）。 |
|roleDefinitionId|String|主体有资格的 [unifiedRoleDefinition](unifiedroledefinition.md) 对象的标识符。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持 `$filter`（`eq`、`ne`）。|
|roleEligibilityScheduleId|String|从中创建此实例的 **unifiedRoleEligibilitySchedule** 对象的标识符。|
|startDateTime|DateTimeOffset|当此实例启动时。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|当角色资格限定到应用时，具有特定于应用范围的详细信息的只读属性。 可为 NULL。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持 `$expand`。|
|directoryScope|[directoryObject](../resources/directoryobject.md)|作为角色资格范围的目录对象。 只读。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持 `$expand`。|
|主要|[directoryObject](../resources/directoryobject.md)|通过请求获得角色资格的主体。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持 `$expand`。|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|通过 **roleDefinitionId** 属性引用的 roleDefinition 对象的详细信息。 继承自 [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)。 支持 `$expand`。|

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

