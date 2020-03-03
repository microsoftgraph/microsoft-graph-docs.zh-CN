---
title: networkInfo 资源类型
description: NetworkInfo 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c24f53054d474ac8a50959127d98f5920789e620
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394688"
---
# <a name="networkinfo-resource-type"></a><span data-ttu-id="c0d63-103">networkInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0d63-103">networkInfo resource type</span></span>

<span data-ttu-id="c0d63-104">命名空间： callRecords</span><span class="sxs-lookup"><span data-stu-id="c0d63-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0d63-105">表示有关在呼叫中使用的网络的信息。</span><span class="sxs-lookup"><span data-stu-id="c0d63-105">Represents information about the network used in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="c0d63-106">属性</span><span class="sxs-lookup"><span data-stu-id="c0d63-106">Properties</span></span>

| <span data-ttu-id="c0d63-107">属性</span><span class="sxs-lookup"><span data-stu-id="c0d63-107">Property</span></span>     | <span data-ttu-id="c0d63-108">类型</span><span class="sxs-lookup"><span data-stu-id="c0d63-108">Type</span></span>        | <span data-ttu-id="c0d63-109">说明</span><span class="sxs-lookup"><span data-stu-id="c0d63-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c0d63-110">bandwidthLowEventRatio</span><span class="sxs-lookup"><span data-stu-id="c0d63-110">bandwidthLowEventRatio</span></span>|<span data-ttu-id="c0d63-111">双精度</span><span class="sxs-lookup"><span data-stu-id="c0d63-111">Double</span></span>|<span data-ttu-id="c0d63-112">媒体终结点检测到可用带宽或带宽策略的呼叫数不足以导致发送的音频质量较差。</span><span class="sxs-lookup"><span data-stu-id="c0d63-112">Fraction of the call that the media endpoint detected the available bandwidth or bandwidth policy was low enough to cause poor quality of the audio sent.</span></span>|
|<span data-ttu-id="c0d63-113">basicServiceSetIdentifier</span><span class="sxs-lookup"><span data-stu-id="c0d63-113">basicServiceSetIdentifier</span></span>|<span data-ttu-id="c0d63-114">String</span><span class="sxs-lookup"><span data-stu-id="c0d63-114">String</span></span>|<span data-ttu-id="c0d63-115">用于连接到网络的媒体终结点的无线 LAN 基本服务集标识符。</span><span class="sxs-lookup"><span data-stu-id="c0d63-115">The wireless LAN basic service set identifier of the media endpoint used to connect to the network.</span></span>|
|<span data-ttu-id="c0d63-116">connectionType</span><span class="sxs-lookup"><span data-stu-id="c0d63-116">connectionType</span></span>|<span data-ttu-id="c0d63-117">String</span><span class="sxs-lookup"><span data-stu-id="c0d63-117">String</span></span>|<span data-ttu-id="c0d63-118">媒体终结点使用的网络类型。</span><span class="sxs-lookup"><span data-stu-id="c0d63-118">Type of network used by the media endpoint.</span></span> <span data-ttu-id="c0d63-119">可取值为：`unknown`、`wired`、`wifi`、`mobile`、`tunnel`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c0d63-119">Possible values are: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c0d63-120">delayEventRatio</span><span class="sxs-lookup"><span data-stu-id="c0d63-120">delayEventRatio</span></span>|<span data-ttu-id="c0d63-121">双精度</span><span class="sxs-lookup"><span data-stu-id="c0d63-121">Double</span></span>|<span data-ttu-id="c0d63-122">媒体终结点检测到网络延迟的一小部分，足以影响实时双向通信的能力。</span><span class="sxs-lookup"><span data-stu-id="c0d63-122">Fraction of the call that the media endpoint detected the network delay was significant enough to impact the ability to have real-time two-way communication.</span></span>|
|<span data-ttu-id="c0d63-123">dnsSuffix</span><span class="sxs-lookup"><span data-stu-id="c0d63-123">dnsSuffix</span></span>|<span data-ttu-id="c0d63-124">String</span><span class="sxs-lookup"><span data-stu-id="c0d63-124">String</span></span>|<span data-ttu-id="c0d63-125">与媒体终结点的网络适配器关联的 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="c0d63-125">DNS suffix associated with the network adapter of the media endpoint.</span></span>|
|<span data-ttu-id="c0d63-126">ipAddress</span><span class="sxs-lookup"><span data-stu-id="c0d63-126">ipAddress</span></span>|<span data-ttu-id="c0d63-127">String</span><span class="sxs-lookup"><span data-stu-id="c0d63-127">String</span></span>|<span data-ttu-id="c0d63-128">媒体终结点的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="c0d63-128">IP address of the media endpoint.</span></span>|
|<span data-ttu-id="c0d63-129">linkSpeed</span><span class="sxs-lookup"><span data-stu-id="c0d63-129">linkSpeed</span></span>|<span data-ttu-id="c0d63-130">Int64</span><span class="sxs-lookup"><span data-stu-id="c0d63-130">Int64</span></span>|<span data-ttu-id="c0d63-131">媒体终结点使用的网络适配器报告的链路速度，以位/秒为单位。</span><span class="sxs-lookup"><span data-stu-id="c0d63-131">Link speed in bits per second reported by the network adapter used by the media endpoint.</span></span>|
|<span data-ttu-id="c0d63-132">macAddress</span><span class="sxs-lookup"><span data-stu-id="c0d63-132">macAddress</span></span>|<span data-ttu-id="c0d63-133">String</span><span class="sxs-lookup"><span data-stu-id="c0d63-133">String</span></span>|<span data-ttu-id="c0d63-134">媒体终结点的网络设备的媒体访问控制（MAC）地址。</span><span class="sxs-lookup"><span data-stu-id="c0d63-134">The media access control (MAC) address of the media endpoint's network device.</span></span>|
|<span data-ttu-id="c0d63-135">端口</span><span class="sxs-lookup"><span data-stu-id="c0d63-135">port</span></span>|<span data-ttu-id="c0d63-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c0d63-136">Int32</span></span>|<span data-ttu-id="c0d63-137">媒体终结点使用的网络端口号。</span><span class="sxs-lookup"><span data-stu-id="c0d63-137">Network port number used by media endpoint.</span></span>|
|<span data-ttu-id="c0d63-138">receivedQualityEventRatio</span><span class="sxs-lookup"><span data-stu-id="c0d63-138">receivedQualityEventRatio</span></span>|<span data-ttu-id="c0d63-139">双精度</span><span class="sxs-lookup"><span data-stu-id="c0d63-139">Double</span></span>|<span data-ttu-id="c0d63-140">媒体终结点检测到网络的呼叫的分数导致收到的音频质量较差。</span><span class="sxs-lookup"><span data-stu-id="c0d63-140">Fraction of the call that the media endpoint detected the network was causing poor quality of the audio received.</span></span>|
|<span data-ttu-id="c0d63-141">reflexiveIPAddress</span><span class="sxs-lookup"><span data-stu-id="c0d63-141">reflexiveIPAddress</span></span>|<span data-ttu-id="c0d63-142">String</span><span class="sxs-lookup"><span data-stu-id="c0d63-142">String</span></span>|<span data-ttu-id="c0d63-143">媒体终结点的 IP 地址，如媒体中继服务器所示。</span><span class="sxs-lookup"><span data-stu-id="c0d63-143">IP address of the media endpoint as seen by the media relay server.</span></span> <span data-ttu-id="c0d63-144">这通常是与终结点关联的公共 internet IP 地址。</span><span class="sxs-lookup"><span data-stu-id="c0d63-144">This is typically the public internet IP address associated to the endpoint.</span></span>|
|<span data-ttu-id="c0d63-145">relayIPAddress</span><span class="sxs-lookup"><span data-stu-id="c0d63-145">relayIPAddress</span></span>|<span data-ttu-id="c0d63-146">String</span><span class="sxs-lookup"><span data-stu-id="c0d63-146">String</span></span>|<span data-ttu-id="c0d63-147">媒体终结点分配的媒体中继服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="c0d63-147">IP address of the media relay server allocated by the media endpoint.</span></span>|
|<span data-ttu-id="c0d63-148">relayPort</span><span class="sxs-lookup"><span data-stu-id="c0d63-148">relayPort</span></span>|<span data-ttu-id="c0d63-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c0d63-149">Int32</span></span>|<span data-ttu-id="c0d63-150">媒体终结点在媒体中继服务器上分配的网络端口号。</span><span class="sxs-lookup"><span data-stu-id="c0d63-150">Network port number allocated on the media relay server by the media endpoint.</span></span>|
|<span data-ttu-id="c0d63-151">sentQualityEventRatio</span><span class="sxs-lookup"><span data-stu-id="c0d63-151">sentQualityEventRatio</span></span>|<span data-ttu-id="c0d63-152">双精度</span><span class="sxs-lookup"><span data-stu-id="c0d63-152">Double</span></span>|<span data-ttu-id="c0d63-153">媒体终结点检测到网络的呼叫的分数导致发送的音频质量较差。</span><span class="sxs-lookup"><span data-stu-id="c0d63-153">Fraction of the call that the media endpoint detected the network was causing poor quality of the audio sent.</span></span>|
|<span data-ttu-id="c0d63-154">子网</span><span class="sxs-lookup"><span data-stu-id="c0d63-154">subnet</span></span>|<span data-ttu-id="c0d63-155">String</span><span class="sxs-lookup"><span data-stu-id="c0d63-155">String</span></span>|<span data-ttu-id="c0d63-156">媒体终结点用于媒体流的子网。</span><span class="sxs-lookup"><span data-stu-id="c0d63-156">Subnet used for media stream by the media endpoint.</span></span>|
|<span data-ttu-id="c0d63-157">wifiBand</span><span class="sxs-lookup"><span data-stu-id="c0d63-157">wifiBand</span></span>|<span data-ttu-id="c0d63-158">String</span><span class="sxs-lookup"><span data-stu-id="c0d63-158">String</span></span>|<span data-ttu-id="c0d63-159">媒体终结点使用的 WiFi 波段。</span><span class="sxs-lookup"><span data-stu-id="c0d63-159">WiFi band used by the media endpoint.</span></span> <span data-ttu-id="c0d63-160">可取值为：`unknown`、`frequency24GHz`、`frequency50GHz`。</span><span class="sxs-lookup"><span data-stu-id="c0d63-160">Possible values are: `unknown`, `frequency24GHz`, `frequency50GHz`.</span></span>|
|<span data-ttu-id="c0d63-161">wifiBatteryCharge</span><span class="sxs-lookup"><span data-stu-id="c0d63-161">wifiBatteryCharge</span></span>|<span data-ttu-id="c0d63-162">Int32</span><span class="sxs-lookup"><span data-stu-id="c0d63-162">Int32</span></span>|<span data-ttu-id="c0d63-163">按媒体终结点报告的百分比估计剩余电池电量。</span><span class="sxs-lookup"><span data-stu-id="c0d63-163">Estimated remaining battery charge in percentage reported by the media endpoint.</span></span>|
|<span data-ttu-id="c0d63-164">wifiChannel</span><span class="sxs-lookup"><span data-stu-id="c0d63-164">wifiChannel</span></span>|<span data-ttu-id="c0d63-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c0d63-165">Int32</span></span>|<span data-ttu-id="c0d63-166">媒体终结点使用的 WiFi 通道。</span><span class="sxs-lookup"><span data-stu-id="c0d63-166">WiFi channel used by the media endpoint.</span></span>|
|<span data-ttu-id="c0d63-167">wifiMicrosoftDriver</span><span class="sxs-lookup"><span data-stu-id="c0d63-167">wifiMicrosoftDriver</span></span>|<span data-ttu-id="c0d63-168">String</span><span class="sxs-lookup"><span data-stu-id="c0d63-168">String</span></span>|<span data-ttu-id="c0d63-169">媒体终结点使用的 Microsoft WiFi 驱动程序的名称。</span><span class="sxs-lookup"><span data-stu-id="c0d63-169">Name of the Microsoft WiFi driver used by the media endpoint.</span></span> <span data-ttu-id="c0d63-170">值可能根据终结点使用的语言进行本地化。</span><span class="sxs-lookup"><span data-stu-id="c0d63-170">Value may be localized based on the language used by endpoint.</span></span>|
|<span data-ttu-id="c0d63-171">wifiMicrosoftDriverVersion</span><span class="sxs-lookup"><span data-stu-id="c0d63-171">wifiMicrosoftDriverVersion</span></span>|<span data-ttu-id="c0d63-172">String</span><span class="sxs-lookup"><span data-stu-id="c0d63-172">String</span></span>|<span data-ttu-id="c0d63-173">媒体终结点使用的 Microsoft WiFi 驱动程序的版本。</span><span class="sxs-lookup"><span data-stu-id="c0d63-173">Version of the Microsoft WiFi driver used by the media endpoint.</span></span>|
|<span data-ttu-id="c0d63-174">wifiRadioType</span><span class="sxs-lookup"><span data-stu-id="c0d63-174">wifiRadioType</span></span>|<span data-ttu-id="c0d63-175">String</span><span class="sxs-lookup"><span data-stu-id="c0d63-175">String</span></span>|<span data-ttu-id="c0d63-176">媒体终结点使用的 WiFi 无线电的类型。</span><span class="sxs-lookup"><span data-stu-id="c0d63-176">Type of WiFi radio used by the media endpoint.</span></span> <span data-ttu-id="c0d63-177">可取值为：`unknown`、`wifi80211a`、`wifi80211b`、`wifi80211g`、`wifi80211n`、`wifi80211ac`、`wifi80211ax`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c0d63-177">Possible values are: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c0d63-178">wifiSignalStrength</span><span class="sxs-lookup"><span data-stu-id="c0d63-178">wifiSignalStrength</span></span>|<span data-ttu-id="c0d63-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c0d63-179">Int32</span></span>|<span data-ttu-id="c0d63-180">以媒体终结点报告的百分比表示的 WiFi 信号强度。</span><span class="sxs-lookup"><span data-stu-id="c0d63-180">WiFi signal strength in percentage reported by the media endpoint.</span></span>|
|<span data-ttu-id="c0d63-181">wifiVendorDriver</span><span class="sxs-lookup"><span data-stu-id="c0d63-181">wifiVendorDriver</span></span>|<span data-ttu-id="c0d63-182">String</span><span class="sxs-lookup"><span data-stu-id="c0d63-182">String</span></span>|<span data-ttu-id="c0d63-183">媒体终结点使用的 WiFi 驱动程序的名称。</span><span class="sxs-lookup"><span data-stu-id="c0d63-183">Name of the WiFi driver used by the media endpoint.</span></span> <span data-ttu-id="c0d63-184">值可能根据终结点使用的语言进行本地化。</span><span class="sxs-lookup"><span data-stu-id="c0d63-184">Value may be localized based on the language used by endpoint.</span></span>|
|<span data-ttu-id="c0d63-185">wifiVendorDriverVersion</span><span class="sxs-lookup"><span data-stu-id="c0d63-185">wifiVendorDriverVersion</span></span>|<span data-ttu-id="c0d63-186">String</span><span class="sxs-lookup"><span data-stu-id="c0d63-186">String</span></span>|<span data-ttu-id="c0d63-187">媒体终结点使用的 WiFi 驱动程序的版本。</span><span class="sxs-lookup"><span data-stu-id="c0d63-187">Version of the WiFi driver used by the media endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0d63-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0d63-188">JSON representation</span></span>

<span data-ttu-id="c0d63-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0d63-189">The following is a JSON representation of the resource.</span></span>

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