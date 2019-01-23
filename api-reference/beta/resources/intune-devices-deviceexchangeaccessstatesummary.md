---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a01a1207801063285d7b59f0fa51c474ae78fb6d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418552"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="39968-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="39968-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="39968-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="39968-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="39968-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="39968-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39968-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="39968-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39968-107">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="39968-107">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="39968-108">属性</span><span class="sxs-lookup"><span data-stu-id="39968-108">Properties</span></span>
|<span data-ttu-id="39968-109">属性</span><span class="sxs-lookup"><span data-stu-id="39968-109">Property</span></span>|<span data-ttu-id="39968-110">类型</span><span class="sxs-lookup"><span data-stu-id="39968-110">Type</span></span>|<span data-ttu-id="39968-111">说明</span><span class="sxs-lookup"><span data-stu-id="39968-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39968-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39968-112">allowedDeviceCount</span></span>|<span data-ttu-id="39968-113">Int32</span><span class="sxs-lookup"><span data-stu-id="39968-113">Int32</span></span>|<span data-ttu-id="39968-114">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="39968-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="39968-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39968-115">blockedDeviceCount</span></span>|<span data-ttu-id="39968-116">Int32</span><span class="sxs-lookup"><span data-stu-id="39968-116">Int32</span></span>|<span data-ttu-id="39968-117">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="39968-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="39968-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39968-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="39968-119">Int32</span><span class="sxs-lookup"><span data-stu-id="39968-119">Int32</span></span>|<span data-ttu-id="39968-120">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="39968-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="39968-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39968-121">unknownDeviceCount</span></span>|<span data-ttu-id="39968-122">Int32</span><span class="sxs-lookup"><span data-stu-id="39968-122">Int32</span></span>|<span data-ttu-id="39968-123">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="39968-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="39968-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39968-124">unavailableDeviceCount</span></span>|<span data-ttu-id="39968-125">Int32</span><span class="sxs-lookup"><span data-stu-id="39968-125">Int32</span></span>|<span data-ttu-id="39968-126">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="39968-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39968-127">关系</span><span class="sxs-lookup"><span data-stu-id="39968-127">Relationships</span></span>
<span data-ttu-id="39968-128">无</span><span class="sxs-lookup"><span data-stu-id="39968-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39968-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39968-129">JSON Representation</span></span>
<span data-ttu-id="39968-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39968-130">Here is a JSON representation of the resource.</span></span>
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




