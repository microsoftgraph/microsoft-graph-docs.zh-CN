---
title: audioConferencing 资源类型
description: 代表 onlineMeeting 电话访问信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd65b094a17ad3fa470471c3ed6dd3908367e578
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977505"
---
# <a name="audioconferencing-resource-type"></a>audioConferencing 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表[onlineMeeting](onlinemeeting.md)电话访问信息。

## <a name="properties"></a>属性

| 属性            | 类型    | Description                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | 字符串  | 指向包含拨入信息的可从外部访问网页的 URL。 |
| leaderPasscode      | 字符串  | 连接到音频会议提供商所需的主持人密码。      |
| participantPasscode | 字符串  | 连接到音频会议提供商所需的参与者密码。 |
| tollFreeNumber      | 字符串  | 要连接到音频会议提供商的免费电话号码。              |
| tollNumber          | 字符串  | 要连接到音频会议提供商的收费电话号码。                   |

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
  "leaderPasscode": "String",
  "participantPasscode": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
