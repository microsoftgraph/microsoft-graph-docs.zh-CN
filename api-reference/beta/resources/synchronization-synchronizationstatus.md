---
title: synchronizationStatus 资源类型
description: 表示 synchronizationJob 的当前状态。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 179eda96e62c124de5c64688352040b62dfc6c77
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520028"
---
# <a name="synchronizationstatus-resource-type"></a>synchronizationStatus 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[synchronizationJob](synchronization-synchronizationjob.md)的当前状态。

## <a name="properties"></a>属性

| 属性                              | 类型      | 说明    |
|:--------------------------------------|:----------|:---------------|
|code|String|同步作业的高级别状态代码。 可取值为：`NotConfigured`、`NotRun`、`Active`、`Paused`、`Quarantine`。|
|countSuccessiveCompleteFailures|Int64|此作业连续失败的次数。|
|escrowsPruned|布尔|`true`在初始同步过程中，如果作业的 escrows （对象级错误）被修剪。 在初始同步过程中，可以对 Escrows 进行修剪，从而达到通常会将作业放入隔离的错误阈值。 同步过程不会进入隔离，而是清除作业的错误并继续，直到初始同步完成。 初始同步完成后，作业将暂停，并等待客户清除错误。|
|lastExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|上次执行作业的详细信息。|
|lastSuccessfulExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|此作业的最后一次执行的详细信息，其中未包含任何错误。|
|lastSuccessfulExecutionWithExports|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|上次执行作业的详细信息，该作业将对象导出到目标目录中。|
|progress|[synchronizationProgress](synchronization-synchronizationprogress.md)集合|完成作业进度的详细信息。|
|隔离|[synchronizationQuarantine](synchronization-quarantine.md)|如果作业在隔离中，则隔离详细信息。|
|steadyStateFirstAchievedTime|DateTimeOffset|稳定状态（不再对进程所做的更改）第一次实现的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|steadyStateLastAchievedTime|DateTimeOffset|上次达到稳定状态（不再对进程所做的更改）的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|synchronizedEntryCountByType|[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)集合|按对象类型列出的已同步对象的计数。|
|troubleshootingUrl|String|出现错误时，将包含问题的故障排除步骤的 URL。|

### <a name="synchronization-status-code-details"></a>同步状态代码详细信息

| 值                              | 说明    |
|:-----------------------------------|:---------------|
|NotConfigured                       |作业未配置且从未运行。 未提供任何授权。 |
|NotRun                              |作业已配置且可能已启动，但尚未完成其第一次运行。|
|活动                              |作业正在定期运行。|
|暂停                              |作业已暂停（通常由管理员执行），当前未在运行，但保留作业的状态。|
|Quarantine                          |作业处于隔离中。 当出现大量错误或严重错误（如已吊销/已过期的凭据）时，可能会发生这种情况。 在隔离过程中，同步过程将尝试以降低的频率运行作业。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
}-->

```json
{
  "code": "String",
  "countSuccessiveCompleteFailures": 1024,
  "escrowsPruned": true,
  "lastExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecutionWithExports": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "progress": [{"@odata.type": "microsoft.graph.synchronizationProgress"}],
  "quarantine": {"@odata.type": "microsoft.graph.synchronizationQuarantine"},
  "steadyStateFirstAchievedTime": "String (timestamp)",
  "steadyStateLastAchievedTime": "String (timestamp)",
  "synchronizedEntryCountByType": [{"@odata.type": "microsoft.graph.stringKeyLongValuePair"}],
  "troubleshootingUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
