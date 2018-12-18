---
title: airPrintDestination 资源类型
description: 代表一个 AirPrint 目标。
author: tfitzmac
ms.openlocfilehash: 046f85c65d382b34e6920f30f6b2718f817371a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361052"
---
# <a name="airprintdestination-resource-type"></a>airPrintDestination 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

代表一个 AirPrint 目标。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ipAddress|String|AirPrint 目标 IP 地址。|
|resourcePath|字符串|与打印机关联的资源路径。 这对应于 _ipps.tcp Bonjour 记录的 rp 参数。 例如： 打印机/Canon_MG5300_series 打印机/Xerox_Phaser_7600、 ipp/打印，Epson_IPP_Printer。|
|port|Int32|AirPrint 目标侦听端口。 如果未指定此项 AirPrint 将使用默认端口。 在 iOS 11.0 中可用和更高版本。|
|forceTls|Boolean|如果 true AirPrint 连接受到保护传输层安全性 (TLS)。 默认值为 false。 在 iOS 11.0 中可用和更高版本。|

## <a name="relationships"></a>Relationships
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





