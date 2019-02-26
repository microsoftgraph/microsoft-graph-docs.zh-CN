---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c336ee6d4b23983f01a4c4756325960c709194f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260513"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="10ce2-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="10ce2-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="10ce2-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10ce2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10ce2-105">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="10ce2-105">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="10ce2-106">属性</span><span class="sxs-lookup"><span data-stu-id="10ce2-106">Properties</span></span>
|<span data-ttu-id="10ce2-107">属性</span><span class="sxs-lookup"><span data-stu-id="10ce2-107">Property</span></span>|<span data-ttu-id="10ce2-108">类型</span><span class="sxs-lookup"><span data-stu-id="10ce2-108">Type</span></span>|<span data-ttu-id="10ce2-109">说明</span><span class="sxs-lookup"><span data-stu-id="10ce2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10ce2-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10ce2-110">allowedDeviceCount</span></span>|<span data-ttu-id="10ce2-111">Int32</span><span class="sxs-lookup"><span data-stu-id="10ce2-111">Int32</span></span>|<span data-ttu-id="10ce2-112">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="10ce2-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="10ce2-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10ce2-113">blockedDeviceCount</span></span>|<span data-ttu-id="10ce2-114">Int32</span><span class="sxs-lookup"><span data-stu-id="10ce2-114">Int32</span></span>|<span data-ttu-id="10ce2-115">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="10ce2-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="10ce2-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10ce2-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="10ce2-117">Int32</span><span class="sxs-lookup"><span data-stu-id="10ce2-117">Int32</span></span>|<span data-ttu-id="10ce2-118">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="10ce2-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="10ce2-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10ce2-119">unknownDeviceCount</span></span>|<span data-ttu-id="10ce2-120">Int32</span><span class="sxs-lookup"><span data-stu-id="10ce2-120">Int32</span></span>|<span data-ttu-id="10ce2-121">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="10ce2-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="10ce2-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10ce2-122">unavailableDeviceCount</span></span>|<span data-ttu-id="10ce2-123">Int32</span><span class="sxs-lookup"><span data-stu-id="10ce2-123">Int32</span></span>|<span data-ttu-id="10ce2-124">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="10ce2-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10ce2-125">关系</span><span class="sxs-lookup"><span data-stu-id="10ce2-125">Relationships</span></span>
<span data-ttu-id="10ce2-126">无</span><span class="sxs-lookup"><span data-stu-id="10ce2-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10ce2-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10ce2-127">JSON Representation</span></span>
<span data-ttu-id="10ce2-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10ce2-128">Here is a JSON representation of the resource.</span></span>
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



