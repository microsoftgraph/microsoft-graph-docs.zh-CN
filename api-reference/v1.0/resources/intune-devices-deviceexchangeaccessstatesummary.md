---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 25bc1fe1592b2aa1a1f0cde1b4bf45b6092a36d9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407034"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="fc675-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc675-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="fc675-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc675-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc675-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc675-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc675-106">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="fc675-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="fc675-107">属性</span><span class="sxs-lookup"><span data-stu-id="fc675-107">Properties</span></span>
|<span data-ttu-id="fc675-108">属性</span><span class="sxs-lookup"><span data-stu-id="fc675-108">Property</span></span>|<span data-ttu-id="fc675-109">类型</span><span class="sxs-lookup"><span data-stu-id="fc675-109">Type</span></span>|<span data-ttu-id="fc675-110">说明</span><span class="sxs-lookup"><span data-stu-id="fc675-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc675-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fc675-111">allowedDeviceCount</span></span>|<span data-ttu-id="fc675-112">Int32</span><span class="sxs-lookup"><span data-stu-id="fc675-112">Int32</span></span>|<span data-ttu-id="fc675-113">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="fc675-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="fc675-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fc675-114">blockedDeviceCount</span></span>|<span data-ttu-id="fc675-115">Int32</span><span class="sxs-lookup"><span data-stu-id="fc675-115">Int32</span></span>|<span data-ttu-id="fc675-116">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="fc675-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="fc675-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fc675-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="fc675-118">Int32</span><span class="sxs-lookup"><span data-stu-id="fc675-118">Int32</span></span>|<span data-ttu-id="fc675-119">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="fc675-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="fc675-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fc675-120">unknownDeviceCount</span></span>|<span data-ttu-id="fc675-121">Int32</span><span class="sxs-lookup"><span data-stu-id="fc675-121">Int32</span></span>|<span data-ttu-id="fc675-122">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="fc675-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="fc675-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fc675-123">unavailableDeviceCount</span></span>|<span data-ttu-id="fc675-124">Int32</span><span class="sxs-lookup"><span data-stu-id="fc675-124">Int32</span></span>|<span data-ttu-id="fc675-125">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="fc675-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc675-126">关系</span><span class="sxs-lookup"><span data-stu-id="fc675-126">Relationships</span></span>
<span data-ttu-id="fc675-127">无</span><span class="sxs-lookup"><span data-stu-id="fc675-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc675-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc675-128">JSON Representation</span></span>
<span data-ttu-id="fc675-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc675-129">Here is a JSON representation of the resource.</span></span>
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







