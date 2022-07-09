---
title: accessReviewScheduleDefinition 资源类型
description: 表示访问评审或访问评审系列。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8df583c8b1993ed7603e1ed56bfbc88e8749bc65
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698084"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>accessReviewScheduleDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示 Azure AD [访问评审](accessreviewsv2-overview.md)的计划。 

accessReviewScheduleDefinition 包含 [accessReviewInstance](accessreviewinstance.md) 对象的列表。 计划定义的每个重复周期都会创建一个实例。 实例还表示要审阅的每个唯一资源。 如果计划定义审查多个资源 (包括多个) 组，则每个资源的每个重复周期都有一个唯一实例。 对于一次性评审，每个资源只创建一个实例。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 accessReviewScheduleDefinitions](../api/accessreviewset-list-definitions.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 集合 | 列出每个 accessReviewScheduleDefinition。 结果中不包括关联的 accessReviewInstance 对象。 |
|[获取 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 获取具有指定 **ID** 的 accessReviewScheduleDefinition。结果中不包括关联的 accessReviewInstance 对象。 |
|[创建 accessReviewScheduleDefinition](../api/accessreviewset-post-definitions.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 创建新的 accessReviewScheduleDefinition。 |
|[删除 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | 无。 | 删除具有指定 **ID** 的 accessReviewScheduleDefinition。 |
|[更新 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | 无。 | 使用指定 ID 更新 accessReviewScheduleDefinition 的 **属性**。 |
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 集合|检索调用用户是一个或多个实例的审阅者的所有定义。|

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :------------------| :-------------- | :---------- |
| additionalNotificationRecipients   |[accessReviewNotificationRecipientItem](../resources/accessReviewNotificationRecipientItem.md) 集合| 定义要收到访问评审进度通知的其他用户或组成员的列表。 |
| createdBy  |[userIdentity](../resources/useridentity.md)  | 创建此评审的用户。 只读。 |
| createdDateTime  |DateTimeOffset  | 创建访问评审系列的时间戳。 支持 `$select`。 只读。 |
| descriptionForAdmins  |String  |  评审创建者提供的说明，用于向管理员提供更多评论上下文。 支持 `$select`。 |
| descriptionForReviewers |String | 评审创建者提供的说明，以便向审阅者提供更多评论上下文。 审阅者会在发送给他们的电子邮件中看到此说明，要求他们进行审阅。 电子邮件通知最多支持 256 个字符。 支持 `$select`。 |
| displayName | String   | 访问评审系列的名称。 支持 `$select` 和 `$orderBy`。 创建时为必需项。 |
| fallbackReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此审阅者范围集合用于定义回退审阅者列表。 如果未从指定的审阅者列表中找到任何用户，则会通知这些回退审阅者采取行动。 如果组所有者被指定为审阅者，但组所有者不存在，或者经理被指定为审阅者，但用户的管理器不存在，则可能会发生这种情况。 请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。 替换 **backupReviewers**。 支持 `$select`。 <br/><br/>**注意：** 如果通过 **stageSettings** 属性分配回退审阅者，则将忽略此属性的值。 |
| id | 字符串 | 访问评审的功能分配的唯一标识符。 支持 `$select`。 只读。|
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | 将评审范围限定到所有 Microsoft 365 组的来宾用户访问权限，并确定评审哪些 Microsoft 365 组时，需要此属性。 每个组将成为访问评审系列的唯一 **accessReviewInstance** 。  有关受支持的范围，请参阅 [accessReviewScope](accessreviewscope.md)。 支持 `$select`。 有关配置 instanceEnumerationScope 的选项示例，请参阅[使用 Microsoft 图形 API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)。 |
| 实例 |[accessReviewInstance](../resources/accessreviewinstance.md) 集合|  此访问评审系列的访问评审实例集。 不定期的访问评审将只有一个实例;否则，每个重复周期都有一个实例。 |
| lastModifiedDateTime | DateTimeOffset   | 上次修改访问评审系列的时间戳。 支持 `$select`。 只读。|
| 评论家   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此访问评审范围集合用于定义谁是审阅者。 仅当将单个用户分配为审阅者时，审阅者属性才可更新。 创建时为必需项。 支持 `$select`。 有关分配审阅者的选项示例，请参阅[使用 Microsoft 图形 API 将审阅者分配到访问评审定义](/graph/accessreviews-reviewers-concept)。 <br/><br/>**注意：** 如果通过 **stageSettings** 属性分配审阅者，则将忽略此属性的值。  |
| 范围  |[accessReviewScope](../resources/accessreviewscope.md)  | 定义对其访问权限进行评审的实体。 有关受支持的范围，请参阅 [accessReviewScope](accessreviewscope.md)。 创建时为必需项。 仅支持 `$select` 和 `$filter` (`contains`) 。 有关配置范围的选项示例，请参阅[使用 Microsoft 图形 API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)。 |
|stageSettings|[accessReviewStageSettings](../resources/accessreviewstagesettings.md) 集合| 只有多阶段访问评审才能定义阶段及其设置。 可以将每个审阅实例分解为最多三个顺序阶段，其中每个阶段可以有一组不同的审阅者、回退审阅者和设置。 阶段将根据 **dependsOn** 属性按顺序创建。 可选。  <br/><br/>定义此属性时，将使用其设置，而不是 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象及其 **设置**、 **审阅者** 和 **fallbackReviewers** 属性中的相应设置。 |
| settings  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| 访问评审系列的设置，请参阅下面的类型定义。 支持 `$select`。 创建时为必需项。 |
| status  |String   | 此只读字段指定访问评审的状态。 典型的状态包括`Initializing`，，，`Starting`，`InProgress`，，`Completed``Completing`，`AutoReviewing`和`AutoReviewed`。 `NotStarted`  <br>仅支持`$select`和 `$orderby``$filter` (`eq`) 。 只读。 |
| backupReviewers (已弃用)  |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此审阅者范围集合用于定义回退审阅者列表。 如果未从指定的审阅者列表中找到任何用户，则会通知这些回退审阅者采取行动。 如果组所有者被指定为审阅者，但组所有者不存在，或者经理被指定为审阅者，但用户的管理器不存在，则可能会发生这种情况。  支持 `$select`。 <br>**注意：** 此属性已替换为 **fallbackReviewers**。 但是，指定 **backupReviewers** 或 **fallbackReviewers** 会自动将相同的值填充到另一个属性。 |


## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| `instances`               |[accessReviewInstance](accessreviewinstance.md) 集合         | 如果是 `accessReviewScheduleDefinition` 定期访问评审，则实例表示每个重复访问。 不重复的审阅将完全有一个实例。 实例还表示正在审查的每个唯一 `accessReviewScheduleDefinition`资源。 如果评审具有多个资源和多个实例，则每个资源将为每个重复周期提供唯一实例。 |

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
