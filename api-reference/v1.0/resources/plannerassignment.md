---
title: plannerAssignment 资源类型
description: '**plannerAssignment** 资源表示向用户分配任务。 此类型在打开类型 plannerAssignments 中使用。'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: ea71ff05e4c649712e9e37566dc8cc71e3529c76
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044361"
---
# <a name="plannerassignment-resource-type"></a>plannerAssignment 资源类型

命名空间：microsoft.graph

**plannerAssignment** 资源表示向用户分配任务。 此类型在打开类型 [plannerAssignments 中使用](plannerassignments.md)。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignedBy|[identitySet](identityset.md)|执行任务分配的用户的标识，即分配者。|
|assignedDateTime|DateTimeOffset|分配任务的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|orderHint|String|用于对任务中的被分配者排序的提示。 格式的定义[如下所述。](planner-order-hint-format.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

