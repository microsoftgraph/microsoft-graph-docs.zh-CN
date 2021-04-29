---
title: dataSourceContainer 资源类型
description: 保管人和非保管人数据源的基类。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e2d7d88a3d747817858853ebc6f2909b2edde65b
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080749"
---
# <a name="datasourcecontainer-resource-type"></a>dataSourceContainer 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

保管人[和非](../resources/ediscovery-custodian.md)[custodialDataSource 的基类](../resources/ediscovery-noncustodialdatasource.md)。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法

无

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|dataSourceContainer 实体的创建日期和时间。|
|displayName|String|dataSourceContainer 实体的显示名称。|
|id|String|dataSourceContainer 的唯一标识符。 继承自 [实体](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|dataSourceContainer 的上次修改日期和时间。|
|releasedDateTime|DateTimeOffset|从案例发布 dataSourceContainer 的日期和时间。|
|状态|microsoft.graph.ediscovery.dataSourceContainerStatus|dataSourceContainer 的最新状态。 可取值为：`Active`、`Released`。|

### <a name="datasourcecontainerstatus-values"></a>dataSourceContainerStatus 值

|成员|说明|
|:---|:---|
|活动|在这种情况下，dataSourceContainer 将保留。|
|已发布|在这种情况下，dataSourceContainer 从保留中释放。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.dataSourceContainer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.dataSourceContainer",
  "id": "String (identifier)",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
