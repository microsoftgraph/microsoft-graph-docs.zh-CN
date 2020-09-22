---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8466628f74aa3098227c0b7714b86021c7eb6f93
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060487"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="a05b8-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="a05b8-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="a05b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a05b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a05b8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a05b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a05b8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a05b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a05b8-107">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="a05b8-107">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="a05b8-108">属性</span><span class="sxs-lookup"><span data-stu-id="a05b8-108">Properties</span></span>
|<span data-ttu-id="a05b8-109">属性</span><span class="sxs-lookup"><span data-stu-id="a05b8-109">Property</span></span>|<span data-ttu-id="a05b8-110">类型</span><span class="sxs-lookup"><span data-stu-id="a05b8-110">Type</span></span>|<span data-ttu-id="a05b8-111">说明</span><span class="sxs-lookup"><span data-stu-id="a05b8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a05b8-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a05b8-112">allowedDeviceCount</span></span>|<span data-ttu-id="a05b8-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a05b8-113">Int32</span></span>|<span data-ttu-id="a05b8-114">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a05b8-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="a05b8-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a05b8-115">blockedDeviceCount</span></span>|<span data-ttu-id="a05b8-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a05b8-116">Int32</span></span>|<span data-ttu-id="a05b8-117">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a05b8-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="a05b8-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a05b8-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="a05b8-119">Int32</span><span class="sxs-lookup"><span data-stu-id="a05b8-119">Int32</span></span>|<span data-ttu-id="a05b8-120">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a05b8-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="a05b8-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a05b8-121">unknownDeviceCount</span></span>|<span data-ttu-id="a05b8-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a05b8-122">Int32</span></span>|<span data-ttu-id="a05b8-123">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a05b8-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="a05b8-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a05b8-124">unavailableDeviceCount</span></span>|<span data-ttu-id="a05b8-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a05b8-125">Int32</span></span>|<span data-ttu-id="a05b8-126">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="a05b8-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a05b8-127">关系</span><span class="sxs-lookup"><span data-stu-id="a05b8-127">Relationships</span></span>
<span data-ttu-id="a05b8-128">无</span><span class="sxs-lookup"><span data-stu-id="a05b8-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a05b8-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a05b8-129">JSON Representation</span></span>
<span data-ttu-id="a05b8-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a05b8-130">Here is a JSON representation of the resource.</span></span>
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






