---
title: patternedRecurrence 资源类型
description: 定期模式和区域。
ms.localizationpriority: medium
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f87ffd54073a4e7f414cbcb6c48bf92755cc33cc
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2021
ms.locfileid: "61545250"
---
# <a name="patternedrecurrence-resource-type"></a>patternedRecurrence 资源类型

命名空间：microsoft.graph

定期模式和区域。 此共享对象用于定义访问评审、日历[事件](event.md)和访问包分配在Azure AD。 [](accessreviewscheduledefinition.md) [](accesspackageassignment.md)

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|模式|[recurrencePattern](recurrencepattern.md)|事件发生的频率。 <br/><br/> 对于访问评审： <li>不要为一次访问评审指定此属性。 <li> 仅 **支持 interval** **、dayOfMonth** 和 **type** (`weekly` `absoluteMonthly` ，) [recurrencePattern 的属性](recurrencepattern.md) 。|
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

