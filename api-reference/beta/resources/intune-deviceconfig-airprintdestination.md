---
title: airPrintDestination 资源类型
description: 表示 AirPrint 目标。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0e457cf44b5a73f14dfd87fd69f2b9e27cef08c3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731937"
---
# <a name="airprintdestination-resource-type"></a>airPrintDestination 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 AirPrint 目标。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ipAddress|String|AirPrint 目标的 IP 地址。|
|resourcePath|String|与打印机关联的资源路径。 这对应于 _ipps tcp Bonjour record 的 rp 参数。 例如： printers/Canon_MG5300_series、printers/Xerox_Phaser_7600、ipp/print、Epson_IPP_Printer。|
|端口|Int32|AirPrint 目标的侦听端口。 如果未指定此项，AirPrint 将使用默认端口。 在 iOS 11.0 和更高版本中可用。|
|forceTls|布尔|如果为 true，则 AirPrint 连接受传输层安全性 (TLS) 的保护。 默认为 false。 在 iOS 11.0 和更高版本中可用。|

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





