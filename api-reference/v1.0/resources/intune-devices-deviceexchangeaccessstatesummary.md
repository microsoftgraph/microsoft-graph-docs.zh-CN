---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ee3f6ddb47025dfc4ff29305f45538cf23bfa8c6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754586"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="cd272-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd272-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="cd272-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd272-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd272-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd272-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd272-106">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="cd272-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="cd272-107">属性</span><span class="sxs-lookup"><span data-stu-id="cd272-107">Properties</span></span>
|<span data-ttu-id="cd272-108">属性</span><span class="sxs-lookup"><span data-stu-id="cd272-108">Property</span></span>|<span data-ttu-id="cd272-109">类型</span><span class="sxs-lookup"><span data-stu-id="cd272-109">Type</span></span>|<span data-ttu-id="cd272-110">Description</span><span class="sxs-lookup"><span data-stu-id="cd272-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd272-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cd272-111">allowedDeviceCount</span></span>|<span data-ttu-id="cd272-112">Int32</span><span class="sxs-lookup"><span data-stu-id="cd272-112">Int32</span></span>|<span data-ttu-id="cd272-113">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="cd272-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="cd272-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cd272-114">blockedDeviceCount</span></span>|<span data-ttu-id="cd272-115">Int32</span><span class="sxs-lookup"><span data-stu-id="cd272-115">Int32</span></span>|<span data-ttu-id="cd272-116">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="cd272-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="cd272-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cd272-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="cd272-118">Int32</span><span class="sxs-lookup"><span data-stu-id="cd272-118">Int32</span></span>|<span data-ttu-id="cd272-119">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="cd272-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="cd272-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cd272-120">unknownDeviceCount</span></span>|<span data-ttu-id="cd272-121">Int32</span><span class="sxs-lookup"><span data-stu-id="cd272-121">Int32</span></span>|<span data-ttu-id="cd272-122">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="cd272-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="cd272-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cd272-123">unavailableDeviceCount</span></span>|<span data-ttu-id="cd272-124">Int32</span><span class="sxs-lookup"><span data-stu-id="cd272-124">Int32</span></span>|<span data-ttu-id="cd272-125">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="cd272-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd272-126">关系</span><span class="sxs-lookup"><span data-stu-id="cd272-126">Relationships</span></span>
<span data-ttu-id="cd272-127">无</span><span class="sxs-lookup"><span data-stu-id="cd272-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd272-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd272-128">JSON Representation</span></span>
<span data-ttu-id="cd272-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd272-129">Here is a JSON representation of the resource.</span></span>
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




