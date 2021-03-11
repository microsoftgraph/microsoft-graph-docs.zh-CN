---
title: synchronizationQuarantine 资源类型
description: 提供有关 synchronizationJob 的隔离状态的信息。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 45381594a242251995de3d43bb7fd02e0638484b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720499"
---
# <a name="synchronizationquarantine-resource-type"></a>synchronizationQuarantine 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供有关 [synchronizationJob](synchronization-synchronizationjob.md)的隔离状态的信息。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|currentBegan|DateTimeOffset|上次评估并强制隔离的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|nextAttempt|DateTimeOffset|下次尝试重新评估隔离的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|reason|String|一个代码，它表示为何实施隔离。 可取值为：`EncounteredBaseEscrowThreshold`、`EncounteredTotalEscrowThreshold`、`EncounteredEscrowProportionThreshold`、`EncounteredQuarantineException`、`QuarantinedOnDemand`、`TooManyDeletes` 或 `Unknown`。|
|seriesBegan|DateTimeOffset|在本系列中首次隔离的日期和时间 (一系列从首次隔离时开始，一旦隔离被解除，就会) 。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|seriesCount|Int64|此系列中对隔离进行重新评估并生效 (系列在首次实施隔离时开始，一旦解除隔离，就会重置) 。|
|error|[synchronizationError](synchronization-synchronizationerror.md)|描述将 () 隔离时发生的错误。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationQuarantine"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "currentBegan": "String (timestamp)",
  "nextAttempt": "String (timestamp)",
  "reason": "String",
  "seriesBegan": "String (timestamp)",
  "seriesCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


