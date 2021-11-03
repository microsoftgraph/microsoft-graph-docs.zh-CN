---
title: broadcastMeetingSettings 资源类型
description: 设置事件相关的Teams事件
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 36e5778761ac792e84096fd54f48c766e524149d
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696530"
---
# <a name="broadcastmeetingsettings-resource-type"></a>broadcastMeetingSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

设置实时事件[Microsoft Teams相关的事件](/microsoftteams/teams-live-events/what-are-teams-live-events)。

## <a name="properties"></a>属性

| 属性                   | 类型                     | 说明                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| allowedAudience            | [broadcastMeetingAudience](#broadcastmeetingaudience-values) | 定义谁可以加入Teams活动。 下表列出了可能的值。 |
| isRecordingEnabled         | 布尔值                  | 指示是否为此实时事件Teams录制。 默认值为 `false`。          |
| isAttendeeReportEnabled    | 布尔值                  | 指示是否为此活动启用了参与者Teams活动。 默认值为 `false`。    |
| isQuestionAndAnswerEnabled | 布尔值                  | 指示是否为此&事件启用了 Q Teams A。 默认值为 `false`。                |
| isVideoOnDemandEnabled     | 布尔值                  | 指示是否为此实时事件启用Teams视频。 默认值为 `false`。    |

### <a name="broadcastmeetingaudience-values"></a>broadcastMeetingAudience 值

| 值              | 说明                                                       |
| ------------------ | ----------------------------------------------------------------- |
| everyone           | 此Teams事件将向任何人开放。 此值为默认值。 |
| 组织       | 组织中的每个人都可以加入此Teams活动。                     |
| roleIsAttendee     | 只有指定的人员才能加入此Teams活动。                |
| unknownFutureValue | 可发展枚举 sentinel 值。 请勿使用。  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.broadcastMeetingSettings"
}-->
```json
{
  "allowedAudience": "String",
  "isRecordingEnabled": "Boolean",
  "isAttendeeReportEnabled": "Boolean",
  "isQuestionAndAnswerEnabled": "Boolean",
  "isVideoOnDemandEnabled": "Boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "broadcastSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
