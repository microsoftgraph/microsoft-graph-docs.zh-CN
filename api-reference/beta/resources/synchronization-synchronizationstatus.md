---
title: synchronizationStatus 资源类型
description: 表示 synchronizationJob 的当前状态。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 86320e6af31dae39f86ebe87f8490e24c7c33f57
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722053"
---
# <a name="synchronizationstatus-resource-type"></a>synchronizationStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [synchronizationJob](synchronization-synchronizationjob.md)的当前状态。

## <a name="properties"></a>属性

| 属性                              | 类型      | 说明    |
|:--------------------------------------|:----------|:---------------|
|code|String|同步作业的高级别状态代码。 可取值为：`NotConfigured`、`NotRun`、`Active`、`Paused`、`Quarantine`。|
|countSuccessiveCompleteFailures|Int64|此作业失败的连续次数。|
|escrowsPruned|布尔|`true` 如果作业的托管 (对象级错误) 在初始同步期间被修剪。 如果在初始同步期间达到通常将作业置于隔离状态的错误阈值，则可能会删除托管。 同步过程不会进入隔离区，而是清除作业的错误，并继续进行，直到初始同步完成。 初始同步完成后，作业将暂停并等待客户清理错误。|
|lastExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|上次执行作业的详细信息。|
|lastSuccessfulExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|上次执行此作业的详细信息，没有任何错误。|
|lastSuccessfulExecutionWithExports|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|上次执行作业的详细信息，该作业将对象导出到目标目录中。|
|progress|[synchronizationProgress](synchronization-synchronizationprogress.md) 集合|作业完成进度的详细信息。|
|隔离|[synchronizationQuarantine](synchronization-quarantine.md)|如果作业位于隔离区中，则隔离详细信息。|
|steadyStateFirstAchievedTime|DateTimeOffset|首次实现稳定状态 (对进程没有) 的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|steadyStateLastAchievedTime|DateTimeOffset|上次达到稳定 (对进程更改) 的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|synchronizedEntryCountByType|[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) 集合|同步对象计数，按对象类型。|
|troubleshootingUrl|String|如果出现错误，URL 将包含问题的疑难解答步骤。|

### <a name="synchronization-status-code-details"></a>同步状态代码详细信息

| 值                              | 说明    |
|:-----------------------------------|:---------------|
|NotConfigured                       |未配置作业，并且从不运行。 未提供授权。 |
|NotRun                              |作业已配置，可能已启动，但尚未完成首次运行。|
|活动                              |作业定期运行。|
|暂停                              |作业已暂停 (管理员) 当前未运行，但作业的状态将保留。|
|隔离                          |作业被隔离。 当存在大量错误或严重错误（如吊销/过期的凭据）时，可能会发生这种情况。 隔离时，同步过程将尝试以降低的频率运行作业。|

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


