---
title: 术语资源类型
description: 定义术语存储中的术语实体。
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 0207c740d52f7e7401ed6c741cf8d9134ec47eb1
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730276"
---
# <a name="term-resource-type"></a>术语资源类型

命名空间：microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示术语 [存储]中使用的术语。 术语可用于表示一个对象，然后该对象可以用作标记内容的元数据。 可在 [集]内以分层方式组织多个术语。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出子项](../api/termstore-term-list-children.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md) 集合|获取术语存储中术语的第一级子 [级]。|
|[列出关系](../api/termstore-term-list-relations.md)|[microsoft.graph.termStore.relation](../resources/termstore-relation.md) 集合|获取术语 [存储]中术语的关系。|
|[创建关系](../api/termstore-relation-post.md)|[microsoft.graph.termStore.relation](../resources/termstore-relation.md)|在术语[存储]中为术语或[集]创建新关系。|
|[创建术语](../api/termstore-term-post.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|在术语 [存储]中创建新的术语对象。|
|[获取术语](../api/termstore-term-get.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|读取术语  [存储]中术语对象的属性和关系。|
|[更新术语](../api/termstore-term-update.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|更新术语 [库]中术语对象的属性。|
|[删除术语](../api/termstore-term-delete.md)|None|删除术语 [存储]中的术语对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|术语创建的日期和时间。 只读。|
|描述|[microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md) 集合|有关依赖于 languageTag 的术语的说明。|
|id|String|术语的唯一标识符。 只读。|
|标签|[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) 集合|术语的标签元数据。|
|lastModifiedDateTime|DateTimeOffset|上次修改术语的日期和时间。 只读。|
|properties|[microsoft.graph.keyValue](../resources/keyvalue.md) 集合|术语上的属性集合。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|children|[microsoft.graph.termStore.term](../resources/termstore-term.md) 集合|当前术语的子级。|
|关系|[microsoft.graph.termStore.relation](../resources/termstore-relation.md) 集合|以固定或重用方式指示与当前术语相关的术语。|
|set|[microsoft.graph.termStore.set](../resources/termstore-set.md)|在其中创建术语的 [集] 。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.term",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.term",
  "id": "String (identifier)",
  "labels": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedLabel"
    }
  ],
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "descriptions": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedDescription"
    }
  ],
  "properties": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ]
}
```

[商店]: ../resources/termstore-store.md
[set]: ../resources/termstore-set.md
[term]: ../resources/termstore-term.md
[group]: ../resources/termstore-group.md

<!--
{
  "type": "#page.annotation",
  "description": "Term is the entity used for tagging in termStore",
  "keywords": "term,facet,resource",
  "section": "documentation",
  "tocPath": "Terms",
  "tocBookmarks": {
    "Resources/termstore-term&quot;: &quot;#"
  },
  "suppressions": []
}
-->


