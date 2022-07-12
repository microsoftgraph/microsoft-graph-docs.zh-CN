---
title: 存储资源类型
description: 表示分类术语存储。
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: f1b38c9fb826ce430614d44a7b41ed1712523481
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735934"
---
# <a name="store-resource-type"></a>存储资源类型

命名空间：microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示分类术语存储。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明
|:---|:---|:---
|[List groups](../api/termstore-list-groups.md)|[microsoft.graph.termStore.group](../resources/termstore-group.md) 集合| 从术语存储对象中获取可用的组。|
|[获取存储](../api/termstore-store-get.md) | [microsoft.graph.termStore.store](../resources/termstore-store.md) | 读取术语库对象的属性和关系。
|[更新存储](../api/termstore-store-update.md) | [microsoft.graph.termStore.store](../resources/termstore-store.md) | 更新术语库对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明
|:---|:---|:---
|defaultLanguageTag | String | 术语存储的默认语言。
|id|String | 术语存储的唯一标识符。 只读。
|languageTags | String collection | 术语存储的语言列表。

## <a name="relationships"></a>关系
|关系|类型|说明
|:---|:---|:---
|groups |[microsoft.graph.termStore.group](../resources/termstore-group.md) 集合 | 术语存储中可用的所有组的集合。
|集 | [microsoft.graph.termStore.set](../resources/termstore-set.md) 集合 | 术语存储中可用的所有集的集合。


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.store",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.store",
  "id": "String (identifier)",
  "defaultLanguageTag": "String",
  "languageTags": [
    "String"
  ]  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "TermStore is the top-level entity used for managing taxonomy for a client",
  "keywords": "termStore,facet,resource",
  "section": "documentation",
  "tocPath": "TermStore",
  "tocBookmarks": {
    "Resources/termStore.store": "#"
  },
  "suppressions": []
}
-->



