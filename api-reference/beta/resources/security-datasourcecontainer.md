---
title: dataSourceContainer 资源类型
description: 保管人和非保管数据源的基类。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 7482e31ab1a43cf4c60e7c211acb38d8cac42bfa
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945318"
---
# <a name="datasourcecontainer-resource-type"></a>dataSourceContainer 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[eDiscoveryCustodian](../resources/security-ediscoverycustodian.md) 和 [eDiscoveryNonCutodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) 的基类这是一种抽象类型。
继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>方法

无。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|holdStatus|String|dataSourceContainer 的保留状态。可能的值为： `notApplied`， ， `applied`， `applying`， `removing``partial`|
|createdDateTime|DateTimeOffset|创建 dataSourceContainer 实体的日期和时间。|
|displayName|String|dataSourceContainer 实体的显示名称。|
|id|String|dataSourceContainer 的唯一标识符。 继承自 [实体](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|dataSourceContainer 的上次修改日期和时间。|
|releasedDateTime|DateTimeOffset|DataSourceContainer 从案例中释放的日期和时间。|
|status|String|dataSourceContainer 的最新状态。 可取值为：`Active`、`Released`。|

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

