---
title: audioConferencing 资源类型
description: 表示联机会议的电话访问信息。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dc60d1cb5bcc1c191d82e9e996014dac8bb9f9bc
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220666"
---
# <a name="audioconferencing-resource-type"></a>audioConferencing 资源类型

命名空间：microsoft.graph

表示 [onlineMeeting 的电话访问信息](onlinemeeting.md)。

## <a name="properties"></a>属性

| 属性                    | 类型              | 说明                                                                    |
| :-------------------------- | :---------------- | :----------------------------------------------------------------------------- |
| dialinUrl                   | String            | 指向包含拨入信息且可从外部访问的网页的 URL。 |
| conferenceId                | 字符串            | 联机会议的会议 ID。                                       |
| tollFreeNumbers             | 字符串集合 | 会议邀请中显示的免费电话号码列表。            |
| tollNumbers                 | 字符串集合 | 会议邀请中显示的收费号码列表。                 |
| tollFreeNumber (弃用)  | 字符串            | 连接到音频会议提供商的免费电话号码。           |
| tollNumber (弃用)      | String            | 连接到音频会议提供商的收费号码。                |

> [!CAUTION]
>
>- **tollFreeNumber** 和 **tollNumber** 属性已弃用。 请 **改为使用 tollFreeNumbers** 和 **tollNumbers** 属性。
>- 为了向后兼容，将 **原始 tollFreeNumber** 添加到新的 **tollFreeNumbers** 集合，并且将原始 **tollNumber** 添加到新的 **tollNumbers** 集合。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "conferenceId": "String",
  "tollFreeNumbers": [ "String" ],
  "tollNumbers": [ "String" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

