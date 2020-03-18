---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c7f26e49217ea43e64e43e9cdd4cce4b88bae561
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785005"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="3e215-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e215-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="3e215-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e215-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e215-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e215-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e215-106">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="3e215-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="3e215-107">属性</span><span class="sxs-lookup"><span data-stu-id="3e215-107">Properties</span></span>
|<span data-ttu-id="3e215-108">属性</span><span class="sxs-lookup"><span data-stu-id="3e215-108">Property</span></span>|<span data-ttu-id="3e215-109">类型</span><span class="sxs-lookup"><span data-stu-id="3e215-109">Type</span></span>|<span data-ttu-id="3e215-110">说明</span><span class="sxs-lookup"><span data-stu-id="3e215-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e215-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e215-111">allowedDeviceCount</span></span>|<span data-ttu-id="3e215-112">Int32</span><span class="sxs-lookup"><span data-stu-id="3e215-112">Int32</span></span>|<span data-ttu-id="3e215-113">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="3e215-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="3e215-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e215-114">blockedDeviceCount</span></span>|<span data-ttu-id="3e215-115">Int32</span><span class="sxs-lookup"><span data-stu-id="3e215-115">Int32</span></span>|<span data-ttu-id="3e215-116">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="3e215-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="3e215-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e215-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="3e215-118">Int32</span><span class="sxs-lookup"><span data-stu-id="3e215-118">Int32</span></span>|<span data-ttu-id="3e215-119">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="3e215-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="3e215-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e215-120">unknownDeviceCount</span></span>|<span data-ttu-id="3e215-121">Int32</span><span class="sxs-lookup"><span data-stu-id="3e215-121">Int32</span></span>|<span data-ttu-id="3e215-122">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="3e215-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="3e215-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e215-123">unavailableDeviceCount</span></span>|<span data-ttu-id="3e215-124">Int32</span><span class="sxs-lookup"><span data-stu-id="3e215-124">Int32</span></span>|<span data-ttu-id="3e215-125">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="3e215-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e215-126">关系</span><span class="sxs-lookup"><span data-stu-id="3e215-126">Relationships</span></span>
<span data-ttu-id="3e215-127">无</span><span class="sxs-lookup"><span data-stu-id="3e215-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e215-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e215-128">JSON Representation</span></span>
<span data-ttu-id="3e215-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e215-129">Here is a JSON representation of the resource.</span></span>
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



