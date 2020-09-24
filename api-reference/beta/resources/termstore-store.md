---
title: 存储资源类型
description: 表示分类术语库。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: de8b0c004da804a4d9a617eec20de22c51e98108
ms.sourcegitcommit: b7e82d0d64f640a09f5da76b38d8ed9f13684f95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2020
ms.locfileid: "48258424"
---
# <a name="store-resource-type"></a>存储资源类型

命名空间： termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示分类术语库。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明
|:---|:---|:---
|[List groups](../api/termstore-list-groups.md)|[Microsoft termStore](../resources/termstore-group.md) 集合| 将组从术语库对象中的提供中获取。|
|[获取存储区](../api/termstore-store-get.md) | [microsoft termStore](../resources/termstore-store.md) | 读取术语库对象的属性和关系。
|[更新存储](../api/termstore-store-update.md) | [microsoft termStore](../resources/termstore-store.md) | 更新术语库对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明
|:---|:---|:---
|defaultLanguageTag | 字符串 | 术语库的默认语言。
|id|字符串 | 术语库的唯一标识符。 只读。
|languageTags | String 集合 | 术语库的语言列表。

## <a name="relationships"></a>关系
|关系|类型|说明
|:---|:---|:---
|groups |[Microsoft termStore](../resources/termstore-group.md) 集合 | 术语库中可用的所有组的集合。
|下例 | [Microsoft termStore](../resources/termstore-set.md) 集合 | 术语库中可用的所有集的集合。


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



