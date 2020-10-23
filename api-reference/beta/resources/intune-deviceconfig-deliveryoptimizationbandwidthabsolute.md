---
title: deliveryOptimizationBandwidthAbsolute 资源类型
description: 带宽限制，以千字节/秒为单位。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 710553bb01eb335eed9cf4075af3d87985239f95
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696249"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a>deliveryOptimizationBandwidthAbsolute 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

带宽限制，以千字节/秒为单位。


继承自 [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|maximumDownloadBandwidthInKilobytesPerSecond|Int64|指定设备可在使用传递优化的所有并发下载活动中使用的最大下载带宽（以千字节/秒为单位）。 有效值为0至4294967295
值 0 (零) 意味着传递优化将动态调整，以使用可用带宽进行下载。 有效值为0至4294967295|
|maximumUploadBandwidthInKilobytesPerSecond|Int64|指定设备将在使用传递优化 (0-4000000) 的所有并发上载活动中使用的最大上载带宽（以千字节/秒为单位）。 有效值为0至4000000
默认值为0，它允许 (优化的无限制的带宽，以最大限度地利用上传带宽) 。 有效值为0至4000000|

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





