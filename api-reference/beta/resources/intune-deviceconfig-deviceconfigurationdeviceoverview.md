---
title: deviceConfigurationDeviceOverview 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e6ded68974f3a4baa307d186e93ea83931f07aa
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773222"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="fa7ec-103">deviceConfigurationDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa7ec-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="fa7ec-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fa7ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa7ec-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fa7ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa7ec-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fa7ec-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="fa7ec-107">方法</span><span class="sxs-lookup"><span data-stu-id="fa7ec-107">Methods</span></span>
|<span data-ttu-id="fa7ec-108">方法</span><span class="sxs-lookup"><span data-stu-id="fa7ec-108">Method</span></span>|<span data-ttu-id="fa7ec-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="fa7ec-109">Return Type</span></span>|<span data-ttu-id="fa7ec-110">说明</span><span class="sxs-lookup"><span data-stu-id="fa7ec-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fa7ec-111">获取 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fa7ec-111">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="fa7ec-112">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fa7ec-112">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="fa7ec-113">读取 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fa7ec-113">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="fa7ec-114">更新 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fa7ec-114">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="fa7ec-115">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fa7ec-115">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="fa7ec-116">更新 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fa7ec-116">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fa7ec-117">属性</span><span class="sxs-lookup"><span data-stu-id="fa7ec-117">Properties</span></span>
|<span data-ttu-id="fa7ec-118">属性</span><span class="sxs-lookup"><span data-stu-id="fa7ec-118">Property</span></span>|<span data-ttu-id="fa7ec-119">类型</span><span class="sxs-lookup"><span data-stu-id="fa7ec-119">Type</span></span>|<span data-ttu-id="fa7ec-120">说明</span><span class="sxs-lookup"><span data-stu-id="fa7ec-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa7ec-121">id</span><span class="sxs-lookup"><span data-stu-id="fa7ec-121">id</span></span>|<span data-ttu-id="fa7ec-122">String</span><span class="sxs-lookup"><span data-stu-id="fa7ec-122">String</span></span>|<span data-ttu-id="fa7ec-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fa7ec-123">Key of the entity.</span></span>|
|<span data-ttu-id="fa7ec-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="fa7ec-124">pendingCount</span></span>|<span data-ttu-id="fa7ec-125">Int32</span><span class="sxs-lookup"><span data-stu-id="fa7ec-125">Int32</span></span>|<span data-ttu-id="fa7ec-126">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="fa7ec-126">Number of pending devices</span></span>|
|<span data-ttu-id="fa7ec-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="fa7ec-127">notApplicableCount</span></span>|<span data-ttu-id="fa7ec-128">Int32</span><span class="sxs-lookup"><span data-stu-id="fa7ec-128">Int32</span></span>|<span data-ttu-id="fa7ec-129">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="fa7ec-129">Number of not applicable devices</span></span>|
|<span data-ttu-id="fa7ec-130">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="fa7ec-130">notApplicablePlatformCount</span></span>|<span data-ttu-id="fa7ec-131">Int32</span><span class="sxs-lookup"><span data-stu-id="fa7ec-131">Int32</span></span>|<span data-ttu-id="fa7ec-132">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="fa7ec-132">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="fa7ec-133">successCount</span><span class="sxs-lookup"><span data-stu-id="fa7ec-133">successCount</span></span>|<span data-ttu-id="fa7ec-134">Int32</span><span class="sxs-lookup"><span data-stu-id="fa7ec-134">Int32</span></span>|<span data-ttu-id="fa7ec-135">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="fa7ec-135">Number of succeeded devices</span></span>|
|<span data-ttu-id="fa7ec-136">errorCount</span><span class="sxs-lookup"><span data-stu-id="fa7ec-136">errorCount</span></span>|<span data-ttu-id="fa7ec-137">Int32</span><span class="sxs-lookup"><span data-stu-id="fa7ec-137">Int32</span></span>|<span data-ttu-id="fa7ec-138">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="fa7ec-138">Number of error devices</span></span>|
|<span data-ttu-id="fa7ec-139">failedCount</span><span class="sxs-lookup"><span data-stu-id="fa7ec-139">failedCount</span></span>|<span data-ttu-id="fa7ec-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fa7ec-140">Int32</span></span>|<span data-ttu-id="fa7ec-141">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="fa7ec-141">Number of failed devices</span></span>|
|<span data-ttu-id="fa7ec-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="fa7ec-142">conflictCount</span></span>|<span data-ttu-id="fa7ec-143">Int32</span><span class="sxs-lookup"><span data-stu-id="fa7ec-143">Int32</span></span>|<span data-ttu-id="fa7ec-144">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="fa7ec-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="fa7ec-145">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="fa7ec-145">lastUpdateDateTime</span></span>|<span data-ttu-id="fa7ec-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa7ec-146">DateTimeOffset</span></span>|<span data-ttu-id="fa7ec-147">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="fa7ec-147">Last update time</span></span>|
|<span data-ttu-id="fa7ec-148">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="fa7ec-148">configurationVersion</span></span>|<span data-ttu-id="fa7ec-149">Int32</span><span class="sxs-lookup"><span data-stu-id="fa7ec-149">Int32</span></span>|<span data-ttu-id="fa7ec-150">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="fa7ec-150">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa7ec-151">关系</span><span class="sxs-lookup"><span data-stu-id="fa7ec-151">Relationships</span></span>
<span data-ttu-id="fa7ec-152">无</span><span class="sxs-lookup"><span data-stu-id="fa7ec-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa7ec-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa7ec-153">JSON Representation</span></span>
<span data-ttu-id="fa7ec-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa7ec-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```





