---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 81f9768deaaeebfaebf02beff35a70e795244050
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983139"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="2d521-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d521-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="2d521-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2d521-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d521-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d521-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d521-106">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="2d521-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="2d521-107">属性</span><span class="sxs-lookup"><span data-stu-id="2d521-107">Properties</span></span>
|<span data-ttu-id="2d521-108">属性</span><span class="sxs-lookup"><span data-stu-id="2d521-108">Property</span></span>|<span data-ttu-id="2d521-109">类型</span><span class="sxs-lookup"><span data-stu-id="2d521-109">Type</span></span>|<span data-ttu-id="2d521-110">说明</span><span class="sxs-lookup"><span data-stu-id="2d521-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d521-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d521-111">allowedDeviceCount</span></span>|<span data-ttu-id="2d521-112">Int32</span><span class="sxs-lookup"><span data-stu-id="2d521-112">Int32</span></span>|<span data-ttu-id="2d521-113">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="2d521-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="2d521-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d521-114">blockedDeviceCount</span></span>|<span data-ttu-id="2d521-115">Int32</span><span class="sxs-lookup"><span data-stu-id="2d521-115">Int32</span></span>|<span data-ttu-id="2d521-116">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="2d521-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="2d521-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d521-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="2d521-118">Int32</span><span class="sxs-lookup"><span data-stu-id="2d521-118">Int32</span></span>|<span data-ttu-id="2d521-119">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="2d521-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="2d521-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d521-120">unknownDeviceCount</span></span>|<span data-ttu-id="2d521-121">Int32</span><span class="sxs-lookup"><span data-stu-id="2d521-121">Int32</span></span>|<span data-ttu-id="2d521-122">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="2d521-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="2d521-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d521-123">unavailableDeviceCount</span></span>|<span data-ttu-id="2d521-124">Int32</span><span class="sxs-lookup"><span data-stu-id="2d521-124">Int32</span></span>|<span data-ttu-id="2d521-125">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="2d521-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d521-126">关系</span><span class="sxs-lookup"><span data-stu-id="2d521-126">Relationships</span></span>
<span data-ttu-id="2d521-127">无</span><span class="sxs-lookup"><span data-stu-id="2d521-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d521-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d521-128">JSON Representation</span></span>
<span data-ttu-id="2d521-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d521-129">Here is a JSON representation of the resource.</span></span>
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





