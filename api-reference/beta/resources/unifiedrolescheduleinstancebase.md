---
title: unifiedRoleScheduleInstanceBase 资源类型
description: 将统一角色计划实例与统角色分配角色资格计划实例组合在一起的统一角色计划实例的基属性
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4f22af61c513f8cc559948fb5519af5ac903d1d7c4ed650d2d11c6f5bf665282
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54238942"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>unifiedRoleScheduleInstanceBase 资源类型

命名空间：microsoft.graph

"将统一角色计划实例与统角色分配角色资格计划实例组合在一起的统一角色计划实例的基属性

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录范围是存储在目录中的多个应用程序可以理解的共享范围。 对租户范围范围使用"/"。 应用程序作用域是仅由此应用程序定义和理解的范围。|
|directoryScopeId|字符串|表示工作分配范围的目录对象的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录范围是存储在目录中的多个应用程序可以理解的共享范围。 应用程序作用域是仅由此应用程序定义和理解的范围。|
|id|String|unifiedRoleAssignmentScheduleInstance 的唯一标识符。 键，不可为 null，只读。|
|principalId|String|要授予分配的主体的 Objectid。|
|roleDefinitionId|String|分配所针对的 unifiedRoleDefinition 的 ID。 只读。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。 包含实体。 |
|directoryScope|[directoryObject](../resources/directoryobject.md)|分配范围的目录对象。 启用目录对象的检索，同时使用 获取 `$expand` 角色分配。 只读。|
|principal|[directoryObject](../resources/directoryobject.md)|通过请求获取角色分配主体。 启用检索主体，同时使用 获取 `$expand` 角色分配。 只读。|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|工作分配的 roleDefinition。 启用检索角色定义，同时使用 获取 `$expand` 角色分配。 自动 roleDefinition.Id 扩展该设置。|

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
