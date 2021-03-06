---
title: regionalAndLanguageSettings 资源类型
description: 表示用户区域和语言首选项的资源
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: d5fd77038735ed1faa175d77ed2bd10b3b2ef784
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516484"
---
# <a name="regionalandlanguagesettings-resource-type"></a>regionalAndLanguageSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一种开放类型，表示用户在各种上下文中的语言首选项，以及驱动默认日历的区域设置和格式设置以及日期和时间的格式设置。

## <a name="methods"></a>方法

| 方法                                                 | 返回类型                                                   | 说明                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [获取](../api/regionalAndLanguageSettings-get.md)       | [regionalAndLanguageSettings](regionalAndLanguageSettings.md) | 读取 **regionalAndLanguageSettings 对象** 的属性。                                       |
| [更新](../api/regionalandlanguagesettings-update.md) | [regionalAndLanguageSettings](regionalAndLanguageSettings.md) | 为用户更新 **regionalAndLanguageSettings** 对象的所有属性或部分属性。 |

## <a name="properties"></a>属性
| 属性                   | 类型                                                  | 说明                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| defaultDisplayLanguage     | [localeInfo](localeinfo.md)                           | 用户的首选用户界面语言 (菜单、按钮、功能区、警告消息) Microsoft Web 应用程序。<br><br>默认返回。 不可为空。 |
| authoringLanguages         | localeInfo 集合                                 | 用户读取和作者使用的语言的优先级列表。<br><br>默认返回。 不可为空。                                                              |
| defaultTranslationLanguage | localeInfo                                            | 用户期望将文档、电子邮件和邮件翻译为的语言。<br><br>默认情况下返回。                                                    |
| defaultSpeechInputLanguage | localeInfo                                            | 用户预期用作文本到语音方案输入的语言。<br><br>默认情况下返回。                                                              |
| defaultRegionalFormat      | localeInfo                                            | 驱动默认日期、时间和日历格式设置区域设置。<br><br>默认情况下返回。                                                                 |
| regionalFormatOverrides    | [regionalFormatOverrides](regionalformatoverrides.md) | 允许用户使用特定于字段的格式替代其默认RegionalFormat。<br><br>默认情况下返回。                                                      |
| translationPreferences     | [translationPreferences](translationPreferences.md)   | 使用翻译的文档、电子邮件、邮件和网站时用户的首选设置。<br><br>默认返回。 不可为空。                                       |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 定义。

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings"
} -->

```json
{
    "defaultDisplayLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "authoringLanguages": [{"@odata.type":"microsoft.graph.localeInfo"}],
    "defaultTranslationLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultSpeechInputLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultRegionalFormat": {"@odata.type":"microsoft.graph.localeInfo"},
    "regionalFormatOverrides": {"@odata.type":"microsoft.graph.regionalFormatOverrides"},
    "translationPreferences":{"@odata.type":"microsoft.graph.translationPreferences"}
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalAndLanguageSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


