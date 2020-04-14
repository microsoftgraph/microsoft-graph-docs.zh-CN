---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f4d336b5ee1cb5b4310298bf091b2f2f88cfaa1a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456869"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="a3ce9-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3ce9-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="a3ce9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3ce9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3ce9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a3ce9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3ce9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3ce9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3ce9-107">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="a3ce9-107">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="a3ce9-108">属性</span><span class="sxs-lookup"><span data-stu-id="a3ce9-108">Properties</span></span>
|<span data-ttu-id="a3ce9-109">属性</span><span class="sxs-lookup"><span data-stu-id="a3ce9-109">Property</span></span>|<span data-ttu-id="a3ce9-110">类型</span><span class="sxs-lookup"><span data-stu-id="a3ce9-110">Type</span></span>|<span data-ttu-id="a3ce9-111">说明</span><span class="sxs-lookup"><span data-stu-id="a3ce9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3ce9-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3ce9-112">allowedDeviceCount</span></span>|<span data-ttu-id="a3ce9-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a3ce9-113">Int32</span></span>|<span data-ttu-id="a3ce9-114">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a3ce9-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="a3ce9-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3ce9-115">blockedDeviceCount</span></span>|<span data-ttu-id="a3ce9-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a3ce9-116">Int32</span></span>|<span data-ttu-id="a3ce9-117">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a3ce9-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="a3ce9-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3ce9-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="a3ce9-119">Int32</span><span class="sxs-lookup"><span data-stu-id="a3ce9-119">Int32</span></span>|<span data-ttu-id="a3ce9-120">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a3ce9-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="a3ce9-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3ce9-121">unknownDeviceCount</span></span>|<span data-ttu-id="a3ce9-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a3ce9-122">Int32</span></span>|<span data-ttu-id="a3ce9-123">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a3ce9-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="a3ce9-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3ce9-124">unavailableDeviceCount</span></span>|<span data-ttu-id="a3ce9-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a3ce9-125">Int32</span></span>|<span data-ttu-id="a3ce9-126">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a3ce9-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3ce9-127">关系</span><span class="sxs-lookup"><span data-stu-id="a3ce9-127">Relationships</span></span>
<span data-ttu-id="a3ce9-128">无</span><span class="sxs-lookup"><span data-stu-id="a3ce9-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3ce9-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3ce9-129">JSON Representation</span></span>
<span data-ttu-id="a3ce9-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3ce9-130">Here is a JSON representation of the resource.</span></span>
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



