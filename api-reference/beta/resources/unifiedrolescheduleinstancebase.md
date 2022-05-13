---
title: unifiedRoleScheduleInstanceBase 资源类型
description: 统一角色分配计划实例和统一角色资格计划实例的统一角色计划实例的基属性
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 78da74c6a867d6beed5dada2576d6248fc68ef37
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399444"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>unifiedRoleScheduleInstanceBase 资源类型

命名空间：microsoft.graph

统一角色计划实例的基属性，该实例结合了统一的角色分配计划实例和统一的角色资格计划实例。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|字符串|分配范围特定于应用时特定于应用的范围的标识符。 分配的范围确定已授予主体访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。 |
|directoryScopeId|String|表示分配范围的目录对象的标识符。 分配的范围确定已授予主体访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。 |
|id|字符串|unifiedRoleAssignmentScheduleInstance 的唯一标识符。 键，不可为 null，只读。|
|principalId|String|要向其授予分配的主体的标识符。 可以是组或用户。 |
|roleDefinitionId|String|工作分配所用于的 unifiedRoleDefinition 的标识符。 只读。 <br> 支持 `$filter`（`eq`）。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|当分配范围特定于应用时，具有特定于应用范围的详细信息的只读属性。 包含实体。 |
|directoryScope|[directoryObject](../resources/directoryobject.md)|作为分配范围的目录对象。 启用在获取角色分配的同时使用的 `$expand` 目录对象的检索。 只读。|
|主要|[directoryObject](../resources/directoryobject.md)|通过请求获取角色分配的主体。 启用在获取角色分配的同时使用的 `$expand` 主体检索。 只读。|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|分配的 roleDefinition。 在获取角色分配的同时，启用 `$expand` 角色定义的检索。 将自动扩展 roleDefinition.Id。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleInstanceBase",
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
