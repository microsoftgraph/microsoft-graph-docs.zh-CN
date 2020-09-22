---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fb64307c12dcaf7b4e4fd0443001db7c6190c6fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091255"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="1eda6-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="1eda6-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="1eda6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1eda6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1eda6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1eda6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1eda6-106">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="1eda6-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="1eda6-107">属性</span><span class="sxs-lookup"><span data-stu-id="1eda6-107">Properties</span></span>
|<span data-ttu-id="1eda6-108">属性</span><span class="sxs-lookup"><span data-stu-id="1eda6-108">Property</span></span>|<span data-ttu-id="1eda6-109">类型</span><span class="sxs-lookup"><span data-stu-id="1eda6-109">Type</span></span>|<span data-ttu-id="1eda6-110">说明</span><span class="sxs-lookup"><span data-stu-id="1eda6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1eda6-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1eda6-111">allowedDeviceCount</span></span>|<span data-ttu-id="1eda6-112">Int32</span><span class="sxs-lookup"><span data-stu-id="1eda6-112">Int32</span></span>|<span data-ttu-id="1eda6-113">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="1eda6-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="1eda6-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1eda6-114">blockedDeviceCount</span></span>|<span data-ttu-id="1eda6-115">Int32</span><span class="sxs-lookup"><span data-stu-id="1eda6-115">Int32</span></span>|<span data-ttu-id="1eda6-116">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="1eda6-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="1eda6-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1eda6-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="1eda6-118">Int32</span><span class="sxs-lookup"><span data-stu-id="1eda6-118">Int32</span></span>|<span data-ttu-id="1eda6-119">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="1eda6-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="1eda6-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1eda6-120">unknownDeviceCount</span></span>|<span data-ttu-id="1eda6-121">Int32</span><span class="sxs-lookup"><span data-stu-id="1eda6-121">Int32</span></span>|<span data-ttu-id="1eda6-122">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="1eda6-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="1eda6-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1eda6-123">unavailableDeviceCount</span></span>|<span data-ttu-id="1eda6-124">Int32</span><span class="sxs-lookup"><span data-stu-id="1eda6-124">Int32</span></span>|<span data-ttu-id="1eda6-125">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="1eda6-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1eda6-126">关系</span><span class="sxs-lookup"><span data-stu-id="1eda6-126">Relationships</span></span>
<span data-ttu-id="1eda6-127">无</span><span class="sxs-lookup"><span data-stu-id="1eda6-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1eda6-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1eda6-128">JSON Representation</span></span>
<span data-ttu-id="1eda6-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1eda6-129">Here is a JSON representation of the resource.</span></span>
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









