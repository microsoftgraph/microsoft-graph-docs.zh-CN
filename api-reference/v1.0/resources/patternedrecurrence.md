---
title: patternedRecurrence 资源类型
description: 定期模式和区域。
ms.localizationpriority: medium
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 23a0e22fe44cac84f017446326beea052e3c067c
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133795"
---
# <a name="patternedrecurrence-resource-type"></a>patternedRecurrence 资源类型

命名空间：microsoft.graph

定期模式和区域。 此共享对象用于定义以下对象的重复周期：
+ [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象Azure AD访问评审 API
+ 日历 API 中[的事件](event.md)对象
+ PIM 中的 [unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) 和 [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) 对象
+ Azure AD权利管理中的 [accessPackageAssignment](accesspackageassignment.md) 对象。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|模式|[recurrencePattern](recurrencepattern.md)|事件发生的频率。 <br/><br/> 对于访问评审： <li>不要为一次性访问评审指定此属性。 <li> 仅支持 **interval**、 **dayOfMonth** 和 **类型** (`weekly`、 `absoluteMonthly` [recurrencePattern](recurrencepattern.md) 的) 属性。|
|range|[recurrenceRange](recurrencerange.md)|事件的持续时间。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedRecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

