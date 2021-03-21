---
title: translationLanguageOverride 资源类型
description: 表示翻译语言替代列表中的条目的资源。
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: c9fa8d600ee3fb503446965d78491563c4ceae2e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954949"
---
# <a name="translationlanguageoverride-resource-type"></a>translationLanguageOverride 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示语言的任何翻译替代。

## <a name="properties"></a>属性

|属性             |类型                                         |说明                                                            |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------|
|languageTag          |String                                       |要应用替代的语言。<br><br>默认返回。 不可为空。       |                   
|translationBehavior  |[translationBehavior](translationPreferences.md#translationbehavior-values)        |语言（如果有）的翻译替代行为。<br><br>默认返回。 不可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 定义。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.translationLanguageOverride"
}-->

```json
{
    "languageTag": "string",
    "translationBehavior": "string"
}
```
<!-- {
  "type": "#page.annotation",
  "description": translationLanguageOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


