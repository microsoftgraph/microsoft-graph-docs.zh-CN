---
title: unifiedRoleEligibilityScheduleRequest 资源类型
description: 表示通过 Azure AD 角色分配符合条件的操作Privileged Identity Management。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5058d77a14ec009f60d5c4d6f4c8ae29b46f393b
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334442"
---
# <a name="unifiedroleeligibilityschedulerequest-resource-type"></a>unifiedRoleEligibilityScheduleRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通过 Azure AD 角色分配符合条件的操作Privileged Identity Management。

`unifiedRoleEligibilityScheduleRequest` 是一个票证模型实体，用于管理目录中符合条件的角色分配的生命周期。 它表示用户和管理员的意图/决定，还提供了实现重复性日程安排、审批入口等的灵活性，与直接公开 、 和 上的操作相比 `POST` `PUT` `DELETE` `unifiedRoleEligibilitySchedule` `unifiedRoleEligibilityInstance` 。

管理员可以使用 创建和/或更新符合条件的角色分配，有/没有 `unifiedRoleEligibilityScheduleRequest` 开始时间和结束时间。 符合条件的管理员可使用它创建请求，以扩展或续订其符合条件的分配。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleEligibilityScheduleRequests](../api/unifiedroleeligibilityschedulerequest-list.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 集合|获取 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象及其属性的列表。|
|[创建 unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-post-unifiedroleeligibilityschedulerequests.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|创建新的 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象。|
|[获取 unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-get.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|读取 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象的属性和关系。|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedulerequest-filterbycurrentuser.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 集合|获取与特定用户相关的 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象及其属性的列表。|
|[取消](../api/unifiedroleeligibilityschedulerequest-cancel.md)|无|立即取消 [unifiedRoleEligibilityScheduleRequest，](../resources/unifiedroleeligibilityschedulerequest.md) 并标记为在 30 天内删除|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|String|表示对项目执行的操作角色分配。 值可以是 <ul><li>`AdminAdd`：管理员将用户/组分配给角色;</li><li>`UserAdd`：用户激活符合条件的分配;</li><li> `AdminUpdate`：管理员更改现有角色分配</li><li>`AdminRemove`：管理员从角色中删除用户/组;<li>`UserRemove`：用户停用活动分配;<li>`UserExtend`：用户请求延长其过期分配;</li><li>`AdminExtend`：管理员扩展即将过期的工作分配。</li><li>`UserRenew`：用户请求续订其已过期的工作分配;</li><li>`AdminRenew`：管理员扩展即将过期的工作分配。</li></ul>|
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 对租户范围范围使用"/"。 应用程序作用域是仅由此应用程序定义和理解的范围。|
|directoryScopeId|String|表示工作分配范围的目录对象的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 应用程序作用域是仅由此应用程序定义和理解的范围。|
|id|String|unifiedRoleEligibilityScheduleRequest 的唯一标识符。|
|isValidationOnly|布尔|确定调用是验证还是实际调用的布尔值。 仅在要检查激活是否受 MFA 等其他规则限制，然后再实际提交请求时设置此属性。|
|justification|String|创建请求时由用户和管理员提供的消息，说明为什么需要该请求。|
|principalId|String| 要授予分配的主体的 Objectid。|
|roleDefinitionId|String|分配所针对的 unifiedRoleDefinition 的 ID。 只读。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|请求的计划角色分配对象。|
|targetScheduleId|String|附加到工作分配的计划对象的 ID。|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|附加到请求的 ticketInfo 角色分配，其中包含票证编号和票证系统的详细信息。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。 包含实体。|
|directoryScope|[directoryObject](../resources/directoryobject.md)|引用作为工作分配范围的目录对象的属性。 提供，以便调用方可以在获取目录对象的同时使用 `$expand` 角色分配。 只读。|
|principal|[directoryObject](../resources/directoryobject.md)|引用通过请求获取角色分配主体的属性。 提供此权限，以便调用方可以使用 与获取 角色分配 同时 `$expand` 使用。 只读。 |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|指示分配所针对的 roleDefinition 的属性。 提供，以便调用方可以在获取角色定义的同时使用 `$expand` 角色分配。 roleDefinition.Id 自动展开|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```

