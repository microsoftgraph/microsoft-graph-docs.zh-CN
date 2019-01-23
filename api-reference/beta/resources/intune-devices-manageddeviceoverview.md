---
title: managedDeviceOverview 资源类型
description: 托管设备的摘要数据
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: db5cebe36850971c871f673d07f18b8d5121cb1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422234"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="c8bb1-103">managedDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8bb1-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="c8bb1-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c8bb1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c8bb1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c8bb1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8bb1-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8bb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8bb1-107">托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="c8bb1-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="c8bb1-108">方法</span><span class="sxs-lookup"><span data-stu-id="c8bb1-108">Methods</span></span>
|<span data-ttu-id="c8bb1-109">方法</span><span class="sxs-lookup"><span data-stu-id="c8bb1-109">Method</span></span>|<span data-ttu-id="c8bb1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c8bb1-110">Return Type</span></span>|<span data-ttu-id="c8bb1-111">说明</span><span class="sxs-lookup"><span data-stu-id="c8bb1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c8bb1-112">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c8bb1-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="c8bb1-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c8bb1-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="c8bb1-114">读取 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c8bb1-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="c8bb1-115">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c8bb1-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="c8bb1-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c8bb1-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="c8bb1-117">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c8bb1-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8bb1-118">属性</span><span class="sxs-lookup"><span data-stu-id="c8bb1-118">Properties</span></span>
|<span data-ttu-id="c8bb1-119">属性</span><span class="sxs-lookup"><span data-stu-id="c8bb1-119">Property</span></span>|<span data-ttu-id="c8bb1-120">类型</span><span class="sxs-lookup"><span data-stu-id="c8bb1-120">Type</span></span>|<span data-ttu-id="c8bb1-121">说明</span><span class="sxs-lookup"><span data-stu-id="c8bb1-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8bb1-122">id</span><span class="sxs-lookup"><span data-stu-id="c8bb1-122">id</span></span>|<span data-ttu-id="c8bb1-123">String</span><span class="sxs-lookup"><span data-stu-id="c8bb1-123">String</span></span>|<span data-ttu-id="c8bb1-124">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="c8bb1-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="c8bb1-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c8bb1-125">enrolledDeviceCount</span></span>|<span data-ttu-id="c8bb1-126">Int32</span><span class="sxs-lookup"><span data-stu-id="c8bb1-126">Int32</span></span>|<span data-ttu-id="c8bb1-127">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="c8bb1-127">Total enrolled device count.</span></span> <span data-ttu-id="c8bb1-128">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="c8bb1-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="c8bb1-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="c8bb1-129">mdmEnrolledCount</span></span>|<span data-ttu-id="c8bb1-130">Int32</span><span class="sxs-lookup"><span data-stu-id="c8bb1-130">Int32</span></span>|<span data-ttu-id="c8bb1-131">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="c8bb1-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="c8bb1-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c8bb1-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="c8bb1-133">Int32</span><span class="sxs-lookup"><span data-stu-id="c8bb1-133">Int32</span></span>|<span data-ttu-id="c8bb1-134">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="c8bb1-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="c8bb1-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="c8bb1-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="c8bb1-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="c8bb1-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="c8bb1-137">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="c8bb1-137">Device operating system summary.</span></span>|
|<span data-ttu-id="c8bb1-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="c8bb1-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="c8bb1-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="c8bb1-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="c8bb1-140">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="c8bb1-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="c8bb1-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="c8bb1-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="c8bb1-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="c8bb1-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="c8bb1-143">模型和托管帐户中的设备的制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="c8bb1-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="c8bb1-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8bb1-144">lastModifiedDateTime</span></span>|<span data-ttu-id="c8bb1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8bb1-145">DateTimeOffset</span></span>|<span data-ttu-id="c8bb1-146">上次修改的日期时间的设备概述 （英文）</span><span class="sxs-lookup"><span data-stu-id="c8bb1-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8bb1-147">关系</span><span class="sxs-lookup"><span data-stu-id="c8bb1-147">Relationships</span></span>
<span data-ttu-id="c8bb1-148">无</span><span class="sxs-lookup"><span data-stu-id="c8bb1-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8bb1-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8bb1-149">JSON Representation</span></span>
<span data-ttu-id="c8bb1-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8bb1-150">Here is a JSON representation of the resource.</span></span>
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




