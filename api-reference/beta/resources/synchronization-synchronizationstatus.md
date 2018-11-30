---
title: synchronizationStatus 资源类型
description: 代表 synchronizationJob 的当前状态。
ms.openlocfilehash: cf1b1e79e5ad784f1f43a2e5bf082c68b41e96ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049415"
---
# <a name="synchronizationstatus-resource-type"></a>synchronizationStatus 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表[synchronizationJob](synchronization-synchronizationjob.md)的当前状态。

## <a name="properties"></a>属性

| 属性                              | 类型      | 说明    |
|:--------------------------------------|:----------|:---------------|
|code|字符串|高级状态代码的同步作业。 可取值为：`NotConfigured`、`NotRun`、`Active`、`Paused`、`Quarantine`。|
|countSuccessiveCompleteFailures|Int64|连续次数此作业失败。|
|escrowsPruned|布尔|`true`如果在初始同步期间已修剪作业的 escrows （对象级错误）。 如果在初始同步过程达到阈值通常会将作业放在隔离的错误，则可以修剪 escrows。 而不是进入隔离，同步过程清除作业的错误，并将继续，直到完成初始同步。 完成初始同步后，此作业将暂停并等待客户清理错误。|
|lastExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|上次执行作业的详细信息。|
|lastSuccessfulExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|上次执行此作业，没有任何错误的详细信息。|
|lastSuccessfulExecutionWithExports|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|导出到目标目录的对象的作业的上次执行的详细信息。|
|进度|[synchronizationProgress](synchronization-synchronizationprogress.md)集合|完成作业的进度的详细信息。|
|隔离|[synchronizationQuarantine](synchronization-quarantine.md)|如果作业在隔离，隔离详细信息。|
|steadyStateFirstAchievedTime|DateTimeOffset|首先达到稳定状态 （过程没有更多更改） 时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|steadyStateLastAchievedTime|DateTimeOffset|上次达到稳定状态 （过程没有更多更改） 时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|synchronizedEntryCountByType|[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)集合|按对象类型列出的同步对象数。|
|troubleshootingUrl|字符串|发生错误，带有问题的疑难解答步骤的 URL。|

### <a name="synchronization-status-code-details"></a>同步状态代码的详细信息

| 值                              | 说明    |
|:-----------------------------------|:---------------|
|NotConfigured                       |作业已未配置，永远不会运行。 提供未授权。 |
|NotRun                              |作业已配置并可能启动，但尚未完成其第一个域。|
|活跃                              |定期运行作业。|
|暂停                              |作业已暂停 （通常是由管理员） 和当前未运行，但保留作业的状态。|
|隔离                          |作业处于隔离。 有大量的错误，或者关键错误，例如吊销过期凭据时，可能发生此错误。 在隔离中同步过程将尝试减少频率运行作业。|

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
