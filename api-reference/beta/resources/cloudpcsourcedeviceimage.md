---
title: cloudPcSourceDeviceImage 资源类型
description: '与 Azure 订阅关联的源映像。 '
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 9bfdb8240d72a9b97f8b4dc89844734416576021
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723567"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a>cloudPcSourceDeviceImage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与 Azure 订阅关联的源映像。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|源图像的 ID。|
|displayName|String|源显示名称的源图像。|
|subscriptionId|String|托管源映像的订阅的 ID。|
|subscriptionDisplayName|String|托管显示名称映像的订阅的订阅组。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcSourceDeviceImage"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
  "id": "String (identifier)",
  "displayName": "String",
  "subscriptionId": "String",
  "subscriptionDisplayName": "String"
}
```
