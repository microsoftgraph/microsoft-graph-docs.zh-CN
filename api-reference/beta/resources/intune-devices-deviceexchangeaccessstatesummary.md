---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b8ca08b026b8e1cdbac4bd0dc73331a9d5df80fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889983"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="805a6-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="805a6-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="805a6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="805a6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="805a6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="805a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="805a6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="805a6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="805a6-107">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="805a6-107">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="805a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="805a6-108">Properties</span></span>
|<span data-ttu-id="805a6-109">属性</span><span class="sxs-lookup"><span data-stu-id="805a6-109">Property</span></span>|<span data-ttu-id="805a6-110">类型</span><span class="sxs-lookup"><span data-stu-id="805a6-110">Type</span></span>|<span data-ttu-id="805a6-111">说明</span><span class="sxs-lookup"><span data-stu-id="805a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="805a6-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="805a6-112">allowedDeviceCount</span></span>|<span data-ttu-id="805a6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="805a6-113">Int32</span></span>|<span data-ttu-id="805a6-114">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="805a6-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="805a6-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="805a6-115">blockedDeviceCount</span></span>|<span data-ttu-id="805a6-116">Int32</span><span class="sxs-lookup"><span data-stu-id="805a6-116">Int32</span></span>|<span data-ttu-id="805a6-117">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="805a6-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="805a6-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="805a6-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="805a6-119">Int32</span><span class="sxs-lookup"><span data-stu-id="805a6-119">Int32</span></span>|<span data-ttu-id="805a6-120">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="805a6-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="805a6-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="805a6-121">unknownDeviceCount</span></span>|<span data-ttu-id="805a6-122">Int32</span><span class="sxs-lookup"><span data-stu-id="805a6-122">Int32</span></span>|<span data-ttu-id="805a6-123">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="805a6-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="805a6-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="805a6-124">unavailableDeviceCount</span></span>|<span data-ttu-id="805a6-125">Int32</span><span class="sxs-lookup"><span data-stu-id="805a6-125">Int32</span></span>|<span data-ttu-id="805a6-126">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="805a6-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="805a6-127">关系</span><span class="sxs-lookup"><span data-stu-id="805a6-127">Relationships</span></span>
<span data-ttu-id="805a6-128">无</span><span class="sxs-lookup"><span data-stu-id="805a6-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="805a6-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="805a6-129">JSON Representation</span></span>
<span data-ttu-id="805a6-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="805a6-130">Here is a JSON representation of the resource.</span></span>
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





