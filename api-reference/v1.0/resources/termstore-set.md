---
title: 设置资源类型
description: 表示术语库中的集。
author: vishriv
localization_priority: Normal
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: d56bc436dca1c645d7e5d24face75a9bf5acd957
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514885"
---
# <a name="set-resource-type"></a>设置资源类型

命名空间：microsoft.graph.termStore

表示术语库 中使用的 [集]。 该集合表示一个包含分层术语集合的单位。 一 [个] 组可以包含多个组。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表集](../api/termstore-group-list-sets.md)|集合 [microsoft.graph.termStore.set] | 返回包含在术语库的 [组] 内的集 [的列表]。 |
|[创建集](../api/termstore-set-post.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)|在术语库中创建新的 set [对象]。|
|[创建术语](../api/termstore-term-post.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|在术语 [存储] 中创建新的术语 [对象]。|
|[获取集](../api/termstore-set-get.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)| 获取术语存储中的 set [对象]。|
|[获取术语](../api/termstore-term-get.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)| 获取 [术语] 存储中的术语 [对象]。|
|[更新集](../api/termstore-set-update.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)|更新术语库 中的 set 对象 [的属性]。|
|[删除集](../api/termstore-set-delete.md)|无|删除术语库 中的 set [对象]。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|集的创建日期和时间。 只读。|
|说明|String|提供有关术语用法的详细信息的说明。|
|id|String|唯一标识符。 只读。|
|localizedNames|[microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md) 集合|每个 languageTag 的集名称。|
|properties|[microsoft.graph.keyValue](../resources/keyvalue.md) 集合|集合的自定义属性。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|children|[microsoft.graph.termStore.term](../resources/termstore-term.md) 集合|术语库 中的子术语 [集]。|
|parentGroup|[microsoft.graph.termStore.group](../resources/termstore-group.md)|包含 [集合] 的父组。|
|relations|[microsoft.graph.termStore.relation](../resources/termstore-relation.md) 集合|指示哪些术语已固定或直接在集合下重复使用。|
|terms|[microsoft.graph.termStore.term](../resources/termstore-term.md) 集合|集合下的所有术语。|

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
[store]: ../resources/termstore-store.md
[组]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
[term]: ../resources/termstore-term.md


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


