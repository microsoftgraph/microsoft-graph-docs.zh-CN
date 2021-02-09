---
title: accessReviewScheduleDefinition 资源类型
description: 表示访问评审或访问评审系列。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f95047602ec1a73549b6b5c4217e32890a5996e6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161157"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>accessReviewScheduleDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure AD 访问评审 [的计划](accessreviewsv2-root.md)。 

accessReviewScheduleDefinition 包含 [accessReviewInstance 对象](accessreviewinstance.md) 的列表。 计划定义的每次重复都会创建一个实例。 实例还表示要审阅的每个唯一组。 如果计划定义审阅多个组，则每个组将每个重复周期具有一个唯一实例。 对于一次评审，每个组只会创建一个实例。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 集合 | 列出每个 accessReviewScheduleDefinition。 在列表中不包括关联的 accessReviewInstance 实例。 |
|[获取 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 获取具有指定 ID 的 accessReviewScheduleDefinition。 |
|[创建 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-create.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 创建新的 accessReviewScheduleDefinition。 |
|[删除 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | 无。 | 删除具有指定标识符的 accessReviewScheduleDefinition。 |
|[更新 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | 无。 | 使用指定标识符更新 accessReviewScheduleDefinition 的属性。 |

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :------------------| :-------------- | :---------- |
| id | String | 访问评审的功能分配的唯一标识符。|
| displayName | String   | 访问评审系列的名称。 创建时为必需项。 |
| createdDateTime  |DateTimeOffset  | 创建审阅系列时的日期时间。 |
| lastModifiedDateTime | DateTimeOffset   | 上次修改审阅系列的日期/时间。|
| 状态  |string   | 此只读字段指定 accessReview 的状态。 典型状态包括 `Initializing` 、 `NotStarted` `Starting` 、 、 、 `InProgress` `Completing` 和 `Completed` `AutoReviewing` `AutoReviewed` 。 |
| descriptionForAdmins  |string  |  评价创建者提供的用于向管理员提供更多评价上下文的说明。 |
| descriptionForReviewers |string | 审阅创建者提供的用于向审阅者提供更多评论上下文的说明。 审阅者将在发送给他们请求审阅的电子邮件中看到此说明。 |
| createdBy  |[userIdentity](../resources/useridentity.md)  | 创建此评论的用户。 |
| 范围  |[accessReviewScope](../resources/accessreviewscope.md)  | 定义在组中审阅的用户范围。 有关支持的范围，请参阅 [accessReviewScope](accessreviewscope.md)。 创建时为必需项。 |
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | 对于所有组审阅，这将确定将审阅哪些组的范围。 每个组将成为访问评审系列的唯一 accessReviewInstance。  有关支持的范围，请参阅 [accessReviewScope](accessreviewscope.md)。 | 
| 设置  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| 访问评审系列的设置，请参阅下面的类型定义。 |
| 审阅者   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此访问评审范围集合用于定义审阅者。 请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。 创建时为必需项。 |
| backupReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此审阅者作用域集合用于定义回退审阅者列表。 如果从指定的审阅者列表中未找到用户，将通知这些回退审阅者采取措施。 当组所有者被指定为审阅者，但组所有者不存在，或者经理被指定为审阅者，但用户的经理不存在时，可能会发生这种情况。 请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。 |
| instances |集合 (microsoft.graph.accessReviewInstance) |  此访问评审系列的访问评审实例集。 不重复的访问评审将只有一个实例;否则，将针对每个重复周期提供一个实例。 |

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| `instances`               |[accessReviewInstance](accessreviewinstance.md) 集合         | 如果 `accessReviewScheduleDefinition` 定期访问评审，实例表示每个定期。 不重复的审阅将只具有一个实例。 实例还表示正在审阅的每个唯一组 `accessReviewScheduleDefinition` 。 如果审阅具有多个组和多个实例，则每个组将具有每个重复周期的唯一实例。 |

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
  "instanceEnumerationScope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScheduleDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
