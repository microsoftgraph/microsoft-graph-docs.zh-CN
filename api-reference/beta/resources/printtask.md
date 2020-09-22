---
title: printTask 资源类型
description: 表示正在执行或已作为通用 Print 事件的结果执行的任务。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: fb41bc68112aa04e1eea825d45982f2f3f0db48c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973790"
---
# <a name="printtask-resource-type"></a>printTask 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示正在执行或已作为通用 Print 事件的结果执行的任务。

有关如何使用此资源将拉取打印支持添加到通用打印的详细信息，请参阅 [扩展通用打印以支持 pull 打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [从 printTaskDefintion 中列出 () ](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | 获取基于特定 printTaskDefinition 创建的任务的列表。 该列表包含当前正在运行的任务和最近完成的任务。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|PrintTask 的标识符。 只读。|
|状态|[printTaskStatus](printtaskstatus.md)|此 printTask 的当前执行状态。 **在处理完成时，调用应用程序负责更新此状态，除非相关的 printJob 已重定向到另一台打印机。** 若未能报告完成，则会导致相关打印作业被阻止打印，并最终删除。 |
|parentUrl|String|触发此任务的打印实体的 URL。 例如，`https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`。 只读。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|触发|[printTaskTrigger](printtasktrigger.md)|触发此任务的执行的 printTaskTrigger。 只读。|
|定义|[printTaskDefinition](printtaskdefinition.md)|用于创建此任务的 printTaskDefinition。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTask",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "status": {"@odata.type": "microsoft.graph.printTaskStatus"},
  "parentUrl": "String",
  "trigger": {"@odata.type": "microsoft.graph.printTaskTrigger"},
  "definition": {"@odata.type": "microsoft.graph.printTaskDefinition"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


