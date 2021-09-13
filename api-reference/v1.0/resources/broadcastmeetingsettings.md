---
title: broadcastMeetingSettings 资源类型
description: 设置实时事件相关的事件
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0a78c4665c42bf11c983bbf24aa72a93cdff323a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59031711"
---
# <a name="broadcastmeetingsettings-resource-type"></a>broadcastMeetingSettings 资源类型

命名空间：microsoft.graph

设置实时事件相关。

## <a name="properties"></a>属性

| 属性                   | 类型                                                         | 说明                                                                                 |
|----------------------------|--------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| allowedAudience            | [broadcastMeetingAudience](#broadcastmeetingaudience-values) | 定义可加入实时事件的人。 下表列出了可能的值。     |
| isRecordingEnabled         | Boolean                                                      | 指示是否为此实时事件启用录制。 默认值为 `false`。       |
| isAttendeeReportEnabled    | 布尔值                                                      | 指示是否为此实时事件启用与会者报告。 默认值为 `false`。 |
| isQuestionAndAnswerEnabled | 布尔值                                                      | 指示是否为此&事件启用了问答。 默认值为 `false`。             |
| isVideoOnDemandEnabled     | Boolean                                                      | 指示是否为此实时事件启用视频按需。 默认值为 `false`。 |

### <a name="broadcastmeetingaudience-values"></a>broadcastMeetingAudience 值

| 值              | 说明                                                       |
|--------------------|-------------------------------------------------------------------|
| everyone           | 实时事件将向任何人开放。 此值为默认值。 |
| 组织       | 组织中的每个人都可以加入实时事件。                     |
| roleIsAttendee     | 只有指定的人员才能加入实时事件。                |
| unknownFutureValue | 可发展枚举 sentinel 值。 请勿使用。                 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.broadcastMeetingSettings"
}-->
```json
{
  "allowedAudience": "everyone | organization | roleIsAttendee | unknownFutureValue",
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
