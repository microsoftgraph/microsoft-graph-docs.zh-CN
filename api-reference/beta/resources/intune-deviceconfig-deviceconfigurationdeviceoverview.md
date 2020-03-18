---
title: deviceConfigurationDeviceOverview 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aebee8db88336468b70ab713e2447475b1e840fb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42793266"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="001ab-103">deviceConfigurationDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="001ab-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="001ab-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="001ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="001ab-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="001ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="001ab-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="001ab-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="001ab-107">方法</span><span class="sxs-lookup"><span data-stu-id="001ab-107">Methods</span></span>
|<span data-ttu-id="001ab-108">方法</span><span class="sxs-lookup"><span data-stu-id="001ab-108">Method</span></span>|<span data-ttu-id="001ab-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="001ab-109">Return Type</span></span>|<span data-ttu-id="001ab-110">说明</span><span class="sxs-lookup"><span data-stu-id="001ab-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="001ab-111">获取 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="001ab-111">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="001ab-112">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="001ab-112">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="001ab-113">读取 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="001ab-113">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="001ab-114">更新 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="001ab-114">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="001ab-115">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="001ab-115">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="001ab-116">更新 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="001ab-116">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="001ab-117">属性</span><span class="sxs-lookup"><span data-stu-id="001ab-117">Properties</span></span>
|<span data-ttu-id="001ab-118">属性</span><span class="sxs-lookup"><span data-stu-id="001ab-118">Property</span></span>|<span data-ttu-id="001ab-119">类型</span><span class="sxs-lookup"><span data-stu-id="001ab-119">Type</span></span>|<span data-ttu-id="001ab-120">说明</span><span class="sxs-lookup"><span data-stu-id="001ab-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="001ab-121">id</span><span class="sxs-lookup"><span data-stu-id="001ab-121">id</span></span>|<span data-ttu-id="001ab-122">String</span><span class="sxs-lookup"><span data-stu-id="001ab-122">String</span></span>|<span data-ttu-id="001ab-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="001ab-123">Key of the entity.</span></span>|
|<span data-ttu-id="001ab-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="001ab-124">pendingCount</span></span>|<span data-ttu-id="001ab-125">Int32</span><span class="sxs-lookup"><span data-stu-id="001ab-125">Int32</span></span>|<span data-ttu-id="001ab-126">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="001ab-126">Number of pending devices</span></span>|
|<span data-ttu-id="001ab-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="001ab-127">notApplicableCount</span></span>|<span data-ttu-id="001ab-128">Int32</span><span class="sxs-lookup"><span data-stu-id="001ab-128">Int32</span></span>|<span data-ttu-id="001ab-129">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="001ab-129">Number of not applicable devices</span></span>|
|<span data-ttu-id="001ab-130">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="001ab-130">notApplicablePlatformCount</span></span>|<span data-ttu-id="001ab-131">Int32</span><span class="sxs-lookup"><span data-stu-id="001ab-131">Int32</span></span>|<span data-ttu-id="001ab-132">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="001ab-132">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="001ab-133">successCount</span><span class="sxs-lookup"><span data-stu-id="001ab-133">successCount</span></span>|<span data-ttu-id="001ab-134">Int32</span><span class="sxs-lookup"><span data-stu-id="001ab-134">Int32</span></span>|<span data-ttu-id="001ab-135">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="001ab-135">Number of succeeded devices</span></span>|
|<span data-ttu-id="001ab-136">errorCount</span><span class="sxs-lookup"><span data-stu-id="001ab-136">errorCount</span></span>|<span data-ttu-id="001ab-137">Int32</span><span class="sxs-lookup"><span data-stu-id="001ab-137">Int32</span></span>|<span data-ttu-id="001ab-138">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="001ab-138">Number of error devices</span></span>|
|<span data-ttu-id="001ab-139">failedCount</span><span class="sxs-lookup"><span data-stu-id="001ab-139">failedCount</span></span>|<span data-ttu-id="001ab-140">Int32</span><span class="sxs-lookup"><span data-stu-id="001ab-140">Int32</span></span>|<span data-ttu-id="001ab-141">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="001ab-141">Number of failed devices</span></span>|
|<span data-ttu-id="001ab-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="001ab-142">conflictCount</span></span>|<span data-ttu-id="001ab-143">Int32</span><span class="sxs-lookup"><span data-stu-id="001ab-143">Int32</span></span>|<span data-ttu-id="001ab-144">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="001ab-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="001ab-145">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="001ab-145">lastUpdateDateTime</span></span>|<span data-ttu-id="001ab-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="001ab-146">DateTimeOffset</span></span>|<span data-ttu-id="001ab-147">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="001ab-147">Last update time</span></span>|
|<span data-ttu-id="001ab-148">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="001ab-148">configurationVersion</span></span>|<span data-ttu-id="001ab-149">Int32</span><span class="sxs-lookup"><span data-stu-id="001ab-149">Int32</span></span>|<span data-ttu-id="001ab-150">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="001ab-150">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="001ab-151">关系</span><span class="sxs-lookup"><span data-stu-id="001ab-151">Relationships</span></span>
<span data-ttu-id="001ab-152">无</span><span class="sxs-lookup"><span data-stu-id="001ab-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="001ab-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="001ab-153">JSON Representation</span></span>
<span data-ttu-id="001ab-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="001ab-154">Here is a JSON representation of the resource.</span></span>
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



