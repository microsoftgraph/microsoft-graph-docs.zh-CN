---
title: translationPreferences 资源类型
description: 表示用户的翻译设置首选项的资源。
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: b2e45f797709067e52f142c3de3f2be566b55201
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518145"
---
# <a name="translationpreferences-resource-type"></a>translationPreferences 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户的翻译语言替代列表中的条目。

## <a name="properties"></a>属性

|属性             |类型                                         |说明                                                            |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------|
|translationBehavior  |[translationBehavior](#translationbehavior-values)       |用户的首选翻译行为。<br><br>默认返回。 不可为空。 |                   
|languageOverrides    |[translationLanguageOverride](translationLanguageOverride.md) 集合                | 语言（如果有）的翻译替代行为。<br><br>默认情况下返回。|
|untranslatedLanguages|字符串集合| 用户不需要翻译的语言列表。 这从 [regionalAndLanguageSettings](regionalandlanguagesettings.md)中的 **authoringLanguages** 集合和 **translationPreferences** 中的 **languageOverrides** 集合计算。 该列表指定中性区域性值，其中包括没有任何国家/地区关联的语言代码。 例如，它会为中性法语区域性指定"fr"，而不是为法国法语指定"fr-FR"。 <br><br>默认情况下返回。 只读。| 

### <a name="translationbehavior-values"></a>translationBehavior 值

|成员 |说明                                                                  |
|-------|-----------------------------------------------------------------------------|
|Ask    |在翻译用户的消息/聊天/网页之前提示用户。|
|是    |自动翻译用户的消息/聊天/网页。           |
|否     |不要为用户提供提示或自动翻译。                 |



## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 定义。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.translationPreferences"
}-->

```json
{
    "translationBehavior": "string",
    "languageOverrides": [{"@odata.type":"microsoft.graph.translationLanguageOverride"}],
    "untranslatedLanguages": ["string"]
}
```
<!-- {
  "type": "#page.annotation",
  "description": translationPreferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


