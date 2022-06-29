---
title: unifiedRoleEligibilityScheduleRequest 资源类型
description: 表示通过 PIM 请求主体的角色资格。 角色资格可以是永久符合条件的，没有过期日期或暂时符合到期日期的条件。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9b5cab64c1784f3f2f63eaf22f2479e0cc5c7f7f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441032"
---
# <a name="unifiedroleeligibilityschedulerequest-resource-type"></a>unifiedRoleEligibilityScheduleRequest 资源类型

命名空间：microsoft.graph

表示通过 PIM 请求主体的角色资格。 角色资格可以是永久符合条件的，没有过期日期或暂时符合到期日期的条件。 继承自 [请求](../resources/request.md)。

有关可通过 **unifiedRoleEligibilityScheduleRequest** 资源类型定义的 PIM 方案的详细信息，请参阅 [通过特权标识管理 (PIM) API 进行角色管理的概述](privilegedidentitymanagementv3-overview.md)。

> [!NOTE]
> 若要激活符合条件的角色分配，请使用 [Create unifiedRoleAssignmentScheduleRequest](../api/rbacapplication-post-roleassignmentschedulerequests.md) API。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleEligibilityScheduleRequests](../api/rbacapplication-list-roleeligibilityschedulerequests.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 集合|检索通过 unifiedRoleEligibilityScheduleRequest 对象发出的主体的角色可选性请求。|
|[创建 unifiedRoleEligibilityScheduleRequest](../api/rbacapplication-post-roleeligibilityschedulerequests.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|通过 unifiedRoleEligibilityScheduleRequest 对象请求主体的角色资格。|
|[获取 unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-get.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|阅读通过 unifiedRoleEligibilityScheduleRequest 对象发出的角色资格请求请求的详细信息。|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedulerequest-filterbycurrentuser.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 集合|在 PIM 中，检索针对特定主体的角色可取性请求。 主体可以是 unifiedRoleEligibilityScheduleRequest 对象的创建者或审批者，也可以是角色资格的目标。|
|[取消](../api/unifiedroleeligibilityschedulerequest-cancel.md)|无|立即取消 **一个统一RoleEligibilityScheduleRequest** 对象，其状态为 `Granted` 并让系统在 30 天后自动删除已取消的请求。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|unifiedRoleScheduleRequestActions|表示角色资格请求的操作类型。 可取值包括：`adminAssign`、`adminUpdate`、`adminRemove`、`selfActivate`、`selfDeactivate`、`adminExtend`、`adminRenew`、`selfExtend`、`selfRenew`、`unknownFutureValue`。 <br/><ul><li>`adminAssign`：让管理员将符合条件的角色分配给主体。</li><li>`adminRemove`：让管理员从主体中删除符合条件的角色。</li><li> `adminUpdate`：让管理员更改现有角色可变性。</li><li>`adminExtend`：让管理员延长即将过期的角色可质性。</li><li>`adminRenew`：让管理员续订过期的可质性。</li><li>`selfActivate`：让用户激活其分配。</li><li>`selfDeactivate`：让用户停用其活动分配。</li><li>`selfExtend`：让用户请求延长其即将到期的分配。</li><li>`selfRenew`：用户请求续订其过期的分配。</li></ul>|
|approvalId|String|请求批准的标识符。 继承自 [请求](../resources/request.md)。|
|appScopeId|String|当角色资格限定到应用时，特定于应用的范围的标识符。 角色资格的范围决定了主体有资格访问的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。 支持`$filter` (`eq`和`ne``null`值) 。|
|completedDateTime|DateTimeOffset|请求完成日期时间。 继承自 [请求](../resources/request.md)。|
|createdBy|[identitySet](../resources/identityset.md)|创建此请求的主体。 继承自 [请求](../resources/request.md)。|
|createdDateTime|DateTimeOffset|请求创建日期时间。 继承自 [请求](../resources/request.md)。|
|customData|String|用于定义请求的任何自定义数据的免费文本字段。 未使用。 继承自 [请求](../resources/request.md)。|
|directoryScopeId|String|表示角色资格范围的目录对象的标识符。 角色资格的范围决定了向主体授予访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。 支持`$filter` (`eq`和`ne``null`值) 。|
|id|String|**unifiedRoleEligibilityScheduleRequest** 对象的唯一标识符。 键，不可为 null，只读。  继承自 [entity](../resources/entity.md)。|
|isValidationOnly|Boolean|确定调用是验证还是实际调用。 仅当要在实际提交请求之前检查激活是否受 MFA 等其他规则约束时，才设置此属性。|
|理由|String|用户和管理员在创建 **统一RoleEligibilityScheduleRequest** 对象时提供的消息。|
|principalId|String|已授予角色资格的主体的标识符。 支持 `$filter`（`eq`、`ne`）。|
|roleDefinitionId|String|分配给主体的 [unifiedRoleDefinition](unifiedroledefinition.md) 对象的标识符。 支持 `$filter`（`eq`、`ne`）。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|角色资格的期限。 当前不支持定期计划。|
|状态|String|角色资格请求的状态。 继承自 [请求](../resources/request.md)。 只读。 支持 `$filter`（`eq`、`ne`）。|
|targetScheduleId|String|链接到资格请求的计划对象的标识符。 支持 `$filter`（`eq`、`ne`）。|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|与角色资格请求链接的票证详细信息，包括票证编号和票证系统的详细信息。 可选。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|当角色资格限定到应用时，具有特定于应用范围的详细信息的只读属性。 可为 NULL。 支持 `$expand`。|
|directoryScope|[directoryObject](../resources/directoryobject.md)|作为角色资格范围的目录对象。 只读。 支持 `$expand`。|
|主要|[directoryObject](../resources/directoryobject.md)|通过请求获得角色资格的主体。 支持 `$expand`。|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|通过 **roleDefinitionId** 属性引用的 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象的详细信息。 支持 `$expand`。|
|targetSchedule|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|通过 **targetScheduleId** 属性引用的角色资格的计划。 支持 `$expand`。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest",
  "baseType": "microsoft.graph.request",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleEligibilityScheduleRequest",
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

