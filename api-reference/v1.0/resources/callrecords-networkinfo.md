---
title: networkInfo 资源类型
description: 表示有关呼叫中使用的网络的信息。
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fe187e7d900b4851de5a647af5313f08394a1ccc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441529"
---
# <a name="networkinfo-resource-type"></a>networkInfo 资源类型

命名空间：microsoft.graph.callRecords

表示有关呼叫中使用的网络的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|bandwidthLowEventRatio|双精度|媒体终结点检测到可用带宽或带宽策略的通话的分数足够低，导致发送的音频质量差。|
|basicServiceSetIdentifier|String|用于连接到网络的媒体终结点的无线 LAN 基本服务集标识符。|
|connectionType|microsoft.graph.callRecords.networkConnectionType|媒体终结点使用的网络类型。 可取值为：`unknown`、`wired`、`wifi`、`mobile`、`tunnel`、`unknownFutureValue`。|
|delayEventRatio|双精度|媒体终结点检测到的网络延迟的通话比例很小，足以影响进行实时双向通信的能力。|
|dnsSuffix|String|与媒体终结点的网络适配器关联的 DNS 后缀。|
|ipAddress|String|媒体终结点的 IP 地址。|
|linkSpeed|Int64|由媒体终结点使用的网络适配器报告的每秒链接速度（以位为单位）。|
|macAddress|String|媒体访问控制 (MAC) 媒体终结点网络设备的地址。|
|networkTransportProtocol|microsoft.graph.callRecords.networkTransportProtocol|用于传输流的网络协议。 可能的值是：`unknown`、`udp`、`tcp`、`unknownFutureValue`。|
|港口|Int32|媒体终结点使用的网络端口号。|
|receivedQualityEventRatio|双精度|媒体终结点检测到网络导致接收的音频质量差的通话的分数。|
|reflexiveIPAddress|String|媒体中继服务器看到的媒体终结点的 IP 地址。 这通常是与终结点关联的公共 Internet IP 地址。|
|relayIPAddress|String|由媒体终结点分配的媒体中继服务器的 IP 地址。|
|relayPort|Int32|媒体终结点在媒体中继服务器上分配的网络端口号。|
|sentQualityEventRatio|双精度|媒体终结点检测到网络导致发送的音频质量差的通话的分数。|
|子|String|媒体终结点用于媒体流的子网。|
|traceRouteHops|[microsoft.graph.callRecords.traceRouteHop](callrecords-traceroutehop.md) 集合|为此媒体流收集的网络跟踪路由跃点列表。\*|
|wifiBand|microsoft.graph.callRecords.wifiBand|媒体终结点使用的 WiFi 带。 可取值为：`unknown`、`frequency24GHz`、`frequency50GHz`、`frequency60GHz`、`unknownFutureValue`。|
|wifiBatteryCharge|Int32|媒体终结点报告的剩余电池电量估计百分比。|
|wifiChannel|Int32|媒体终结点使用的 WiFi 通道。|
|wifiMicrosoftDriver|String|媒体终结点使用的 Microsoft WiFi 驱动程序的名称。 值可以根据终结点使用的语言进行本地化。|
|wifiMicrosoftDriverVersion|String|媒体终结点使用的 Microsoft WiFi 驱动程序的版本。|
|wifiRadioType|microsoft.graph.callRecords.wifiRadioType|媒体终结点使用的 WiFi 无线电的类型。 可取值为：`unknown`、`wifi80211a`、`wifi80211b`、`wifi80211g`、`wifi80211n`、`wifi80211ac`、`wifi80211ax`、`unknownFutureValue`。|
|wifiSignalStrength|Int32|由媒体终结点报告的 WiFi 信号强度百分比。|
|wifiVendorDriver|String|媒体终结点使用的 WiFi 驱动程序的名称。 值可以根据终结点使用的语言进行本地化。|
|wifiVendorDriverVersion|String|媒体终结点使用的 WiFi 驱动程序的版本。|

> [!NOTE]
> \*默认情况下， **traceRouteHops** 将始终返回空数组。 请联系 Microsoft 支持部门，为组织启用跟踪路由数据报告。

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
  "linkSpeed": "Int64",
  "macAddress": "String",
  "networkTransportProtocol": "String",
  "port": "Int32",
  "receivedQualityEventRatio": "Double",
  "reflexiveIPAddress": "String",
  "relayIPAddress": "String",
  "relayPort": "Int32",
  "sentQualityEventRatio": "Double",
  "subnet": "String",
  "traceRouteHops": [{"@odata.type": "microsoft.graph.callRecords.traceRouteHop"}],
  "wifiBand": "String",
  "wifiBatteryCharge": "Int32",
  "wifiChannel": "Int32",
  "wifiMicrosoftDriver": "String",
  "wifiMicrosoftDriverVersion": "String",
  "wifiRadioType": "String",
  "wifiSignalStrength": "Int32",
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
