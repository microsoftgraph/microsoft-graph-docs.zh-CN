---
title: 存储资源类型
description: 表示分类术语库。
author: vishriv
localization_priority: Normal
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: 840e22fc3031787cbc550f0ee0e32d5e6243bed9
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514884"
---
# <a name="store-resource-type"></a>存储资源类型

命名空间：microsoft.graph.termStore

表示分类术语库。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List groups](../api/termstore-list-groups.md)|[microsoft.graph.termStore.group](../resources/termstore-group.md) 集合| 获取术语库对象中的可用组。|
|[获取应用商店](../api/termstore-store-get.md) | [microsoft.graph.termStore.store](../resources/termstore-store.md) | 读取术语库对象的属性和关系。|
|[更新存储](../api/termstore-store-update.md) | [microsoft.graph.termStore.store](../resources/termstore-store.md) | 更新术语库对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|defaultLanguageTag | String | 术语库的默认语言。|
|id|String | 术语库的唯一标识符。 只读。|
|languageTags | String collection | 术语库的语言列表。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groups |[microsoft.graph.termStore.group](../resources/termstore-group.md) 集合 | 术语存储中所有可用组的集合。|
|sets | [microsoft.graph.termStore.set](../resources/termstore-set.md) 集合 | 术语存储中所有可用集的集合。|


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



