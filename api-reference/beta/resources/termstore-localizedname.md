---
title: localizedName 资源类型
description: 表示术语库中使用的本地化名称，用于标识本地化语言中的名称。
author: mohitpcad
ms.author: mopathak
localization_priority: Normal
ms.prod: sharepoint-taxonomy
doc_type: resourcePageType
ms.openlocfilehash: 5c9e6d4cd614c242e8f915fde71eadd07aa5de15
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973601"
---
# <a name="localizedname-resource-type"></a>localizedName 资源类型

命名空间： termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示术语 [库]中使用的本地化名称，用于标识本地化语言中的名称。 有关详细信息，请参阅 [localizedLabel]。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|languageTag|String|标签的语言标记。|
|name|String|本地化语言中的名称。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedName",
  "name": "String",
  "languageTag": "String"
}
```

[microsoft.graph.termStore.localizedLabel]: termstore-localizedlabel.md
[microsoft.graph.termstore.store]: termstore-store.md
[商店]: ../resources/termstore-store.md
[localizedLabel]: ../resources/termstore-localizedlabel.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedName is the facet for containing the name of termGroup",
  "keywords": "termLocalizedLNameFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedNameFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedName": "#"
  },
  "suppressions": []
}
-->


