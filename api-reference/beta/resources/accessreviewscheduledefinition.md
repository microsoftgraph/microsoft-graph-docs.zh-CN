---
title: accessReviewScheduleDefinition 资源类型
description: 表示访问评审或访问评审系列。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e4820cf85d3160c04372df79072b4b40708ef868
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443174"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>accessReviewScheduleDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示 Azure AD 访问评审 [的计划](accessreviewsv2-root.md)。 

accessReviewScheduleDefinition 包含 [accessReviewInstance](accessreviewinstance.md) 对象的列表。 计划定义的每次重复都会创建一个实例。 实例还表示要审阅的每个唯一组。 如果计划定义检查多个组，则每个组将具有每个重复周期的唯一实例。 对于一次检查，每个组将仅创建一个实例。

## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 集合 | 列出每个 accessReviewScheduleDefinition。 在列表中不包括关联的 accessReviewInstance 实例。 |
|[获取 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 获取具有指定 ID 的 accessReviewScheduleDefinition。 |
|[创建 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-create.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 创建新的 accessReviewScheduleDefinition。 |
|[删除 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | 无。 | 删除具有指定标识符的 accessReviewScheduleDefinition。 |
|[更新 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | 无。 | 使用指定的标识符更新 accessReviewScheduleDefinition 的属性。 |

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :------------------| :-------------- | :---------- |
| id | String | 访问评审的功能分配的唯一标识符。|
| displayName | String   | 访问评审系列的名称。 创建时为必需项。 |
| createdDateTime  |DateTimeOffset  | 创建审阅系列的日期/时间。 |
| lastModifiedDateTime | DateTimeOffset   | 上次修改审阅系列的日期/时间。|
| 状态  |string   | 此只读字段指定 accessReview 的状态。 典型状态包括 `Initializing` 、 `NotStarted` `Starting` 、 、 、 `InProgress` `Completing` 和 `Completed` `AutoReviewing` `AutoReviewed` 。 |
| descriptionForAdmins  |string  |  评价创建者提供的用于向管理员提供更多评价上下文的说明。 |
| descriptionForReviewers |string | 审阅创建者提供的用于向审阅者提供更多审阅上下文的说明。 审阅者将在发送给其请求审阅的电子邮件中看到此说明。 |
| createdBy  |[userIdentity](../resources/useridentity.md)  | 创建此评价的用户。 |
| 范围  |[accessReviewScope](../resources/accessreviewscope.md)  | 定义已审阅用户的范围。 有关支持的范围，请参阅 [accessReviewScope](accessreviewscope.md)。 创建时为必需项。 |
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | 如果审阅所有 Microsoft 365 组的来宾用户，这将确定将审阅哪些组的范围。 每个组将成为访问评审系列的唯一 accessReviewInstance。  有关支持的范围，请参阅 [accessReviewScope](accessreviewscope.md)。 | 
| settings  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| 访问评审系列的设置，请参阅下面的类型定义。 |
| 审阅者   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此访问评审范围集合用于定义审阅者。 请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。 创建时为必需项。 |
| backupReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此审阅者作用域集合用于定义回退审阅者列表。 如果从指定的审阅者列表中找不到用户，将通知这些回退审阅者采取措施。 如果组所有者被指定为审阅者，但组所有者不存在，或者经理被指定为审阅者，但用户的经理不存在，则可能发生此情况。 请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。 |
| instances |集合 (microsoft.graph.accessReviewInstance) |  此访问评审系列的访问评审实例集。 不重复的访问评审将只有一个实例;否则，将存在每个重复周期的实例。 |

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| `instances`               |[accessReviewInstance](accessreviewinstance.md) 集合         | 如果是 `accessReviewScheduleDefinition` 定期访问评审，则实例表示每个重复周期。 不重复的审阅将只具有一个实例。 实例还表示正在审阅的每个唯一资源 `accessReviewScheduleDefinition` 。 如果审阅具有多个资源和多个实例，则每个资源将具有每个重复周期的唯一实例。 |

### <a name="supported-queries-for-accessreviewscheduledefinition"></a>accessReviewScheduleDefinition 支持的查询
以下是基于[accessReviewScope](accessreviewscope.md)的[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)上支持的查询。

|应用场景| 查询 |
|--|--|
| 列出每个组 (排除作用域为具有来宾用户的所有 `accessReviewScheduleDefinition` Microsoft 365 组)  | /beta/identityGovernance/accessReviews/definitions？$filter=contains (scope/query， '/groups')  |
| 列出特定组上的每个 (不包括作用域为具有来宾用户的所有 `accessReviewScheduleDefinition` Microsoft 365 组)  | /beta/identityGovernance/accessReviews/definitions？$filter=contains (scope/query， '/groups/{group id}')  |
| 列出 `accessReviewScheduleDefinition` 每个作用域为具有来宾用户的 Microsoft 365 组 | /beta/identityGovernance/accessReviews/definitions？$filter=contains (scope/query， './members')  |

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
