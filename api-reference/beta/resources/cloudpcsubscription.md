---
title: cloudPcSubscription 资源类型
description: 表示云电脑订阅。
author: xhan2077
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 425ada12758e2602d8cf262e27c34087722bf84f
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366303"
---
# <a name="cloudpcsubscription-resource-type"></a>cloudPcSubscription 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可用于存储云电脑的快照或快照以进行取证分析的订阅信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|subscriptionId|String|订阅的 ID。|
|subscriptionName|String|订阅的名称。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "subscriptionId",
  "@odata.type": "microsoft.graph.cloudPcSubscription",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSubscription",
  "subscriptionId": "String",
  "subscriptionName": "String"
}
```
