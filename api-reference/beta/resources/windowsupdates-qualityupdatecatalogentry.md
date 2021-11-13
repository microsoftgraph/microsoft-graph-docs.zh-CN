---
title: qualityUpdateCatalogEntry 资源类型
description: 可以批准Windows 10质量更新的元数据。
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 23301d5de5d089ed47dc884ad62a88b0660cd0ec
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891177"
---
# <a name="qualityupdatecatalogentry-resource-type"></a>qualityUpdateCatalogEntry 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以批准Windows 10质量更新的元数据。

Windows 10质量更新每月发布一次或多次。 这些更新包含安全和质量修补程序，并且通常在每个月的第二个星期二发布，尽管它们可能随时发布。 这些更新是累积更新，因此更高版本始终包含所有以前的修补程序。 Microsoft 强烈建议在设备可用时立即安装最新质量更新，使设备保持最新状态。 

继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|内容不再可用于使用服务部署的日期。 只读。 继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。|
|displayName|String|内容的显示名称。 只读。 继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。|
|id|String|目录项的唯一标识符。 只读。 继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。|
|isExpeditable|Boolean|指示内容是否可以部署为快速质量更新。 只读。|
|qualityUpdateClassification|microsoft.graph.windowsUpdates.qualityUpdateClassification|质量更新的分类。 可取值为：`all`、`security`、`nonSecurity`、`unknownFutureValue`。 只读。|
|releaseDateTime|DateTimeOffset|内容的发布日期。 只读。 继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)",
  "isExpeditable": "Boolean",
  "qualityUpdateClassification": "String"
}
```

