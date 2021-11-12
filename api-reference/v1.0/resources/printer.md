---
title: 打印机资源类型
description: 表示已在通用打印服务中注册的物理打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 1c88a70f642c02303104220b13aea1dc8fe09122
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60946879"
---
# <a name="printer-resource-type"></a>打印机资源类型

命名空间：microsoft.graph

表示已在通用打印服务中注册的打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。

该资源支持：
* [订阅更改通知](/graph/universal-print-webhook-notifications)。

继承自 [printerBase](../resources/printerbase.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
| [创建](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | 创建 (通用) 新打印机进行注册。 |
| [获取](../api/printer-get.md) | [打印机](printer.md) | 读取打印机对象的属性和关系。 |
| [更新](../api/printer-update.md) | [打印机](printer.md) | 更新打印机对象。 |
| [删除](../api/printer-delete.md) | 无 | 从通用打印服务中注销物理打印机。 |
| [restoreFactoryDefaults](../api/printer-restorefactorydefaults.md) | 无 | 将打印机的默认设置还原到制造商指定的值。 |
| [列出作业](../api/printer-list-jobs.md) | [printJob](printjob.md) 集合 | 获取已排队等待打印机处理的打印作业的列表。 |
| [创建作业](../api/printer-post-jobs.md) | [printJob](printjob.md) | 为打印机创建新的打印作业。 若要开始打印作业 [，请使用](../api/printjob-start.md)start 。 |
| [List connectors](../api/printer-list-connectors.md) | [printConnector](printconnector.md) 集合 | 获取与此打印机关联的连接器列表。 |
| [列出共享项](../api/printer-list-shares.md) | [printerShare](printerShare.md) 集合 | 获取与此打印机关联的 printerShares 列表。 目前，只有一个 printerShare 可以与打印机关联。 |
| [List taskTriggers](../api/printer-list-tasktriggers.md) | 无 | 列出[与此打印机关联的 printTaskTrigger。](printtasktrigger.md) |
| [Create taskTrigger](../api/printer-post-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) | 创建[在打印事件发生时运行的 printTaskTrigger。](printtasktrigger.md) |
| [Delete taskTrigger](../api/printer-delete-tasktrigger.md) | 无 | 删除[与打印机关联的 printTaskTrigger。](printtasktrigger.md) |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|文档的标识符。 继承自 [printerBase](../resources/printerbase.md)。 只读。|
|displayName|String|打印机的名称。 继承自 [printerBase](../resources/printerbase.md)。|
|manufacturer|String|打印机报告的制造商。 继承自 [printerBase](../resources/printerbase.md)。|
|model|String|打印机报告的型号名称。 继承自 [printerBase](../resources/printerbase.md)。|
|registeredDateTime|DateTimeOffset|注册打印机时的日期时间Offset。 只读。|
|status|[printerStatus](printerstatus.md)|打印机的处理状态，包括任何错误。 继承自 [printerBase](../resources/printerbase.md)。|
|isShared|Boolean|如果共享打印机，则其为 True;否则为 false。 只读。|
|hasPhysicalDevice|Boolean|如此 如果打印机具有用于打印的物理设备。 只读。|
|isAcceptingJobs|Boolean|打印机当前是否接受新的打印作业。 继承自 [printerBase](../resources/printerbase.md)。|
|位置|[printerLocation](printerlocation.md)|打印机的物理和/或组织位置。 继承自 [printerBase](../resources/printerbase.md)。|
|defaults|[printerDefaults](printerdefaults.md)|打印机的默认打印设置。 继承自 [printerBase](../resources/printerbase.md)。|
|capabilities|[printerCapabilities](printercapabilities.md)|与此打印机共享关联的打印机的功能。 继承自 [printerBase](../resources/printerbase.md)。|
|lastSeenDateTime|DateTimeOffset|打印机与通用打印交互时的最新 dateTimeOffset。 只读。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|jobs|[printJob](printjob.md) 集合| 由打印机排入打印队列的作业列表。  继承自 [printerBase](../resources/printerbase.md)。|
|shares|[printerShare](printershare.md) 集合| printerShares 与打印机关联的列表。 目前，只有一个 printerShare 可以与打印机关联。 只读。 可为 Null。|
|连接器|[printConnector](printconnector.md)|与打印机关联的连接器。|
|taskTriggers|[printTaskTrigger](printtasktrigger.md) 集合|与打印机关联的任务触发器列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printer",
  "baseType": "microsoft.graph.printerBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printer",
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isAcceptingJobs": "Boolean",
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  },
  "registeredDateTime": "String (timestamp)",
  "isShared": "Boolean",
  "hasPhysicalDevice": "Boolean",
  "lastSeenDateTime": "String (timestamp)"
}
```

