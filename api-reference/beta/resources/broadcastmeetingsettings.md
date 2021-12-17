---
title: broadcastMeetingSettings 资源类型
description: 表示与活动实时事件相关的Microsoft Teams。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c91dda07a2a339bdee40e5ea2f953c2eab65ad98
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2021
ms.locfileid: "61545355"
---
# <a name="broadcastmeetingsettings-resource-type"></a>broadcastMeetingSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与活动实时[事件相关的](/microsoftteams/teams-live-events/what-are-teams-live-events)Microsoft Teams。

## <a name="properties"></a>属性

| 属性                   | 类型                     | 说明                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| allowedAudience            | [broadcastMeetingAudience](#broadcastmeetingaudience-values) | 定义谁可以加入Teams活动。 下表列出了可能的值。 |
| captions | [broadcastMeetingCaptionSettings](../resources/broadcastmeetingcaptionsettings.md) | 实时事件的标题Teams设置。 |
| isRecordingEnabled         | Boolean                  | 指示是否为此实时事件Teams录制。 默认值为 `false`。          |
| isAttendeeReportEnabled    | Boolean                  | 指示是否为此实时事件启用Teams报告。 默认值为 `false`。    |
| isQuestionAndAnswerEnabled | Boolean                  | 指示是否为此&事件启用了 Q Teams A。 默认值为 `false`。                |
| isVideoOnDemandEnabled     | Boolean                  | 指示是否为此实时事件启用Teams视频。 默认值为 `false`。    |

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
  "@odata.type": "microsoft.graph.broadcastMeetingSettings"
}-->
```json
{
  "@odata.type": "#microsoft.graph.broadcastMeetingSettings",
  "allowedAudience": "String",
  "isRecordingEnabled": "Boolean",
  "isAttendeeReportEnabled": "Boolean",
  "isQuestionAndAnswerEnabled": "Boolean",
  "isVideoOnDemandEnabled": "Boolean",
  "captions": {
    "@odata.type": "microsoft.graph.broadcastMeetingCaptionSettings"
  }
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
