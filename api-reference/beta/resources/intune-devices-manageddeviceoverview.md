---
title: managedDeviceOverview 资源类型
description: 托管设备的摘要数据
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e2a0345b19c2c2954b0bce231ca05d1bc2d2adcb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158490"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="e494e-103">managedDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="e494e-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="e494e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e494e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e494e-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e494e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e494e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e494e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e494e-107">托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="e494e-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="e494e-108">方法</span><span class="sxs-lookup"><span data-stu-id="e494e-108">Methods</span></span>
|<span data-ttu-id="e494e-109">方法</span><span class="sxs-lookup"><span data-stu-id="e494e-109">Method</span></span>|<span data-ttu-id="e494e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e494e-110">Return Type</span></span>|<span data-ttu-id="e494e-111">说明</span><span class="sxs-lookup"><span data-stu-id="e494e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e494e-112">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e494e-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="e494e-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e494e-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="e494e-114">读取 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e494e-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="e494e-115">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e494e-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="e494e-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e494e-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="e494e-117">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e494e-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e494e-118">属性</span><span class="sxs-lookup"><span data-stu-id="e494e-118">Properties</span></span>
|<span data-ttu-id="e494e-119">属性</span><span class="sxs-lookup"><span data-stu-id="e494e-119">Property</span></span>|<span data-ttu-id="e494e-120">类型</span><span class="sxs-lookup"><span data-stu-id="e494e-120">Type</span></span>|<span data-ttu-id="e494e-121">说明</span><span class="sxs-lookup"><span data-stu-id="e494e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e494e-122">id</span><span class="sxs-lookup"><span data-stu-id="e494e-122">id</span></span>|<span data-ttu-id="e494e-123">String</span><span class="sxs-lookup"><span data-stu-id="e494e-123">String</span></span>|<span data-ttu-id="e494e-124">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="e494e-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="e494e-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e494e-125">enrolledDeviceCount</span></span>|<span data-ttu-id="e494e-126">Int32</span><span class="sxs-lookup"><span data-stu-id="e494e-126">Int32</span></span>|<span data-ttu-id="e494e-127">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="e494e-127">Total enrolled device count.</span></span> <span data-ttu-id="e494e-128">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="e494e-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="e494e-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="e494e-129">mdmEnrolledCount</span></span>|<span data-ttu-id="e494e-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e494e-130">Int32</span></span>|<span data-ttu-id="e494e-131">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="e494e-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="e494e-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e494e-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="e494e-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e494e-133">Int32</span></span>|<span data-ttu-id="e494e-134">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="e494e-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="e494e-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="e494e-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="e494e-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="e494e-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="e494e-137">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="e494e-137">Device operating system summary.</span></span>|
|<span data-ttu-id="e494e-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="e494e-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="e494e-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="e494e-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="e494e-140">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="e494e-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="e494e-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="e494e-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="e494e-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="e494e-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="e494e-143">帐户中托管设备的型号和制造产品</span><span class="sxs-lookup"><span data-stu-id="e494e-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="e494e-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e494e-144">lastModifiedDateTime</span></span>|<span data-ttu-id="e494e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e494e-145">DateTimeOffset</span></span>|<span data-ttu-id="e494e-146">设备概述的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="e494e-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="e494e-147">关系</span><span class="sxs-lookup"><span data-stu-id="e494e-147">Relationships</span></span>
<span data-ttu-id="e494e-148">无</span><span class="sxs-lookup"><span data-stu-id="e494e-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e494e-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e494e-149">JSON Representation</span></span>
<span data-ttu-id="e494e-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e494e-150">Here is a JSON representation of the resource.</span></span>
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
    "androidCorporateWorkProfileCount": 1024,
    "configMgrDeviceCount": 1024,
    "aospUserlessCount": 1024,
    "aospUserAssociatedCount": 1024
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




