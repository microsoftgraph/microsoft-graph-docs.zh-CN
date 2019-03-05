---
title: deliveryOptimizationBandwidthAbsolute 资源类型
description: 带宽限制, 以千字节/秒为单位。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9eca95ad33ced19e437e760663a73158aacc25d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178267"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a>deliveryOptimizationBandwidthAbsolute 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

带宽限制, 以千字节/秒为单位。


继承自[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|maximumDownloadBandwidthInKilobytesPerSecond|Int64|指定设备可在使用传递优化的所有并发下载活动中使用的最大下载带宽 (以千字节/秒为单位)。 有效值为0至4294967295
值为 0 (零) 表示传递优化将动态调整, 以使用可用带宽进行下载。 有效值为0至4294967295|
|maximumUploadBandwidthInKilobytesPerSecond|Int64|指定设备将使用传递优化 (0-4000000) 在所有并发上载活动中使用的最大上载带宽 (以千字节/秒为单位)。 有效值为0至4000000
默认值为 0, 它允许无限制的可能带宽 (针对最小上载带宽的使用情况进行了优化)。 有效值为0至4000000|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthAbsolute",
  "maximumDownloadBandwidthInKilobytesPerSecond": 1024,
  "maximumUploadBandwidthInKilobytesPerSecond": 1024
}
```




