---
title: dataSourceContainer 资源类型
description: 保管人和非保管数据源的基类。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 36039c4e548b8db771cacb97c0adbb3c5361729c
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839191"
---
# <a name="datasourcecontainer-resource-type"></a>dataSourceContainer 资源类型

命名空间：microsoft.graph.security



[eDiscoveryCustodian](../resources/security-ediscoverycustodian.md) 和 [eDiscoveryNonCutodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) 资源的基类。

这是一种抽象类型。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>方法

无。
## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|dataSourceContainer 的保留状态。 可能的值为： `notApplied`， `applied`， `applying`， `removing``partial`|
|createdDateTime|DateTimeOffset|创建 dataSourceContainer 实体的日期和时间。|
|displayName|String|dataSourceContainer 实体的显示名称。|
|id|String|dataSourceContainer 的唯一标识符。 继承自 [实体](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|dataSourceContainer 的上次修改日期和时间。|
|releasedDateTime|DateTimeOffset|DataSourceContainer 从案例中释放的日期和时间。|
|status|microsoft.graph.security.dataSourceContainerStatus|dataSourceContainer 的最新状态。 可取值为：`Active`、`Released`。|

### <a name="datasourcecontainerstatus-values"></a>dataSourceContainerStatus 值

|成员|说明|
|:----|-----------|
| 积极| 数据源容器处于活动状态。|
| 释放 | 数据源容器已发布。|

### <a name="datasourceholdstatus-values"></a>dataSourceHoldStatus 值

|成员|说明|
|:----|-----------|
| notApplied | 数据源容器未处于保留状态。|
| 应用 | 数据源容器处于保留状态。|
| 应用 | 数据源容器在应用保留状态 (已触发的 applyHold 操作) 。|
| 删除 | 数据源容器正在删除 () 触发的 removeHold 操作的保留状态。|
| 部分 | 数据源容器处于混合状态，其中某些源处于保留状态，有些源未处于保留或错误状态。|
## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.dataSourceContainer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.dataSourceContainer",
  "id": "String (identifier)",
  "status": "String",
  "holdStatus": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

