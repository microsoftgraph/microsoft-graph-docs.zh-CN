---
title: managedDeviceOverview 资源类型
description: 托管设备的摘要数据
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 091871ed88903f4fcb3a3ad8be86e7b997f173b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932510"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="aab91-103">managedDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="aab91-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="aab91-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aab91-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aab91-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aab91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aab91-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aab91-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aab91-107">托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="aab91-107">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="aab91-108">方法</span><span class="sxs-lookup"><span data-stu-id="aab91-108">Methods</span></span>
|<span data-ttu-id="aab91-109">方法</span><span class="sxs-lookup"><span data-stu-id="aab91-109">Method</span></span>|<span data-ttu-id="aab91-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="aab91-110">Return Type</span></span>|<span data-ttu-id="aab91-111">说明</span><span class="sxs-lookup"><span data-stu-id="aab91-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aab91-112">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="aab91-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="aab91-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="aab91-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="aab91-114">读取 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aab91-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="aab91-115">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="aab91-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="aab91-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="aab91-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="aab91-117">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aab91-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aab91-118">属性</span><span class="sxs-lookup"><span data-stu-id="aab91-118">Properties</span></span>
|<span data-ttu-id="aab91-119">属性</span><span class="sxs-lookup"><span data-stu-id="aab91-119">Property</span></span>|<span data-ttu-id="aab91-120">类型</span><span class="sxs-lookup"><span data-stu-id="aab91-120">Type</span></span>|<span data-ttu-id="aab91-121">说明</span><span class="sxs-lookup"><span data-stu-id="aab91-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aab91-122">id</span><span class="sxs-lookup"><span data-stu-id="aab91-122">id</span></span>|<span data-ttu-id="aab91-123">String</span><span class="sxs-lookup"><span data-stu-id="aab91-123">String</span></span>|<span data-ttu-id="aab91-124">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="aab91-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="aab91-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aab91-125">enrolledDeviceCount</span></span>|<span data-ttu-id="aab91-126">Int32</span><span class="sxs-lookup"><span data-stu-id="aab91-126">Int32</span></span>|<span data-ttu-id="aab91-127">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="aab91-127">Total enrolled device count.</span></span> <span data-ttu-id="aab91-128">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="aab91-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="aab91-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="aab91-129">mdmEnrolledCount</span></span>|<span data-ttu-id="aab91-130">Int32</span><span class="sxs-lookup"><span data-stu-id="aab91-130">Int32</span></span>|<span data-ttu-id="aab91-131">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="aab91-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="aab91-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aab91-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="aab91-133">Int32</span><span class="sxs-lookup"><span data-stu-id="aab91-133">Int32</span></span>|<span data-ttu-id="aab91-134">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="aab91-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="aab91-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="aab91-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="aab91-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="aab91-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="aab91-137">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="aab91-137">Device operating system summary.</span></span>|
|<span data-ttu-id="aab91-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="aab91-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="aab91-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="aab91-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="aab91-140">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="aab91-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="aab91-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="aab91-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="aab91-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="aab91-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="aab91-143">模型和托管帐户中的设备的制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="aab91-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="aab91-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aab91-144">lastModifiedDateTime</span></span>|<span data-ttu-id="aab91-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aab91-145">DateTimeOffset</span></span>|<span data-ttu-id="aab91-146">上次修改的日期时间的设备概述 （英文）</span><span class="sxs-lookup"><span data-stu-id="aab91-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="aab91-147">Relationships</span><span class="sxs-lookup"><span data-stu-id="aab91-147">Relationships</span></span>
<span data-ttu-id="aab91-148">无</span><span class="sxs-lookup"><span data-stu-id="aab91-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aab91-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aab91-149">JSON Representation</span></span>
<span data-ttu-id="aab91-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aab91-150">Here is a JSON representation of the resource.</span></span>
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





