---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c336ee6d4b23983f01a4c4756325960c709194f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541988"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="ce48a-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce48a-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="ce48a-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce48a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce48a-105">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="ce48a-105">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="ce48a-106">属性</span><span class="sxs-lookup"><span data-stu-id="ce48a-106">Properties</span></span>
|<span data-ttu-id="ce48a-107">属性</span><span class="sxs-lookup"><span data-stu-id="ce48a-107">Property</span></span>|<span data-ttu-id="ce48a-108">类型</span><span class="sxs-lookup"><span data-stu-id="ce48a-108">Type</span></span>|<span data-ttu-id="ce48a-109">说明</span><span class="sxs-lookup"><span data-stu-id="ce48a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce48a-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ce48a-110">allowedDeviceCount</span></span>|<span data-ttu-id="ce48a-111">Int32</span><span class="sxs-lookup"><span data-stu-id="ce48a-111">Int32</span></span>|<span data-ttu-id="ce48a-112">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="ce48a-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="ce48a-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ce48a-113">blockedDeviceCount</span></span>|<span data-ttu-id="ce48a-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ce48a-114">Int32</span></span>|<span data-ttu-id="ce48a-115">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="ce48a-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="ce48a-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ce48a-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="ce48a-117">Int32</span><span class="sxs-lookup"><span data-stu-id="ce48a-117">Int32</span></span>|<span data-ttu-id="ce48a-118">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="ce48a-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="ce48a-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ce48a-119">unknownDeviceCount</span></span>|<span data-ttu-id="ce48a-120">Int32</span><span class="sxs-lookup"><span data-stu-id="ce48a-120">Int32</span></span>|<span data-ttu-id="ce48a-121">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="ce48a-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="ce48a-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ce48a-122">unavailableDeviceCount</span></span>|<span data-ttu-id="ce48a-123">Int32</span><span class="sxs-lookup"><span data-stu-id="ce48a-123">Int32</span></span>|<span data-ttu-id="ce48a-124">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="ce48a-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce48a-125">关系</span><span class="sxs-lookup"><span data-stu-id="ce48a-125">Relationships</span></span>
<span data-ttu-id="ce48a-126">无</span><span class="sxs-lookup"><span data-stu-id="ce48a-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce48a-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce48a-127">JSON Representation</span></span>
<span data-ttu-id="ce48a-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce48a-128">Here is a JSON representation of the resource.</span></span>
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



