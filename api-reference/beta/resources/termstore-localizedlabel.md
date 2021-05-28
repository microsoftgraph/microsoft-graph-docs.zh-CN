---
title: localizedLabel 资源类型
description: 表示术语存储中术语的标签。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4d7de3c9567c20659af4c863d2cf1ac248beff6b
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696308"
---
# <a name="localizedlabel-resource-type"></a>localizedLabel 资源类型

命名空间：microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示术语存储 [中] 术语 [的标签]。

标识与给定术语关联的标签。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isDefault|Boolean|指示标签是否是默认标签。|
|languageTag|String|标签的语言标记。|
|name|String|标签的名称。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedLabel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedLabel",
  "name": "String",
  "isDefault": "Boolean",
  "languageTag": "String"
}
```


[microsoft.graph.termStore.term]: termstore-term.md
[microsoft.graph.termStore.localizedName]: termstore-localizedname.md
[microsoft.graph.termStore.store]: termstore-store.md
[term]: ../resources/termstore-term.md
[store]: ../resources/termstore-store.md


<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedLabelFacet is the facet for containing the label of a term",
  "keywords": "termLocalizedLabelFacet,facet,resource",
  "section": "documentation",
  "tocPath": "termstorelocalizedlabel",
  "tocBookmarks": {
    "Resources/termStore.termstorelocalizedlabel&quot;: &quot;#"
  },
  "suppressions": []
}
-->


