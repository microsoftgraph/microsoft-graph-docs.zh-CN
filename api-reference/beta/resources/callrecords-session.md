---
title: 会话资源类型
description: 会话类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 48983f3a6c4adf12184802722ba2607780c7b531
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720219"
---
# <a name="session-resource-type"></a>会话资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示User-User呼叫时User-Meeting通信或通信。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列表会话](../api/callrecords-session-list.md) | [microsoft.graph.callRecords.session](callrecords-session.md) 集合 | 检索与 [callRecord](callrecords-callrecord.md) 对象关联的会话列表。
 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|string|会话的唯一标识符。 只读。|
|调用方|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|启动会话的终结点。|
|被叫方|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|应答会话的终结点。|
|failureInfo|[microsoft.graph.callRecords.failureInfo](callrecords-failureinfo.md)|与会话关联的失败信息（如果会话失败）。|
|形式|microsoft.graph.callRecords.modality 集合|会话中存在的模式列表。 可取值为：`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data`、`screenSharing` 或 `unknownFutureValue`。|
|startDateTime|DateTimeOffset|第一个用户加入会话时 UTC fime。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|endDateTime|DateTimeOffset|最后一个用户离开会话的 UTC 时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|


## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|段|[microsoft.graph.callRecords.segment](callrecords-segment.md) 集合|会话中涉及的分段列表。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.session",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "caller": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "callee": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "failureInfo": {"@odata.type": "microsoft.graph.callRecords.failureInfo"},
  "modalities": ["string"],
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "session resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

