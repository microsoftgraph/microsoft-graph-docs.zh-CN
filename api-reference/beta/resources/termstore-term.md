---
title: 术语资源类型
description: 定义术语存储中的术语实体。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5645b85a5d017fd05010e04e118853a904a78b6c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516176"
---
# <a name="term-resource-type"></a>术语资源类型

命名空间：microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示术语库中使用的 [术语]。 术语可用于表示一个对象，然后该对象可用作标记内容的元数据。 多个术语可以在一组内以分层方式 [组织]。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出子项](../api/termstore-term-list-children.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md) 集合|获取术语存储中术语的第一级 [子级]。|
|[列出关系](../api/termstore-term-list-relations.md)|[microsoft.graph.termStore.relation](../resources/termstore-relation.md) 集合|获取术语存储中术语 [的关系]。|
|[创建关系](../api/termstore-relation-post.md)|[microsoft.graph.termStore.relation](../resources/termstore-relation.md)|在术语存储中为 [术语或集] 创建新 [关系]。|
|[创建术语](../api/termstore-term-post.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|在术语存储中创建新的术语 [对象]。|
|[获取术语](../api/termstore-term-get.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|读取术语存储中术语对象  [的属性和关系]。|
|[更新术语](../api/termstore-term-update.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|更新术语存储中术语对象 [的属性]。|
|[删除术语](../api/termstore-term-delete.md)|无|删除术语存储中的术语 [对象]。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|术语创建日期和时间。 只读|
|说明|[microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md) 集合|有关依赖于 languageTag 的术语的说明|
|id|String|术语的唯一标识符。 只读|
|labels|[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) 集合|术语的标签元数据|
|lastModifiedDateTime|DateTimeOffset|上次修改术语的日期和时间。 只读|
|properties|[microsoft.graph.keyValue](../resources/keyvalue.md) 集合|术语的属性集合|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|children|[microsoft.graph.termStore.term](../resources/termstore-term.md) 集合|当前术语的子项|
|relations|[microsoft.graph.termStore.relation](../resources/termstore-relation.md) 集合|指示与当前术语相关的术语（固定或重复使用）|
|set|[microsoft.graph.termStore.set](../resources/termstore-set.md)|[创建]术语的集|

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

[store]: ../resources/termstore-store.md
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
    "Resources/termstore-term": "#"
  },
  "suppressions": []
}
-->


