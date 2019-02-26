---
title: managedDeviceOverview 资源类型
description: 托管设备的摘要数据
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: accc6d976db80421cd06fd8071417bf07684a71a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250612"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="d3122-103">managedDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3122-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="d3122-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3122-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3122-105">托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="d3122-105">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="d3122-106">方法</span><span class="sxs-lookup"><span data-stu-id="d3122-106">Methods</span></span>
|<span data-ttu-id="d3122-107">方法</span><span class="sxs-lookup"><span data-stu-id="d3122-107">Method</span></span>|<span data-ttu-id="d3122-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d3122-108">Return Type</span></span>|<span data-ttu-id="d3122-109">说明</span><span class="sxs-lookup"><span data-stu-id="d3122-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d3122-110">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d3122-110">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="d3122-111">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d3122-111">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="d3122-112">读取 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d3122-112">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="d3122-113">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d3122-113">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="d3122-114">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d3122-114">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="d3122-115">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d3122-115">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d3122-116">属性</span><span class="sxs-lookup"><span data-stu-id="d3122-116">Properties</span></span>
|<span data-ttu-id="d3122-117">属性</span><span class="sxs-lookup"><span data-stu-id="d3122-117">Property</span></span>|<span data-ttu-id="d3122-118">类型</span><span class="sxs-lookup"><span data-stu-id="d3122-118">Type</span></span>|<span data-ttu-id="d3122-119">说明</span><span class="sxs-lookup"><span data-stu-id="d3122-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3122-120">id</span><span class="sxs-lookup"><span data-stu-id="d3122-120">id</span></span>|<span data-ttu-id="d3122-121">String</span><span class="sxs-lookup"><span data-stu-id="d3122-121">String</span></span>|<span data-ttu-id="d3122-122">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="d3122-122">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="d3122-123">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3122-123">enrolledDeviceCount</span></span>|<span data-ttu-id="d3122-124">Int32</span><span class="sxs-lookup"><span data-stu-id="d3122-124">Int32</span></span>|<span data-ttu-id="d3122-125">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="d3122-125">Total enrolled device count.</span></span> <span data-ttu-id="d3122-126">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="d3122-126">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="d3122-127">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="d3122-127">mdmEnrolledCount</span></span>|<span data-ttu-id="d3122-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d3122-128">Int32</span></span>|<span data-ttu-id="d3122-129">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="d3122-129">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="d3122-130">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3122-130">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="d3122-131">Int32</span><span class="sxs-lookup"><span data-stu-id="d3122-131">Int32</span></span>|<span data-ttu-id="d3122-132">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="d3122-132">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="d3122-133">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="d3122-133">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="d3122-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="d3122-134">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="d3122-135">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="d3122-135">Device operating system summary.</span></span>|
|<span data-ttu-id="d3122-136">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="d3122-136">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="d3122-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="d3122-137">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="d3122-138">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="d3122-138">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3122-139">关系</span><span class="sxs-lookup"><span data-stu-id="d3122-139">Relationships</span></span>
<span data-ttu-id="d3122-140">无</span><span class="sxs-lookup"><span data-stu-id="d3122-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3122-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3122-141">JSON Representation</span></span>
<span data-ttu-id="d3122-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3122-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 1024,
    "iosCount": 1024,
    "macOSCount": 1024,
    "windowsMobileCount": 1024,
    "windowsCount": 1024,
    "unknownCount": 1024
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 1024,
    "blockedDeviceCount": 1024,
    "quarantinedDeviceCount": 1024,
    "unknownDeviceCount": 1024,
    "unavailableDeviceCount": 1024
  }
}
```



