---
title: plannerChecklistItem 资源类型
description: '**plannerChecklistItem** 资源表示任务清单中的一个项目。 任务上的清单由 checklistItems 对象表示。'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: a8ba68b0b9e9bb3bf6979ad9eb3d498fe55b80ee
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113544"
---
# <a name="plannerchecklistitem-resource-type"></a>plannerChecklistItem 资源类型

命名空间：microsoft.graph


**plannerChecklistItem** 资源表示任务清单中的一个项目。 任务上的清单由 [checklistItems](plannerchecklistitems.md)对象表示。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|isChecked|Boolean|如果项目 `true` 已选中，则值为 ，否则 `false` 为 。|
|lastModifiedBy|[identitySet](identityset.md)| 只读。 上次修改的用户 ID。|
|lastModifiedDateTime|DateTimeOffset|只读。 上次修改的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|orderHint|String|用于设置清单中项目的相对顺序。 格式的定义[如下所述。](planner-order-hint-format.md)|
|title|String|清单项的标题|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

