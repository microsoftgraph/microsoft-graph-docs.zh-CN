---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: tfitzmac
ms.openlocfilehash: dd2784078e8b44b1a02cb5a0013c1e38804912c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301741"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="af8e9-103">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="af8e9-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="af8e9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="af8e9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af8e9-105">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="af8e9-105">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="af8e9-106">属性</span><span class="sxs-lookup"><span data-stu-id="af8e9-106">Properties</span></span>
|<span data-ttu-id="af8e9-107">属性</span><span class="sxs-lookup"><span data-stu-id="af8e9-107">Property</span></span>|<span data-ttu-id="af8e9-108">类型</span><span class="sxs-lookup"><span data-stu-id="af8e9-108">Type</span></span>|<span data-ttu-id="af8e9-109">说明</span><span class="sxs-lookup"><span data-stu-id="af8e9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af8e9-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="af8e9-110">allowedDeviceCount</span></span>|<span data-ttu-id="af8e9-111">Int32</span><span class="sxs-lookup"><span data-stu-id="af8e9-111">Int32</span></span>|<span data-ttu-id="af8e9-112">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="af8e9-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="af8e9-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="af8e9-113">blockedDeviceCount</span></span>|<span data-ttu-id="af8e9-114">Int32</span><span class="sxs-lookup"><span data-stu-id="af8e9-114">Int32</span></span>|<span data-ttu-id="af8e9-115">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="af8e9-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="af8e9-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="af8e9-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="af8e9-117">Int32</span><span class="sxs-lookup"><span data-stu-id="af8e9-117">Int32</span></span>|<span data-ttu-id="af8e9-118">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="af8e9-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="af8e9-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="af8e9-119">unknownDeviceCount</span></span>|<span data-ttu-id="af8e9-120">Int32</span><span class="sxs-lookup"><span data-stu-id="af8e9-120">Int32</span></span>|<span data-ttu-id="af8e9-121">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="af8e9-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="af8e9-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="af8e9-122">unavailableDeviceCount</span></span>|<span data-ttu-id="af8e9-123">Int32</span><span class="sxs-lookup"><span data-stu-id="af8e9-123">Int32</span></span>|<span data-ttu-id="af8e9-124">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="af8e9-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af8e9-125">关系</span><span class="sxs-lookup"><span data-stu-id="af8e9-125">Relationships</span></span>
<span data-ttu-id="af8e9-126">无</span><span class="sxs-lookup"><span data-stu-id="af8e9-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="af8e9-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af8e9-127">JSON Representation</span></span>
<span data-ttu-id="af8e9-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af8e9-128">Here is a JSON representation of the resource.</span></span>
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



