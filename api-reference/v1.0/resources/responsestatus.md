---
title: responseStatus 资源类型
description: 会议请求的响应状态。
ms.localizationpriority: medium
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e1b2861386fc32589d35d6354345b1ba24471d98
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108868"
---
# <a name="responsestatus-resource-type"></a>responseStatus 资源类型

命名空间：microsoft.graph

会议请求的与会者或组织者的响应状态。

可以通过事件的 **responseStatus** 属性或与会者 的 **status** 属性获取与会者或 [](event.md)组织者 [的响应状态](attendee.md)。

## <a name="properties"></a>属性

| 属性 | 类型           | 说明 |
|:---------|:---------------|:------------|
| 响应 | responseType   | 响应类型。 可取值为：`none`、`organizer`、`tentativelyAccepted`、`accepted`、`declined`、`notResponded`。<br><br>为了区分 和 ：，例如，如果与会者 Alex 尚未响应会议请求，在 Alex 的日历中获取 Alex 对该事件的响应 `none` `notResponded` 状态将返回 `notResponded` 。 从任何其他与会者或组织者的日历获取 Alex 的响应将返回 `none` 。 获取组织者对任何人日历中事件的响应也会返回 `none` 。 
| 时间     | DateTimeOffset | 响应返回的日期和时间。 它使用 ISO 8601 格式，并始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

