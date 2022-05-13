---
title: unifiedRoleAssignmentScheduleRequest 资源类型
description: 表示通过 Azure AD Privileged Identity Management执行活动角色分配操作的请求。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 14578e3f35403bc549dbb1fa64c1a104f059f13a
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397942"
---
# <a name="unifiedroleassignmentschedulerequest-resource-type"></a>unifiedRoleAssignmentScheduleRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通过 Azure Active Directory (Azure AD) Privileged Identity Management 执行活动角色分配操作的请求。

**unifiedRoleAssignmentScheduleRequest** 是一个票证建模实体，用于管理目录中活动角色分配的生命周期。 它表示用户和管理员的意图或决定，并提供了灵活性，使实施定期计划，审批门等，相比直接公开 `POST`， `PUT`和 `DELETE` 操作上 `unifiedRoleAssignmentSchedule` 和 `unifiedRoleAssignmentInstance`。

管理员可以使用或不使用 `unifiedRoleAssignmentScheduleRequest` 开始和结束时间创建活动角色分配。 虽然管理员可以使用它来创建一个请求，以激活由 [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) 表示的符合条件的角色分配。

继承自 [请求](request.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleAssignmentScheduleRequests](../api/unifiedroleassignmentschedulerequest-list.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 集合|获取 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象及其属性的列表。|
|[创建 unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-post-unifiedroleassignmentschedulerequests.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|创建新的 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象。|
|[获取 unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-get.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|读取 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象的属性和关系。|
|[filterByCurrentUser](../api/unifiedroleassignmentschedulerequest-filterbycurrentuser.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 集合|获取 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象及其与特定用户相关的属性的列表。|
|[取消](../api/unifiedroleassignmentschedulerequest-cancel.md)|无|立即取消 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) ，并在 30 天内将其标记为删除|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|字符串|表示角色分配上的操作类型。 可能的值有： <ul><li>`AdminAssign`：让管理员将角色分配给用户或组。</li><li>`AdminRemove`：让管理员从角色中删除用户或组。</li><li> `AdminUpdate`：让管理员更改现有角色分配。</li><li>`AdminExtend`：让管理员延长即将过期的分配。</li><li>`AdminRenew`：让管理员续订过期的分配。</li><li>`SelfActivate`：让用户激活其分配。</li><li>`SelfDeactivate`：让用户停用其活动分配。</li><li>`SelfExtend`：让用户请求延长其即将到期的分配。</li><li>`SelfRenew`：用户请求续订其过期的分配。</li></ul>|
|approvalId|String|请求批准的标识符。 继承自 [请求](request.md)。|
|appScopeId|字符串|分配范围特定于应用时特定于应用的范围的标识符。 分配的范围确定已授予主体访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。|
|completedDateTime|DateTimeOffset|请求完成日期时间。 继承自 [请求](request.md)。|
|createdBy|[identitySet](identityset.md)|创建此请求的用户。 继承自 [请求](request.md)。|
|createdDateTime|DateTimeOffset|请求创建日期时间。 继承自 [请求](request.md)。|
|customData|字符串|用于定义请求的任何自定义数据的免费文本字段。 未使用。 继承自 [请求](request.md)。|
|directoryScopeId|String|表示分配范围的目录对象的标识符。 分配的范围确定已授予主体访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。|
|id|String|unifiedRoleAssignmentScheduleRequest 的唯一标识符。 键，不可为 null，只读。|
|isValidationOnly|Boolean|一个布尔值，用于确定调用是验证还是实际调用。 仅当要在实际提交请求之前检查激活是否受 MFA 等其他规则约束时，才设置此属性。|
|理由|String|用户和管理员在创建有关为何需要它的请求时提供的消息。|
|principalId|String| 要向其授予分配的主体的标识符。|
|roleDefinitionId|String|工作分配所用于的 unifiedRoleDefinition 的标识符。 只读。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|角色分配请求的计划对象。|
|status|String|角色分配请求的计划对象。 继承自 [请求](request.md)。|
|targetScheduleId|String|附加到分配的计划对象的标识符。|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|附加到角色分配请求的 ticketInfo 对象，其中包括票证编号和票证系统的详细信息。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|如果请求来自符合条件的管理员来激活角色，则此参数将显示该激活的相关合格分配。|
|appScope|[appScope](../resources/appscope.md)|当分配范围特定于应用时，具有特定于应用范围的详细信息的只读属性。 包含实体。|
|directoryScope|[directoryObject](../resources/directoryobject.md)|引用分配范围的目录对象的属性。 通过提供，调用方可以在获取角色分配的同时获取使用 `$expand` 目录对象。 只读。 |
|主要|[directoryObject](../resources/directoryobject.md)|引用通过请求获取角色分配的主体的属性。 提供此功能，使调用方可以在获取角色分配的同时获取主体 `$expand` 。 只读。 |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|指示分配所用于的 roleDefinition 的属性。 提供此功能，使调用方可以在获取角色分配的同时获取 `$expand` 角色定义。 roleDefinition.Id 将自动展开。|
|targetSchedule|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)| 指示符合条件的角色分配的计划的属性。 |

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

