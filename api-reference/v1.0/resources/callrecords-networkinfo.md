---
title: networkInfo 资源类型
description: networkInfo 类型
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e5f3115b5f450c3998ffb93f8b843dcc80e9f6d9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59029155"
---
# <a name="networkinfo-resource-type"></a>networkInfo 资源类型

命名空间：microsoft.graph.callRecords

表示有关呼叫中使用的网络的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|bandwidthLowEventRatio|双精度|媒体终结点检测到可用带宽或带宽策略低到足以导致已发送音频质量差的呼叫的一小部分。|
|basicServiceSetIdentifier|String|用于连接到网络的媒体终结点的无线 LAN 基本服务集标识符。|
|connectionType|microsoft.graph.callRecords.networkConnectionType|媒体终结点使用的网络类型。 可取值为：`unknown`、`wired`、`wifi`、`mobile`、`tunnel`、`unknownFutureValue`。|
|delayEventRatio|双精度|满足以下比例的通话：媒体终结点检测到网络延迟足以影响实时双向通信能力。|
|dnsSuffix|String|与媒体终结点的网络适配器关联的 DNS 后缀。|
|ipAddress|String|媒体终结点的 IP 地址。|
|linkSpeed|Int64|媒体终结点使用的网络适配器报告的链接速度（以位/秒为单位）。|
|macAddress|String|媒体访问控制 (MAC) 终结点的网络设备的地址。|
|端口|Int32|媒体终结点使用的网络端口号。|
|receivedQualityEventRatio|双精度|媒体终结点检测到网络导致接收的音频质量差的通话的一小部分。|
|将iveIPAddress|String|媒体中继服务器所看到的媒体终结点的 IP 地址。 这通常是与终结点关联的公共 Internet IP 地址。|
|relayIPAddress|String|媒体终结点分配的媒体中继服务器的 IP 地址。|
|relayPort|Int32|媒体终结点在媒体中继服务器上分配的网络端口号。|
|sentQualityEventRatio|双精度|媒体终结点检测到网络导致已发送音频质量差的通话的一小部分。|
|子网|String|媒体终结点用于媒体流的子网。|
|wifiBand|microsoft.graph.callRecords.wifiBand|媒体终结点使用的 WiFi 频带。 可取值为：`unknown`、`frequency24GHz`、`frequency50GHz`、`frequency60GHz`、`unknownFutureValue`。|
|wifiBatteryCharge|Int32|按媒体终结点报告的百分比表示的电池剩余电量的估计值。|
|wifiChannel|Int32|媒体终结点使用的 WiFi 通道。|
|wifiMicrosoftDriver|String|媒体终结点使用的 Microsoft WiFi 驱动程序的名称。 值可能会基于终结点使用的语言进行本地化。|
|wifiMicrosoftDriverVersion|String|媒体终结点使用的 Microsoft WiFi 驱动程序的版本。|
|wifiRadioType|microsoft.graph.callRecords.wifiRadioType|媒体终结点使用的 WiFi 无线电的类型。 可取值为：`unknown`、`wifi80211a`、`wifi80211b`、`wifi80211g`、`wifi80211n`、`wifi80211ac`、`wifi80211ax`、`unknownFutureValue`。|
|wifiSignalStrength|Int32|媒体终结点报告的 WiFi 信号强度百分比。|
|wifiVendorDriver|String|媒体终结点使用的 WiFi 驱动程序的名称。 值可能会基于终结点使用的语言进行本地化。|
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
