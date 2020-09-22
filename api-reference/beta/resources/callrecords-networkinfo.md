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
# <a name="networkinfo-resource-type"></a><span data-ttu-id="d597d-103">networkInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="d597d-103">networkInfo resource type</span></span>

<span data-ttu-id="d597d-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="d597d-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d597d-105">表示有关在呼叫中使用的网络的信息。</span><span class="sxs-lookup"><span data-stu-id="d597d-105">Represents information about the network used in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="d597d-106">属性</span><span class="sxs-lookup"><span data-stu-id="d597d-106">Properties</span></span>

| <span data-ttu-id="d597d-107">属性</span><span class="sxs-lookup"><span data-stu-id="d597d-107">Property</span></span>     | <span data-ttu-id="d597d-108">类型</span><span class="sxs-lookup"><span data-stu-id="d597d-108">Type</span></span>        | <span data-ttu-id="d597d-109">说明</span><span class="sxs-lookup"><span data-stu-id="d597d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d597d-110">bandwidthLowEventRatio</span><span class="sxs-lookup"><span data-stu-id="d597d-110">bandwidthLowEventRatio</span></span>|<span data-ttu-id="d597d-111">双精度</span><span class="sxs-lookup"><span data-stu-id="d597d-111">Double</span></span>|<span data-ttu-id="d597d-112">媒体终结点检测到可用带宽或带宽策略的呼叫数不足以导致发送的音频质量较差。</span><span class="sxs-lookup"><span data-stu-id="d597d-112">Fraction of the call that the media endpoint detected the available bandwidth or bandwidth policy was low enough to cause poor quality of the audio sent.</span></span>|
|<span data-ttu-id="d597d-113">basicServiceSetIdentifier</span><span class="sxs-lookup"><span data-stu-id="d597d-113">basicServiceSetIdentifier</span></span>|<span data-ttu-id="d597d-114">String</span><span class="sxs-lookup"><span data-stu-id="d597d-114">String</span></span>|<span data-ttu-id="d597d-115">用于连接到网络的媒体终结点的无线 LAN 基本服务集标识符。</span><span class="sxs-lookup"><span data-stu-id="d597d-115">The wireless LAN basic service set identifier of the media endpoint used to connect to the network.</span></span>|
|<span data-ttu-id="d597d-116">connectionType</span><span class="sxs-lookup"><span data-stu-id="d597d-116">connectionType</span></span>|<span data-ttu-id="d597d-117">callRecords。 networkConnectionType</span><span class="sxs-lookup"><span data-stu-id="d597d-117">microsoft.graph.callRecords.networkConnectionType</span></span>|<span data-ttu-id="d597d-118">媒体终结点使用的网络类型。</span><span class="sxs-lookup"><span data-stu-id="d597d-118">Type of network used by the media endpoint.</span></span> <span data-ttu-id="d597d-119">可取值为：`unknown`、`wired`、`wifi`、`mobile`、`tunnel`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d597d-119">Possible values are: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d597d-120">delayEventRatio</span><span class="sxs-lookup"><span data-stu-id="d597d-120">delayEventRatio</span></span>|<span data-ttu-id="d597d-121">双精度</span><span class="sxs-lookup"><span data-stu-id="d597d-121">Double</span></span>|<span data-ttu-id="d597d-122">媒体终结点检测到网络延迟的一小部分，足以影响实时双向通信的能力。</span><span class="sxs-lookup"><span data-stu-id="d597d-122">Fraction of the call that the media endpoint detected the network delay was significant enough to impact the ability to have real-time two-way communication.</span></span>|
|<span data-ttu-id="d597d-123">dnsSuffix</span><span class="sxs-lookup"><span data-stu-id="d597d-123">dnsSuffix</span></span>|<span data-ttu-id="d597d-124">String</span><span class="sxs-lookup"><span data-stu-id="d597d-124">String</span></span>|<span data-ttu-id="d597d-125">与媒体终结点的网络适配器关联的 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="d597d-125">DNS suffix associated with the network adapter of the media endpoint.</span></span>|
|<span data-ttu-id="d597d-126">ipAddress</span><span class="sxs-lookup"><span data-stu-id="d597d-126">ipAddress</span></span>|<span data-ttu-id="d597d-127">String</span><span class="sxs-lookup"><span data-stu-id="d597d-127">String</span></span>|<span data-ttu-id="d597d-128">媒体终结点的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="d597d-128">IP address of the media endpoint.</span></span>|
|<span data-ttu-id="d597d-129">linkSpeed</span><span class="sxs-lookup"><span data-stu-id="d597d-129">linkSpeed</span></span>|<span data-ttu-id="d597d-130">Int64</span><span class="sxs-lookup"><span data-stu-id="d597d-130">Int64</span></span>|<span data-ttu-id="d597d-131">媒体终结点使用的网络适配器报告的链路速度，以位/秒为单位。</span><span class="sxs-lookup"><span data-stu-id="d597d-131">Link speed in bits per second reported by the network adapter used by the media endpoint.</span></span>|
|<span data-ttu-id="d597d-132">macAddress</span><span class="sxs-lookup"><span data-stu-id="d597d-132">macAddress</span></span>|<span data-ttu-id="d597d-133">String</span><span class="sxs-lookup"><span data-stu-id="d597d-133">String</span></span>|<span data-ttu-id="d597d-134">媒体访问控制 (MAC) 媒体终结点的网络设备的地址。</span><span class="sxs-lookup"><span data-stu-id="d597d-134">The media access control (MAC) address of the media endpoint's network device.</span></span>|
|<span data-ttu-id="d597d-135">端口</span><span class="sxs-lookup"><span data-stu-id="d597d-135">port</span></span>|<span data-ttu-id="d597d-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d597d-136">Int32</span></span>|<span data-ttu-id="d597d-137">媒体终结点使用的网络端口号。</span><span class="sxs-lookup"><span data-stu-id="d597d-137">Network port number used by media endpoint.</span></span>|
|<span data-ttu-id="d597d-138">receivedQualityEventRatio</span><span class="sxs-lookup"><span data-stu-id="d597d-138">receivedQualityEventRatio</span></span>|<span data-ttu-id="d597d-139">双精度</span><span class="sxs-lookup"><span data-stu-id="d597d-139">Double</span></span>|<span data-ttu-id="d597d-140">媒体终结点检测到网络的呼叫的分数导致收到的音频质量较差。</span><span class="sxs-lookup"><span data-stu-id="d597d-140">Fraction of the call that the media endpoint detected the network was causing poor quality of the audio received.</span></span>|
|<span data-ttu-id="d597d-141">reflexiveIPAddress</span><span class="sxs-lookup"><span data-stu-id="d597d-141">reflexiveIPAddress</span></span>|<span data-ttu-id="d597d-142">String</span><span class="sxs-lookup"><span data-stu-id="d597d-142">String</span></span>|<span data-ttu-id="d597d-143">媒体终结点的 IP 地址，如媒体中继服务器所示。</span><span class="sxs-lookup"><span data-stu-id="d597d-143">IP address of the media endpoint as seen by the media relay server.</span></span> <span data-ttu-id="d597d-144">这通常是与终结点关联的公共 internet IP 地址。</span><span class="sxs-lookup"><span data-stu-id="d597d-144">This is typically the public internet IP address associated to the endpoint.</span></span>|
|<span data-ttu-id="d597d-145">relayIPAddress</span><span class="sxs-lookup"><span data-stu-id="d597d-145">relayIPAddress</span></span>|<span data-ttu-id="d597d-146">String</span><span class="sxs-lookup"><span data-stu-id="d597d-146">String</span></span>|<span data-ttu-id="d597d-147">媒体终结点分配的媒体中继服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="d597d-147">IP address of the media relay server allocated by the media endpoint.</span></span>|
|<span data-ttu-id="d597d-148">relayPort</span><span class="sxs-lookup"><span data-stu-id="d597d-148">relayPort</span></span>|<span data-ttu-id="d597d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d597d-149">Int32</span></span>|<span data-ttu-id="d597d-150">媒体终结点在媒体中继服务器上分配的网络端口号。</span><span class="sxs-lookup"><span data-stu-id="d597d-150">Network port number allocated on the media relay server by the media endpoint.</span></span>|
|<span data-ttu-id="d597d-151">sentQualityEventRatio</span><span class="sxs-lookup"><span data-stu-id="d597d-151">sentQualityEventRatio</span></span>|<span data-ttu-id="d597d-152">双精度</span><span class="sxs-lookup"><span data-stu-id="d597d-152">Double</span></span>|<span data-ttu-id="d597d-153">媒体终结点检测到网络的呼叫的分数导致发送的音频质量较差。</span><span class="sxs-lookup"><span data-stu-id="d597d-153">Fraction of the call that the media endpoint detected the network was causing poor quality of the audio sent.</span></span>|
|<span data-ttu-id="d597d-154">子网</span><span class="sxs-lookup"><span data-stu-id="d597d-154">subnet</span></span>|<span data-ttu-id="d597d-155">String</span><span class="sxs-lookup"><span data-stu-id="d597d-155">String</span></span>|<span data-ttu-id="d597d-156">媒体终结点用于媒体流的子网。</span><span class="sxs-lookup"><span data-stu-id="d597d-156">Subnet used for media stream by the media endpoint.</span></span>|
|<span data-ttu-id="d597d-157">wifiBand</span><span class="sxs-lookup"><span data-stu-id="d597d-157">wifiBand</span></span>|<span data-ttu-id="d597d-158">callRecords。 wifiBand</span><span class="sxs-lookup"><span data-stu-id="d597d-158">microsoft.graph.callRecords.wifiBand</span></span>|<span data-ttu-id="d597d-159">媒体终结点使用的 WiFi 波段。</span><span class="sxs-lookup"><span data-stu-id="d597d-159">WiFi band used by the media endpoint.</span></span> <span data-ttu-id="d597d-160">可取值为：`unknown`、`frequency24GHz`、`frequency50GHz`、`frequency60GHz`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d597d-160">Possible values are: `unknown`, `frequency24GHz`, `frequency50GHz`, `frequency60GHz`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d597d-161">wifiBatteryCharge</span><span class="sxs-lookup"><span data-stu-id="d597d-161">wifiBatteryCharge</span></span>|<span data-ttu-id="d597d-162">Int32</span><span class="sxs-lookup"><span data-stu-id="d597d-162">Int32</span></span>|<span data-ttu-id="d597d-163">按媒体终结点报告的百分比估计剩余电池电量。</span><span class="sxs-lookup"><span data-stu-id="d597d-163">Estimated remaining battery charge in percentage reported by the media endpoint.</span></span>|
|<span data-ttu-id="d597d-164">wifiChannel</span><span class="sxs-lookup"><span data-stu-id="d597d-164">wifiChannel</span></span>|<span data-ttu-id="d597d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d597d-165">Int32</span></span>|<span data-ttu-id="d597d-166">媒体终结点使用的 WiFi 通道。</span><span class="sxs-lookup"><span data-stu-id="d597d-166">WiFi channel used by the media endpoint.</span></span>|
|<span data-ttu-id="d597d-167">wifiMicrosoftDriver</span><span class="sxs-lookup"><span data-stu-id="d597d-167">wifiMicrosoftDriver</span></span>|<span data-ttu-id="d597d-168">String</span><span class="sxs-lookup"><span data-stu-id="d597d-168">String</span></span>|<span data-ttu-id="d597d-169">媒体终结点使用的 Microsoft WiFi 驱动程序的名称。</span><span class="sxs-lookup"><span data-stu-id="d597d-169">Name of the Microsoft WiFi driver used by the media endpoint.</span></span> <span data-ttu-id="d597d-170">值可能根据终结点使用的语言进行本地化。</span><span class="sxs-lookup"><span data-stu-id="d597d-170">Value may be localized based on the language used by endpoint.</span></span>|
|<span data-ttu-id="d597d-171">wifiMicrosoftDriverVersion</span><span class="sxs-lookup"><span data-stu-id="d597d-171">wifiMicrosoftDriverVersion</span></span>|<span data-ttu-id="d597d-172">String</span><span class="sxs-lookup"><span data-stu-id="d597d-172">String</span></span>|<span data-ttu-id="d597d-173">媒体终结点使用的 Microsoft WiFi 驱动程序的版本。</span><span class="sxs-lookup"><span data-stu-id="d597d-173">Version of the Microsoft WiFi driver used by the media endpoint.</span></span>|
|<span data-ttu-id="d597d-174">wifiRadioType</span><span class="sxs-lookup"><span data-stu-id="d597d-174">wifiRadioType</span></span>|<span data-ttu-id="d597d-175">callRecords。 wifiRadioType</span><span class="sxs-lookup"><span data-stu-id="d597d-175">microsoft.graph.callRecords.wifiRadioType</span></span>|<span data-ttu-id="d597d-176">媒体终结点使用的 WiFi 无线电的类型。</span><span class="sxs-lookup"><span data-stu-id="d597d-176">Type of WiFi radio used by the media endpoint.</span></span> <span data-ttu-id="d597d-177">可取值为：`unknown`、`wifi80211a`、`wifi80211b`、`wifi80211g`、`wifi80211n`、`wifi80211ac`、`wifi80211ax`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d597d-177">Possible values are: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d597d-178">wifiSignalStrength</span><span class="sxs-lookup"><span data-stu-id="d597d-178">wifiSignalStrength</span></span>|<span data-ttu-id="d597d-179">Int32</span><span class="sxs-lookup"><span data-stu-id="d597d-179">Int32</span></span>|<span data-ttu-id="d597d-180">以媒体终结点报告的百分比表示的 WiFi 信号强度。</span><span class="sxs-lookup"><span data-stu-id="d597d-180">WiFi signal strength in percentage reported by the media endpoint.</span></span>|
|<span data-ttu-id="d597d-181">wifiVendorDriver</span><span class="sxs-lookup"><span data-stu-id="d597d-181">wifiVendorDriver</span></span>|<span data-ttu-id="d597d-182">String</span><span class="sxs-lookup"><span data-stu-id="d597d-182">String</span></span>|<span data-ttu-id="d597d-183">媒体终结点使用的 WiFi 驱动程序的名称。</span><span class="sxs-lookup"><span data-stu-id="d597d-183">Name of the WiFi driver used by the media endpoint.</span></span> <span data-ttu-id="d597d-184">值可能根据终结点使用的语言进行本地化。</span><span class="sxs-lookup"><span data-stu-id="d597d-184">Value may be localized based on the language used by endpoint.</span></span>|
|<span data-ttu-id="d597d-185">wifiVendorDriverVersion</span><span class="sxs-lookup"><span data-stu-id="d597d-185">wifiVendorDriverVersion</span></span>|<span data-ttu-id="d597d-186">String</span><span class="sxs-lookup"><span data-stu-id="d597d-186">String</span></span>|<span data-ttu-id="d597d-187">媒体终结点使用的 WiFi 驱动程序的版本。</span><span class="sxs-lookup"><span data-stu-id="d597d-187">Version of the WiFi driver used by the media endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d597d-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d597d-188">JSON representation</span></span>

<span data-ttu-id="d597d-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d597d-189">The following is a JSON representation of the resource.</span></span>

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

