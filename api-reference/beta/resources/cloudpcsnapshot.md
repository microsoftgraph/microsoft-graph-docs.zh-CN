---
title: cloudPcSnapshot 资源类型
description: 表示云电脑快照。
author: xintaozMS
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 14cf7ecffe7980db32abf81d475f45ac5725c64c
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878772"
---
# <a name="cloudpcsnapshot-resource-type"></a>cloudPcSnapshot 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可用于还原设备系统的云电脑的设备设置的快照。


继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列表快照](../api/virtualendpoint-list-snapshots.md)|[cloudPcSnapshot](../resources/cloudpcsnapshot.md) 集合|获取 [cloudPcSnapshot 对象](../resources/cloudpcsnapshot.md) 及其属性的列表。|
|[获取 cloudPcSnapshot](../api/cloudpcsnapshot-get.md)|[cloudPcSnapshot](../resources/cloudpcsnapshot.md)|读取 [cloudPcSnapshot 对象的属性和](../resources/cloudpcsnapshot.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|cloudPcId|String|云电脑的唯一标识符。|
|createdDateTime|DateTimeOffset|拍摄快照的日期和时间。 时间戳以 ISO 8601 格式显示，协调世界时 (UTC) 。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|id|String|特定时间点云电脑设备快照的唯一标识符。 继承自 [实体](../resources/entity.md)。|
|lastRestoredDateTime|DateTimeOffset|上次使用快照还原云电脑设备的日期和时间。 时间戳以 ISO 8601 格式显示，协调世界时 (UTC) 。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|状态|[cloudPcSnapshotStatus](#cloudpcsnapshotstatus-values)|云电脑快照的状态。 可能的值是：、`ready``unknownFutureValue`。|

### <a name="cloudpcsnapshotstatus-values"></a>cloudPcSnapshotStatus 值 

|成员|说明|
|:---|:---|
|ready|快照已准备好还原云电脑设备。|
|unknownFutureValue|可发展枚举 sentinel 值。 请勿使用。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcSnapshot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSnapshot",
  "cloudPcId": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastRestoredDateTime": "String (timestamp)",
  "status": "String"
}
```

