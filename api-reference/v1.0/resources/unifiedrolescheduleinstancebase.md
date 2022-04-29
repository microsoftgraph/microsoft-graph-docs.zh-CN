---
title: unifiedRoleScheduleInstanceBase 资源类型
description: 公开 unifiedRoleAssignmentScheduleInstance 和 unifiedRoleEligibilityScheduleInstance 资源类型中使用的属性和关系的模板。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 241c0af15867d87775490e00bd0f098e13e9dd9a
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134088"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>unifiedRoleScheduleInstanceBase 资源类型

命名空间：microsoft.graph

公开 [unifiedRoleAssignmentScheduleInstance](unifiedroleassignmentscheduleinstance.md) 和 [unifiedRoleEligibilityScheduleInstance](unifiedroleeligibilityscheduleinstance.md) 资源类型中使用的属性和关系的模板。


继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods

无。 

<!--
|Method|Return type|Description|
|:---|:---|:---|
|[List unifiedRoleScheduleInstanceBases](../api/unifiedrolescheduleinstancebase-list.md)|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) collection|Get a list of the [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) objects and their properties.|
|[Get unifiedRoleScheduleInstanceBase](../api/unifiedrolescheduleinstancebase-get.md)|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Read the properties and relationships of an [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) object.|
|[Update unifiedRoleScheduleInstanceBase](../api/unifiedrolescheduleinstancebase-update.md)|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Update the properties of an [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) object.|
|[Delete unifiedRoleScheduleInstanceBase](../api/unifiedrolescheduleinstancebase-delete.md)|None|Deletes an [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) object.|
|[List appScope](../api/unifiedrolescheduleinstancebase-list-appscope.md)|[appScope](../resources/appscope.md) collection|Get the appScope resources from the appScope navigation property.|
|[Add appScope](../api/unifiedrolescheduleinstancebase-post-appscope.md)|[appScope](../resources/appscope.md)|Add appScope by posting to the appScope collection.|
|[List directoryScope](../api/unifiedrolescheduleinstancebase-list-directoryscope.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the directoryScope navigation property.|
|[Add directoryScope](../api/unifiedrolescheduleinstancebase-post-directoryscope.md)|[directoryObject](../resources/directoryobject.md)|Add directoryScope by posting to the directoryScope collection.|
|[List principal](../api/unifiedrolescheduleinstancebase-list-principal.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the principal navigation property.|
|[Add principal](../api/unifiedrolescheduleinstancebase-post-principal.md)|[directoryObject](../resources/directoryobject.md)|Add principal by posting to the principal collection.|
|[List unifiedRoleDefinition](../api/unifiedrolescheduleinstancebase-list-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection|Get the unifiedRoleDefinition resources from the roleDefinition navigation property.|
|[Add unifiedRoleDefinition](../api/unifiedrolescheduleinstancebase-post-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Add roleDefinition by posting to the roleDefinition collection.|
-->

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|分配或角色资格限定到应用时特定于应用的范围的标识符。 分配或角色资格的范围决定了为其授予主体访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。|
|directoryScopeId|String|表示分配或角色资格范围的目录对象的标识符。 分配或角色资格的范围决定了为其授予主体访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。|
|id|String|计划对象的唯一标识符。 继承自 [entity](../resources/entity.md)。|
|principalId|String|已授予角色分配或符合角色条件的主体的标识符。|
|roleDefinitionId|String|分配给主体或主体有资格的 [unifiedRoleDefinition](unifiedroledefinition.md) 对象的标识符。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|当分配或角色资格限定到应用时，具有特定于应用范围的详细信息的只读属性。 可为 NULL。|
|directoryScope|[directoryObject](../resources/directoryobject.md)|作为分配或角色资格范围的目录对象。 只读。|
|主要|[directoryObject](../resources/directoryobject.md)|通过请求获得角色分配或角色资格的主体。|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|通过 **roleDefinitionId** 属性引用的 roleDefinition 对象的详细信息。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleInstanceBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleScheduleInstanceBase",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String"
}
```

