---
title: 打印机资源类型
description: 表示已在通用打印服务中注册的物理打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: fab3e933608143846555c556a215025e39666257
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934868"
---
# <a name="printer-resource-type"></a>打印机资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示已在通用打印服务中注册的打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。

该资源支持：
* [订阅更改通知](/graph/universal-print-webhook-notifications)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | 创建 (通用) 新打印机进行注册。 |
| [获取](../api/printer-get.md) | [printer](printer.md) | 读取打印机对象的属性和关系。 |
| [更新](../api/printer-update.md) | [printer](printer.md) | 更新打印机对象。 |
| [删除](../api/printer-delete.md) | 无 | 从通用打印服务中注销物理打印机。 |
| [restoreFactoryDefaults](../api/printer-restorefactorydefaults.md) | 无 | 将打印机的默认设置还原到制造商指定的值。 |
| [列出作业](../api/printer-list-jobs.md) | [printJob](printjob.md) 集合 | 获取由打印机排队进行处理的打印作业的列表。 |
| [创建作业](../api/printer-post-jobs.md) | [printJob](printjob.md) | 为打印机创建新的打印作业。 若要开始打印作业，请使用"开始["。](../api/printjob-start.md) |
| [List connectors](../api/printer-list-connectors.md) | [printConnector](printconnector.md) 集合 | 获取与此打印机关联的连接器列表。 |
| [List taskTriggers](../api/printer-list-tasktriggers.md) | 无 | 列出[与此打印机关联的 printTaskTriggers。](printtasktrigger.md) |
| [Create taskTrigger](../api/printer-post-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) | 创建在打印事件发生时运行的[printTaskTrigger。](printtasktrigger.md) |
| [Delete taskTrigger](../api/printer-delete-tasktrigger.md) | 无 | 删除[与打印机关联的 printTaskTrigger。](printtasktrigger.md) |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|文档的标识符。 只读。|
|displayName|String|打印机的名称。|
|manufacturer|String|打印机报告的制造商。|
|model|String|打印机报告的型号名称。|
|registeredDateTime|DateTimeOffset|注册打印机时的日期时间Offset。 只读。|
|状态|[printerStatus](printerstatus.md)|打印机的处理状态，包括任何错误。|
|isShared|Boolean|如果共享打印机，则其为 True;否则为 false。 只读。|
|hasPhysicalDevice|Boolean|如此 如果打印机具有用于打印的物理设备。 只读。|
|isAcceptingJobs|Boolean|打印机当前是否接受新的打印作业。|
|location|[printerLocation](printerlocation.md)|打印机的物理和/或组织位置。|
|defaults|[printerDefaults](printerdefaults.md)|打印机的默认打印设置。|
|capabilities|[printerCapabilities](printercapabilities.md)|与此打印机共享关联的打印机的功能。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|jobs|[printJob](printjob.md) 集合| 由打印机排入打印队列的作业列表。|
|shares|[printerShare](printershare.md) 集合| 与打印机关联的 printerShares 列表。 目前，只能将一个 printerShare 与打印机关联。 只读。 可为 Null。|
|连接器|[printConnector](printconnector.md)|与打印机关联的连接器。|
|taskTriggers|[printTaskTrigger](printtasktrigger.md) 集合|与打印机关联的任务触发器列表。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printer",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isShared": true,
  "registeredDateTime": "String (timestamp)",
  "isAcceptingJobs": true,
  "hasPhysicalDevice": true,
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"},
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


