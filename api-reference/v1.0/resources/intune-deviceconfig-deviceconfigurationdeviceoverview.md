---
title: deviceConfigurationDeviceOverview 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8fe0f897ea15014e77160e14fa73386b7402e263
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447828"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="deaf0-103">deviceConfigurationDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="deaf0-103">deviceConfigurationDeviceOverview resource type</span></span>

<span data-ttu-id="deaf0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deaf0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="deaf0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="deaf0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="deaf0-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="deaf0-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="deaf0-107">方法</span><span class="sxs-lookup"><span data-stu-id="deaf0-107">Methods</span></span>
|<span data-ttu-id="deaf0-108">方法</span><span class="sxs-lookup"><span data-stu-id="deaf0-108">Method</span></span>|<span data-ttu-id="deaf0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="deaf0-109">Return Type</span></span>|<span data-ttu-id="deaf0-110">说明</span><span class="sxs-lookup"><span data-stu-id="deaf0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="deaf0-111">获取 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="deaf0-111">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="deaf0-112">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="deaf0-112">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="deaf0-113">读取 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="deaf0-113">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="deaf0-114">更新 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="deaf0-114">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="deaf0-115">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="deaf0-115">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="deaf0-116">更新 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="deaf0-116">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="deaf0-117">属性</span><span class="sxs-lookup"><span data-stu-id="deaf0-117">Properties</span></span>
|<span data-ttu-id="deaf0-118">属性</span><span class="sxs-lookup"><span data-stu-id="deaf0-118">Property</span></span>|<span data-ttu-id="deaf0-119">类型</span><span class="sxs-lookup"><span data-stu-id="deaf0-119">Type</span></span>|<span data-ttu-id="deaf0-120">说明</span><span class="sxs-lookup"><span data-stu-id="deaf0-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="deaf0-121">id</span><span class="sxs-lookup"><span data-stu-id="deaf0-121">id</span></span>|<span data-ttu-id="deaf0-122">String</span><span class="sxs-lookup"><span data-stu-id="deaf0-122">String</span></span>|<span data-ttu-id="deaf0-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="deaf0-123">Key of the entity.</span></span>|
|<span data-ttu-id="deaf0-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="deaf0-124">pendingCount</span></span>|<span data-ttu-id="deaf0-125">Int32</span><span class="sxs-lookup"><span data-stu-id="deaf0-125">Int32</span></span>|<span data-ttu-id="deaf0-126">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="deaf0-126">Number of pending devices</span></span>|
|<span data-ttu-id="deaf0-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="deaf0-127">notApplicableCount</span></span>|<span data-ttu-id="deaf0-128">Int32</span><span class="sxs-lookup"><span data-stu-id="deaf0-128">Int32</span></span>|<span data-ttu-id="deaf0-129">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="deaf0-129">Number of not applicable devices</span></span>|
|<span data-ttu-id="deaf0-130">successCount</span><span class="sxs-lookup"><span data-stu-id="deaf0-130">successCount</span></span>|<span data-ttu-id="deaf0-131">Int32</span><span class="sxs-lookup"><span data-stu-id="deaf0-131">Int32</span></span>|<span data-ttu-id="deaf0-132">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="deaf0-132">Number of succeeded devices</span></span>|
|<span data-ttu-id="deaf0-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="deaf0-133">errorCount</span></span>|<span data-ttu-id="deaf0-134">Int32</span><span class="sxs-lookup"><span data-stu-id="deaf0-134">Int32</span></span>|<span data-ttu-id="deaf0-135">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="deaf0-135">Number of error devices</span></span>|
|<span data-ttu-id="deaf0-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="deaf0-136">failedCount</span></span>|<span data-ttu-id="deaf0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="deaf0-137">Int32</span></span>|<span data-ttu-id="deaf0-138">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="deaf0-138">Number of failed devices</span></span>|
|<span data-ttu-id="deaf0-139">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="deaf0-139">lastUpdateDateTime</span></span>|<span data-ttu-id="deaf0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="deaf0-140">DateTimeOffset</span></span>|<span data-ttu-id="deaf0-141">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="deaf0-141">Last update time</span></span>|
|<span data-ttu-id="deaf0-142">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="deaf0-142">configurationVersion</span></span>|<span data-ttu-id="deaf0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="deaf0-143">Int32</span></span>|<span data-ttu-id="deaf0-144">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="deaf0-144">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="deaf0-145">关系</span><span class="sxs-lookup"><span data-stu-id="deaf0-145">Relationships</span></span>
<span data-ttu-id="deaf0-146">无</span><span class="sxs-lookup"><span data-stu-id="deaf0-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="deaf0-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="deaf0-147">JSON Representation</span></span>
<span data-ttu-id="deaf0-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="deaf0-148">Here is a JSON representation of the resource.</span></span>
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
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```







