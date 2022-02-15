---
title: accessReviewScheduleDefinition 资源类型
description: 代表访问评审或访问评审系列。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a2ef3d4ccaaef05140ebc71f48825262cf34f956
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816047"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>accessReviewScheduleDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示对访问Azure AD[计划](accessreviewsv2-overview.md)。 

accessReviewScheduleDefinition 包含 [accessReviewInstance 对象](accessreviewinstance.md) 的列表。 每次重复执行计划定义时，将创建一个实例。 实例还表示要审阅的每个唯一资源。 如果计划定义检查多个资源 (包括多个组) ，则每个资源在每个重复周期中都有一个唯一实例。 对于一次评审，每个资源只创建一个实例。

## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 accessReviewScheduleDefinitions](../api/accessreviewset-list-definitions.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 集合 | 列出每个 accessReviewScheduleDefinition。 结果中不包括关联的 accessReviewInstance 对象。 |
|[获取 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 获取具有指定 ID 的 accessReviewScheduleDefinition **。** 结果中不包括关联的 accessReviewInstance 对象。 |
|[创建 accessReviewScheduleDefinition](../api/accessreviewset-post-definitions.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 创建新的 accessReviewScheduleDefinition。 |
|[删除 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | 无。 | 删除具有指定 ID 的 accessReviewScheduleDefinition **。** |
|[更新 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | 无。 | 使用指定 ID 更新 accessReviewScheduleDefinition **的属性**。 |
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 集合|检索调用用户作为一个或多个实例的审阅者的所有定义。|

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :------------------| :-------------- | :---------- |
| additionalNotificationRecipients   |[accessReviewNotificationRecipientItem](../resources/accessReviewNotificationRecipientItem.md) 集合| 定义要接收访问评审进度通知的其他用户或组成员的列表。 |
| createdBy  |[userIdentity](../resources/useridentity.md)  | 创建此评价的用户。 只读。 |
| createdDateTime  |DateTimeOffset  | 创建访问评审系列时时间戳。 支持 `$select`。 只读。 |
| descriptionForAdmins  |字符串  |  评价创建者提供的说明，用于向管理员提供评论的更多上下文。 支持 `$select`。 |
| descriptionForReviewers |String | 审阅创建者提供的说明，用于向审阅者提供审阅的更多上下文。 审阅者将在发送给他们请求审阅的电子邮件中看到此说明。 电子邮件通知最多支持 256 个字符。 支持 `$select`。 |
| displayName | String   | 访问评审系列的名称。 支持 `$select` 和 `$orderBy`。 创建时为必需项。 |
| fallbackReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此审阅者范围集合用于定义回退审阅者列表。 如果从指定的审阅者列表中找不到用户，将通知这些回退审阅者采取措施。 当组所有者指定为审阅者，但组所有者不存在时，或者将经理指定为审阅者但用户的经理不存在时，可能会发生这种情况。 请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。 替换 **backupReviewers**。 支持 `$select`。 <br/><br/>**注意：** 如果通过 **stageSettings** 属性分配回退审阅者，则忽略此属性的值。 |
| id | String | 访问评审的功能分配的唯一标识符。 支持 `$select`。 只读。|
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | 将审阅范围确定为来宾用户跨所有组访问Microsoft 365此属性是必需的，并确定Microsoft 365哪些组。 每个组将成为访问评审系列 **的唯一 accessReviewInstance** 。  有关支持的范围，请参阅 [accessReviewScope](accessreviewscope.md)。 支持 `$select`。 有关配置 instanceEnumerationScope 的选项示例，请参阅使用 Microsoft Graph [API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)。 |
| 实例 |[accessReviewInstance](../resources/accessreviewinstance.md) 集合|  此访问评审系列的访问评审实例集。 不重复的访问评审将只有一个实例;否则，每个重复周期都有一个实例。 |
| lastModifiedDateTime | DateTimeOffset   | 上次修改访问评审系列的时间戳。 支持 `$select`。 只读。|
| reviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此访问评审范围集合用于定义审阅者。 只有在将单个用户分配为审阅者时，审阅者属性才可更新。 创建时为必需项。 支持 `$select`。 有关分配审阅者的选项示例，请参阅使用 Microsoft Graph API 将审阅者分配给你的访问[Graph定义](/graph/accessreviews-reviewers-concept)。 <br/><br/>**注意：** 如果通过 **stageSettings** 属性分配审阅者，则忽略此属性的值。  |
| 范围  |[accessReviewScope](../resources/accessreviewscope.md)  | 定义将检查其访问权限的实体。 有关支持的范围，请参阅 [accessReviewScope](accessreviewscope.md)。 创建时为必需项。 仅 `$select` 支持 `$filter` (`contains` 和) 。 有关配置作用域的选项示例，请参阅使用 Microsoft Graph [API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)。 |
|stageSettings|[accessReviewStageSettings](../resources/accessreviewstagesettings.md) 集合| 仅需要多阶段访问评审才能定义阶段及其设置。 可以将每个审阅实例分解为最多三个连续阶段，其中每个阶段可以有一组不同的审阅者、回退审阅者和设置。 阶段将基于 **dependsOn 属性按顺序** 创建。 可选。  <br/><br/>定义此属性时，会使用该属性的设置，而不是 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象中的相应设置及其设置、审阅者和 **fallbackReviewers** 属性。 |
| settings  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| 访问评审系列的设置，请参阅下面的类型定义。 支持 `$select`。 创建时为必需项。 |
| 状态  |String   | 此只读字段指定访问评审的状态。 典型状态包括 、`Initializing`、`NotStarted`、`Starting`、`InProgress``Completing`、`Completed`、`AutoReviewing`和 `AutoReviewed`。  <br>仅 `$select`支持 `$orderby`、 (`$filter` `eq` 和) 。 只读。 |
| backupReviewers (弃)  |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此审阅者范围集合用于定义回退审阅者列表。 如果从指定的审阅者列表中找不到用户，将通知这些回退审阅者采取措施。 当组所有者指定为审阅者，但组所有者不存在时，或者将经理指定为审阅者但用户的经理不存在时，可能会发生这种情况。  支持 `$select`。 <br>**注意：** 此属性已被 **fallbackReviewers 取代**。 但是，指定 **backupReviewers** 或 **fallbackReviewers** 会自动向另一个属性填充相同的值。 |


## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| `instances`               |[accessReviewInstance](accessreviewinstance.md) 集合         | 如果 为 `accessReviewScheduleDefinition` 定期访问评审，则实例表示每个重复周期。 不重复的审阅将只具有一个实例。 实例还表示 中正在审阅的每个唯一资源 `accessReviewScheduleDefinition`。 如果审阅具有多个资源和多个实例，则每个资源将具有每个重复周期的唯一实例。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "descriptionForAdmins": "String",
  "descriptionForReviewers": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "fallbackReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "backupReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "instanceEnumerationScope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "stageSettings": [
    {
      "@odata.type": "microsoft.graph.accessReviewStageSettings"
    }
  ],
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
  },
  "additionalNotificationRecipients": [
    {
        "@odata.type": "microsoft.graph.accessReviewNotificationRecipientItem"
    }
  ]
}
```
