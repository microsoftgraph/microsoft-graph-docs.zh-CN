---
title: teleconferenceDeviceQuality 资源类型
description: 表示视频电话会议设备会话级别质量数据。
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4d76114a35a9ac7d0c9901437b672697c295ebbf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42763268"
---
# <a name="teleconferencedevicequality-resource-type"></a><span data-ttu-id="6fe04-103">teleconferenceDeviceQuality 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fe04-103">teleconferenceDeviceQuality resource type</span></span>

<span data-ttu-id="6fe04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fe04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fe04-105">表示视频电话会议设备会话级别质量数据。</span><span class="sxs-lookup"><span data-stu-id="6fe04-105">Represents video teleconferencing device session-level quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="6fe04-106">属性</span><span class="sxs-lookup"><span data-stu-id="6fe04-106">Properties</span></span>

| <span data-ttu-id="6fe04-107">属性</span><span class="sxs-lookup"><span data-stu-id="6fe04-107">Property</span></span>     | <span data-ttu-id="6fe04-108">类型</span><span class="sxs-lookup"><span data-stu-id="6fe04-108">Type</span></span>        | <span data-ttu-id="6fe04-109">说明</span><span class="sxs-lookup"><span data-stu-id="6fe04-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6fe04-110">callChainId</span><span class="sxs-lookup"><span data-stu-id="6fe04-110">callChainId</span></span>|<span data-ttu-id="6fe04-111">Guid</span><span class="sxs-lookup"><span data-stu-id="6fe04-111">Guid</span></span>|<span data-ttu-id="6fe04-112">会议中所有参与者调用的唯一标识符，或在 P2P 呼叫中两个参与者呼叫的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6fe04-112">A unique identifier for all  the participant calls in a conference or a unique identifier for two participant calls in P2P call.</span></span> <span data-ttu-id="6fe04-113">这需要通过复制`Microsoft.Graph.Call.CallChainId`。</span><span class="sxs-lookup"><span data-stu-id="6fe04-113">This needs to be copied over from `Microsoft.Graph.Call.CallChainId`.</span></span>|
|<span data-ttu-id="6fe04-114">cloudServiceDeploymentEnvironment</span><span class="sxs-lookup"><span data-stu-id="6fe04-114">cloudServiceDeploymentEnvironment</span></span>|<span data-ttu-id="6fe04-115">String</span><span class="sxs-lookup"><span data-stu-id="6fe04-115">String</span></span>|<span data-ttu-id="6fe04-116">部署服务的地理区域，例如`ProdNoam`。</span><span class="sxs-lookup"><span data-stu-id="6fe04-116">A geo-region where the service is deployed, such as `ProdNoam`.</span></span>|
|<span data-ttu-id="6fe04-117">cloudServiceDeploymentId</span><span class="sxs-lookup"><span data-stu-id="6fe04-117">cloudServiceDeploymentId</span></span>|<span data-ttu-id="6fe04-118">String</span><span class="sxs-lookup"><span data-stu-id="6fe04-118">String</span></span>|<span data-ttu-id="6fe04-119">由 Azure 分配的唯一部署标识符。</span><span class="sxs-lookup"><span data-stu-id="6fe04-119">A unique deployment identifier assigned by Azure.</span></span>|
|<span data-ttu-id="6fe04-120">cloudServiceInstanceName</span><span class="sxs-lookup"><span data-stu-id="6fe04-120">cloudServiceInstanceName</span></span>|<span data-ttu-id="6fe04-121">String</span><span class="sxs-lookup"><span data-stu-id="6fe04-121">String</span></span>|<span data-ttu-id="6fe04-122">Azure 部署的云服务实例名称，例如`FrontEnd_IN_3`。</span><span class="sxs-lookup"><span data-stu-id="6fe04-122">The Azure deployed cloud service instance name, such as `FrontEnd_IN_3`.</span></span>|
|<span data-ttu-id="6fe04-123">cloudServiceName</span><span class="sxs-lookup"><span data-stu-id="6fe04-123">cloudServiceName</span></span>|<span data-ttu-id="6fe04-124">String</span><span class="sxs-lookup"><span data-stu-id="6fe04-124">String</span></span>|<span data-ttu-id="6fe04-125">Azure 部署的云服务名称，例如`contoso.cloudapp.net`。</span><span class="sxs-lookup"><span data-stu-id="6fe04-125">The Azure deployed cloud service name, such as `contoso.cloudapp.net`.</span></span>|
|<span data-ttu-id="6fe04-126">deviceDescription</span><span class="sxs-lookup"><span data-stu-id="6fe04-126">deviceDescription</span></span>|<span data-ttu-id="6fe04-127">String</span><span class="sxs-lookup"><span data-stu-id="6fe04-127">String</span></span>|<span data-ttu-id="6fe04-128">任何其他说明，如`VTC Bldg 30/21`。</span><span class="sxs-lookup"><span data-stu-id="6fe04-128">Any additional description, such as `VTC Bldg 30/21`.</span></span>|
|<span data-ttu-id="6fe04-129">deviceName</span><span class="sxs-lookup"><span data-stu-id="6fe04-129">deviceName</span></span>|<span data-ttu-id="6fe04-130">String</span><span class="sxs-lookup"><span data-stu-id="6fe04-130">String</span></span>|<span data-ttu-id="6fe04-131">用户媒体代理名称，例如`Cisco SX80`。</span><span class="sxs-lookup"><span data-stu-id="6fe04-131">The user media agent name, such as `Cisco SX80`.</span></span>|
|<span data-ttu-id="6fe04-132">mediaLegId</span><span class="sxs-lookup"><span data-stu-id="6fe04-132">mediaLegId</span></span>|<span data-ttu-id="6fe04-133">Guid</span><span class="sxs-lookup"><span data-stu-id="6fe04-133">Guid</span></span>|<span data-ttu-id="6fe04-134">会议中参与者的特定媒体腿的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6fe04-134">A unique identifier for a specific media leg of a participant in a conference.</span></span>  <span data-ttu-id="6fe04-135">如果发生 retargeting，一个参与者可以有多个媒体支线标识符。</span><span class="sxs-lookup"><span data-stu-id="6fe04-135">One participant can have multiple media leg identifiers if retargeting happens.</span></span> <span data-ttu-id="6fe04-136">CVI 合作伙伴将分配此值。</span><span class="sxs-lookup"><span data-stu-id="6fe04-136">CVI partner assigns this value.</span></span>|
|<span data-ttu-id="6fe04-137">mediaQualityList</span><span class="sxs-lookup"><span data-stu-id="6fe04-137">mediaQualityList</span></span>|<span data-ttu-id="6fe04-138">[teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md)集合</span><span class="sxs-lookup"><span data-stu-id="6fe04-138">[teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md) collection</span></span>|<span data-ttu-id="6fe04-139">媒体会话（呼叫）中的媒体质量列表，例如音频质量、视频质量和/或屏幕共享质量。</span><span class="sxs-lookup"><span data-stu-id="6fe04-139">The list of media qualities in a media session (call), such as audio quality, video quality, and/or screen sharing quality.</span></span>|
|<span data-ttu-id="6fe04-140">participantId</span><span class="sxs-lookup"><span data-stu-id="6fe04-140">participantId</span></span>|<span data-ttu-id="6fe04-141">Guid</span><span class="sxs-lookup"><span data-stu-id="6fe04-141">Guid</span></span>|<span data-ttu-id="6fe04-142">会议中的特定参与者的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6fe04-142">A unique identifier for a specific participant in a conference.</span></span> <span data-ttu-id="6fe04-143">CVI 合作伙伴需要复制`Call.MyParticipantId`到此属性。</span><span class="sxs-lookup"><span data-stu-id="6fe04-143">The CVI partner needs to copy over `Call.MyParticipantId` to this property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fe04-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fe04-144">JSON representation</span></span>

<span data-ttu-id="6fe04-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fe04-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceQuality",
  "baseType": null
}-->

```json
{
  "callChainId": "Guid",
  "cloudServiceDeploymentEnvironment": "String",
  "cloudServiceDeploymentId": "String",
  "cloudServiceInstanceName": "String",
  "cloudServiceName": "String",
  "deviceDescription": "String",
  "deviceName": "String",
  "mediaLegId": "Guid",
  "mediaQualityList": [{"@odata.type": "microsoft.graph.teleconferenceDeviceMediaQuality"}],
  "participantId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teleconferenceDeviceQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
