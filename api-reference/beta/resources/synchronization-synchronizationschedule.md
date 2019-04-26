---
title: synchronizationSchedule 资源类型
description: 定义用于运行 synchronizationJob 的计划。
localization_priority: Normal
ms.openlocfilehash: 2ae5473463e84fdf27882df1b243049cc98ab043
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340034"
---
# <a name="synchronizationschedule-resource-type"></a>synchronizationSchedule 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义用于运行[synchronizationJob](synchronization-synchronizationjob.md)的计划。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|时间|DateTimeOffset|此作业将到期的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|interval|持续时间|同步迭代之间的时间间隔。|
|state|String| 可取值为：`Active`、`Disabled`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchedule"
}-->

```json
{
  "expiration": "String (timestamp)",
  "interval": "String (duration)",
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
