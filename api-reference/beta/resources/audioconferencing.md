---
title: audioConferencing 资源类型
description: 表示联机会议的电话访问信息。
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5f0c9338aefa592ed030585a6b0342d03e7717d0
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896695"
---
# <a name="audioconferencing-resource-type"></a>audioConferencing 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [onlineMeeting 的电话访问信息](onlinemeeting.md)。

## <a name="properties"></a>属性

| 属性                    | 类型              | 说明                                                                    |
| :-------------------------- | :---------------- | :----------------------------------------------------------------------------- |
| dialinUrl                   | String            | 指向包含拨入信息且可从外部访问的网页的 URL。 |
| conferenceId                | String            | 联机会议的会议 ID。                                       |
| tollFreeNumber (弃用)  | String            | 连接到音频会议提供商的免费电话号码。           |
| tollFreeNumbers             | 字符串集合 | 会议邀请中显示的免费电话号码列表。            |
| tollNumber (弃用)      | String            | 连接到音频会议提供商的收费号码。                |
| tollNumbers                 | 字符串集合 | 会议邀请中显示的收费号码列表。                 |

> [!CAUTION]
>
>- **tollFreeNumber 和** **tollNumber** 属性已弃用。 请 **改为使用 tollFreeNumbers** 和 **tollNumbers** 属性。
>- 为了向后兼容，将 **原始 tollFreeNumber** 添加到新的 **tollFreeNumbers** 集合，并且将原始 **tollNumber** 添加到新的 **tollNumbers** 集合中。

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
  "tollFreeNumbers": ["String"],
  "tollNumbers": ["String"]
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


