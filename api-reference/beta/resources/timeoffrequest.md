---
title: timeOffRequest 资源类型
description: 表示一种要休息的班次请求类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 31d855f21164f933fe27acc824759cee08e16c16
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786066"
---
# <a name="timeoffrequest-resource-type"></a>timeOffRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一种班次请求采取 [时间Off](../resources/timeoff.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/timeoffrequest-list.md) | [timeOffRequest](timeoffrequest.md) 集合 | 获取此 **计划中的 timeOffRequest** 对象列表。|
| [获取](../api/timeoffrequest-get.md) | [timeOffRequest](timeoffrequest.md) | 读取 **timeOffRequest** 对象的属性和关系。 |
| [删除](../api/timeoffrequest-delete.md) | 无 | 删除 **timeOffRequest** 对象。 |
| [批准](../api/timeoffrequest-approve.md)|无|批准请假请求。|
| [拒绝](../api/timeoffrequest-decline.md)|无|拒绝请假请求。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|startDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|timeOffReasonId|String|请假的原因。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeOffRequest"
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "timeOffReasonId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


