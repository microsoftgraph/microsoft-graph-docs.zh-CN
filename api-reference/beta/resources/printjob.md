---
title: printJob 资源类型
description: 代表已对打印机排队的打印作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2c0a1bdb4ec3ebe3c87b5b40595d30cf9108c5bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048735"
---
# <a name="printjob-resource-type"></a>printJob 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表已对打印机排队的打印作业。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取](../api/printjob-get.md) | [printJob](printjob.md) | 读取 printJob 对象的属性和关系。 |
| [创建](../api/printer-post-jobs.md) | [printJob](printjob.md) | 创建新的打印作业对象。 |
| [开始](../api/printjob-startprintjob.md)|无|启动打印作业。|
| [Cancel](../api/printjob-cancelprintjob.md)|无|取消打印作业。|
| [将 (重定向到另一台打印机) ](../api/printjob-redirect.md) | [printJob](printjob.md) | 排队等候目标打印机的打印作业。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|打印机的 GUID。 只读。|
|createdDateTime|DateTimeOffset|创建作业时的 DateTimeOffset。 只读。|
|状态|[printJobStatus](printjobstatus.md)|打印作业的状态。 只读。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|createdBy|[userIdentity](useridentity.md)| 只读。 可为 Null。|
|单据|[printDocument](printdocument.md) 集合| 只读。|
|tasks|[printTask](printtask.md) 集合|此打印作业触发的 [printTasks](printtask.md) 的列表。|

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
  "status": {"@odata.type": "microsoft.graph.printJobStatus"},
  "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
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

