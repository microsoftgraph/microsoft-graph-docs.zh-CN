---
title: resourceConnection 资源类型
description: 表示要从中派生更多专用连接的外部资源的连接。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: dd21fba95209dbcc1ce5f868b98fa818fe34b254
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856707"
---
# <a name="resourceconnection-resource-type"></a>resourceConnection 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与外部资源的连接，从中将派生更多专用连接（如 [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) ）。

这是一种抽象类型。

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 resourceConnections](../api/windowsupdates-updates-list-resourceconnections.md)|[microsoft.graph.windowsUpdates.resourceConnection](../resources/windowsupdates-resourceconnection.md) 集合|获取 [resourceConnection](../resources/windowsupdates-resourceconnection.md) 对象及其属性的列表。|
|[获取 resourceConnection](../api/windowsupdates-resourceconnection-get.md)|[microsoft.graph.windowsUpdates.resourceConnection](../resources/windowsupdates-resourceconnection.md)|读取 [resourceConnection](../resources/windowsupdates-resourceconnection.md) 对象的属性和关系。|
|[删除 resourceConnection](../api/windowsupdates-resourceconnection-delete.md)|无|删除 [resourceConnection](../resources/windowsupdates-resourceconnection.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|资源连接的标识符。 键。 不可为 null。 只读。 默认情况下返回。|
|state|microsoft.graph.windowsUpdates.resourceConnectionState|连接的状态。 可能的值包括 `connected`、`notAuthorized`、`notFound`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.resourceConnection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.resourceConnection",
  "id": "String (identifier)",
  "state": "String"
}
```

