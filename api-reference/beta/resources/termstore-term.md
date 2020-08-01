---
title: 术语资源类型
description: 定义术语库中的术语实体。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 77f907ee80c0710e33771efb33c3a3eee893f2ed
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539232"
---
# <a name="term-resource-type"></a>术语资源类型

命名空间： termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表术语[库]中使用的术语。 术语可用于表示一个对象，该对象随后可用作标记 conent 的元数据。 可以在[集合]中以分层方式组织多个术语。

继承自[entity](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出子项](../api/termstore-term-list-children.md)|[Microsoft termStore](../resources/termstore-term.md)集合|在术语[库]中获取术语的第一级子级。|
|[列表关系](../api/termstore-term-list-relations.md)|[termStore](../resources/termstore-relation.md)集合的关系|获取术语[库]中术语的关系。|
|[创建关系](../api/termstore-relation-post.md)|[microsoft termStore](../resources/termstore-relation.md)|为术语[库]中的术语或[集]创建新的关系。|
|[创建术语](../api/termstore-term-post.md)|[microsoft termStore](../resources/termstore-term.md)|在术语[库]中创建新的术语对象。|
|[获取术语](../api/termstore-term-get.md)|[microsoft termStore](../resources/termstore-term.md)|读取术语[库]中术语对象的属性和关系。|
|[更新术语](../api/termstore-term-update.md)|[microsoft termStore](../resources/termstore-term.md)|更新术语[库]中术语对象的属性。|
|[删除术语](../api/termstore-term-delete.md)|无|删除术语[库]中的术语对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|创建术语的日期和时间。 只读|
|说明|[termStore](../resources/termstore-localizeddescription.md)集合的 localizedDescription|依赖于 languageTag 的术语的说明|
|id|String|术语的唯一标识符。 只读|
|标题|[termStore](../resources/termstore-localizedlabel.md)集合的 localizedLabel||术语的标签元数据|
|lastModifiedDateTime|DateTimeOffset|上次修改术语的日期和时间。 只读|
|properties|[键值](../resources/keyvalue.md)集合|术语的属性集合|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|children|[Microsoft termStore](../resources/termstore-term.md)集合|当前术语的子项|
|公关|[termStore](../resources/termstore-relation.md)集合的关系|指示与当前术语相关的术语，无论是固定的还是重用的|
|set|[termStore 设置](../resources/termstore-set.md)|在其中创建术语的[集]|

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

[microsoft]: ../resources/termstore-store.md
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
