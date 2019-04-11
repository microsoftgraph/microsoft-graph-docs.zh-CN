---
title: managedDeviceOverview 资源类型
description: 托管设备的摘要数据
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 07a6bda1e62088eabc3450cf2dcefc945f3ca898
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771199"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="f31d3-103">managedDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="f31d3-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="f31d3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f31d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f31d3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f31d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f31d3-106">托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="f31d3-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="f31d3-107">方法</span><span class="sxs-lookup"><span data-stu-id="f31d3-107">Methods</span></span>
|<span data-ttu-id="f31d3-108">方法</span><span class="sxs-lookup"><span data-stu-id="f31d3-108">Method</span></span>|<span data-ttu-id="f31d3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f31d3-109">Return Type</span></span>|<span data-ttu-id="f31d3-110">说明</span><span class="sxs-lookup"><span data-stu-id="f31d3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f31d3-111">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f31d3-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="f31d3-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f31d3-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="f31d3-113">读取 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f31d3-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="f31d3-114">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f31d3-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="f31d3-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f31d3-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="f31d3-116">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f31d3-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f31d3-117">属性</span><span class="sxs-lookup"><span data-stu-id="f31d3-117">Properties</span></span>
|<span data-ttu-id="f31d3-118">属性</span><span class="sxs-lookup"><span data-stu-id="f31d3-118">Property</span></span>|<span data-ttu-id="f31d3-119">类型</span><span class="sxs-lookup"><span data-stu-id="f31d3-119">Type</span></span>|<span data-ttu-id="f31d3-120">说明</span><span class="sxs-lookup"><span data-stu-id="f31d3-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f31d3-121">id</span><span class="sxs-lookup"><span data-stu-id="f31d3-121">id</span></span>|<span data-ttu-id="f31d3-122">String</span><span class="sxs-lookup"><span data-stu-id="f31d3-122">String</span></span>|<span data-ttu-id="f31d3-123">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="f31d3-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="f31d3-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f31d3-124">enrolledDeviceCount</span></span>|<span data-ttu-id="f31d3-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f31d3-125">Int32</span></span>|<span data-ttu-id="f31d3-126">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="f31d3-126">Total enrolled device count.</span></span> <span data-ttu-id="f31d3-127">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="f31d3-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="f31d3-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="f31d3-128">mdmEnrolledCount</span></span>|<span data-ttu-id="f31d3-129">Int32</span><span class="sxs-lookup"><span data-stu-id="f31d3-129">Int32</span></span>|<span data-ttu-id="f31d3-130">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="f31d3-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="f31d3-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f31d3-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="f31d3-132">Int32</span><span class="sxs-lookup"><span data-stu-id="f31d3-132">Int32</span></span>|<span data-ttu-id="f31d3-133">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="f31d3-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="f31d3-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="f31d3-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="f31d3-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="f31d3-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="f31d3-136">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="f31d3-136">Device operating system summary.</span></span>|
|<span data-ttu-id="f31d3-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f31d3-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="f31d3-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f31d3-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="f31d3-139">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="f31d3-139">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="f31d3-140">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="f31d3-140">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="f31d3-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="f31d3-141">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="f31d3-142">帐户中托管设备的模型和制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="f31d3-142">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="f31d3-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f31d3-143">lastModifiedDateTime</span></span>|<span data-ttu-id="f31d3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f31d3-144">DateTimeOffset</span></span>|<span data-ttu-id="f31d3-145">设备的上次修改日期时间概述</span><span class="sxs-lookup"><span data-stu-id="f31d3-145">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="f31d3-146">关系</span><span class="sxs-lookup"><span data-stu-id="f31d3-146">Relationships</span></span>
<span data-ttu-id="f31d3-147">无</span><span class="sxs-lookup"><span data-stu-id="f31d3-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f31d3-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f31d3-148">JSON Representation</span></span>
<span data-ttu-id="f31d3-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f31d3-149">Here is a JSON representation of the resource.</span></span>
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
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "String"
    ],
    "deviceManufacturers": [
      "String"
    ]
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```





