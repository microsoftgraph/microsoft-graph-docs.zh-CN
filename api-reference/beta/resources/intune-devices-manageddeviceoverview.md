---
title: managedDeviceOverview 资源类型
description: 托管设备的摘要数据
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7bff057f872a8b315e0335f5d68633fce6d04e71
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783947"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="3bbb2-103">managedDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="3bbb2-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="3bbb2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3bbb2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bbb2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3bbb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bbb2-106">托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="3bbb2-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="3bbb2-107">方法</span><span class="sxs-lookup"><span data-stu-id="3bbb2-107">Methods</span></span>
|<span data-ttu-id="3bbb2-108">方法</span><span class="sxs-lookup"><span data-stu-id="3bbb2-108">Method</span></span>|<span data-ttu-id="3bbb2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3bbb2-109">Return Type</span></span>|<span data-ttu-id="3bbb2-110">说明</span><span class="sxs-lookup"><span data-stu-id="3bbb2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3bbb2-111">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3bbb2-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="3bbb2-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3bbb2-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="3bbb2-113">读取 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3bbb2-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="3bbb2-114">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3bbb2-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="3bbb2-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3bbb2-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="3bbb2-116">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3bbb2-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3bbb2-117">属性</span><span class="sxs-lookup"><span data-stu-id="3bbb2-117">Properties</span></span>
|<span data-ttu-id="3bbb2-118">属性</span><span class="sxs-lookup"><span data-stu-id="3bbb2-118">Property</span></span>|<span data-ttu-id="3bbb2-119">类型</span><span class="sxs-lookup"><span data-stu-id="3bbb2-119">Type</span></span>|<span data-ttu-id="3bbb2-120">说明</span><span class="sxs-lookup"><span data-stu-id="3bbb2-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bbb2-121">id</span><span class="sxs-lookup"><span data-stu-id="3bbb2-121">id</span></span>|<span data-ttu-id="3bbb2-122">String</span><span class="sxs-lookup"><span data-stu-id="3bbb2-122">String</span></span>|<span data-ttu-id="3bbb2-123">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="3bbb2-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="3bbb2-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3bbb2-124">enrolledDeviceCount</span></span>|<span data-ttu-id="3bbb2-125">Int32</span><span class="sxs-lookup"><span data-stu-id="3bbb2-125">Int32</span></span>|<span data-ttu-id="3bbb2-126">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="3bbb2-126">Total enrolled device count.</span></span> <span data-ttu-id="3bbb2-127">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="3bbb2-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="3bbb2-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="3bbb2-128">mdmEnrolledCount</span></span>|<span data-ttu-id="3bbb2-129">Int32</span><span class="sxs-lookup"><span data-stu-id="3bbb2-129">Int32</span></span>|<span data-ttu-id="3bbb2-130">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="3bbb2-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="3bbb2-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3bbb2-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="3bbb2-132">Int32</span><span class="sxs-lookup"><span data-stu-id="3bbb2-132">Int32</span></span>|<span data-ttu-id="3bbb2-133">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="3bbb2-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="3bbb2-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="3bbb2-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="3bbb2-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="3bbb2-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="3bbb2-136">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="3bbb2-136">Device operating system summary.</span></span>|
|<span data-ttu-id="3bbb2-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="3bbb2-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="3bbb2-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="3bbb2-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="3bbb2-139">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="3bbb2-139">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="3bbb2-140">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="3bbb2-140">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="3bbb2-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="3bbb2-141">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="3bbb2-142">帐户中托管设备的模型和制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="3bbb2-142">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="3bbb2-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bbb2-143">lastModifiedDateTime</span></span>|<span data-ttu-id="3bbb2-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bbb2-144">DateTimeOffset</span></span>|<span data-ttu-id="3bbb2-145">设备的上次修改日期时间概述</span><span class="sxs-lookup"><span data-stu-id="3bbb2-145">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="3bbb2-146">关系</span><span class="sxs-lookup"><span data-stu-id="3bbb2-146">Relationships</span></span>
<span data-ttu-id="3bbb2-147">无</span><span class="sxs-lookup"><span data-stu-id="3bbb2-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bbb2-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3bbb2-148">JSON Representation</span></span>
<span data-ttu-id="3bbb2-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3bbb2-149">Here is a JSON representation of the resource.</span></span>
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
    "unknownCount": 1024,
    "androidDedicatedCount": 1024,
    "androidDeviceAdminCount": 1024,
    "androidFullyManagedCount": 1024,
    "androidWorkProfileCount": 1024,
    "configMgrDeviceCount": 1024
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



