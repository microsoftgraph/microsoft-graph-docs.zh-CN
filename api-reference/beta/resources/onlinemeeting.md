---
title: onlineMeeting 资源类型
description: 捕获有关会议的信息，包括联接 URL、与会者列表和说明。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 611731673d932d6c5135c0115d735e4d642b1bfe
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792784"
---
# <a name="onlinemeeting-resource-type"></a>onlineMeeting 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

捕获有关会议的信息，包括联接 URL、与会者列表和说明。

## <a name="methods"></a>方法

| 方法         | 返回类型 | 说明 |
|:---------------|:--------|:----------|
| [获取 onlineMeeting](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | 读取 onlineMeeting 对象的属性和关系。 |

## <a name="properties"></a>属性

| 属性                  | 类型                                                   | 说明                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| accessLevel               | String                                                 | 控制联机会议的许可的访问级别。 可取值为：`everyone`、`invited`、`locked`、`sameEnterprise`、`unknown`。 |
| audioConferencing         | [audioConferencing](audioconferencing.md)              | 表示 onlineMeeting 的电话访问信息。 |
| canceledDateTime          | 日期时间                                               | 取消会议的时间。 |
| chatInfo                  | [chatInfo](chatinfo.md)                                | 与此会议关联的聊天。 |
| creationDateTime          | 日期时间                                               | 会议的创建时间。 只读。
| endDateTime               | 日期时间                                               | 会议的结束时间。 |
| entryExitAnnouncement     | Boolean                                                | 联机会议的出席通知状态。 启用出席通知后，联机会议将通知通过音频加入会议的参与者的姓名。 |
| expirationDateTime        | 日期时间                                               | 可在其后删除联机会议的绝对协调通用时间（UTC）日期和时间。 日期和时间必须在服务器上的当前日期和时间之后的一年前一年和之后10年。 |
| id                        | 字符串                                                 | 与联机会议相关联的 ID。 在 GET HTTP 请求中用作 ID。 只读。 由服务器生成。 |
| isCancelled               | Boolean                                                | 会议是否已被取消。 |
| joinUrl                   | String                                                 | 从 web 加入联机会议时使用的 URL。 |
| meetingType               | String                                                 | 可能的值为`meetNow`： `scheduled`、 `recurring`、 `broadcast` 、（注意： [create onlineMeeting](../api/application-post-onlinemeetings.md)仅`meetNow`支持）。 |
| participants              | [meetingParticipants](meetingparticipants.md)          | 与联机会议关联的参与者。  这包括组织者和与会者。 |
| startDateTime             | 日期时间                                               | 会议的开始时间。 |
| subject                   | String                                                 | 联机会议的主题。 |
| capabilities              | String collection                                      | 会议功能的列表。 可能的值是`questionAndAnswer`：。 |
| videoTeleconferenceId     | String                                                 | 视频电话会议 id。 |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "accessLevel": "everyone | invited | locked | sameEnterprise",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "entryExitAnnouncement": true,
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCancelled": false,
  "joinUrl": "String",
  "meetingType": "meetNow | scheduled | recurring | broadcast",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "capabilities": [ "questionAndAnswer" ],
  "videoTeleconferenceId": "String"
}
```