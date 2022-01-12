---
title: qualityUpdateCatalogEntry 资源类型
description: 您可以批准Windows 10更新的元数据。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: bdac770931e6986ac4233bf32d0eb82bc9a08be4
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61863010"
---
# <a name="qualityupdatecatalogentry-resource-type"></a>qualityUpdateCatalogEntry 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以批准Windows 10更新的元数据。

Windows 10质量更新每月发布一次或多次。 这些更新包含安全和质量修补程序，并且通常在每个月的第二个星期二发布，尽管它们可能随时发布。 这些更新是累积更新，因此更高版本始终包含所有以前的修补程序。 Microsoft 强烈建议在设备可用时立即安装最新质量更新，使设备保持最新状态。 

继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|内容不再可用于使用服务部署的日期。 只读。 继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。|
|displayName|String|内容的显示名称。 只读。 继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。|
|id|String|目录项的唯一标识符。 只读。 继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。|
|isExpeditable|布尔|指示内容是否可以部署为快速质量更新。 只读。|
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

