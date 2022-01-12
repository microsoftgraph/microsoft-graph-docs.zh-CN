---
title: featureUpdateCatalogEntry 资源类型
description: 您可以批准Windows 10部署的功能更新的元数据。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 94403127fdbc8c263df546c2dfd1359c87894a06
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861639"
---
# <a name="featureupdatecatalogentry-resource-type"></a>featureUpdateCatalogEntry 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以批准Windows 10部署的功能更新的元数据。

Windows 10功能更新每两年发布一次，其中包含适用于Windows 10。 安装这些更新会增加Windows 10内部版本数，并且通常会导致新的服务生命周期和服务结束日期。 Microsoft 建议组织定期部署新功能更新，作为采用新Windows 即服务。

继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|内容不再可用于使用服务部署的日期。 只读。 继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。|
|displayName|String|内容的显示名称。 只读。 继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。|
|id|String|目录项的唯一标识符。 只读。 继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。|
|releaseDateTime|DateTimeOffset|内容的发布日期。 只读。 继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。|
|version|String|功能更新的版本。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)",
  "version": "String"
}
```

