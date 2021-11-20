---
title: responseStatus 资源类型
description: 会议请求的响应状态。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: outlook
author: harini84
ms.openlocfilehash: 860afaffc2ce6bcc42a4730b7672983922b066b9
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2021
ms.locfileid: "61123893"
---
# <a name="responsestatus-resource-type"></a>responseStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会议请求的与会者或组织者的响应状态。

可以通过事件的 **responseStatus** 属性或与会者 的 **status** 属性获取与会者或 [](event.md)组织者 [的响应状态](attendee.md)。

## <a name="properties"></a>属性

| 属性 | 类型           | 说明 |
|:---------|:---------------|:------------|
| 响应 | String         | 响应类型。 可取值为：`none`、`organizer`、`tentativelyAccepted`、`accepted`、`declined`、`notResponded`。<br><br>区分和 `none` `notResponded` ： <br><br> `none` – 从组织者的角度来看。 将与会者/参与者的状态报告给会议的组织者时，使用此值。 <br><br> `notResponded` – 从参与的角度看。 指示与会者尚未响应会议请求。 <br><br> 客户端可以处理 `notResponded`  ==  `none` 。 <br><br> 例如，如果与会者 Alex 尚未响应会议请求，在 Alex 的日历中获取 Alex 对该事件的响应状态将返回 `notResponded` 。 从任何其他与会者或组织者的日历获取 Alex 的响应将返回 `none` 。 获取任何人的日历中事件的组织者响应也会返回 `none` 。 
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
<!--
{
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


