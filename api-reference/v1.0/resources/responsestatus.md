---
title: responseStatus 资源类型
description: 会议请求的响应状态。
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1aebaa2672b741798a2c6bbf95c8c9d966cabfd1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722382"
---
# <a name="responsestatus-resource-type"></a>responseStatus 资源类型

命名空间：microsoft.graph

会议请求的响应状态。

## <a name="properties"></a>属性

| 属性 | 类型           | 说明 |
|:---------|:---------------|:------------|
| 响应 | responseType   | 响应类型。 可能的值包括 `None`、`Organizer`、`TentativelyAccepted`、`Accepted`、`Declined`、`NotResponded`。
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

