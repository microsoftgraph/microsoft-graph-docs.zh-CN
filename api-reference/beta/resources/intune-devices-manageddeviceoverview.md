---
title: managedDeviceOverview 资源类型
description: 托管设备的摘要数据
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e6c7187bc5cb984e4ca7e607068e6010f747f868
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175001"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="1343d-103">managedDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="1343d-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="1343d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1343d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1343d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1343d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1343d-106">托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="1343d-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="1343d-107">方法</span><span class="sxs-lookup"><span data-stu-id="1343d-107">Methods</span></span>
|<span data-ttu-id="1343d-108">方法</span><span class="sxs-lookup"><span data-stu-id="1343d-108">Method</span></span>|<span data-ttu-id="1343d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1343d-109">Return Type</span></span>|<span data-ttu-id="1343d-110">说明</span><span class="sxs-lookup"><span data-stu-id="1343d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1343d-111">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1343d-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="1343d-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1343d-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="1343d-113">读取 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1343d-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="1343d-114">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1343d-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="1343d-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1343d-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="1343d-116">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1343d-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1343d-117">属性</span><span class="sxs-lookup"><span data-stu-id="1343d-117">Properties</span></span>
|<span data-ttu-id="1343d-118">属性</span><span class="sxs-lookup"><span data-stu-id="1343d-118">Property</span></span>|<span data-ttu-id="1343d-119">类型</span><span class="sxs-lookup"><span data-stu-id="1343d-119">Type</span></span>|<span data-ttu-id="1343d-120">说明</span><span class="sxs-lookup"><span data-stu-id="1343d-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1343d-121">id</span><span class="sxs-lookup"><span data-stu-id="1343d-121">id</span></span>|<span data-ttu-id="1343d-122">String</span><span class="sxs-lookup"><span data-stu-id="1343d-122">String</span></span>|<span data-ttu-id="1343d-123">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="1343d-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="1343d-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1343d-124">enrolledDeviceCount</span></span>|<span data-ttu-id="1343d-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1343d-125">Int32</span></span>|<span data-ttu-id="1343d-126">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="1343d-126">Total enrolled device count.</span></span> <span data-ttu-id="1343d-127">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="1343d-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="1343d-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="1343d-128">mdmEnrolledCount</span></span>|<span data-ttu-id="1343d-129">Int32</span><span class="sxs-lookup"><span data-stu-id="1343d-129">Int32</span></span>|<span data-ttu-id="1343d-130">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="1343d-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="1343d-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1343d-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="1343d-132">Int32</span><span class="sxs-lookup"><span data-stu-id="1343d-132">Int32</span></span>|<span data-ttu-id="1343d-133">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="1343d-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="1343d-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="1343d-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="1343d-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="1343d-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="1343d-136">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="1343d-136">Device operating system summary.</span></span>|
|<span data-ttu-id="1343d-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="1343d-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="1343d-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="1343d-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="1343d-139">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="1343d-139">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="1343d-140">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="1343d-140">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="1343d-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="1343d-141">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="1343d-142">帐户中托管设备的模型和制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="1343d-142">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="1343d-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1343d-143">lastModifiedDateTime</span></span>|<span data-ttu-id="1343d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1343d-144">DateTimeOffset</span></span>|<span data-ttu-id="1343d-145">设备的上次修改日期时间概述</span><span class="sxs-lookup"><span data-stu-id="1343d-145">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="1343d-146">关系</span><span class="sxs-lookup"><span data-stu-id="1343d-146">Relationships</span></span>
<span data-ttu-id="1343d-147">无</span><span class="sxs-lookup"><span data-stu-id="1343d-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1343d-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1343d-148">JSON Representation</span></span>
<span data-ttu-id="1343d-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1343d-149">Here is a JSON representation of the resource.</span></span>
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




