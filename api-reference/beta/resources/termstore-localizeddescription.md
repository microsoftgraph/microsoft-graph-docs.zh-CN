---
title: localizedDescription 资源类型
description: 表示用于描述术语库中的术语的本地化说明。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 738555750c22f3ffdd5fbd43c8b1849888e0a40f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973615"
---
# <a name="localizeddescription-resource-type"></a>localizedDescription 资源类型

命名空间： termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用于描述术语[库]中的[术语]的本地化说明。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|本地化语言中的说明。|
|languageTag|String|标签的语言标记。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedDescription"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedDescription",
  "description": "String",
  "languageTag": "String"
}
```

[microsoft.graph.termStore.term]: termStore-term.md
[microsoft.graph.termStore.store]: termStore-store.md
[术语]: ../resources/termstore-term.md
[microsoft]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedDescriptionFacet is the facet for containing the description of a set",
  "keywords": "termLocalizedDescriptionFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedDescriptionFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedDescription": "#"
  },
  "suppressions": []
}
-->


