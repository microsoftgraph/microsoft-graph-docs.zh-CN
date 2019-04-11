---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39f944b7559abf72d144f5c1608ec4efec014530
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792438"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="a4298-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4298-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="a4298-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4298-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4298-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4298-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4298-106">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="a4298-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="a4298-107">属性</span><span class="sxs-lookup"><span data-stu-id="a4298-107">Properties</span></span>
|<span data-ttu-id="a4298-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4298-108">Property</span></span>|<span data-ttu-id="a4298-109">类型</span><span class="sxs-lookup"><span data-stu-id="a4298-109">Type</span></span>|<span data-ttu-id="a4298-110">说明</span><span class="sxs-lookup"><span data-stu-id="a4298-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4298-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4298-111">allowedDeviceCount</span></span>|<span data-ttu-id="a4298-112">Int32</span><span class="sxs-lookup"><span data-stu-id="a4298-112">Int32</span></span>|<span data-ttu-id="a4298-113">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a4298-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="a4298-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4298-114">blockedDeviceCount</span></span>|<span data-ttu-id="a4298-115">Int32</span><span class="sxs-lookup"><span data-stu-id="a4298-115">Int32</span></span>|<span data-ttu-id="a4298-116">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a4298-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="a4298-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4298-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="a4298-118">Int32</span><span class="sxs-lookup"><span data-stu-id="a4298-118">Int32</span></span>|<span data-ttu-id="a4298-119">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a4298-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="a4298-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4298-120">unknownDeviceCount</span></span>|<span data-ttu-id="a4298-121">Int32</span><span class="sxs-lookup"><span data-stu-id="a4298-121">Int32</span></span>|<span data-ttu-id="a4298-122">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a4298-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="a4298-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4298-123">unavailableDeviceCount</span></span>|<span data-ttu-id="a4298-124">Int32</span><span class="sxs-lookup"><span data-stu-id="a4298-124">Int32</span></span>|<span data-ttu-id="a4298-125">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a4298-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4298-126">关系</span><span class="sxs-lookup"><span data-stu-id="a4298-126">Relationships</span></span>
<span data-ttu-id="a4298-127">无</span><span class="sxs-lookup"><span data-stu-id="a4298-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4298-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4298-128">JSON Representation</span></span>
<span data-ttu-id="a4298-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4298-129">Here is a JSON representation of the resource.</span></span>
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





