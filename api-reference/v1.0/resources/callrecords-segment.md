---
title: 分段资源类型
description: 线段类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6c38dac3d0e2e30c8b90e9fb0029d463b700f124
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492018"
---
# <a name="segment-resource-type"></a>分段资源类型

命名空间：microsoft.graph.callRecords

表示用户用户通信的一部分或会议呼叫时的用户会议通信。 典型的 VOIP 呼叫将每个会话包含一个分段。 在某些情况下，例如 PSTN 呼叫，由于连接呼叫需要额外的服务器到服务器通信，因此每个会话会有多个分段。

## <a name="methods"></a>Methods

不存在直接访问分段的方法。 请使用[Get callRecord](../api/callrecords-callrecord-get.md) api With `$expand=sessions($expand=segments)` 或[List session](../api/callrecords-session-list.md) api with `$expand=segments` to 获取[callRecord](callrecords-callrecord.md)的段。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|分段的唯一标识符。 只读。|
|者|[callRecords。](callrecords-endpoint.md)|启动了此段的终结点。|
|约定|[callRecords。](callrecords-endpoint.md)|应答此段的终结点。|
|failureInfo|[callRecords。 failureInfo](callrecords-failureinfo.md)|与分段相关联的失败信息失败。|
|光盘|[Microsoft callRecords](callrecords-media.md)集合|与此分段关联的媒体。|
|startDateTime|DateTimeOffset|段启动时的 UTC 时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|段结束时的 UTC 时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.segment",
  "baseType": "",
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