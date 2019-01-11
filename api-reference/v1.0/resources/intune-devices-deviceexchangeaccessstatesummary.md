---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 10eb3738e14e8239f92f8578d01b9d4888b06b24
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829818"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="7a083-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a083-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="7a083-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7a083-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a083-105">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="7a083-105">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="7a083-106">属性</span><span class="sxs-lookup"><span data-stu-id="7a083-106">Properties</span></span>
|<span data-ttu-id="7a083-107">属性</span><span class="sxs-lookup"><span data-stu-id="7a083-107">Property</span></span>|<span data-ttu-id="7a083-108">类型</span><span class="sxs-lookup"><span data-stu-id="7a083-108">Type</span></span>|<span data-ttu-id="7a083-109">说明</span><span class="sxs-lookup"><span data-stu-id="7a083-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a083-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a083-110">allowedDeviceCount</span></span>|<span data-ttu-id="7a083-111">Int32</span><span class="sxs-lookup"><span data-stu-id="7a083-111">Int32</span></span>|<span data-ttu-id="7a083-112">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="7a083-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="7a083-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a083-113">blockedDeviceCount</span></span>|<span data-ttu-id="7a083-114">Int32</span><span class="sxs-lookup"><span data-stu-id="7a083-114">Int32</span></span>|<span data-ttu-id="7a083-115">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="7a083-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="7a083-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a083-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="7a083-117">Int32</span><span class="sxs-lookup"><span data-stu-id="7a083-117">Int32</span></span>|<span data-ttu-id="7a083-118">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="7a083-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="7a083-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a083-119">unknownDeviceCount</span></span>|<span data-ttu-id="7a083-120">Int32</span><span class="sxs-lookup"><span data-stu-id="7a083-120">Int32</span></span>|<span data-ttu-id="7a083-121">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="7a083-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="7a083-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a083-122">unavailableDeviceCount</span></span>|<span data-ttu-id="7a083-123">Int32</span><span class="sxs-lookup"><span data-stu-id="7a083-123">Int32</span></span>|<span data-ttu-id="7a083-124">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="7a083-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a083-125">关系</span><span class="sxs-lookup"><span data-stu-id="7a083-125">Relationships</span></span>
<span data-ttu-id="7a083-126">无</span><span class="sxs-lookup"><span data-stu-id="7a083-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7a083-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a083-127">JSON Representation</span></span>
<span data-ttu-id="7a083-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a083-128">Here is a JSON representation of the resource.</span></span>
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



