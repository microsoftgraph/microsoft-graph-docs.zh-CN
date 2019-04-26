---
title: 参与者资源类型
description: 参与者类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f49526824b2b6c4eb4a5065f05ab4c765d299faa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568637"
---
# <a name="participant-resource-type"></a>参与者资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

参与者类型。

## <a name="methods"></a>方法

| 方法                                                          | 返回类型                              | 说明                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [获取参与者](../api/participant-get.md)                    | [参与者](participant.md)            | 读取**参与者**对象的属性。    |
| [ConfigureMixer](../api/participant-configuremixer.md)          | [commsOperation](commsoperation.md)      | 配置参与者音频混合器。            |
| [邀请](../api/participant-invite.md)                          | [commsOperation](commsoperation.md)      | 邀请参与者加入呼叫。                 |
| [参与者静音](../api/participant-mute.md)                  | [commsOperation](commsoperation.md)      | 将呼叫中的参与者静音。                     |
| [所有参与者静音](../api/participant-muteall.md)          | [commsOperation](commsoperation.md)      | 将会议中的所有参与者设为静音。         |

## <a name="properties"></a>属性

| 属性             | 类型                                     | 说明                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | String                                   | 参与者 id。                                          |
| info                 | [participantInfo](participantinfo.md)    | 参与者的参与者。                          |
| isInLobby            | 布尔                                  | 如果参与者在会议厅中, 则为 true                          |
| isMuted              | 布尔                                  | 如果参与者处于静音 (客户端或服务器为静音)    |
| mediaStreams         | [mediaStream](mediastream.md)集合 | 媒体流的列表。                                   |
| metadata             | String                                   | 名单中的参与者提供的数据 blob     |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | 有关参与者是否有录制功能的信息。 |

## <a name="relationships"></a>关系
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
<!--
{
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/participant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
