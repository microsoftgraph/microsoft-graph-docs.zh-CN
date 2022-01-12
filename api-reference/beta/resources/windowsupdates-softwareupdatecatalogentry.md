---
title: softwareUpdateCatalogEntry 资源类型
description: 可以批准部署的软件更新的元数据。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 7103fbb2f6ed62cec5a5e530a10e190ea46067e0
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61862774"
---
# <a name="softwareupdatecatalogentry-resource-type"></a>softwareUpdateCatalogEntry 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以批准部署的软件更新的元数据。

继承自 [catalogEntry](../resources/windowsupdates-catalogentry.md)。 [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md)和[qualityUpdateCatalogEntry 的基类型](../resources/windowsupdates-qualityupdatecatalogentry.md)。

这是一个抽象类型。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|内容不再可用于使用服务部署的日期。 只读。 继承自 [catalogEntry](../resources/windowsupdates-catalogentry.md)。|
|displayName|String|内容的显示名称。 只读。 继承自 [catalogEntry](../resources/windowsupdates-catalogentry.md)。|
|id|String|目录项的唯一标识符。 只读。 继承自 [catalogEntry](../resources/windowsupdates-catalogentry.md)。|
|releaseDateTime|DateTimeOffset|内容的发布日期。 只读。 继承自 [catalogEntry](../resources/windowsupdates-catalogentry.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.catalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)"
}
```

