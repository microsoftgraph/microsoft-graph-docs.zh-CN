---
title: relation 资源类型
description: 表示术语存储中的术语之间的关系。
author: vishriv
ms.localizationpriority: medium
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: 88276a66949a55f0ee953f556977a2380ed415d9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128030"
---
# <a name="relation-resource-type"></a>relation 资源类型

命名空间：microsoft.graph.termStore

表示术语库 [中的](../resources/termstore-term.md) 术语 [之间的关系]。 目前，支持两种类型的关系：**固定和****重复使用**。 

在固定关系中，术语可以固定在不同的术语集的不同术语下。 在固定关系中，术语的新子项只能添加到创建术语的术语集。 术语下的层次结构的任何更改将反映在固定术语的集内。 

重用关系类似于固定关系，只不过对重复使用的术语的更改可以从重复使用该术语的任何层次结构进行。 此外，对重复使用的术语进行层次结构更改不会反映在重复使用该术语的其他术语集。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出关系](../api/termstore-term-list-relations.md)|[microsoft.graph.termStore.relation](../resources/termstore-relation.md) 集合|检索 relation **对象的列表** 。|
|[创建关系](../api/termstore-relation-post.md)|[microsoft.graph.termStore.relation](../resources/termstore-relation.md)|创建新的 **relation** 对象。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|关系的 ID。|
|关系|microsoft.graph.termStore.relationType|关系的类型。 可取值为：`pin`、`reuse`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|fromTerm|[microsoft.graph.termStore.term](../resources/termstore-term.md)|关系的 [from] 术语。 定义关系的术语。 空 *值* 表示关系与集 [直接相关]。 |
|set|[microsoft.graph.termStore.set](../resources/termstore-set.md)|[关系]相关的集。|
|toTerm|[microsoft.graph.termStore.term](../resources/termstore-term.md)|关系的 [to] 术语。 定义关系的术语。|

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
[term]: ../resources/termstore-term.md
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


