---
title: 参与者资源类型
description: 参与者类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c4bcaca9ea85a85d87e0584f37f0efeb89ed3773
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38748012"
---
# <a name="participant-resource-type"></a>参与者资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

参与者类型。

## <a name="methods"></a>方法

| 方法                                                 | 返回类型                                                 | 说明                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [获取参与者](../api/participant-get.md)           | [参与者](participant.md)                               | 读取**参与者**对象的属性。 |
| [ConfigureMixer](../api/participant-configuremixer.md) | [commsOperation](commsoperation.md)                         | 配置参与者音频混合器。         |
| [邀请](../api/participant-invite.md)                 | [commsOperation](commsoperation.md)                         | 邀请参与者加入呼叫。              |
| [静音参与者](../api/participant-mute.md)         | [muteParticipantOperation](muteparticipantoperation.md)     | 将呼叫中的参与者静音。                  |
| [为所有参与者静音](../api/participant-muteall.md) | [commsOperation](commsoperation.md) | 将会议中的所有参与者设为静音。      |

## <a name="properties"></a>属性

| 属性             | 类型                                     | 说明                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | String                                   | 参与者 ID。                                          |
| info                 | [participantInfo](participantinfo.md)    | 参与者的参与者。                          |
| isInLobby            | 布尔                                  | `true`如果参与者处于会议厅中。                          |
| isMuted              | 布尔                                  | `true`如果参与者处于静音（客户端或服务器为静音）。    |
| mediaStreams         | [mediaStream](mediastream.md)集合 | 媒体流的列表。                                   |
| metadata             | String                                   | 名单中参与者提供的数据的 blob。     |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | 有关参与者是否有录制功能的信息。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "String (identifier)",
  "info": {"@odata.type": "#microsoft.graph.participantInfo"},
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ],
  "metadata": "String",
  "recordingInfo": { "@odata.type": "#microsoft.graph.recordingInfo" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
