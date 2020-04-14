---
title: deliveryOptimizationMaxCacheSizeAbsolute 资源类型
description: 传递优化最大缓存大小绝对类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a15b1bfea6da2af43c360ff143d8bb55bc44f6b6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420455"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a>deliveryOptimizationMaxCacheSizeAbsolute 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

传递优化最大缓存大小绝对类型。


继承自[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|maximumCacheSizeInGigabytes|Int64|指定传递优化缓存的最大大小（以 GB 为单位）。 有效值为0至4294967295
值为0（零）表示 "无限制" 缓存。 当设备的磁盘空间不足时，传递优化将清除缓存。 有效值为0至4294967295|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute",
  "maximumCacheSizeInGigabytes": 1024
}
```



