---
title: unifiedRoleScheduleBase 资源类型
description: 公开 unifiedRoleAssignmentSchedule 和 unifiedRoleEligibilitySchedule 资源类型中使用的属性和关系的模板。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9f778ac684ddb0ef9ae04647c4aa12193dff919c
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134079"
---
# <a name="unifiedroleschedulebase-resource-type"></a>unifiedRoleScheduleBase 资源类型

命名空间：microsoft.graph

公开 [unifiedRoleAssignmentSchedule](unifiedroleassignmentschedule.md) 和 [unifiedRoleEligibilitySchedule](unifiedroleeligibilityschedule.md) 资源类型中使用的属性和关系的模板。


继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods

无。

<!--
|Method|Return type|Description|
|:---|:---|:---|
|[List unifiedRoleScheduleBases](../api/unifiedroleschedulebase-list.md)|[unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) collection|Get a list of the [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) objects and their properties.|
|[Get unifiedRoleScheduleBase](../api/unifiedroleschedulebase-get.md)|[unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|Read the properties and relationships of an [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) object.|
|[Update unifiedRoleScheduleBase](../api/unifiedroleschedulebase-update.md)|[unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|Update the properties of an [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) object.|
|[Delete unifiedRoleScheduleBase](../api/unifiedroleschedulebase-delete.md)|None|Deletes an [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) object.|
|[List appScope](../api/unifiedroleschedulebase-list-appscope.md)|[appScope](../resources/appscope.md) collection|Get the appScope resources from the appScope navigation property.|
|[Add appScope](../api/unifiedroleschedulebase-post-appscope.md)|[appScope](../resources/appscope.md)|Add appScope by posting to the appScope collection.|
|[List directoryScope](../api/unifiedroleschedulebase-list-directoryscope.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the directoryScope navigation property.|
|[Add directoryScope](../api/unifiedroleschedulebase-post-directoryscope.md)|[directoryObject](../resources/directoryobject.md)|Add directoryScope by posting to the directoryScope collection.|
|[List principal](../api/unifiedroleschedulebase-list-principal.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the principal navigation property.|
|[Add principal](../api/unifiedroleschedulebase-post-principal.md)|[directoryObject](../resources/directoryobject.md)|Add principal by posting to the principal collection.|
|[List unifiedRoleDefinition](../api/unifiedroleschedulebase-list-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection|Get the unifiedRoleDefinition resources from the roleDefinition navigation property.|
|[Add unifiedRoleDefinition](../api/unifiedroleschedulebase-post-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Add roleDefinition by posting to the roleDefinition collection.|

-->

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|分配或资格限定到应用时特定于应用的范围的标识符。 分配或资格的范围决定了为其授予主体访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。|
|createdDateTime|DateTimeOffset|创建计划时。|
|createdUsing|String|创建此计划所通过的对象的标识符。|
|directoryScopeId|String|表示分配或资格范围的目录对象的标识符。 分配或资格的范围决定了为其授予主体访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。|
|id|String|计划对象的唯一标识符。 继承自 [entity](../resources/entity.md)。|
|modifiedDateTime|DateTimeOffset|上次修改计划的时间。|
|principalId|String|已授予角色分配或资格的主体的标识符。|
|roleDefinitionId|String|分配给主体或主体有资格的 [unifiedRoleDefinition](unifiedroledefinition.md) 对象的标识符。|
|状态|String|角色分配或资格请求的状态。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|当角色资格或分配范围限定到应用时，具有特定于应用范围的详细信息的只读属性。 可为 NULL。|
|directoryScope|[directoryObject](../resources/directoryobject.md)|作为角色资格或分配范围的目录对象。 只读。|
|主要|[directoryObject](../resources/directoryobject.md)|获取角色分配或有资格通过请求担任角色的主体。|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|通过 **roleDefinitionId** 属性引用的 roleDefinition 对象的详细信息。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleScheduleBase",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "createdUsing": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "status": "String"
}
```

