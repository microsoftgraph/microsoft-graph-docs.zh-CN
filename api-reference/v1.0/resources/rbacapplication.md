---
title: rbacApplication 资源类型
description: Microsoft 365基于角色的访问控制 (RBAC) 提供程序的角色定义和角色分配的容器
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9949ea7f219cee7e92f2c1406fe140469d67ad8c
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133781"
---
# <a name="rbacapplication-resource-type"></a>rbacApplication 资源类型

命名空间：microsoft.graph

Microsoft 365基于角色的访问控制 (RBAC) 提供程序的统一角色定义和角色分配的角色管理容器。 角色分配仅支持单个主体和单个范围。 目前 **，目录** 和 **entitlementManagement** 支持两个 RBAC 提供程序。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods

无

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的唯一标识符。 继承自 [entity](../resources/entity.md)。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|roleAssignments|[unifiedRoleAssignment](../resources/unifiedroleassignment.md) 集合| 向用户或组授予访问权限的资源。 |
|roleAssignmentScheduleInstances|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) 集合| 活动角色分配的实例。  |
|roleAssignmentScheduleRequests|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 集合| 通过 PIM 向主体请求活动角色分配。 |
|roleAssignmentSchedules|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) 集合|活动角色分配操作的计划。|
|roleDefinitions|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) 集合| 表示 RBAC 提供程序允许的角色以及分配给角色的权限的资源。 |
|roleEligibilityScheduleInstances|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) 集合|角色资格请求的实例。|
|roleEligibilityScheduleRequests|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 集合| 通过 PIM 请求主体的角色可视性。|
|roleEligibilitySchedules|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 集合|角色资格操作的计划。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.rbacApplication",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rbacApplication",
  "id": "String (identifier)"
}
```
