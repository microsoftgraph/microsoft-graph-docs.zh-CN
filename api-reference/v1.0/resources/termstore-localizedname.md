---
title: localizedName 资源类型
description: 表示术语库中使用的本地化名称，该名称用本地化语言标识该名称。
author: vishriv
ms.localizationpriority: medium
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: e4ef39aff45906c70195a92dfe6c4cabe87385e8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128044"
---
# <a name="localizedname-resource-type"></a>localizedName 资源类型

命名空间：microsoft.graph.termStore

表示术语库 中使用的 [本地化名称，]该名称用本地化语言标识该名称。 有关详细信息，请参阅 [localizedLabel]。

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
    "Resources/termStore.termLocalizedName&quot;: &quot;#"
  },
  "suppressions": []
}
-->


