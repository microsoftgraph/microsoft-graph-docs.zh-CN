---
title: printJob 资源类型
description: 表示已排入打印机队列的打印作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 170f413c7607933c2651720c9c9c463f90cf55df
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516526"
---
# <a name="printjob-resource-type"></a>printJob 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示已排入打印机队列的打印作业。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取](../api/printjob-get.md) | [printJob](printjob.md) | 读取 printJob 对象的属性和关系。 |
| [创建](../api/printer-post-jobs.md) | [printJob](printjob.md) | 创建新的打印作业对象。 |
| [更新](../api/printjob-update.md) | [printJob](printjob.md) | 更新打印作业对象。 |
| [开始](../api/printjob-start.md)|无|启动打印作业。|
| [Cancel](../api/printjob-cancel.md)|无|取消打印作业。|
| [中止](../api/printjob-abort.md)|无|中止打印作业。|
| [将 (重定向到另一个打印机) ](../api/printjob-redirect.md) | [printJob](printjob.md) | 已排入目标打印机队列的打印作业。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|打印机的 GUID。 只读。|
|createdDateTime|DateTimeOffset|创建作业时的日期时间Offset。 只读。|
|状态|[printJobStatus](printjobstatus.md)|打印作业的状态。 只读。|
|configuration|[printJobConfiguration](printJobConfiguration.md)|打印机用于打印作业的一组设置。|
|isFetchable|Edm.Boolean|如果为 true，则打印机可以提取文档。|
|redirectedFrom|Edm.String|包含源作业 URL（如果作业已从另一台打印机重定向）。|
|redirectedTo|Edm.String|如果作业已重定向到另一台打印机，则包含目标作业 URL。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|createdBy|[userIdentity](useridentity.md)| 只读。 可为 NULL。|
|documents|[printDocument](printdocument.md) 集合| 只读。|
|tasks|[printTask](printtask.md) 集合|此打印作业触发的 [printTasks](printtask.md) 列表。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJob",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "isFetchable": "Boolean",
  "redirectedFrom": "String",
  "redirectedTo": "String",
  "status": {"@odata.type": "microsoft.graph.printJobStatus"},
  "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
  "configuration": {"@odata.type": "microsoft.graph.printJobConfiguration"},
  "documents": [ {"@odata.type": "microsoft.graph.printDocument"} ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

