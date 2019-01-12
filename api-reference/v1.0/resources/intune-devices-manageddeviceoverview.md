---
title: managedDeviceOverview 资源类型
description: 托管设备的摘要数据
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7a5abdd3b5455272de7d1cf73044a1356d728dd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981194"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="20517-103">managedDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="20517-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="20517-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="20517-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20517-105">托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="20517-105">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="20517-106">方法</span><span class="sxs-lookup"><span data-stu-id="20517-106">Methods</span></span>
|<span data-ttu-id="20517-107">方法</span><span class="sxs-lookup"><span data-stu-id="20517-107">Method</span></span>|<span data-ttu-id="20517-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="20517-108">Return Type</span></span>|<span data-ttu-id="20517-109">说明</span><span class="sxs-lookup"><span data-stu-id="20517-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="20517-110">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="20517-110">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="20517-111">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="20517-111">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="20517-112">读取 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="20517-112">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="20517-113">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="20517-113">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="20517-114">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="20517-114">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="20517-115">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="20517-115">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="20517-116">属性</span><span class="sxs-lookup"><span data-stu-id="20517-116">Properties</span></span>
|<span data-ttu-id="20517-117">属性</span><span class="sxs-lookup"><span data-stu-id="20517-117">Property</span></span>|<span data-ttu-id="20517-118">类型</span><span class="sxs-lookup"><span data-stu-id="20517-118">Type</span></span>|<span data-ttu-id="20517-119">说明</span><span class="sxs-lookup"><span data-stu-id="20517-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20517-120">id</span><span class="sxs-lookup"><span data-stu-id="20517-120">id</span></span>|<span data-ttu-id="20517-121">String</span><span class="sxs-lookup"><span data-stu-id="20517-121">String</span></span>|<span data-ttu-id="20517-122">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="20517-122">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="20517-123">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="20517-123">enrolledDeviceCount</span></span>|<span data-ttu-id="20517-124">Int32</span><span class="sxs-lookup"><span data-stu-id="20517-124">Int32</span></span>|<span data-ttu-id="20517-125">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="20517-125">Total enrolled device count.</span></span> <span data-ttu-id="20517-126">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="20517-126">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="20517-127">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="20517-127">mdmEnrolledCount</span></span>|<span data-ttu-id="20517-128">Int32</span><span class="sxs-lookup"><span data-stu-id="20517-128">Int32</span></span>|<span data-ttu-id="20517-129">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="20517-129">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="20517-130">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="20517-130">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="20517-131">Int32</span><span class="sxs-lookup"><span data-stu-id="20517-131">Int32</span></span>|<span data-ttu-id="20517-132">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="20517-132">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="20517-133">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="20517-133">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="20517-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="20517-134">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="20517-135">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="20517-135">Device operating system summary.</span></span>|
|<span data-ttu-id="20517-136">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="20517-136">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="20517-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="20517-137">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="20517-138">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="20517-138">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="20517-139">关系</span><span class="sxs-lookup"><span data-stu-id="20517-139">Relationships</span></span>
<span data-ttu-id="20517-140">无</span><span class="sxs-lookup"><span data-stu-id="20517-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="20517-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20517-141">JSON Representation</span></span>
<span data-ttu-id="20517-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20517-142">Here is a JSON representation of the resource.</span></span>
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



