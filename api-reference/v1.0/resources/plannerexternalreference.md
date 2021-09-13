---
title: plannerExternalReference 资源类型
description: '**plannerExternalReference** 资源表示引用的元数据 (附件，如文件、URL) 。 它是 externalReferences 对象中属性值对的值。'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 225a4fb53875629eab093586193bf569d31693c4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019270"
---
# <a name="plannerexternalreference-resource-type"></a>plannerExternalReference 资源类型

命名空间：microsoft.graph

**plannerExternalReference** 资源表示引用的元数据 (附件，如文件、URL) 。 它是 [externalReferences](plannerexternalreferences.md)对象中的属性值对的值。



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|alias|String|用于描述引用的名称别名。|
|lastModifiedBy|[identitySet](identityset.md)|只读。 上次修改的用户 ID。|
|lastModifiedDateTime|DateTimeOffset|只读。 上次修改的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|previewPriority|String|用于设置引用在任务上显示为预览的相对优先级顺序。|
|type|String|用于描述引用的类型。 类型包括 `PowerPoint` `Word` `Excel` ：、、、。 `Other`|

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

