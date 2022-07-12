---
title: 设置资源类型
description: 表示术语存储中的一个集。
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: b9374c1d41ef713b6edfeb3dd0ec4614b5562c2a
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734226"
---
# <a name="set-resource-type"></a>设置资源类型

命名空间：microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示术语 [存储]中使用的集。 该集表示包含分层术语集合的单元。 [组]可以包含多个集。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列表集](../api/termstore-group-list-sets.md)|collection [microsoft.graph.termStore.set] | 返回术语[存储][组]中包含的集的列表 |
|[创建集](../api/termstore-set-post.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)|在术语 [存储]中创建新的 set 对象。|
|[创建术语](../api/termstore-term-post.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|在术语[存储]中创建新的[术语]对象。|
|[获取集](../api/termstore-set-get.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)| 获取术语 [存储]中的 set 对象。|
|[获取术语](../api/termstore-term-get.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)| 获取术语[存储]中的[术语]对象。|
|[更新集](../api/termstore-set-update.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)|更新术语 [存储]中 set 对象的属性。|
|[删除集](../api/termstore-set-delete.md)|None|删除术语 [存储]中的 set 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|创建集的日期和时间。 只读。|
|说明|字符串|说明，提供有关术语使用情况的详细信息。|
|id|String|唯一标识符。 只读。|
|localizedNames|[microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md) 集合|每个 languageTag 的集的名称。|
|properties|[microsoft.graph.keyValue](../resources/keyvalue.md) 集合|集的自定义属性。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|children|[microsoft.graph.termStore.term](../resources/termstore-term.md) 集合|术语 [存储]中设置的子术语。|
|parentGroup|[microsoft.graph.termStore.group](../resources/termstore-group.md)|包含该集的父 [组] 。|
|关系|[microsoft.graph.termStore.relation](../resources/termstore-relation.md) 集合|指示已直接在集下固定或重复使用的术语。|
|条款|[microsoft.graph.termStore.term](../resources/termstore-term.md) 集合|集下的所有术语。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.set",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.set",
  "id": "String (identifier)",
  "localizedNames": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedName"
    }
  ],
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "properties": [
    {
      "@odata.type": "microsoft.graph.termStore.keyValue"
    }
  ]
}
```

[microsoft.graph.termStore.term]: termstore-term.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[microsoft.graph.termStore.store]: termstore-store.md
[microsoft.graph.termStore.localizedName]: termstore-localizedname.md
[商店]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
[术语]: ../resources/termstore-term.md


<!--
{
  "type": "#page.annotation",
  "description": "TermSet is the entity containing the particular taxonomy for a tenant",
  "keywords": "termSet,facet,resource",
  "section": "documentation",
  "tocPath": "TermSet",
  "tocBookmarks": {
    "Resources/termStore.set&quot;: &quot;#"
  },
  "suppressions": []
}
-->


