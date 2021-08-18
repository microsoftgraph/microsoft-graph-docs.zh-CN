---
title: deliveryOptimizationMaxCacheSizePercentage 资源类型
description: 传递优化 最大缓存大小百分比类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4fcf646bd7288802918413667f402902be7288b4c3bd2bbe8e4d3f1adb84b77d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54131183"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a>deliveryOptimizationMaxCacheSizePercentage 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

传递优化 最大缓存大小百分比类型。


继承自 [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|maximumCacheSizePercentage|Int32|指定传递优化可以利用的最大缓存大小，以 1-100 (磁盘大小的百分比) 。 有效值为 1 到 100|

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




