---
title: 调用： logTeleconferenceDeviceQuality
description: 日志视频电话会议设备质量数据。
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 664c86f7aee5d5e720f428b0f5ca502b0445c605
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42729982"
---
# <a name="call-logteleconferencedevicequality"></a><span data-ttu-id="b43a9-103">调用： logTeleconferenceDeviceQuality</span><span class="sxs-lookup"><span data-stu-id="b43a9-103">call: logTeleconferenceDeviceQuality</span></span>

<span data-ttu-id="b43a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b43a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b43a9-105">日志视频电话会议设备质量数据。</span><span class="sxs-lookup"><span data-stu-id="b43a9-105">Log video teleconferencing device quality data.</span></span>

<span data-ttu-id="b43a9-106">云视频互操作（CVI） bot 代表视频电话会议（VTC）设备，可充当会议呼叫中的 VTC 设备的后端代理。</span><span class="sxs-lookup"><span data-stu-id="b43a9-106">The Cloud Video Interop (CVI) bot represents video teleconferencing (VTC) devices and acts as a back-to-back agent for a VTC device in a conference call.</span></span> <span data-ttu-id="b43a9-107">由于 CVI bot 位于 VTC 和 Microsoft 团队基础结构的中间作为 VTC 代理，因此它具有两个媒体支线。</span><span class="sxs-lookup"><span data-stu-id="b43a9-107">Because a CVI bot is in the middle of the VTC and Microsoft Teams infrastructure as a VTC proxy, it has two media legs.</span></span> <span data-ttu-id="b43a9-108">一个媒体条在 CVI bot 和团队基础结构之间，例如团队会议服务器或团队客户端。</span><span class="sxs-lookup"><span data-stu-id="b43a9-108">One media leg is between the CVI bot and Teams infrastructure, such as Teams conference server or a Teams client.</span></span> <span data-ttu-id="b43a9-109">其他媒体腿位于 CVI bot 和 VTC 设备之间。</span><span class="sxs-lookup"><span data-stu-id="b43a9-109">The other media leg is between the CVI bot and the VTC device.</span></span> 

<span data-ttu-id="b43a9-110">第三方合作伙伴拥有 VTC 媒体腿，并且团队基础结构无法访问第三方呼叫线路的质量数据。</span><span class="sxs-lookup"><span data-stu-id="b43a9-110">The third-party partners own the VTC media leg and the Teams infrastructure cannot access the quality data of the third-party call leg.</span></span>  <span data-ttu-id="b43a9-111">此方法仅供 CVI 合作伙伴提供其媒体质量数据。</span><span class="sxs-lookup"><span data-stu-id="b43a9-111">This method is only for the CVI partners to provide their media quality data.</span></span>

## <a name="permissions"></a><span data-ttu-id="b43a9-112">权限</span><span class="sxs-lookup"><span data-stu-id="b43a9-112">Permissions</span></span>

<span data-ttu-id="b43a9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b43a9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b43a9-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="b43a9-115">Permission type</span></span>                        | <span data-ttu-id="b43a9-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b43a9-116">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b43a9-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b43a9-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="b43a9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b43a9-118">Not supported.</span></span> |
| <span data-ttu-id="b43a9-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b43a9-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b43a9-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="b43a9-120">Not supported.</span></span> |
| <span data-ttu-id="b43a9-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="b43a9-121">Application</span></span>                            | <span data-ttu-id="b43a9-122">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="b43a9-122">Calls.AccessMedia.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b43a9-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b43a9-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /communications/calls/logTeleconferenceDeviceQuality
```

## <a name="request-headers"></a><span data-ttu-id="b43a9-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="b43a9-124">Request headers</span></span>

| <span data-ttu-id="b43a9-125">名称</span><span class="sxs-lookup"><span data-stu-id="b43a9-125">Name</span></span>          | <span data-ttu-id="b43a9-126">说明</span><span class="sxs-lookup"><span data-stu-id="b43a9-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b43a9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b43a9-127">Authorization</span></span> | <span data-ttu-id="b43a9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b43a9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b43a9-130">用户代理</span><span class="sxs-lookup"><span data-stu-id="b43a9-130">User-Agent</span></span>    | <span data-ttu-id="b43a9-131">描述调用应用程序的名称和版本。</span><span class="sxs-lookup"><span data-stu-id="b43a9-131">Describes the name and version of the calling application.</span></span> <span data-ttu-id="b43a9-132">详细信息将在 Azure 信息保护分析中显现。</span><span class="sxs-lookup"><span data-stu-id="b43a9-132">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="b43a9-133">建议的格式为 "ApplicationName/版本"。</span><span class="sxs-lookup"><span data-stu-id="b43a9-133">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="b43a9-134">必需。</span><span class="sxs-lookup"><span data-stu-id="b43a9-134">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b43a9-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="b43a9-135">Request body</span></span>

<span data-ttu-id="b43a9-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b43a9-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b43a9-137">参数</span><span class="sxs-lookup"><span data-stu-id="b43a9-137">Parameter</span></span>    | <span data-ttu-id="b43a9-138">类型</span><span class="sxs-lookup"><span data-stu-id="b43a9-138">Type</span></span>        | <span data-ttu-id="b43a9-139">说明</span><span class="sxs-lookup"><span data-stu-id="b43a9-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b43a9-140">品质</span><span class="sxs-lookup"><span data-stu-id="b43a9-140">quality</span></span>|[<span data-ttu-id="b43a9-141">teleconferenceDeviceQuality</span><span class="sxs-lookup"><span data-stu-id="b43a9-141">teleconferenceDeviceQuality</span></span>](../resources/teleconferencedevicequality.md)|<span data-ttu-id="b43a9-142">VTC 媒体腿的质量数据。</span><span class="sxs-lookup"><span data-stu-id="b43a9-142">Quality data of VTC media leg.</span></span>|

## <a name="response"></a><span data-ttu-id="b43a9-143">响应</span><span class="sxs-lookup"><span data-stu-id="b43a9-143">Response</span></span>

<span data-ttu-id="b43a9-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b43a9-p106">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b43a9-146">示例</span><span class="sxs-lookup"><span data-stu-id="b43a9-146">Examples</span></span>

<span data-ttu-id="b43a9-147">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b43a9-147">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b43a9-148">请求</span><span class="sxs-lookup"><span data-stu-id="b43a9-148">Request</span></span>

<span data-ttu-id="b43a9-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b43a9-149">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "call_logteleconferencedevicequality"
}-->

```http
POST https://graph.microsoft.com/v1.0/app/calls/logTeleconferenceDeviceQuality
Content-type: application/json

{
  "quality": {
    "@odata.type": "#microsoft.graph.teleconferenceDeviceQuality",
    "callChainId": "0622673d-9f69-49b3-9d4f-5ec64f42ecce",
    "participantId": "ea078406-b5d4-4d3c-b85e-90103dcec7f6",
    "mediaLegId": "bd9ee398-4b9d-42c7-8b8d-4e8efad9435f",
    "deviceName": "TestAgent",
    "deviceDescription": "TestDescription",
    "mediaQualityList": [
      {
        "@odata.type": "#microsoft.graph.teleconferenceDeviceAudioQuality",
        "channelIndex": 1,
        "mediaDuration": "PT20M",
        "networkLinkSpeedInBytes": 13000,
        "localIPAddress": "127.0.0.1",
        "localPort": 6300,
        "remoteIPAddress": "102.1.1.101",
        "remotePort": 6301,
        "inboundPackets": 5500,
        "outboundPackets": 5400,
        "averageInboundPacketLossRateInPercentage": 0.01,
        "averageOutboundPacketLossRateInPercentage": 0.02,
        "maximumInboundPacketLossRateInPercentage": 0.05,
        "maximumOutboundPacketLossRateInPercentage": 0.06,
        "averageInboundRoundTripDelay": "PT0.03S",
        "averageOutboundRoundTripDelay": "PT0.04S",
        "maximumInboundRoundTripDelay": "PT0.13S",
        "maximumOutboundRoundTripDelay": "PT0.14S",
        "averageInboundJitter": "PT0.01S",
        "averageOutboundJitter": "PT0.015S",
        "maximumInboundJitter": "PT0.023S",
        "maximumOutboundJitter": "PT0.024S"
      },
      {
        "@odata.type": "#microsoft.graph.teleconferenceDeviceVideoQuality",
        "channelIndex": 1,
        "mediaDuration": "PT20M",
        "networkLinkSpeedInBytes": 13000,
        "localIPAddress": "127.0.0.1",
        "localPort": 6300,
        "remoteIPAddress": "102.1.1.101",
        "remotePort": 6301,
        "inboundPackets": 5500,
        "outboundPackets": 5400,
        "averageInboundPacketLossRateInPercentage": 0.01,
        "averageOutboundPacketLossRateInPercentage": 0.02,
        "maximumInboundPacketLossRateInPercentage": 0.05,
        "maximumOutboundPacketLossRateInPercentage": 0.06,
        "averageInboundRoundTripDelay": "PT0.03S",
        "averageOutboundRoundTripDelay": "PT0.04S",
        "maximumInboundRoundTripDelay": "PT0.13S",
        "maximumOutboundRoundTripDelay": "PT0.14S",
        "averageInboundJitter": "PT0.01S",
        "averageOutboundJitter": "PT0.015S",
        "maximumInboundJitter": "PT0.023S",
        "maximumOutboundJitter": "PT0.024S"
      },
      {
        "@odata.type": "#microsoft.graph.teleconferenceDeviceScreenSharingQuality",
        "channelIndex": 1,
        "mediaDuration": "PT20M",
        "networkLinkSpeedInBytes": 13000,
        "localIPAddress": "127.0.0.1",
        "localPort": 6300,
        "remoteIPAddress": "102.1.1.101",
        "remotePort": 6301,
        "inboundPackets": 5500,
        "outboundPackets": 5400,
        "averageInboundPacketLossRateInPercentage": 0.01,
        "averageOutboundPacketLossRateInPercentage": 0.02,
        "maximumInboundPacketLossRateInPercentage": 0.05,
        "maximumOutboundPacketLossRateInPercentage": 0.06,
        "averageInboundRoundTripDelay": "PT0.03S",
        "averageOutboundRoundTripDelay": "PT0.04S",
        "maximumInboundRoundTripDelay": "PT0.13S",
        "maximumOutboundRoundTripDelay": "PT0.14S",
        "averageInboundJitter": "PT0.01S",
        "averageOutboundJitter": "PT0.015S",
        "maximumInboundJitter": "PT0.023S",
        "maximumOutboundJitter": "PT0.024S"
      }
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="b43a9-150">响应</span><span class="sxs-lookup"><span data-stu-id="b43a9-150">Response</span></span>

<span data-ttu-id="b43a9-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b43a9-151">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: logTeleconferenceDeviceQuality",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
