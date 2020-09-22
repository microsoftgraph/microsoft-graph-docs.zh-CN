---
title: networkInfo 资源类型
description: NetworkInfo 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f465ea20335b5c30c27596d296dd8dd3581d0b58
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071379"
---
# <a name="networkinfo-resource-type"></a>networkInfo 资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关在呼叫中使用的网络的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|bandwidthLowEventRatio|双精度|媒体终结点检测到可用带宽或带宽策略的呼叫数不足以导致发送的音频质量较差。|
|basicServiceSetIdentifier|String|用于连接到网络的媒体终结点的无线 LAN 基本服务集标识符。|
|connectionType|callRecords。 networkConnectionType|媒体终结点使用的网络类型。 可取值为：`unknown`、`wired`、`wifi`、`mobile`、`tunnel`、`unknownFutureValue`。|
|delayEventRatio|双精度|媒体终结点检测到网络延迟的一小部分，足以影响实时双向通信的能力。|
|dnsSuffix|String|与媒体终结点的网络适配器关联的 DNS 后缀。|
|ipAddress|String|媒体终结点的 IP 地址。|
|linkSpeed|Int64|媒体终结点使用的网络适配器报告的链路速度，以位/秒为单位。|
|macAddress|String|媒体访问控制 (MAC) 媒体终结点的网络设备的地址。|
|端口|Int32|媒体终结点使用的网络端口号。|
|receivedQualityEventRatio|双精度|媒体终结点检测到网络的呼叫的分数导致收到的音频质量较差。|
|reflexiveIPAddress|String|媒体终结点的 IP 地址，如媒体中继服务器所示。 这通常是与终结点关联的公共 internet IP 地址。|
|relayIPAddress|String|媒体终结点分配的媒体中继服务器的 IP 地址。|
|relayPort|Int32|媒体终结点在媒体中继服务器上分配的网络端口号。|
|sentQualityEventRatio|双精度|媒体终结点检测到网络的呼叫的分数导致发送的音频质量较差。|
|子网|String|媒体终结点用于媒体流的子网。|
|wifiBand|callRecords。 wifiBand|媒体终结点使用的 WiFi 波段。 可取值为：`unknown`、`frequency24GHz`、`frequency50GHz`、`frequency60GHz`、`unknownFutureValue`。|
|wifiBatteryCharge|Int32|按媒体终结点报告的百分比估计剩余电池电量。|
|wifiChannel|Int32|媒体终结点使用的 WiFi 通道。|
|wifiMicrosoftDriver|String|媒体终结点使用的 Microsoft WiFi 驱动程序的名称。 值可能根据终结点使用的语言进行本地化。|
|wifiMicrosoftDriverVersion|String|媒体终结点使用的 Microsoft WiFi 驱动程序的版本。|
|wifiRadioType|callRecords。 wifiRadioType|媒体终结点使用的 WiFi 无线电的类型。 可取值为：`unknown`、`wifi80211a`、`wifi80211b`、`wifi80211g`、`wifi80211n`、`wifi80211ac`、`wifi80211ax`、`unknownFutureValue`。|
|wifiSignalStrength|Int32|以媒体终结点报告的百分比表示的 WiFi 信号强度。|
|wifiVendorDriver|String|媒体终结点使用的 WiFi 驱动程序的名称。 值可能根据终结点使用的语言进行本地化。|
|wifiVendorDriverVersion|String|媒体终结点使用的 WiFi 驱动程序的版本。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.networkInfo",
  "baseType": null
}-->

```json
{
  "bandwidthLowEventRatio": "Double",
  "basicServiceSetIdentifier": "String",
  "connectionType": "String",
  "delayEventRatio": "Double",
  "dnsSuffix": "String",
  "ipAddress": "String",
  "linkSpeed": 1024,
  "macAddress": "String",
  "port": 1024,
  "receivedQualityEventRatio": "Double",
  "reflexiveIPAddress": "String",
  "relayIPAddress": "String",
  "relayPort": 1024,
  "sentQualityEventRatio": "Double",
  "subnet": "String",
  "wifiBand": "String",
  "wifiBatteryCharge": 1024,
  "wifiChannel": 1024,
  "wifiMicrosoftDriver": "String",
  "wifiMicrosoftDriverVersion": "String",
  "wifiRadioType": "String",
  "wifiSignalStrength": 1024,
  "wifiVendorDriver": "String",
  "wifiVendorDriverVersion": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

