---
title: deliveryOptimizationBandwidthPercentage 资源类型
description: 指定为百分比的带宽限制。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8f1aab20ff6bbb7ab4e353e6d82fd2b19dd62281
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820455"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a>deliveryOptimizationBandwidthPercentage 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定为百分比的带宽限制。


继承自 [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|maximumBackgroundBandwidthPercentage|Int32|指定传递优化在所有并发下载活动中使用的最大后台下载带宽，以 0-100 (下载带宽的百分比) 。 有效值为 0 至 100
默认值 0 (零) 意味着传递优化动态调整以使用可用带宽进行后台下载。 有效值为 0 至 100|
|maximumForegroundBandwidthPercentage|Int32|指定传递优化在所有并发下载活动中使用的最大前台下载带宽，以 0-100 (下载带宽的百分比) 。 有效值为 0 至 100
默认值 0 (零) 表示传递优化动态调整以使用前台下载的可用带宽。 有效值为 0 至 100|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthPercentage",
  "maximumBackgroundBandwidthPercentage": 1024,
  "maximumForegroundBandwidthPercentage": 1024
}
```



