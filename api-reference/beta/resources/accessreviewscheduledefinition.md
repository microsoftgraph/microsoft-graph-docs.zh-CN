---
title: accessReviewScheduleDefinition 资源类型
description: 代表访问评审或访问评审系列。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f8ee04dde7ee19d24be5de58237f08b4fb538e8c
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000830"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>accessReviewScheduleDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure AD [访问评审](accessreviewsv2-root.md)的日程安排。 

AccessReviewScheduleDefinition 包含 [accessReviewInstance](accessreviewinstance.md) 对象的列表。 计划定义的每个重复将创建一个实例。 实例还表示要审阅的每个唯一组。 如果计划定义检查多个组，每个组将为每个重复周期提供一个唯一的实例。 在一次性审核的情况下，每个组只会创建一个实例。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 集合 | 列出每个 accessReviewScheduleDefinition。 不包括列表中关联的 accessReviewInstance 实例。 |
|[获取 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 获取具有指定 id 的 accessReviewScheduleDefinition。 |
|[创建 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-create.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 创建新的 accessReviewScheduleDefinition。 |
|[删除 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | 无。 | 删除具有指定标识符的 accessReviewScheduleDefinition。 |
|[更新 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | 无。 | 使用指定的标识符更新 accessReviewScheduleDefinition 的属性。 |

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :------------------| :-------------- | :---------- |
| id | 字符串 | 用于访问评审的功能分配的唯一标识符。|
| displayName | 字符串   | 访问审阅系列的名称。 创建时为必需项。 |
| createdDateTime  |DateTimeOffset  | 创建审阅系列时的日期时间。 |
| lastModifiedDateTime | DateTimeOffset   | 上次修改审阅系列的日期时间。|
| 状态  |string   | 此只读字段指定 accessReview 的状态。 典型状态包括、、、、、、 `Initializing` `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` 和 `AutoReviewed` 。 |
| descriptionForAdmins  |string  |  由审阅创建者提供的说明，用于向管理员提供评审的更多上下文。 |
| descriptionForReviewers |string | 由审阅创建者提供的说明，用于向审阅者提供评审的更多上下文。 审阅者将在发送给他们的电子邮件中看到此说明，以请求他们进行审阅。 |
| createdBy  |[userIdentity](../resources/useridentity.md)  | 创建此评审的用户。 |
| 范围  |[accessReviewScope](../resources/accessreviewscope.md)  | 定义在组中审阅的用户的范围。 有关支持的作用域，请参阅 [accessReviewScope](accessreviewscope.md)。 创建时为必需项。 |
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | 在所有组评审的情况下，这将确定将检查哪些组的范围。 每个组将成为 access 审阅系列的唯一 accessReviewInstance。  有关支持的作用域，请参阅 [accessReviewScope](accessreviewscope.md)。 | 
| settings  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| Access 审阅系列的设置，请参阅下面的类型定义。 |
| 审批   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此访问审核作用域集用于定义谁是审阅者。 请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。 创建时为必需项。 |
| backupReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 这一组审阅者范围用于定义回退审阅者的列表。 如果在指定的审阅者列表中找不到用户，将会通知这些回退审阅者采取行动。 如果将组所有者指定为审阅者，但组所有者不存在，或将经理指定为审阅者但用户的经理不存在，则可能会出现此情况。 请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。 |
| 实例 |AccessReviewInstance) 的集合 (|  此访问评审系列的一组访问审核实例。 不重复的 Access 审阅将只有一个实例;否则，每个定期都将有一个实例。 |

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| `instances`               |[accessReviewInstance](accessreviewinstance.md) 集合         | 如果 `accessReviewScheduleDefinition` 是定期访问审核，则实例表示每个重复周期。 不重复的审阅将只有一个实例。 实例还表示中的 "查看" 下的每个唯一组 `accessReviewScheduleDefinition` 。 如果评审包含多个组和多个实例，则每个组都将具有每个重复的唯一实例。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "baseType": "",
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
