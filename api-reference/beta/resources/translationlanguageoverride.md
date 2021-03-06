---
title: translationLanguageOverride 资源类型
description: 表示翻译语言替代列表中的条目的资源。
localization_priority: Normal
author: jasonbro
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 791908546c64cbb0ea7ee7434bece3dca5c894cc
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518146"
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


