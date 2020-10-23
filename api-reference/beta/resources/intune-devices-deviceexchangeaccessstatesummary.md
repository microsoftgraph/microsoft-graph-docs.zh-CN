---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cd20f76a810f37fde239cb523800d98bd8246700
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728235"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="0530d-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="0530d-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="0530d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0530d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0530d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0530d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0530d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0530d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0530d-107">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="0530d-107">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="0530d-108">属性</span><span class="sxs-lookup"><span data-stu-id="0530d-108">Properties</span></span>
|<span data-ttu-id="0530d-109">属性</span><span class="sxs-lookup"><span data-stu-id="0530d-109">Property</span></span>|<span data-ttu-id="0530d-110">类型</span><span class="sxs-lookup"><span data-stu-id="0530d-110">Type</span></span>|<span data-ttu-id="0530d-111">说明</span><span class="sxs-lookup"><span data-stu-id="0530d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0530d-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0530d-112">allowedDeviceCount</span></span>|<span data-ttu-id="0530d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="0530d-113">Int32</span></span>|<span data-ttu-id="0530d-114">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="0530d-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="0530d-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0530d-115">blockedDeviceCount</span></span>|<span data-ttu-id="0530d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="0530d-116">Int32</span></span>|<span data-ttu-id="0530d-117">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="0530d-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="0530d-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0530d-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="0530d-119">Int32</span><span class="sxs-lookup"><span data-stu-id="0530d-119">Int32</span></span>|<span data-ttu-id="0530d-120">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="0530d-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="0530d-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0530d-121">unknownDeviceCount</span></span>|<span data-ttu-id="0530d-122">Int32</span><span class="sxs-lookup"><span data-stu-id="0530d-122">Int32</span></span>|<span data-ttu-id="0530d-123">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="0530d-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="0530d-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0530d-124">unavailableDeviceCount</span></span>|<span data-ttu-id="0530d-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0530d-125">Int32</span></span>|<span data-ttu-id="0530d-126">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="0530d-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0530d-127">关系</span><span class="sxs-lookup"><span data-stu-id="0530d-127">Relationships</span></span>
<span data-ttu-id="0530d-128">无</span><span class="sxs-lookup"><span data-stu-id="0530d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0530d-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0530d-129">JSON Representation</span></span>
<span data-ttu-id="0530d-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0530d-130">Here is a JSON representation of the resource.</span></span>
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





