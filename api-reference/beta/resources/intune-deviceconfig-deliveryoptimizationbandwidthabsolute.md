---
title: deliveryOptimizationBandwidthAbsolute 资源类型
description: 带宽限制（以 KB/秒为单位）。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 28aa1fa0ff3d305392842a4aae1ada0c2c3ad6954502430e94a7db9c8e7cf304
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54241931"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a>deliveryOptimizationBandwidthAbsolute 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

带宽限制（以 KB/秒为单位）。


继承自 [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|maximumDownloadBandwidthInKilobytesPerSecond|Int64|指定设备可使用传递优化跨所有并发下载活动使用的最大下载带宽（以 Kb/秒为单位）。 有效值为 0 到 4294967295
值 0 (零) 表示传递优化动态调整以使用可用带宽进行下载。 有效值为 0 到 4294967295|
|maximumUploadBandwidthInKilobytesPerSecond|Int64|指定设备将使用传递优化 (0-40000000 (所有并发上载活动的最大上载带宽（以 KB/秒) ）。 有效值为 0 到 40000000
默认值为 0，表示允许无限可能的带宽 (优化，以尽可能减少上载带宽) 。 有效值为 0 到 40000000|

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




