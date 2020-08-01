---
title: 设置资源类型
description: 代表术语库中的集合。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5e74e0a603d088c7964b13fad51018171642c6ec
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539159"
---
# <a name="set-resource-type"></a>设置资源类型

命名空间： termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表术语[库]中使用的集合。 该集合表示包含分层术语集合的单位。 一个[组]可以包含多个集。

继承自[entity](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表集](../api/termstore-group-list-sets.md)|[termStore 的]集合 | 返回术语[存储][组]中包含的集的列表 |
|[创建集](../api/termstore-set-post.md)|[termStore 设置](../resources/termstore-set.md)|在术语[库]中创建新的 set 对象。|
|[创建术语](../api/termstore-term-post.md)|[microsoft termStore](../resources/termstore-term.md)|在术语[库]中创建新的[术语]对象。|
|[Get set](../api/termstore-set-get.md)|[termStore 设置](../resources/termstore-set.md)| 在术语[库]中获取一个 set 对象。|
|[获取术语](../api/termstore-term-get.md)|[microsoft termStore](../resources/termstore-term.md)| 在术语[库]中获取[术语]对象。|
|[更新集](../api/termstore-set-update.md)|[termStore 设置](../resources/termstore-set.md)|更新术语[库]中的 set 对象的属性。|
|[删除集](../api/termstore-set-delete.md)|无|删除术语[库]中的 set 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|创建集的日期和时间。 只读。|
|说明|String|说明：提供有关术语用法的详细信息。|
|id|字符串|唯一标识符。 只读。|
|localizedNames|[termStore](../resources/termstore-localizedname.md)集合的 localizedName|每个 languageTag 的集的名称。|
|properties|[键值](../resources/keyvalue.md)集合|集的自定义属性。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|children|[Microsoft termStore](../resources/termstore-term.md)集合|术语[库]中设置的子术语。|
|parentGroup|[termStore 的组](../resources/termstore-group.md)|包含集的父[组]。|
|公关|[termStore](../resources/termstore-relation.md)集合的关系|指示已固定或直接在集合下重复使用的术语。|
|而言|[Microsoft termStore](../resources/termstore-term.md)集合|该集下的所有条件。|

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
[termStore 设置]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[microsoft.graph.termStore.store]: termstore-store.md
[microsoft.graph.termStore.localizedName]: termstore-localizedname.md
[microsoft]: ../resources/termstore-store.md
[组]: ../resources/termstore-group.md
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
    "Resources/termStore.set": "#"
  },
  "suppressions": []
}
-->
