---
title: 目录资源类型
description: 表示可以批准部署的内容目录的实体。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3fc0630a36d123e6c3e208838d81ee7c33c62853
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067981"
---
# <a name="catalog-resource-type"></a>目录资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可以批准部署的内容目录的实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表条目](../api/windowsupdates-catalog-list-entries.md)|[microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md) 集合|从条目导航属性获取 [catalogEntry](../resources/windowsupdates-catalogentry.md) 资源。 返回 **以下派生类型的 catalogEntry** 资源 [：featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) [、qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md)。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|目录的标识符。 只读。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|条目|[microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md) 集合|列出可以批准部署的内容。 只读。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.catalog",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.catalog",
  "id": "String (identifier)"
}
```

