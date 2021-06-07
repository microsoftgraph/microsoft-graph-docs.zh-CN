---
title: managedDeviceOverview 资源类型
description: 托管设备的摘要数据
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dd87163c5e8aff363027ec74eeb060fc23c55fb4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751368"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="0967e-103">managedDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="0967e-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="0967e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0967e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0967e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0967e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0967e-106">托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="0967e-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="0967e-107">Methods</span><span class="sxs-lookup"><span data-stu-id="0967e-107">Methods</span></span>
|<span data-ttu-id="0967e-108">方法</span><span class="sxs-lookup"><span data-stu-id="0967e-108">Method</span></span>|<span data-ttu-id="0967e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0967e-109">Return Type</span></span>|<span data-ttu-id="0967e-110">Description</span><span class="sxs-lookup"><span data-stu-id="0967e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0967e-111">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0967e-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="0967e-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0967e-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="0967e-113">读取 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0967e-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="0967e-114">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0967e-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="0967e-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0967e-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="0967e-116">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0967e-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0967e-117">属性</span><span class="sxs-lookup"><span data-stu-id="0967e-117">Properties</span></span>
|<span data-ttu-id="0967e-118">属性</span><span class="sxs-lookup"><span data-stu-id="0967e-118">Property</span></span>|<span data-ttu-id="0967e-119">类型</span><span class="sxs-lookup"><span data-stu-id="0967e-119">Type</span></span>|<span data-ttu-id="0967e-120">说明</span><span class="sxs-lookup"><span data-stu-id="0967e-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0967e-121">id</span><span class="sxs-lookup"><span data-stu-id="0967e-121">id</span></span>|<span data-ttu-id="0967e-122">String</span><span class="sxs-lookup"><span data-stu-id="0967e-122">String</span></span>|<span data-ttu-id="0967e-123">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="0967e-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="0967e-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0967e-124">enrolledDeviceCount</span></span>|<span data-ttu-id="0967e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0967e-125">Int32</span></span>|<span data-ttu-id="0967e-126">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="0967e-126">Total enrolled device count.</span></span> <span data-ttu-id="0967e-127">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="0967e-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="0967e-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="0967e-128">mdmEnrolledCount</span></span>|<span data-ttu-id="0967e-129">Int32</span><span class="sxs-lookup"><span data-stu-id="0967e-129">Int32</span></span>|<span data-ttu-id="0967e-130">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="0967e-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="0967e-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0967e-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="0967e-132">Int32</span><span class="sxs-lookup"><span data-stu-id="0967e-132">Int32</span></span>|<span data-ttu-id="0967e-133">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="0967e-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="0967e-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="0967e-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="0967e-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="0967e-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="0967e-136">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="0967e-136">Device operating system summary.</span></span>|
|<span data-ttu-id="0967e-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="0967e-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="0967e-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="0967e-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="0967e-139">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="0967e-139">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="0967e-140">关系</span><span class="sxs-lookup"><span data-stu-id="0967e-140">Relationships</span></span>
<span data-ttu-id="0967e-141">无</span><span class="sxs-lookup"><span data-stu-id="0967e-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0967e-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0967e-142">JSON Representation</span></span>
<span data-ttu-id="0967e-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0967e-143">Here is a JSON representation of the resource.</span></span>
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




