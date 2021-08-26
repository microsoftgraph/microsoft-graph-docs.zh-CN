---
title: localizedLabel 资源类型
description: 表示术语存储中术语的标签。
author: vishriv
localization_priority: Normal
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: da9e3fb1a3cff98823771c1c99db052b92ba7e38
ms.sourcegitcommit: 998c63e6290cfb5ad4a6bd3eb3e249d282f962a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/26/2021
ms.locfileid: "58533720"
---
# <a name="localizedlabel-resource-type"></a>localizedLabel 资源类型

命名空间：microsoft.graph.termStore

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


