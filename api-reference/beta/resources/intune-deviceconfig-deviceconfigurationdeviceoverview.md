---
title: deviceConfigurationDeviceOverview 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ead4ad9af39a4f40eb4dae971510098105d8b3c6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735286"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="444b6-103">deviceConfigurationDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="444b6-103">deviceConfigurationDeviceOverview resource type</span></span>

<span data-ttu-id="444b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="444b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="444b6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="444b6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="444b6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="444b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="444b6-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="444b6-107">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="444b6-108">Methods</span><span class="sxs-lookup"><span data-stu-id="444b6-108">Methods</span></span>
|<span data-ttu-id="444b6-109">方法</span><span class="sxs-lookup"><span data-stu-id="444b6-109">Method</span></span>|<span data-ttu-id="444b6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="444b6-110">Return Type</span></span>|<span data-ttu-id="444b6-111">说明</span><span class="sxs-lookup"><span data-stu-id="444b6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="444b6-112">获取 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="444b6-112">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="444b6-113">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="444b6-113">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="444b6-114">读取 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="444b6-114">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="444b6-115">更新 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="444b6-115">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="444b6-116">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="444b6-116">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="444b6-117">更新 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="444b6-117">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="444b6-118">属性</span><span class="sxs-lookup"><span data-stu-id="444b6-118">Properties</span></span>
|<span data-ttu-id="444b6-119">属性</span><span class="sxs-lookup"><span data-stu-id="444b6-119">Property</span></span>|<span data-ttu-id="444b6-120">类型</span><span class="sxs-lookup"><span data-stu-id="444b6-120">Type</span></span>|<span data-ttu-id="444b6-121">说明</span><span class="sxs-lookup"><span data-stu-id="444b6-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="444b6-122">id</span><span class="sxs-lookup"><span data-stu-id="444b6-122">id</span></span>|<span data-ttu-id="444b6-123">String</span><span class="sxs-lookup"><span data-stu-id="444b6-123">String</span></span>|<span data-ttu-id="444b6-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="444b6-124">Key of the entity.</span></span>|
|<span data-ttu-id="444b6-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="444b6-125">pendingCount</span></span>|<span data-ttu-id="444b6-126">Int32</span><span class="sxs-lookup"><span data-stu-id="444b6-126">Int32</span></span>|<span data-ttu-id="444b6-127">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="444b6-127">Number of pending devices</span></span>|
|<span data-ttu-id="444b6-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="444b6-128">notApplicableCount</span></span>|<span data-ttu-id="444b6-129">Int32</span><span class="sxs-lookup"><span data-stu-id="444b6-129">Int32</span></span>|<span data-ttu-id="444b6-130">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="444b6-130">Number of not applicable devices</span></span>|
|<span data-ttu-id="444b6-131">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="444b6-131">notApplicablePlatformCount</span></span>|<span data-ttu-id="444b6-132">Int32</span><span class="sxs-lookup"><span data-stu-id="444b6-132">Int32</span></span>|<span data-ttu-id="444b6-133">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="444b6-133">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="444b6-134">successCount</span><span class="sxs-lookup"><span data-stu-id="444b6-134">successCount</span></span>|<span data-ttu-id="444b6-135">Int32</span><span class="sxs-lookup"><span data-stu-id="444b6-135">Int32</span></span>|<span data-ttu-id="444b6-136">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="444b6-136">Number of succeeded devices</span></span>|
|<span data-ttu-id="444b6-137">errorCount</span><span class="sxs-lookup"><span data-stu-id="444b6-137">errorCount</span></span>|<span data-ttu-id="444b6-138">Int32</span><span class="sxs-lookup"><span data-stu-id="444b6-138">Int32</span></span>|<span data-ttu-id="444b6-139">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="444b6-139">Number of error devices</span></span>|
|<span data-ttu-id="444b6-140">failedCount</span><span class="sxs-lookup"><span data-stu-id="444b6-140">failedCount</span></span>|<span data-ttu-id="444b6-141">Int32</span><span class="sxs-lookup"><span data-stu-id="444b6-141">Int32</span></span>|<span data-ttu-id="444b6-142">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="444b6-142">Number of failed devices</span></span>|
|<span data-ttu-id="444b6-143">conflictCount</span><span class="sxs-lookup"><span data-stu-id="444b6-143">conflictCount</span></span>|<span data-ttu-id="444b6-144">Int32</span><span class="sxs-lookup"><span data-stu-id="444b6-144">Int32</span></span>|<span data-ttu-id="444b6-145">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="444b6-145">Number of devices in conflict</span></span>|
|<span data-ttu-id="444b6-146">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="444b6-146">lastUpdateDateTime</span></span>|<span data-ttu-id="444b6-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="444b6-147">DateTimeOffset</span></span>|<span data-ttu-id="444b6-148">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="444b6-148">Last update time</span></span>|
|<span data-ttu-id="444b6-149">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="444b6-149">configurationVersion</span></span>|<span data-ttu-id="444b6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="444b6-150">Int32</span></span>|<span data-ttu-id="444b6-151">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="444b6-151">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="444b6-152">关系</span><span class="sxs-lookup"><span data-stu-id="444b6-152">Relationships</span></span>
<span data-ttu-id="444b6-153">无</span><span class="sxs-lookup"><span data-stu-id="444b6-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="444b6-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="444b6-154">JSON Representation</span></span>
<span data-ttu-id="444b6-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="444b6-155">Here is a JSON representation of the resource.</span></span>
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





