---
title: operationalInsightsConnection 资源类型
description: 表示将 Log Analytics 工作区链接到 Windows 更新 for Business 部署服务的专用 resourceConnection。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 07725da7d19cdf4c7fdb232f45823e75ffe37d2d
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856708"
---
# <a name="operationalinsightsconnection-resource-type"></a>operationalInsightsConnection 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示将 Log Analytics 工作区链接到 Windows 更新 for Business 部署服务的专用 [resourceConnection](../resources/windowsupdates-resourceconnection.md)。

继承自 [resourceConnection](../resources/windowsupdates-resourceconnection.md)。

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 operationalInsightsConnections](../api/windowsupdates-updates-list-resourceconnections-operationalinsightsconnection.md)|[microsoft.graph.windowsUpdates.operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) 集合|获取 [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) 对象及其属性的列表。|
|[创建 operationalInsightsConnection](../api/windowsupdates-updates-post-resourceconnections-operationalinsightsconnection.md)|[microsoft.graph.windowsUpdates.operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md)|创建新的 [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) 对象。|
|[获取 operationalInsightsConnection](../api/windowsupdates-operationalinsightsconnection-get.md)|[microsoft.graph.windowsUpdates.operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md)|读取 [operationalInsightsConnection 对象的](../resources/windowsupdates-operationalinsightsconnection.md) 属性和关系。|
|[删除 operationalInsightsConnection](../api/windowsupdates-operationalinsightsconnection-delete.md)|无|删除 [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|azureResourceGroupName|String|包含 Log Analytics 工作区的 Azure 资源组的名称。|
|azureSubscriptionId|字符串|包含 Log Analytics 工作区的 Azure 订阅 ID。|
|id|String|资源连接的标识符。 键。 不可为 null。 只读。 默认情况下返回。|
|state|microsoft.graph.windowsUpdates.resourceConnectionState|连接的状态。 可能的值包括 `connected`、`notAuthorized`、`notFound`、`unknownFutureValue`。|
|workspaceName|String|Log Analytics 工作区的名称。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.operationalInsightsConnection",
  "baseType": "microsoft.graph.windowsUpdates.resourceConnection",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.operationalInsightsConnection",
  "azureResourceGroupName": "String",  
  "azureSubscriptionId": "String",
  "id": "String (identifier)",
  "state": "String",
  "workspaceName": "String"
}
```

