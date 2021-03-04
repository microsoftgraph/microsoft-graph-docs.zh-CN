---
title: managedDeviceOverview 资源类型
description: 托管设备的摘要数据
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e519f3fd5653e1e3512da8ee58d369df03cc69c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444187"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="b50b7-103">managedDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="b50b7-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="b50b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b50b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b50b7-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b50b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b50b7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b50b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b50b7-107">托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="b50b7-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="b50b7-108">Methods</span><span class="sxs-lookup"><span data-stu-id="b50b7-108">Methods</span></span>
|<span data-ttu-id="b50b7-109">方法</span><span class="sxs-lookup"><span data-stu-id="b50b7-109">Method</span></span>|<span data-ttu-id="b50b7-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b50b7-110">Return Type</span></span>|<span data-ttu-id="b50b7-111">说明</span><span class="sxs-lookup"><span data-stu-id="b50b7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b50b7-112">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b50b7-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="b50b7-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b50b7-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="b50b7-114">读取 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b50b7-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="b50b7-115">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b50b7-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="b50b7-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b50b7-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="b50b7-117">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b50b7-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b50b7-118">属性</span><span class="sxs-lookup"><span data-stu-id="b50b7-118">Properties</span></span>
|<span data-ttu-id="b50b7-119">属性</span><span class="sxs-lookup"><span data-stu-id="b50b7-119">Property</span></span>|<span data-ttu-id="b50b7-120">类型</span><span class="sxs-lookup"><span data-stu-id="b50b7-120">Type</span></span>|<span data-ttu-id="b50b7-121">说明</span><span class="sxs-lookup"><span data-stu-id="b50b7-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b50b7-122">id</span><span class="sxs-lookup"><span data-stu-id="b50b7-122">id</span></span>|<span data-ttu-id="b50b7-123">String</span><span class="sxs-lookup"><span data-stu-id="b50b7-123">String</span></span>|<span data-ttu-id="b50b7-124">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b50b7-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="b50b7-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b50b7-125">enrolledDeviceCount</span></span>|<span data-ttu-id="b50b7-126">Int32</span><span class="sxs-lookup"><span data-stu-id="b50b7-126">Int32</span></span>|<span data-ttu-id="b50b7-127">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="b50b7-127">Total enrolled device count.</span></span> <span data-ttu-id="b50b7-128">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="b50b7-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="b50b7-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="b50b7-129">mdmEnrolledCount</span></span>|<span data-ttu-id="b50b7-130">Int32</span><span class="sxs-lookup"><span data-stu-id="b50b7-130">Int32</span></span>|<span data-ttu-id="b50b7-131">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="b50b7-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="b50b7-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b50b7-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="b50b7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="b50b7-133">Int32</span></span>|<span data-ttu-id="b50b7-134">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="b50b7-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="b50b7-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b50b7-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="b50b7-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b50b7-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="b50b7-137">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="b50b7-137">Device operating system summary.</span></span>|
|<span data-ttu-id="b50b7-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b50b7-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="b50b7-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b50b7-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="b50b7-140">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="b50b7-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="b50b7-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="b50b7-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="b50b7-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="b50b7-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="b50b7-143">帐户中托管设备的型号和制造商</span><span class="sxs-lookup"><span data-stu-id="b50b7-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="b50b7-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b50b7-144">lastModifiedDateTime</span></span>|<span data-ttu-id="b50b7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b50b7-145">DateTimeOffset</span></span>|<span data-ttu-id="b50b7-146">设备概述的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="b50b7-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="b50b7-147">关系</span><span class="sxs-lookup"><span data-stu-id="b50b7-147">Relationships</span></span>
<span data-ttu-id="b50b7-148">无</span><span class="sxs-lookup"><span data-stu-id="b50b7-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b50b7-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b50b7-149">JSON Representation</span></span>
<span data-ttu-id="b50b7-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b50b7-150">Here is a JSON representation of the resource.</span></span>
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
    "aospUserAssociatedCount": 1024,
    "linuxCount": 1024
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




