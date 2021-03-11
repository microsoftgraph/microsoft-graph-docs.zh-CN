---
title: 线段资源类型
description: 线段类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5cb95c665ed3967aeb9b18fcefd262ad52490306
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720226"
---
# <a name="segment-resource-type"></a>线段资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示电话会议User-User通信或User-Meeting通信的一部分。 典型的 VOIP 呼叫将每个会话具有一个段。 在某些情况下（如 PSTN 呼叫）中，由于连接呼叫需要其他服务器到服务器通信，每个会话将有多个分段。

## <a name="methods"></a>方法

不存在直接访问线段的方法。 Please use the [Get callRecord](../api/callrecords-callrecord-get.md) api with `$expand=sessions($expand=segments)` or the List [session](../api/callrecords-session-list.md) api with to get the segments for `$expand=segments` a [callRecord.](callrecords-callrecord.md)

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|线段的唯一标识符。 只读。|
|调用方|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|启动此段的终结点。|
|被叫方|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|应答此段的终结点。|
|failureInfo|[microsoft.graph.callRecords.failureInfo](callrecords-failureinfo.md)|与段关联的失败信息（如果失败）。|
|media|[microsoft.graph.callRecords.media](callrecords-media.md) 集合|与此段关联的媒体。|
|startDateTime|DateTimeOffset|段开始的 UTC 时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|endDateTime|DateTimeOffset|段结束时的 UTC 时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.segment",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "caller": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "callee": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "failureInfo": {"@odata.type": "microsoft.graph.callRecords.failureInfo"},
  "media": [{"@odata.type": "microsoft.graph.callRecords.media"}],
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "segment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

