---
title: airPrintDestination 资源类型
description: 表示 AirPrint 目标。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f09301bd791b5fd8b3fa430b50f7cdf58de43944
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167331"
---
# <a name="airprintdestination-resource-type"></a>airPrintDestination 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 AirPrint 目标。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ipAddress|String|AirPrint 目标的 IP 地址。|
|resourcePath|String|与打印机关联的资源路径。 这对应于 _ipps Bonjour 记录的 rp 参数。 例如: printers/Canon_MG5300_series、printers/Xerox_Phaser_7600、ipp/print、Epson_IPP_Printer。|
|port|Int32|AirPrint 目标的侦听端口。 如果未指定此项, AirPrint 将使用默认端口。 在 iOS 11.0 和更高版本中可用。|
|forceTls|Boolean|如果为 true, 则 AirPrint 连接通过传输层安全性 (TLS) 进行保护。 默认值为 false。 在 iOS 11.0 和更高版本中可用。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.airPrintDestination"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.airPrintDestination",
  "ipAddress": "String",
  "resourcePath": "String",
  "port": 1024,
  "forceTls": true
}
```




