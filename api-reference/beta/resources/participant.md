---
title: 参与者的资源类型
description: 参与者类型。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: c125589506dbd529d2b45df4171e9d54b346cbba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869830"
---
# <a name="participant-resource-type"></a>参与者的资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

参与者类型。

## <a name="methods"></a>方法

| 方法                                                          | 返回类型                              | 说明                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [获取参与者](../api/participant-get.md)                    | [参与者](participant.md)            | 阅读**参与者**对象的属性。    |
| [ConfigureMixer](../api/participant-configuremixer.md)          | [commsOperation](commsoperation.md)      | 配置参与者音频混音器。            |
| [邀请](../api/participant-invite.md)                          | [commsOperation](commsoperation.md)      | 邀请参与者加入呼叫。                 |
| [设置为静音的参与者](../api/participant-mute.md)                  | [commsOperation](commsoperation.md)      | 将呼叫中的参与者设为静音。                     |
| [将所有参与者设为都静音](../api/participant-muteall.md)          | [commsOperation](commsoperation.md)      | 将会议中的所有参与者设为都静音。         |

## <a name="properties"></a>属性

| 属性             | 类型                                     | 说明                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | 字符串                                   | 参与者的 id。                                          |
| 信息                 | [participantInfo](participantinfo.md)    | 参与者的参与者。                          |
| isInLobby            | boolean                                  | true 如果参与者位于会议厅                          |
| isMuted              | boolean                                  | 如果参与者处于静音状态，则 true （客户端或服务器静音）    |
| mediaStreams         | [mediaStream](mediastream.md)集合 | 媒体流的列表。                                   |
| 元数据             | 字符串                                   | 提供在名单中的参与者的数据的 blob     |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | 参与者是否具有录制功能的信息。 |

## <a name="relationships"></a>Relationships
无

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

## <a name="example"></a>示例

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus"
  },
  "isInLobby": false,
  "isMuted": false,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "status": "recordingCapable"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
