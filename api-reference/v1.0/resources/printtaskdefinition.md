---
title: printTaskDefinition 资源类型
description: 表示在通用打印中发生各种事件时可以触发的任务。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 9a8a8c78d1e165dfe0f9417c5aa052f9f0b2383b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517313"
---
# <a name="printtaskdefinition-resource-type"></a>printTaskDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示在通用打印中发生各种事件时可以触发的任务的抽象定义。

有关如何使用此资源向通用打印添加拉页打印支持的详细信息，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。

该资源支持：
* [订阅更改通知](/graph/universal-print-webhook-notifications)。

## <a name="methods"></a>Methods
| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/print-list-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) 集合 | 获取在通用打印中创建的 printTaskDefinitions 的完整列表。 |
| [创建](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | 创建新的 printTaskDefinition。 |
| [更新](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | 更新 printTaskDefinition。 |
| [删除](../api/print-delete-taskdefinition.md) | 无 | 删除 printTaskDefinition。 |
| [列出任务](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | 获取已基于此定义创建的任务列表。 该列表包括当前运行的任务和最近完成的任务。 |
| [获取任务](../api/printtask-get.md) | [printTask](printtask.md) | 获取已基于此定义创建的任务。 |
| [更新任务](../api/printtaskdefinition-update-task.md) | [printTask](printtask.md) | 更新已基于此定义创建的任务。 **注册任务触发器的应用程序负责在处理完成后更新任务状态，除非相关 printJob 已重定向到另一台打印机。** 未能报告完成操作将导致相关打印作业被阻止打印并最终被删除。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|printTaskDefinition 的标识符。 只读。|
|displayName|String|printTaskDefinition 的名称。|
|createdBy|[appIdentity](appidentity.md)|创建 printTaskDefinition 的应用程序。 只读。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|tasks|[printTask](printtask.md) 集合|已基于此定义创建的任务列表。 该列表包括当前运行的任务和最近完成的任务。 只读。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.appIdentity"
  }
}
```

