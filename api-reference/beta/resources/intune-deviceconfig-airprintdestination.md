---
title: airPrintDestination 资源类型
description: 代表 AirPrint 目标。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad603ab29c7914ccb16845ceeddda89581a40568
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095693"
---
# <a name="airprintdestination-resource-type"></a>airPrintDestination 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

代表 AirPrint 目标。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ipAddress|String|AirPrint 目的地的 IP 地址。|
|resourcePath|String|与打印机关联的资源路径。 这对应于 _ipps.tcp 的 rp 参数。 例如：printers/Canon_MG5300_series、printers/Xerox_Phaser_7600、ipp/print、Epson_IPP_Printer。|
|端口|Int32|AirPrint 目的地的侦听端口。 如果未指定此键，AirPrint 将使用默认端口。 在 iOS 11.0 及更高版本中可用。|
|forceTls|Boolean|如果真正的 AirPrint 连接由传输层安全性 (TLS) 。 默认为 false。 在 iOS 11.0 及更高版本中可用。|

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



