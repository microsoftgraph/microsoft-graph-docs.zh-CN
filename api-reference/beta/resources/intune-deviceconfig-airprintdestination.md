---
title: airPrintDestination 资源类型
description: 代表一个 AirPrint 目标。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f56578427427d45a69c4c64fe9fde3cf31f8fd9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422493"
---
# <a name="airprintdestination-resource-type"></a>airPrintDestination 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

代表一个 AirPrint 目标。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ipAddress|String|AirPrint 目标 IP 地址。|
|resourcePath|String|与打印机关联的资源路径。 这对应于 _ipps.tcp Bonjour 记录的 rp 参数。 例如： 打印机/Canon_MG5300_series 打印机/Xerox_Phaser_7600、 ipp/打印，Epson_IPP_Printer。|
|port|Int32|AirPrint 目标侦听端口。 如果未指定此项 AirPrint 将使用默认端口。 在 iOS 11.0 中可用和更高版本。|
|forceTls|Boolean|如果 true AirPrint 连接受到保护传输层安全性 (TLS)。 默认值为 false。 在 iOS 11.0 中可用和更高版本。|

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




