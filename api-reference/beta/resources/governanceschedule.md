---
title: governanceSchedule 资源类型
description: '表示 governanceRoleAssignmentRequest 的计划。 对于角色分配请求，计划控制何时执行角色分配操作、何时停止角色分配以及执行角色分配操作的频率。 '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 1182409b573684b59b40cec14e976ea00ee4d966
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397949"
---
# <a name="governanceschedule-resource-type"></a>governanceSchedule 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2AADRoles-deprecation.md)]

表示 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 的计划。 对于角色分配请求，计划控制何时执行角色分配操作、何时停止角色分配以及执行角色分配操作的频率。



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|startDateTime|DateTimeOffset|角色分配的开始时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|endDateTime|DateTimeOffset|角色分配的结束时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 *注意：如果值为 `null`，则表示永久性分配。*|
|type|字符串|角色分配计划类型。 目前仅 `Once` 支持此项。
|duration|期限|角色分配的持续时间。 它采用 TimeSpan 格式。|

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


