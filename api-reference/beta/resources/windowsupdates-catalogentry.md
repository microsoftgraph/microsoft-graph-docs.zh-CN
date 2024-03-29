---
title: catalogEntry 资源类型
description: 您可以批准部署的内容段的元数据。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 2e81fd688dde08522ff59322444b1c1cd0646054
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792132"
---
# <a name="catalogentry-resource-type"></a>catalogEntry 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以批准部署的内容段的元数据。

所有目录条目作为以下派生类型之一存在 [：featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) 和 [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md)。

[softwareUpdateCatalogEntry 的基类型](../resources/windowsupdates-softwareupdatecatalogentry.md)。

这是一个抽象类型。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|使用该服务不再提供内容部署的日期。 只读。|
|displayName|String|内容的显示名称。 只读。|
|id|String|目录项的唯一标识符。 只读。|
|releaseDateTime|DateTimeOffset|内容的发布日期。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.catalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.catalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)"
}
```

