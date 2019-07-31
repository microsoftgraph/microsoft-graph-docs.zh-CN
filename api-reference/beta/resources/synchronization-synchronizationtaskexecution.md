---
title: synchronizationTaskExecution 资源类型
description: 概述同步作业的运行结果。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4e5a863111861d78b8a4131b68b8637b005aba49
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007751"
---
# <a name="synchronizationtaskexecution-resource-type"></a>synchronizationTaskExecution 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

概述同步作业的运行结果。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|activityIdentifier           |String |作业运行的标识符。|
|countEntitled                |Int64  |为此应用程序分配的已处理项的计数。|
|countEntitledForProvisioning |Int64  |为设置分配的已处理项的计数。|
|countEscrowed                |Int64  |Escrowed (错误) 的项的计数。|
|countEscrowedRaw             |Int64  |Escrowed 的条目数, 包括系统生成的 escrows。|
|countExported                |Int64  |已导出条目的计数。|
|countExports                 |Int64  |预期要导出的条目数。|
|countImported                |Int64  |导入的条目数。|
|countImportedDeltas          |Int64  |导入的增量更改的计数。|
|countImportedReferenceDeltas |Int64  |与引用更改相关的导入的 delta 更改的计数。|
|error                        |[synchronizationError](synchronization-synchronizationerror.md)|如果遇到错误, 则包含包含详细信息的**synchronizationError**对象。|
|state                        |String |对此运行的结果进行汇总的代码。 可取值为：`Succeeded`、`Failed`、`EntryLevelErrors`。|
|timeBegan                    |DateTimeOffset|开始运行此作业的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|timeEnded                    |DateTimeOffset|此作业运行结束的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTaskExecution"
}-->

```json
{
  "activityIdentifier": "String",
  "countEntitled": 1024,
  "countEntitledForProvisioning": 1024,
  "countEscrowed": 1024,
  "countEscrowedRaw": 1024,
  "countExported": 1024,
  "countExports": 1024,
  "countImported": 1024,
  "countImportedDeltas": 1024,
  "countImportedReferenceDeltas": 1024,
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "state": "String",
  "timeBegan": "String (timestamp)",
  "timeEnded": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
