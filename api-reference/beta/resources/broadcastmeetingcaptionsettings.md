---
title: broadcastMeetingCaptionSettings 资源类型
description: 代表实时事件Microsoft Teams标题设置。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 52239562480eed674b5b41000d9d3bedb7abfc54
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2021
ms.locfileid: "61547674"
---
# <a name="broadcastmeetingcaptionsettings-resource-type"></a>broadcastMeetingCaptionSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示实时事件 Microsoft Teams[标题设置](/microsoftteams/teams-live-events/what-are-teams-live-events)。 有关在客户端中如何使用实时Teams的详细信息，请参阅在实时事件[使用实时字幕](https://support.microsoft.com/en-us/office/use-live-captions-in-a-live-event-1d6778d4-6c65-4189-ab13-e2d77beb9e2a)。

## <a name="properties"></a>属性

| 属性             | 类型              | 说明                                                     |
|:---------------------|:------------------|:----------------------------------------------------------------|
| isCaptionEnabled     | Boolean           | 指示是否为此事件启用Teams实时事件。 |
| spokenLanguage       | String            | 语音语言。                                            |
| translationLanguages | String collection | 翻译语言 (最多选择 6) 。                     |

> [!TIP]
>
> 翻译语言不能包含与语音语言相同的语言代码。

### <a name="spokenlanguage-values"></a>spokenLanguage 值

下表显示了语音语言支持的语言代码。

| 语音语言           | 值   |
|:--------------------------|:--------|
| 简 (中文（中国)  | zh-Hans |
| 荷兰语（荷兰）       | nl      |
| 英语（美国）   | en      |
| 法语（加拿大）           | fr-ca   |
| 法语（法国）           | fr      |
| 德语（德国）          | de      |
| 印地语 (印度)              | hi      |
| 意大利语（意大利）           | it      |
| 日语（日本）          | ja      |
| 朝鲜语（韩国）            | ko      |
| 葡萄牙语（巴西）       | pt      |
| 俄语（俄罗斯）          | ru      |
| 西班牙语（西班牙）           | es      |
| 西班牙语（墨西哥）          | es-mx   |
| 瑞典语（瑞典）          | sv      |

### <a name="translationlanguaes-values"></a>translationLanguaes 值

下表显示了翻译语言支持的语言代码。

| 翻译语言                     | 值   |
|------------------------------------------|---------|
| 南非荷兰语 (南非)                  | af      |
| 阿拉伯语（埃及）                           | ar      |
| 波斯尼亚语(拉丁语)                          | bs      |
| 保加利亚 (保加利亚)                      | bg      |
| 加泰罗尼亚语                                  | ca      |
| 简 (中文（中国)                 | zh-Hans |
| 中文 (（香港特别行政区）)  | yue     |
| 中文 (Tranditional)                    | zh-Hant |
| 法罗 (法罗尼)                            | ht      |
| 克罗地亚语（克罗地亚）                       | hr      |
| 捷克语（捷克共和国）                   | cs      |
| 丹麦语（丹麦）                         | da      |
| 荷兰语（荷兰）                      | nl      |
| 英语（美国）                  | en      |
| 爱沙尼亚 (爱沙尼亚)                        | et      |
| 菲律宾语（菲律宾）                   | fil     |
| 芬兰语（芬兰）                        | fi      |
| 法语（加拿大）                          | fr-ca   |
| 法语（法国）                          | fr      |
| 德语（德国）                         | de      |
| 希腊语（希腊）                           | el      |
| 希伯来语（以色列）                          | he      |
| 印地语 (印度)                             | hi      |
| Hmong                                    | mww     |
| 匈牙利语（匈牙利）                      | hu      |
| 印度尼西亚语                               | id      |
| 意大利语（意大利）                          | it      |
| 日语（日本）                         | ja      |
| 百年                                  | tlh     |
| 朝鲜语（韩国）                           | ko      |
| 拉脱维亚语 (拉脱维亚)                          | lv      |
| 立陶宛语 (立陶宛)                    | lt      |
| 马耳他语 (省)                     | mg      |
| 马来语(马来西亚)                         | ms      |
| 马耳他语（马耳他）                          | mt      |
| 波斯 (波斯)                            | fa      |
| 波兰语（波兰）                          | pl      |
| 葡萄牙语（巴西）                      | pt      |
| Querétaro Otomi                          | otq     |
| 罗马尼亚 (罗马尼亚)                        | ro      |
| 俄语（俄罗斯）                         | ru      |
| 萨摩亚                                   | sm      |
| 塞尔维亚语(拉丁语)                          | sr-latn |
| Serbian Cyrillic                         | sr-cyrl |
| 斯洛伐克 (斯洛伐克)                         | sk      |
| 斯洛文尼亚语                                | sl      |
| 西班牙语（西班牙）                          | es      |
| 肯尼亚 (斯瓦希里语)                           | sw      |
| 瑞典语（瑞典）                         | sv      |
| 塔尼西亚语                                 | ty      |
| 泰国 (泰国)                           | th      |
| 汤加语                                   | 更改为      |
| 土耳其 (土耳其)                          | tr      |
| 乌克兰 (乌克兰)                       | uk      |
| 巴基斯坦 (都语共和国)       | ur      |
| 越南 (越南)                      | vi      |
| 英国 (的)                    | cy      |
| Yucatec Maya                             | yua     |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.broadcastMeetingCaptionSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.broadcastMeetingCaptionSettings",
  "isCaptionEnabled": "Boolean",
  "spokenLanguage": "String",
  "translationLanguages": [
    "String"
  ]
}
```
