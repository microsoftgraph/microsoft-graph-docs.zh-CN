---
title: regionalAndLanguageSettings 资源类型
description: 表示用户区域和语言首选项的资源
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: ba8666b78023b7345d936516fc3aec2b116520ad
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845678"
---
# <a name="regionalandlanguagesettings-resource-type"></a>regionalAndLanguageSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一种开放类型，表示用户对各种上下文中的语言的首选项，以及用于驱动默认日历的区域区域设置和格式以及日期和时间的格式设置。

## <a name="methods"></a>Methods

| 方法                                                 | 返回类型                                                   | 说明                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [获取](../api/regionalAndLanguageSettings-get.md)       | [regionalAndLanguageSettings](regionalAndLanguageSettings.md) | 读取**regionalAndLanguageSettings**对象的属性。                                       |
| [更新](../api/regionalandlanguagesettings-update.md) | [regionalAndLanguageSettings](regionalAndLanguageSettings.md) | 更新用户的**regionalAndLanguageSettings**对象的全部或属性子集。 |

## <a name="properties"></a>属性
| 属性                   | 类型                                                  | Description                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| defaultDisplayLanguage     | [localeInfo](localeinfo.md)                           | 适用于 Microsoft web 应用程序的用户首选用户界面语言（菜单、按钮、功能区、警告消息）。<br><br>默认返回。 不可为空。 |
| authoringLanguages         | localeInfo 集合                                 | 用户读取和作者的语言的优先顺序列表。<br><br>默认返回。 不可为空。                                                              |
| defaultTranslationLanguage | localeInfo                                            | 用户希望将文档、电子邮件和邮件翻译为的语言。<br><br>默认情况下返回。                                                    |
| defaultSpeechInputLanguage | localeInfo                                            | 用户预期用作语音文本到语音方案的输入的语言。<br><br>默认情况下返回。                                                              |
| defaultRegionalFormat      | localeInfo                                            | 驱动默认的日期、时间和日历格式的区域设置。<br><br>默认情况下返回。                                                                 |
| regionalFormatOverrides    | [regionalFormatOverrides](regionalformatoverrides.md) | 允许用户使用特定于字段的格式替代其 defaultRegionalFormat。<br><br>默认情况下返回。                                                      |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 定义。

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings"
} -->

```json
{
    "defaultDisplayLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "authoringLanguages":[{"@odata.type":"microsoft.graph.localeInfo"}] ,
    "defaultTranslationLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultSpeechInputLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultRegionalFormat":{"@odata.type":"microsoft.graph.localeInfo"} ,
    "regionalFormatOverrides":{"@odata.type":"microsoft.graph.regionalFormatOverrides"}
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalAndLanguageSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
