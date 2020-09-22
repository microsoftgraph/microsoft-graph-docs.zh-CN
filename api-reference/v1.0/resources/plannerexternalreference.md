---
title: plannerExternalReference 资源类型
description: '**PlannerExternalReference**资源表示 (附件（如 FILE、URL) ）的引用的元数据。 它是 externalReferences 对象中的属性-值对的值。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 518a6b33212603a83bc0d2a99e51b8ab7ab10507
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037491"
---
# <a name="plannerexternalreference-resource-type"></a>plannerExternalReference 资源类型

命名空间：microsoft.graph

**PlannerExternalReference**资源表示 (附件（如 FILE、URL) ）的引用的元数据。 它是 [externalReferences 对象](plannerexternalreferences.md)中的属性-值对的值。



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|alias|String|用于描述引用的名称别名。|
|lastModifiedBy|[identitySet](identityset.md)|只读。 上次修改此 ID 的用户 ID。|
|lastModifiedDateTime|DateTimeOffset|只读。 上次修改的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|previewPriority|String|用于设置引用将显示为任务预览的相对优先级顺序。|
|type|String|用于描述引用的类型。 类型包括： `PowerPoint` 、 `Word` 、 `Excel` 、 `Other` 。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

