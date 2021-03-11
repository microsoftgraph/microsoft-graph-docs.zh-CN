---
title: synchronizationTaskExecution 资源类型
description: 汇总同步作业运行的结果。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d83092949e1f27c9dac9744d2b4b16be4bcbae0d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722046"
---
# <a name="synchronizationtaskexecution-resource-type"></a>synchronizationTaskExecution 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

汇总同步作业运行的结果。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|activityIdentifier           |String |作业运行的标识符。|
|countEntitled                |Int64  |为此应用程序分配的已处理条目计数。|
|countEntitledForProvisioning |Int64  |已分配用于预配的已处理条目计数。|
|countEscrowed                |Int64  |托管的条目数 (错误) 。|
|countEscrowedRaw             |Int64  |托管的条目计数，包括系统生成的托管。|
|countExported                |Int64  |导出条目的计数。|
|countExports                 |Int64  |预期要导出的条目计数。|
|countImported                |Int64  |导入的条目计数。|
|countImportedDeltas          |Int64  |导入的增量更改计数。|
|countImportedReferenceDeltas |Int64  |与引用更改相关的导入增量更改计数。|
|error                        |[synchronizationError](synchronization-synchronizationerror.md)|如果遇到错误，则包含 **包含详细信息的 synchronizationError** 对象。|
|state                        |String |汇总此运行结果的代码。 可取值为：`Succeeded`、`Failed`、`EntryLevelErrors`。|
|timeBegan                    |DateTimeOffset|此作业运行开始的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|timeEnded                    |DateTimeOffset|此作业运行结束的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|

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


