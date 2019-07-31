---
title: governanceSchedule 资源类型
description: '代表 governanceRoleAssignmentRequest 的日程安排。 对于角色分配请求, 日程安排控制何时执行角色分配操作、何时停止角色分配以及执行角色分配操作的频率。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 36a2b4c73f5f85439a34a42ea2aa23cfe861c4ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006372"
---
# <a name="governanceschedule-resource-type"></a>governanceSchedule 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的日程安排。 对于角色分配请求, 日程安排控制何时执行角色分配操作、何时停止角色分配以及执行角色分配操作的频率。 



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|startDateTime|DateTimeOffset|角色分配的开始时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|角色分配的结束时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 *注意: 如果值为`null`, 则表示永久分配。*|
|type|String|角色分配计划类型。 目前`Once`仅支持。
|duration|持续时间|角色分配的持续时间。 它的格式为 TimeSpan。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSchedule"
}-->

```json
{
  "duration": "String (timespan)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
