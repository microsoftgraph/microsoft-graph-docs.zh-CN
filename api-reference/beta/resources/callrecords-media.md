---
title: 媒体资源类型
description: 媒体类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f550c898eda95026d5058c09d0e03f1064887509
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071534"
---
# <a name="media-resource-type"></a><span data-ttu-id="75c37-103">媒体资源类型</span><span class="sxs-lookup"><span data-stu-id="75c37-103">media resource type</span></span>

<span data-ttu-id="75c37-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="75c37-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75c37-105">表示在呼叫中使用的媒体 (音频、视频、基于视频的屏幕共享等 ) 。</span><span class="sxs-lookup"><span data-stu-id="75c37-105">Represents the media (audio, video, video-based screen-sharing, etc.) used in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="75c37-106">属性</span><span class="sxs-lookup"><span data-stu-id="75c37-106">Properties</span></span>

| <span data-ttu-id="75c37-107">属性</span><span class="sxs-lookup"><span data-stu-id="75c37-107">Property</span></span>     | <span data-ttu-id="75c37-108">类型</span><span class="sxs-lookup"><span data-stu-id="75c37-108">Type</span></span>        | <span data-ttu-id="75c37-109">说明</span><span class="sxs-lookup"><span data-stu-id="75c37-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="75c37-110">label</span><span class="sxs-lookup"><span data-stu-id="75c37-110">label</span></span>|<span data-ttu-id="75c37-111">String</span><span class="sxs-lookup"><span data-stu-id="75c37-111">String</span></span>|<span data-ttu-id="75c37-112">媒体在媒体协商阶段中的标识方式。</span><span class="sxs-lookup"><span data-stu-id="75c37-112">How the media was identified during media negotiation stage.</span></span>|
|<span data-ttu-id="75c37-113">callerDevice</span><span class="sxs-lookup"><span data-stu-id="75c37-113">callerDevice</span></span>|[<span data-ttu-id="75c37-114">callRecords。 deviceInfo</span><span class="sxs-lookup"><span data-stu-id="75c37-114">microsoft.graph.callRecords.deviceInfo</span></span>](callrecords-deviceinfo.md)|<span data-ttu-id="75c37-115">与此媒体的呼叫方终结点关联的设备信息。</span><span class="sxs-lookup"><span data-stu-id="75c37-115">Device information associated with the caller endpoint of this media.</span></span>|
|<span data-ttu-id="75c37-116">callerNetwork</span><span class="sxs-lookup"><span data-stu-id="75c37-116">callerNetwork</span></span>|[<span data-ttu-id="75c37-117">callRecords。 networkInfo</span><span class="sxs-lookup"><span data-stu-id="75c37-117">microsoft.graph.callRecords.networkInfo</span></span>](callrecords-networkinfo.md)|<span data-ttu-id="75c37-118">与此媒体的呼叫方终结点关联的网络信息。</span><span class="sxs-lookup"><span data-stu-id="75c37-118">Network information associated with the caller endpoint of this media.</span></span>|
|<span data-ttu-id="75c37-119">calleeDevice</span><span class="sxs-lookup"><span data-stu-id="75c37-119">calleeDevice</span></span>|[<span data-ttu-id="75c37-120">callRecords。 deviceInfo</span><span class="sxs-lookup"><span data-stu-id="75c37-120">microsoft.graph.callRecords.deviceInfo</span></span>](callrecords-deviceinfo.md)|<span data-ttu-id="75c37-121">与此媒体的被呼叫者终结点关联的设备信息。</span><span class="sxs-lookup"><span data-stu-id="75c37-121">Device information associated with the callee endpoint of this media.</span></span>|
|<span data-ttu-id="75c37-122">calleeNetwork</span><span class="sxs-lookup"><span data-stu-id="75c37-122">calleeNetwork</span></span>|[<span data-ttu-id="75c37-123">callRecords。 networkInfo</span><span class="sxs-lookup"><span data-stu-id="75c37-123">microsoft.graph.callRecords.networkInfo</span></span>](callrecords-networkinfo.md)|<span data-ttu-id="75c37-124">与此媒体的被呼叫者终结点关联的网络信息。</span><span class="sxs-lookup"><span data-stu-id="75c37-124">Network information associated with the callee endpoint of this media.</span></span>|
|<span data-ttu-id="75c37-125">连续流</span><span class="sxs-lookup"><span data-stu-id="75c37-125">streams</span></span>|<span data-ttu-id="75c37-126">[callRecords](callrecords-mediastream.md) 集合的 mediaStream</span><span class="sxs-lookup"><span data-stu-id="75c37-126">[microsoft.graph.callRecords.mediaStream](callrecords-mediastream.md) collection</span></span>|<span data-ttu-id="75c37-127">与此媒体关联的网络流。</span><span class="sxs-lookup"><span data-stu-id="75c37-127">Network streams associated with this media.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75c37-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75c37-128">JSON representation</span></span>

<span data-ttu-id="75c37-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75c37-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.media",
  "baseType": null
}-->

```json
{
  "label": "String",
  "callerDevice": {"@odata.type": "microsoft.graph.callRecords.deviceInfo"},
  "callerNetwork": {"@odata.type": "microsoft.graph.callRecords.networkInfo"},
  "calleeDevice": {"@odata.type": "microsoft.graph.callRecords.deviceInfo"},
  "calleeNetwork": {"@odata.type": "microsoft.graph.callRecords.networkInfo"},
  "streams": [{"@odata.type": "microsoft.graph.callRecords.mediaStream"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "media resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

