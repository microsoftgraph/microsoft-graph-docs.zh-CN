---
title: unifiedRoleAssignmentScheduleRequest 资源类型
description: 表示通过 PIM 向主体分配活动角色的请求。 角色分配可以在到期日期或未过期日期的情况下永久活动，也可以在激活符合条件的分配后暂时处于活动状态。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9c30760412982a00d6d0a45773f181f5e0cfbbc4
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134053"
---
# <a name="unifiedroleassignmentschedulerequest-resource-type"></a>unifiedRoleAssignmentScheduleRequest 资源类型

命名空间：microsoft.graph

表示通过 PIM 向主体分配活动角色的请求。 角色分配可以在到期日期或未过期日期的情况下永久活动，也可以在激活符合条件的分配后暂时处于活动状态。 继承自 [请求](../resources/request.md)。

有关可通过 **unifiedRoleAssignmentScheduleRequest** 资源类型定义的 PIM 方案的详细信息，请参阅 [通过特权标识管理 (PIM) API 进行角色管理的概述](privilegedidentitymanagementv3-overview.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleAssignmentScheduleRequests](../api/rbacapplication-list-roleassignmentschedulerequests.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 集合| 检索通过 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象进行的活动角色分配的请求。|
|[创建 unifiedRoleAssignmentScheduleRequest](../api/rbacapplication-post-roleassignmentschedulerequests.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|为活动和持久角色分配创建请求，或者激活、停用、扩展或续订符合条件的角色分配。|
|[获取 unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-get.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|检索通过 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象进行的活动角色分配的请求。|
|[取消](../api/unifiedroleassignmentschedulerequest-cancel.md)|无| 取消对活动角色分配的请求。 |
|[filterByCurrentUser](../api/unifiedroleassignmentschedulerequest-filterbycurrentuser.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 集合| 检索针对特定主体的活动角色分配的请求。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|unifiedRoleScheduleRequestActions|表示角色分配请求上的操作类型。 可取值包括：`adminAssign`、`adminUpdate`、`adminRemove`、`selfActivate`、`selfDeactivate`、`adminExtend`、`adminRenew`、`selfExtend`、`selfRenew`、`unknownFutureValue`。 <br/><ul><li>`adminAssign`：让管理员将角色分配给主体。</li><li>`adminRemove`：让管理员从角色中删除主体。</li><li> `adminUpdate`：让管理员更改现有角色分配。</li><li>`adminExtend`：让管理员延长即将过期的分配。</li><li>`adminRenew`：让管理员续订过期的分配。</li><li>`selfActivate`：让主体激活其分配。</li><li>`selfDeactivate`：让主体停用其活动分配。</li><li>`selfExtend`：让主体请求延长其即将过期的分配。</li><li>`selfRenew`：让主体请求续订其过期的分配。</li></ul>|
|approvalId|String|请求批准的标识符。 继承自 [请求](../resources/request.md)。|
|appScopeId|String|分配作用域为应用时特定于应用的范围的标识符。 分配的范围确定已授予主体访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。 支持`$filter` (`eq`和`ne``null`值) 。|
|completedDateTime|DateTimeOffset|请求完成日期时间。 继承自 [请求](../resources/request.md)。|
|createdBy|[identitySet](../resources/identityset.md)|创建此请求的主体。 继承自 [请求](../resources/request.md)。 只读。 支持`$filter` (`eq`和`ne``null`值) 。|
|createdDateTime|DateTimeOffset|请求创建日期时间。 继承自 [请求](../resources/request.md)。 只读。|
|customData|String|用于定义请求的任何自定义数据的免费文本字段。 未使用。 继承自 [请求](../resources/request.md)。|
|directoryScopeId|String|表示分配范围的目录对象的标识符。 分配的范围确定已授予主体访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。 支持`$filter` (`eq`和`ne``null`值) 。|
|id|String|**unifiedRoleAssignmentScheduleRequest** 对象的唯一标识符。 键，不可为 null，只读。 继承自 [entity](../resources/entity.md)。 支持 `$filter`（`eq`、`ne`）。|
|isValidationOnly|Boolean|确定调用是验证还是实际调用。 仅当要在实际提交请求之前检查激活是否受 MFA 等其他规则约束时，才设置此属性。|
|理由|String|用户和管理员创建 **unifiedRoleAssignmentScheduleRequest** 对象时提供的消息。|
|principalId|String|已授予分配的主体的标识符。 支持 `$filter`（`eq`、`ne`）。|
|roleDefinitionId|String|分配给主体的 [unifiedRoleDefinition](unifiedroledefinition.md) 对象的标识符。 支持 `$filter`（`eq`、`ne`）。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|角色分配的周期。 当前不支持定期计划。|
|状态|String|角色分配请求的状态。 继承自 [请求](../resources/request.md)。 只读。 支持 `$filter`（`eq`、`ne`）。|
|targetScheduleId|String|链接到分配请求的计划对象的标识符。 支持 `$filter`（`eq`、`ne`）。|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|链接到角色分配请求的票证详细信息，包括票证编号和票证系统的详细信息。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|如果请求来自符合条件的管理员来激活角色，则此参数将显示该激活的相关合格分配。 否则，它是 `null`. 支持 `$expand`。|
|appScope|[appScope](../resources/appscope.md)| 当分配范围限定到应用时，具有特定于应用范围的详细信息的只读属性。 可为 NULL。 支持 `$expand`。|
|directoryScope|[directoryObject](../resources/directoryobject.md)|作为分配范围的目录对象。 只读。 支持 `$expand`。|
|主要|[directoryObject](../resources/directoryobject.md)|通过请求获取角色分配的主体。 支持 `$expand`。|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)| 通过 **roleDefinitionId** 属性引用的 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象的详细信息。 支持 `$expand`。|
|targetSchedule|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|通过 **targetScheduleId** 属性引用的符合条件的角色分配的计划。 支持 `$expand`。|

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
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "approvalId": "String",
  "customData": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
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

