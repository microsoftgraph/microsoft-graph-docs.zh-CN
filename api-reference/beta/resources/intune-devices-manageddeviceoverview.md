---
title: managedDeviceOverview 资源类型
description: 托管设备的摘要数据
author: tfitzmac
ms.openlocfilehash: 223f11b49ee3cbc9b114047f25b301d9b0c08b24
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317533"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="b8b0b-103">managedDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8b0b-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="b8b0b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b8b0b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8b0b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b8b0b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8b0b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b8b0b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8b0b-107">托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="b8b0b-107">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="b8b0b-108">方法</span><span class="sxs-lookup"><span data-stu-id="b8b0b-108">Methods</span></span>
|<span data-ttu-id="b8b0b-109">方法</span><span class="sxs-lookup"><span data-stu-id="b8b0b-109">Method</span></span>|<span data-ttu-id="b8b0b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b8b0b-110">Return Type</span></span>|<span data-ttu-id="b8b0b-111">说明</span><span class="sxs-lookup"><span data-stu-id="b8b0b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b8b0b-112">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b8b0b-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="b8b0b-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b8b0b-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="b8b0b-114">读取 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8b0b-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="b8b0b-115">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b8b0b-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="b8b0b-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b8b0b-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="b8b0b-117">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b8b0b-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8b0b-118">属性</span><span class="sxs-lookup"><span data-stu-id="b8b0b-118">Properties</span></span>
|<span data-ttu-id="b8b0b-119">属性</span><span class="sxs-lookup"><span data-stu-id="b8b0b-119">Property</span></span>|<span data-ttu-id="b8b0b-120">类型</span><span class="sxs-lookup"><span data-stu-id="b8b0b-120">Type</span></span>|<span data-ttu-id="b8b0b-121">说明</span><span class="sxs-lookup"><span data-stu-id="b8b0b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8b0b-122">id</span><span class="sxs-lookup"><span data-stu-id="b8b0b-122">id</span></span>|<span data-ttu-id="b8b0b-123">String</span><span class="sxs-lookup"><span data-stu-id="b8b0b-123">String</span></span>|<span data-ttu-id="b8b0b-124">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b8b0b-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="b8b0b-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8b0b-125">enrolledDeviceCount</span></span>|<span data-ttu-id="b8b0b-126">Int32</span><span class="sxs-lookup"><span data-stu-id="b8b0b-126">Int32</span></span>|<span data-ttu-id="b8b0b-127">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="b8b0b-127">Total enrolled device count.</span></span> <span data-ttu-id="b8b0b-128">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="b8b0b-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="b8b0b-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="b8b0b-129">mdmEnrolledCount</span></span>|<span data-ttu-id="b8b0b-130">Int32</span><span class="sxs-lookup"><span data-stu-id="b8b0b-130">Int32</span></span>|<span data-ttu-id="b8b0b-131">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="b8b0b-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="b8b0b-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8b0b-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="b8b0b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="b8b0b-133">Int32</span></span>|<span data-ttu-id="b8b0b-134">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="b8b0b-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="b8b0b-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b8b0b-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="b8b0b-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b8b0b-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="b8b0b-137">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="b8b0b-137">Device operating system summary.</span></span>|
|<span data-ttu-id="b8b0b-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b8b0b-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="b8b0b-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b8b0b-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="b8b0b-140">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="b8b0b-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="b8b0b-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="b8b0b-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="b8b0b-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="b8b0b-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="b8b0b-143">模型和托管帐户中的设备的制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="b8b0b-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="b8b0b-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8b0b-144">lastModifiedDateTime</span></span>|<span data-ttu-id="b8b0b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8b0b-145">DateTimeOffset</span></span>|<span data-ttu-id="b8b0b-146">上次修改的日期时间的设备概述 （英文）</span><span class="sxs-lookup"><span data-stu-id="b8b0b-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8b0b-147">Relationships</span><span class="sxs-lookup"><span data-stu-id="b8b0b-147">Relationships</span></span>
<span data-ttu-id="b8b0b-148">无</span><span class="sxs-lookup"><span data-stu-id="b8b0b-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8b0b-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8b0b-149">JSON Representation</span></span>
<span data-ttu-id="b8b0b-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8b0b-150">Here is a JSON representation of the resource.</span></span>
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





