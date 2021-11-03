---
title: governanceSchedule 资源类型
description: '表示 governanceRoleAssignmentRequest 的计划。 对于角色分配请求，计划控制何时执行 角色分配 操作、何时停止 角色分配 以及执行 角色分配 操作的频率。 '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 87abccdfac02bea7a3158feb786b39aad23fac3f
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694265"
---
# <a name="governanceschedule-resource-type"></a>governanceSchedule 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1resourceroles-deprecation](../../includes/pim-v1aadroles-deprecation.md)]

表示 [governanceRoleAssignmentRequest 的计划](../resources/governanceroleassignmentrequest.md)。 对于角色分配请求，计划控制何时执行 角色分配 操作、何时停止 角色分配 以及执行 角色分配 操作的频率。



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|startDateTime|DateTimeOffset|会议开始时间角色分配。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|endDateTime|DateTimeOffset|会议结束角色分配。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 *注意：如果值为 `null` ，则指示永久分配。*|
|type|String|计划角色分配类型。 目前 `Once` 仅受支持。
|duration|期限|项目持续时间角色分配。 其格式为 TimeSpan。|

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


