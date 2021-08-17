---
title: 参与者资源类型
description: 表示参与者类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3bada1be911bda02e49229a20793289b61934f74
ms.sourcegitcommit: 1e9a53e7b8e67349288f5cfbabe8355de83817b0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2021
ms.locfileid: "58367140"
---
# <a name="participant-resource-type"></a>参与者资源类型

命名空间：microsoft.graph

表示呼叫中的参与者。

## <a name="methods"></a>Methods

| 方法                                                 | 返回类型                                                 | 说明                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [列出参与者](../api/participant-get.md)          | [participant](participant.md)                               | 检索调用 **中的参与者** 对象列表。 |
| [获取参与者](../api/participant-get.md)           | [参与者](participant.md)                               | 读取 participant **对象** 的属性。 |
| [删除参与者](../api/participant-delete.md)         | 无   | 删除呼叫中的参与者。                  |
| [邀请](../api/participant-invite.md)                 | [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md)                        | 邀请参与者加入呼叫。              |
| [参与者静音](../api/participant-mute.md)         | [muteParticipantOperation](muteparticipantoperation.md)     | 将呼叫中的参与者静音。                  |

## <a name="properties"></a>属性

| 属性             | 类型                                     | 说明                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | String                                   | 参与者 ID。                                          |
| info                 | [participantInfo](participantinfo.md)    | 有关参与者的信息。                          |
| isInLobby            | 布尔值                                  | `true` 如果参与者在大厅中。                          |
| isMuted              | 布尔值                                  | `true` 如果参与者在客户端或服务器 (静音，则) 。    |
| mediaStreams         | [mediaStream](mediastream.md) 集合 | 媒体流列表。                                   |
| metadata             | String                                   | 名单中的参与者提供的数据 blob。     |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | 有关参与者是否具有录制功能的信息。 |

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

