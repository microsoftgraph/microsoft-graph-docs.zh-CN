---
title: callRecord 资源类型
description: 表示多个参与者之间的单个对等呼叫或组呼叫，有时称为联机会议。
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1d142572859f56bfcb14e942ff4bd767dc67b7ad
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720262"
---
# <a name="callrecord-resource-type"></a>callRecord 资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示多个参与者之间的单个对等呼叫或组呼叫，有时称为联机会议。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 callRecord](../api/callrecords-callrecord-get.md) | [microsoft.graph.callRecords.callRecord](callrecords-callrecord.md) | 读取 **callRecord** 对象的属性和关系。 |
| [获取 PSTN 呼叫](../api/callrecords-callrecord-getpstncalls.md) | [microsoft.graph.callRecords.pstnCallLogRow](callrecords-pstncalllogrow.md)| 读取 **pstnCallLogRow 对象** 的属性。 |
| [获取直接路由呼叫](../api/callrecords-callrecord-getdirectroutingcalls.md) | [microsoft.graph.callRecords.directRoutingLogRow](callrecords-directroutinglogrow.md)| 读取 **directRoutingLogRow 对象** 的属性。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|最后一个用户离开呼叫的 UTC 时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|id|String|呼叫记录的唯一标识符。 只读。|
|joinWebUrl|String|与呼叫关联的会议 URL。 peerToPeer 呼叫记录类型可能不可用。|
|lastModifiedDateTime|DateTimeOffset|创建呼叫记录时 UTC 时间。 DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|形式|microsoft.graph.callRecords.modality 集合|调用中使用的所有形式的列表。 可取值为：`unknown`、`audio`、`video`、`videoBasedScreenSharing`、`data`、`screenSharing` 或 `unknownFutureValue`。|
|organizer － 组织者|[identitySet](identityset.md)|组织方的身份。|
|participants|[identitySet](identityset.md) 集合|调用中涉及不同标识的列表。|
|startDateTime|DateTimeOffset|第一个用户加入呼叫的 UTC 时间。 DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|type|microsoft.graph.callRecords.callType|指示呼叫的类型。 可取值为：`unknown`、`groupCall`、`peerToPeer`、`unknownFutureValue`。|
|version|Int64|单调增加的呼叫记录版本。 与较低版本相比，具有相同 ID 的更高版本呼叫记录包含其他数据。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|sessions|[microsoft.graph.callRecords.session](callrecords-session.md) 集合|呼叫中涉及的会话列表。 对等呼叫通常只有一个会话，而组呼叫通常每个参与者至少具有一个会话。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.callRecord",
  "keyProperty": "id"
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "modalities": ["string"],
  "organizer": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}],
  "startDateTime": "String (timestamp)",
  "type": "string",
  "version": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


