---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 389bba96adc477e90244f6f9800da09ff3e87992
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990535"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="04b00-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="04b00-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="04b00-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="04b00-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04b00-105">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="04b00-105">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="04b00-106">属性</span><span class="sxs-lookup"><span data-stu-id="04b00-106">Properties</span></span>
|<span data-ttu-id="04b00-107">属性</span><span class="sxs-lookup"><span data-stu-id="04b00-107">Property</span></span>|<span data-ttu-id="04b00-108">类型</span><span class="sxs-lookup"><span data-stu-id="04b00-108">Type</span></span>|<span data-ttu-id="04b00-109">说明</span><span class="sxs-lookup"><span data-stu-id="04b00-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04b00-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="04b00-110">allowedDeviceCount</span></span>|<span data-ttu-id="04b00-111">Int32</span><span class="sxs-lookup"><span data-stu-id="04b00-111">Int32</span></span>|<span data-ttu-id="04b00-112">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="04b00-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="04b00-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="04b00-113">blockedDeviceCount</span></span>|<span data-ttu-id="04b00-114">Int32</span><span class="sxs-lookup"><span data-stu-id="04b00-114">Int32</span></span>|<span data-ttu-id="04b00-115">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="04b00-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="04b00-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="04b00-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="04b00-117">Int32</span><span class="sxs-lookup"><span data-stu-id="04b00-117">Int32</span></span>|<span data-ttu-id="04b00-118">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="04b00-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="04b00-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="04b00-119">unknownDeviceCount</span></span>|<span data-ttu-id="04b00-120">Int32</span><span class="sxs-lookup"><span data-stu-id="04b00-120">Int32</span></span>|<span data-ttu-id="04b00-121">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="04b00-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="04b00-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="04b00-122">unavailableDeviceCount</span></span>|<span data-ttu-id="04b00-123">Int32</span><span class="sxs-lookup"><span data-stu-id="04b00-123">Int32</span></span>|<span data-ttu-id="04b00-124">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="04b00-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04b00-125">关系</span><span class="sxs-lookup"><span data-stu-id="04b00-125">Relationships</span></span>
<span data-ttu-id="04b00-126">无</span><span class="sxs-lookup"><span data-stu-id="04b00-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="04b00-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04b00-127">JSON Representation</span></span>
<span data-ttu-id="04b00-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04b00-128">Here is a JSON representation of the resource.</span></span>
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



