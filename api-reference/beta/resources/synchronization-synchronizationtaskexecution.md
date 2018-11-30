---
title: synchronizationTaskExecution 资源类型
description: 总结了运行同步作业的结果。
ms.openlocfilehash: 4aefba4bdf9ab850892344e6e34683e81d1a1afa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045243"
---
# <a name="synchronizationtaskexecution-resource-type"></a>synchronizationTaskExecution 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

总结了运行同步作业的结果。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|activityIdentifier           |字符串 |运行作业的标识符。|
|countEntitled                |Int64  |处理已分配为此应用程序的条目数。|
|countEntitledForProvisioning |Int64  |处理已分配的资源调配的条目数。|
|countEscrowed                |Int64  |保管 （错误） 的条目数。|
|countEscrowedRaw             |Int64  |已保管，包括 escrows 系统生成的条目数。|
|countExported                |Int64  |导出的条目数。|
|countExports                 |Int64  |预计要导出的条目数。|
|countImported                |Int64  |导入的项目数。|
|countImportedDeltas          |Int64  |导入的增量更改的计数。|
|countImportedReferenceDeltas |Int64  |导入增量-更改与引用更改的计数。|
|error                        |[synchronizationError](synchronization-synchronizationerror.md)|如果遇到错误，将包含一个**synchronizationError**详细信息。|
|状态                        |字符串 |汇总结果的此次运行的代码。 可取值为：`Succeeded`、`Failed`、`EntryLevelErrors`。|
|timeBegan                    |DateTimeOffset|开始此作业的运行时的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|timeEnded                    |DateTimeOffset|结束此作业的运行时的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->