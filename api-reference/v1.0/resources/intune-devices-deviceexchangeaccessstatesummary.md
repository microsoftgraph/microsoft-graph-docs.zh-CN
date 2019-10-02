---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3210643c68a7b5a94bfa3b4f601a2e34efe68e13
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356973"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="5fe07-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="5fe07-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="5fe07-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5fe07-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fe07-105">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="5fe07-105">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="5fe07-106">属性</span><span class="sxs-lookup"><span data-stu-id="5fe07-106">Properties</span></span>
|<span data-ttu-id="5fe07-107">属性</span><span class="sxs-lookup"><span data-stu-id="5fe07-107">Property</span></span>|<span data-ttu-id="5fe07-108">类型</span><span class="sxs-lookup"><span data-stu-id="5fe07-108">Type</span></span>|<span data-ttu-id="5fe07-109">说明</span><span class="sxs-lookup"><span data-stu-id="5fe07-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fe07-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5fe07-110">allowedDeviceCount</span></span>|<span data-ttu-id="5fe07-111">Int32</span><span class="sxs-lookup"><span data-stu-id="5fe07-111">Int32</span></span>|<span data-ttu-id="5fe07-112">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="5fe07-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="5fe07-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5fe07-113">blockedDeviceCount</span></span>|<span data-ttu-id="5fe07-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5fe07-114">Int32</span></span>|<span data-ttu-id="5fe07-115">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="5fe07-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="5fe07-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5fe07-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="5fe07-117">Int32</span><span class="sxs-lookup"><span data-stu-id="5fe07-117">Int32</span></span>|<span data-ttu-id="5fe07-118">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="5fe07-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="5fe07-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5fe07-119">unknownDeviceCount</span></span>|<span data-ttu-id="5fe07-120">Int32</span><span class="sxs-lookup"><span data-stu-id="5fe07-120">Int32</span></span>|<span data-ttu-id="5fe07-121">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="5fe07-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="5fe07-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5fe07-122">unavailableDeviceCount</span></span>|<span data-ttu-id="5fe07-123">Int32</span><span class="sxs-lookup"><span data-stu-id="5fe07-123">Int32</span></span>|<span data-ttu-id="5fe07-124">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="5fe07-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fe07-125">关系</span><span class="sxs-lookup"><span data-stu-id="5fe07-125">Relationships</span></span>
<span data-ttu-id="5fe07-126">无</span><span class="sxs-lookup"><span data-stu-id="5fe07-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fe07-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5fe07-127">JSON Representation</span></span>
<span data-ttu-id="5fe07-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fe07-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```




