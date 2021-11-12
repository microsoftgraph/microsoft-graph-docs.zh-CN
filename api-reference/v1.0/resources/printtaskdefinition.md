---
title: printTaskDefinition 资源类型
description: 表示可在通用打印中发生各种事件时触发的任务。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d1173cfe72aacce5f422dc47c49f557e373c1ce2
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60924192"
---
# <a name="printtaskdefinition-resource-type"></a>printTaskDefinition 资源类型

命名空间：microsoft.graph

表示在通用打印中发生各种事件时可以触发的任务的抽象定义。

有关如何使用此资源向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持下拉打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。

该资源支持：
* [订阅更改通知](/graph/universal-print-webhook-notifications)。

## <a name="methods"></a>Methods
| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/print-list-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) 集合 | 获取在通用打印中创建的 printTaskDefinitions 的完整列表。 |
| [创建](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | 创建新的 printTaskDefinition。 |
| [更新](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | 更新 printTaskDefinition。 |
| [删除](../api/print-delete-taskdefinition.md) | 无 | 删除 printTaskDefinition。 |
| [List tasks](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | 获取基于此定义创建的任务列表。 该列表包括当前运行的任务和最近完成的任务。 |
| [获取任务](../api/printtask-get.md) | [printTask](printtask.md) | 获取已基于此定义创建的任务。 |
| [更新任务](../api/printtaskdefinition-update-task.md) | [printTask](printtask.md) | 更新基于此定义创建的任务。 **注册任务触发器的应用程序负责在处理完成后更新任务状态，除非相关 printJob 已重定向到另一台打印机。** 如果未能报告完成，将导致相关打印作业被阻止打印并最终被删除。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|printTaskDefinition 的标识符。 只读。|
|displayName|String|printTaskDefinition 的名称。|
|createdBy|[appIdentity](appidentity.md)|创建 printTaskDefinition 的应用程序。 只读。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|tasks|[printTask](printtask.md) 集合|基于此定义创建的任务列表。 该列表包括当前运行的任务和最近完成的任务。 只读。|

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

