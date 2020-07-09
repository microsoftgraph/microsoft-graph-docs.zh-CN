---
title: printTaskDefinition 资源类型
description: 表示在通用打印中发生各种事件时可触发的任务。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 013d2756455abebc0f20bbe5a1d186a0a4d65648
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091576"
---
# <a name="printtaskdefinition-resource-type"></a>printTaskDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在通用打印中发生各种事件时可触发的任务的抽象定义。

有关如何使用此资源将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持 pull 打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [List](../api/print-list-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md)集合 | 获取在通用打印中创建的 printTaskDefinitions 的完整列表。 |
| [创建](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | 创建新的 printTaskDefinition。 |
| [更新](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | 更新 printTaskDefinition。 |
| [删除](../api/print-delete-taskdefinition.md) | 无 | 删除 printTaskDefinition。 |
| [List tasks](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | 获取基于此定义创建的任务的列表。 该列表包含当前正在运行的任务和最近完成的任务。 |
| [获取任务](../api/printtask-get.md) | [printTask](printtask.md) | 获取已基于此定义创建的任务。 |
| [更新任务](../api/printtaskdefinition-update-task.md) | 无 | 更新基于此定义创建的任务。 **注册任务触发器的应用程序负责在处理完成后更新任务状态，除非相关的 printJob 已重定向到另一台打印机。** 若未能报告完成，则会导致相关打印作业被阻止打印，并最终删除。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|PrintTaskDefinition 的标识符。 只读。|
|displayName|String|PrintTaskDefinition 的名称。|
|createdBy|[appIdentity](appidentity.md)|创建 printTaskDefinition 的应用程序。 只读。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|tasks|[printTask](printtask.md)集合|基于此定义创建的任务的列表。 该列表包含当前正在运行的任务和最近完成的任务。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {"@odata.type": "microsoft.graph.appIdentity"},
  "tasks": [{"@odata.type": "microsoft.graph.printTask"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->