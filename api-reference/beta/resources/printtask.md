---
title: printTask 资源类型
description: 表示由于通用 Print 事件而正在执行或已执行的任务。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c684ff64aa4c3667214b61b70a422690381525b3
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766299"
---
# <a name="printtask-resource-type"></a>printTask 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示由于通用 Print 事件而正在执行或已执行的任务。

有关如何使用此资源向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持下拉打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 (printTaskDefintion) ](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | 获取基于特定 printTaskDefinition 创建的任务列表。 该列表包括当前运行的任务和最近完成的任务。 |
| [Get](../api/printtask-get.md) | [printTask](printtask.md) | 获取有关打印任务的详细信息。 |
| [更新](../api/printtaskdefinition-update-task.md) | [printTask](printtask.md) | 更新打印任务。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|printTask 的标识符。 只读。|
|状态|[printTaskStatus](printtaskstatus.md)|此 printTask 的当前执行状态。 **除非相关 printJob 已重定向到另一台打印机，否则调用应用程序负责在处理完成时更新此状态。** 如果未能报告完成，将导致相关打印作业被阻止打印并最终被删除。 |
|parentUrl|String|触发此任务的打印实体的 URL。 例如，`https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`。 只读。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|trigger|[printTaskTrigger](printtasktrigger.md)|触发此任务执行的 printTaskTrigger。 只读。|
|definition|[printTaskDefinition](printtaskdefinition.md)|用于创建此任务的 printTaskDefinition。 只读。|

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


