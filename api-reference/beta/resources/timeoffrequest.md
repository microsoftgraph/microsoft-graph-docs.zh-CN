---
title: timeOffRequest 资源类型
description: 表示要采用 timeoff 的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 73fa72d403bd20e6a966b01a0529d09689e5ed66
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519713"
---
# <a name="timeoffrequest-resource-type"></a>timeOffRequest 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示要采用[timeoff](../resources/timeoff.md)的班次请求的类型。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取](../api/timeoffrequest-get.md) | [timeOffRequest](timeoffrequest.md) | 读取**timeOffRequest**对象的属性和关系。 |
| [更新](../api/timeoffrequest-update.md) | [timeOffRequest](timeoffrequest.md) | 更新**timeOffRequest**对象。 |
| [删除](../api/timeoffrequest-delete.md) | 无 | 删除**timeOffRequest**对象。 |
|[批准](../api/timeoffrequest-approve.md)|无|批准请假时间请求。|
|[拒绝](../api/timeoffrequest-decline.md)|无|拒绝休息时间请求。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|startDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|timeOffReasonId|String|休息时间的原因。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeOffRequest",
  "baseType": ""
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
