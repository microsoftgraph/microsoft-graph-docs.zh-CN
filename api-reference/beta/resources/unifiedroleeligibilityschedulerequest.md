---
title: unifiedRoleEligibilityScheduleRequest 资源类型
description: 表示通过 Azure AD Privileged Identity Management执行符合条件的角色分配操作的请求。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 82224699c7bbe80e9ec14e39494fd8a37c1d31be
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461350"
---
# <a name="unifiedroleeligibilityschedulerequest-resource-type"></a>unifiedRoleEligibilityScheduleRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通过 Azure AD Privileged Identity Management进行符合条件的角色分配的请求。

**unifiedRoleEligibilityScheduleRequest** 是一个票证建模实体，用于管理目录中符合条件的角色分配的生命周期。 它表示用户和管理员的意图或决策，也提供了实现定期计划、审批门等的灵活性，与直接公开`POST`相比，`PUT``DELETE`以及 **对 unifiedRoleEligibilitySchedule** 和 **unifiedRoleEligibilityInstance** 资源的操作。

管理员可以使用 **unifiedRoleEligibilityScheduleRequest'** 创建和/或更新符合条件的角色分配，无论是否开始和结束时间。 符合条件的管理员可以使用它来创建一个请求来扩展或续订其符合条件的分配。

继承自 [请求](request.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedRoleEligibilityScheduleRequests](../api/rbacapplication-list-roleeligibilityschedulerequests.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 集合|获取 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象及其属性的列表。|
|[创建 unifiedRoleEligibilityScheduleRequest](../api/rbacapplication-post-roleeligibilityschedulerequests.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|创建新的 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象。|
|[获取 unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-get.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|读取 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象的属性和关系。|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedulerequest-filterbycurrentuser.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 集合|获取 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象及其与特定用户相关的属性的列表。|
|[取消](../api/unifiedroleeligibilityschedulerequest-cancel.md)|无|立即取消 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) ，并在 30 天内将其标记为删除|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|String|表示角色资格分配的操作类型。 可能的值有： <ul><li>`AdminAssign`：让管理员将角色资格分配给用户或组的角色。</li><li>`AdminExtend`：让管理员延长即将过期的分配。</li><li>`AdminUpdate`：让管理员更改现有角色分配。</li><li>`AdminRenew`：让管理员续订过期的分配。</li><li>`AdminRemove`：让管理员从符合条件的角色中删除用户或组。</li><li>`UserAdd`：让用户激活其符合条件的分配。</li><li>`UserExtend`：用户请求延长其即将到期的合格分配。</li><li>`UserRemove`：让用户停用其活动符合条件的分配。</li><li>`UserRenew`：用户请求续订其过期的合格分配。</li></ul>|
|approvalId|字符串|请求批准的标识符。 继承自 [请求](request.md)。|
|appScopeId|String|分配范围特定于应用时特定于应用的范围的标识符。 分配的范围确定已授予主体访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。|
|completedDateTime|DateTimeOffset|请求完成日期时间。 继承自 [请求](request.md)。|
|createdBy|[identitySet](identityset.md)|创建此请求的用户。 继承自 [请求](request.md)。|
|createdDateTime|DateTimeOffset|请求创建日期时间。 继承自 [请求](request.md)。|
|customData|字符串|用于定义请求的任何自定义数据的免费文本字段。 未使用。 继承自 [请求](request.md)。|
|directoryScopeId|String|表示分配范围的目录对象的标识符。 分配的范围确定已授予主体访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。|
|id|字符串|unifiedRoleEligibilityScheduleRequest 的唯一标识符。 只读。|
|isValidationOnly|布尔值|一个布尔值，用于确定调用是验证还是实际调用。 仅当要在实际提交请求之前检查激活是否受 MFA 等其他规则约束时，才设置此属性。|
|理由|字符串|用户和管理员在创建有关为何需要它的请求时提供的消息。|
|principalId|字符串| 要向其授予分配的主体的标识符。 例如，用户或组。 对于组，必须将其分配给角色，即设置为`true`的组属性的 **isAssignableToRole**。|
|roleDefinitionId|字符串|工作分配所用于的 unifiedRoleDefinition 的标识符。 只读。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|角色分配请求的计划对象。|
|status|String|角色资格请求的计划对象。 继承自 [请求](request.md)。|
|targetScheduleId|String|资格分配有效的时间段。|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|附加到角色分配请求的票证号和票证系统的详细信息。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|当分配范围特定于应用时，具有特定于应用范围的详细信息的只读属性。 包含实体。|
|directoryScope|[directoryObject](../resources/directoryobject.md)|引用分配范围的目录对象的属性。 通过提供，调用方可以在获取角色分配的同时获取使用 `$expand` 目录对象。 只读。|
|主要|[directoryObject](../resources/directoryobject.md)|引用通过请求获取角色分配的主体的属性。 提供此功能，使调用方可以在获取角色分配的同时获取主体 `$expand` 。 只读。 |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|指示分配所用于的 roleDefinition 的属性。 提供此功能，使调用方可以在获取角色分配的同时获取 `$expand` 角色定义。 roleDefinition.Id 将自动展开。|
|targetSchedule|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)| 指示符合条件的角色分配的计划的属性。 |

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

