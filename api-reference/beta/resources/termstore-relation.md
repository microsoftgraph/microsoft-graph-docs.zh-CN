---
title: 关系资源类型
description: 表示术语库中术语之间的关系。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 12d976a189b5ebc50e993b5c1203800e4afd68da
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289055"
---
# <a name="relation-resource-type"></a>关系资源类型

命名空间： termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示术语[库]中[术语](../resources/termstore-term.md)之间的关系。 目前支持两种类型的关系： pin 和重用。 

在 pin 关系中，术语可固定在不同术语集中的不同术语下。 在固定的关系中，只能在创建了术语的术语集中添加术语的新子项。 术语下的层次结构中的任何更改都将反映到固定术语的集中。 

重复使用关系类似于固定的关系，不同之处在于，可重复使用的术语的更改可从任何可重用术语的层次结构进行。 此外，对重复使用的术语的层次结构更改不会反映在重复使用该术语的其他术语集中。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表关系](../api/termstore-term-list-relations.md)|[termstore](../resources/termstore-relation.md) 集合的关系|检索 **关系** 对象的列表。|
|[创建关系](../api/termstore-relation-post.md)|[microsoft termstore](../resources/termstore-relation.md)|创建新的 **relation** 对象。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|关系的 ID。|
|关系|字符串|关系的类型。 可取值为：`pin`、`reuse`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|fromTerm|[microsoft termStore](../resources/termstore-term.md)|关系的 from [术语] 。 定义关系的术语。 空值指示关系是直接与 [集]。 |
|set|[termStore 设置](../resources/termstore-set.md)|与关系相关的 [集合] 。|
|toTerm|[microsoft termStore](../resources/termstore-term.md)|关系的 to [术语] 。 关系定义到的术语。|

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
[microsoft]: ../resources/termstore-store.md
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
    "Resources/termStore.relation": "#"
  },
  "suppressions": []
}
-->


