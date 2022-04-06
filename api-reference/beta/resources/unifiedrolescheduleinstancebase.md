---
title: unifiedRoleScheduleInstanceBase 资源类型
description: 将统一角色计划实例与统角色分配角色资格计划实例组合在一起的统一角色计划实例的基属性
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 58fa78adf75381e3444d2be492077f7388e9ba9b
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510623"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>unifiedRoleScheduleInstanceBase 资源类型

命名空间：microsoft.graph

统一角色计划实例的基属性，它将统一角色分配和统一角色资格计划实例组合在一起。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 应用程序作用域是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将作用域限制为特定的目录对象，例如管理单元。 |
|directoryScopeId|字符串|表示工作分配范围的目录对象的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 用于 `/` 租户范围范围。 使用 **appScopeId** 将作用域限制为仅应用程序。 |
|id|String|unifiedRoleAssignmentScheduleInstance 的唯一标识符。 键，不可为 null，只读。|
|principalId|字符串|要向其中授予工作分配的主体的标识符。 可以是组或用户。 |
|roleDefinitionId|String|分配所针对的 unifiedRoleDefinition 的标识符。 只读。 <br> 支持 `$filter`（`eq`）。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。 包含实体。 |
|directoryScope|[directoryObject](../resources/directoryobject.md)|分配范围的目录对象。 启用目录对象的检索，同时 `$expand` 使用 获取角色分配。 只读。|
|principal|[directoryObject](../resources/directoryobject.md)|通过请求获取角色分配主体。 启用检索主体，同时 `$expand` 使用 获取角色分配。 只读。|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|工作分配的 roleDefinition。 启用检索角色定义，同时 `$expand` 使用 获取角色分配。 将自动 roleDefinition.Id 扩展该设置。|

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
