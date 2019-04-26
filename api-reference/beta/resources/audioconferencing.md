---
title: audioConferencing 资源类型
description: 表示 onlineMeeting 的电话访问信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1371e80830bf148588f6bda91326b0521fcdda42
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328372"
---
# <a name="audioconferencing-resource-type"></a>audioConferencing 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[onlineMeeting](onlinemeeting.md)的电话访问信息。

## <a name="properties"></a>属性

| 属性            | 类型    | 说明                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | String  | 包含拨入信息的可从外部访问的网页的 URL。 |
| leaderPasscode      | String  | 连接到音频会议提供商所需的领导者密码。      |
| participantPasscode | String  | 连接到音频会议提供商所需的参与者密码。 |
| tollFreeNumber      | String  | 要连接到音频会议提供商的免费电话号码。              |
| tollNumber          | String  | 要连接到音频会议提供商的收费号码。                   |

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
