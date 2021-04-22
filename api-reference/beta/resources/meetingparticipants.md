---
title: meetingParticipants 资源类型
description: 会议参与者。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 93ca3d73518f9739cc3115c80efd2aec551629b5
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944161"
---
# <a name="meetingparticipants-resource-type"></a>meetingParticipants 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会议参与者。

## <a name="properties"></a>属性

| 属性                  | 类型                                                           | 说明                           |
| :------------------------ | :------------------------------------------------------------- | :------------------------------------ |
| attendees                 | [meetingParticipantInfo](meetingparticipantinfo.md) 集合 | 与会者的信息。 |
| organizer － 组织者                 | [meetingParticipantInfo](meetingparticipantinfo.md)            | 会议组织者的信息。 |
| 创建 (已弃)     | [meetingParticipantInfo](meetingparticipantinfo.md) 集合 | 仅适用于直播会议。           |
| 参与者 (弃用)  | [meetingParticipantInfo](meetingparticipantinfo.md) 集合 | 仅适用于直播会议。           |

> [!CAUTION]
> 创建 **者和****参与者** 属性已弃用。 所有会议参与者都返回到 **与会者集合** 中。 使用[meetingParticipantInfo](meetingparticipantinfo.md)的 role 属性标识与会者的会议角色。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"},
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipants resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


