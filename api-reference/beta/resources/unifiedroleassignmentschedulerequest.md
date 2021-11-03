---
title: unifiedRoleAssignmentScheduleRequest 资源类型
description: 表示通过活动角色分配活动Azure AD Privileged Identity Management。
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 055119e6b49fee02e4d018b6e028e20a07a141eb
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696679"
---
# <a name="unifiedroleassignmentschedulerequest-resource-type"></a>unifiedRoleAssignmentScheduleRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通过活动角色分配活动Azure Active Directory (Azure AD) Privileged Identity Management。

**unifiedRoleAssignmentScheduleRequest** 是一种票证模型实体，用于管理目录中活动角色分配的生命周期。 它表示用户和管理员的意图或决策，还提供了实现重复性日程安排、审批入口等的灵活性，与直接公开 、 和 上的操作相比 `POST` `PUT` `DELETE` `unifiedRoleAssignmentSchedule` `unifiedRoleAssignmentInstance` 。

管理员可以使用 创建 `unifiedRoleAssignmentScheduleRequest` 具有或没有开始时间和结束时间的活动角色分配。 尽管管理员可以使用它创建一个请求，以激活由 [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md)角色分配符合条件的用户。

继承自 [请求](request.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleAssignmentScheduleRequests](../api/unifiedroleassignmentschedulerequest-list.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 集合|获取 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象及其属性的列表。|
|[创建 unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-post-unifiedroleassignmentschedulerequests.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|创建新的 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象。|
|[获取 unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-get.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|读取 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象的属性和关系。|
|[filterByCurrentUser](../api/unifiedroleassignmentschedulerequest-filterbycurrentuser.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 集合|获取与特定用户相关的 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象及其属性的列表。|
|[取消](../api/unifiedroleassignmentschedulerequest-cancel.md)|无|立即取消 [unifiedRoleAssignmentScheduleRequest，](../resources/unifiedroleassignmentschedulerequest.md) 并标记为在 30 天内删除|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|字符串|表示对项目执行的操作角色分配。 可能的值有： <ul><li>`AdminAssign`：供管理员向用户或组分配角色。</li><li>`AdminRemove`：供管理员从角色中删除用户或组。</li><li> `AdminUpdate`：供管理员更改现有角色分配。</li><li>`AdminExtend`：供管理员扩展即将过期的工作分配。</li><li>`AdminRenew`：供管理员续订已过期的工作分配。</li><li>`SelfActivate`：供用户激活其工作分配。</li><li>`SelfDeactivate`：供用户停用其活动分配。</li><li>`SelfExtend`：用户请求延长其过期分配。</li><li>`SelfRenew`：用户请求续订其已过期的工作分配。</li></ul>|
|approvalId|字符串|请求审批的标识符。 继承自 [请求](request.md)。|
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 应用程序作用域是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将作用域限制为特定目录对象，例如管理单元。|
|completedDateTime|DateTimeOffset|请求完成日期时间。 继承自 [请求](request.md)。|
|createdBy|[identitySet](identityset.md)|创建此请求的用户。 继承自 [请求](request.md)。|
|createdDateTime|DateTimeOffset|请求创建日期时间。 继承自 [请求](request.md)。|
|customData|String|用于定义请求的任何自定义数据的免费文本字段。 未使用。 继承自 [请求](request.md)。|
|directoryScopeId|字符串|表示工作分配范围的目录对象的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 目录范围是存储在目录中的多个应用程序可以理解的共享范围。 用于 `/` 租户范围范围。 使用 **appScopeId** 将作用域限制为仅应用程序。|
|id|字符串|unifiedRoleAssignmentScheduleRequest 的唯一标识符。 键，不可为 null，只读。|
|isValidationOnly|布尔值|确定调用是验证还是实际调用的布尔值。 仅在要检查激活是否受 MFA 等其他规则限制，然后再实际提交请求时设置此属性。|
|justification|字符串|创建请求时由用户和管理员提供的消息，说明为什么需要该请求。|
|principalId|字符串| 要向其中授予工作分配的主体的标识符。|
|roleDefinitionId|String|分配所针对的 unifiedRoleDefinition 的标识符。 只读。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|请求的计划角色分配对象。|
|status|String|请求的计划角色分配对象。 继承自 [请求](request.md)。|
|targetScheduleId|String|附加到工作分配的计划对象的标识符。|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|附加到请求的 ticketInfo 角色分配，其中包含票证编号和票证系统的详细信息。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|如果请求来自符合条件的管理员以激活角色，则此参数将显示该激活的相关符合条件的分配。|
|appScope|[appScope](../resources/appscope.md)|只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。 包含实体。|
|directoryScope|[directoryObject](../resources/directoryobject.md)|引用作为工作分配范围的目录对象的属性。 提供，以便调用方可以在获取目录对象的同时获取 `$expand` 角色分配。 只读。 |
|principal|[directoryObject](../resources/directoryobject.md)|引用通过请求获取角色分配的属性。 提供此权限，以便调用方可以使用 与获取 角色分配 `$expand` 同时使用。 只读。 |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|指示分配所针对的 roleDefinition 的属性。 提供，以便调用方可以在获取角色定义的同时使用 `$expand` 角色分配。 roleDefinition.Id 自动展开。|
|targetSchedule|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)| 指示符合条件的项目计划角色分配。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest",
  "baseType": "microsoft.graph.request",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleRequest",
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

