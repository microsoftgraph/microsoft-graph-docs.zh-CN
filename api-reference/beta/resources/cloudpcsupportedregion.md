---
title: cloudPcSupportedRegion 资源类型
description: 表示为云电脑建立 Azure 网络连接的支持区域。
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d13bfb6709d856119dcfaa700d819b9ed6f55258
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588566"
---
# <a name="cloudpcsupportedregion-resource-type"></a>cloudPcSupportedRegion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示为云电脑建立 Azure 网络连接的支持区域。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 cloudPcSupportedRegions](../api/virtualendpoint-list-supportedregions.md)|[cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md) 集合|列出可用于创建云电脑连接的受支持区域。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|受支持区域的唯一标识符。 只读。|
|displayName|String|支持区域的名称。 只读。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcSupportedRegion",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSupportedRegion",
  "id": "String (identifier)",
  "displayName": "String"
}
```
