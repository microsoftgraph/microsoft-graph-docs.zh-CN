---
title: 关系资源类型
description: 表示术语存储中的术语之间的关系。
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 18753cf6cb246eea25f9a497ebebc197ac23cb93
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732658"
---
# <a name="relation-resource-type"></a>关系资源类型

命名空间：microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示术语[存储]中的[术语](../resources/termstore-term.md)之间的关系。 目前支持两种类型的关系：固定和重复使用。 

在固定关系中，可以将术语固定在其他术语集中的不同术语下。 在固定关系中，只能在创建术语的术语集中添加术语的新子级。 术语下层次结构中的任何更改都反映在固定术语的集内。 

重复使用关系类似于固定关系，只是可以从重复使用该术语的任何层次结构对重复使用的术语进行更改。 此外，对重复使用的术语所做的层次结构更改不会反映在重复使用该术语的其他术语集中。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出关系](../api/termstore-term-list-relations.md)|[microsoft.graph.termstore.relation](../resources/termstore-relation.md) 集合|检索 **关系** 对象的列表。|
|[创建关系](../api/termstore-relation-post.md)|[microsoft.graph.termstore.relation](../resources/termstore-relation.md)|创建新的 **关系** 对象。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|关系的 ID。|
|关系|String|关系的类型。 可取值为：`pin`、`reuse`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|fromTerm|[microsoft.graph.termStore.term](../resources/termstore-term.md)|关系的从 [术语] 。 定义关系的术语。 null 值表示关系与 [集]直接相关。 |
|set|[microsoft.graph.termStore.set](../resources/termstore-set.md)|关系相关的 [集] 。|
|toTerm|[microsoft.graph.termStore.term](../resources/termstore-term.md)|关系的 [字词] 。 定义关系的术语。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.relation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "id": "String (identifier)",
  "relationship": "String"
}
```

[microsoft.graph.termStore.term]: termstore-term.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.relations]: termstore-relation.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[商店]: ../resources/termstore-store.md
[术语]: ../resources/termstore-term.md
[set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "TermRelation is the entity for mapping relations between different terms",
  "keywords": "termRelation,facet,resource",
  "section": "documentation",
  "tocPath": "TermRelation",
  "tocBookmarks": {
    "Resources/termStore.relation&quot;: &quot;#"
  },
  "suppressions": []
}
-->


