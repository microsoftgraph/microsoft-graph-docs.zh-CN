---
title: localizedDescription 资源类型
description: 表示用于描述术语存储中的术语的本地化说明。
author: vishriv
ms.localizationpriority: medium
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: 856b0632e0ed1d167d45be55437c4fee97d99e4e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084060"
---
# <a name="localizeddescription-resource-type"></a>localizedDescription 资源类型

命名空间：microsoft.graph.termStore

表示用于描述术语库中的 [术语] 的本地化 [说明]。


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
[term]: ../resources/termstore-term.md
[store]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedDescriptionFacet is the facet for containing the description of a set",
  "keywords": "termLocalizedDescriptionFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedDescriptionFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedDescription&quot;: &quot;#"
  },
  "suppressions": []
}
-->


