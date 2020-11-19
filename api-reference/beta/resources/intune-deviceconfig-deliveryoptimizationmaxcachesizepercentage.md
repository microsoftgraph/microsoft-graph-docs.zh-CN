---
title: deliveryOptimizationMaxCacheSizePercentage 资源类型
description: 传递优化最大缓存大小百分比类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 53a32220a72b994bbbff4c39a16923fb27049051
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288724"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a>deliveryOptimizationMaxCacheSizePercentage 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

传递优化最大缓存大小百分比类型。


继承自 [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|maximumCacheSizePercentage|Int32|指定传递优化可以使用的最大缓存大小，以磁盘大小的百分比 (1-100) 为依据。 有效值为1至100|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizePercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizePercentage",
  "maximumCacheSizePercentage": 1024
}
```




