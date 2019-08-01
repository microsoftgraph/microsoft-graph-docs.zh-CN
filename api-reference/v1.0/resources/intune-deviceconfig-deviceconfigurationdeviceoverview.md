---
title: deviceConfigurationDeviceOverview 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 25abfce9ad69ea6f658a8883cb227806362a6cff
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028439"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="05c1a-103">deviceConfigurationDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="05c1a-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="05c1a-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05c1a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05c1a-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="05c1a-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="05c1a-106">方法</span><span class="sxs-lookup"><span data-stu-id="05c1a-106">Methods</span></span>
|<span data-ttu-id="05c1a-107">方法</span><span class="sxs-lookup"><span data-stu-id="05c1a-107">Method</span></span>|<span data-ttu-id="05c1a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="05c1a-108">Return Type</span></span>|<span data-ttu-id="05c1a-109">说明</span><span class="sxs-lookup"><span data-stu-id="05c1a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="05c1a-110">获取 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="05c1a-110">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="05c1a-111">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="05c1a-111">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="05c1a-112">读取 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="05c1a-112">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="05c1a-113">更新 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="05c1a-113">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="05c1a-114">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="05c1a-114">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="05c1a-115">更新 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="05c1a-115">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="05c1a-116">属性</span><span class="sxs-lookup"><span data-stu-id="05c1a-116">Properties</span></span>
|<span data-ttu-id="05c1a-117">属性</span><span class="sxs-lookup"><span data-stu-id="05c1a-117">Property</span></span>|<span data-ttu-id="05c1a-118">类型</span><span class="sxs-lookup"><span data-stu-id="05c1a-118">Type</span></span>|<span data-ttu-id="05c1a-119">说明</span><span class="sxs-lookup"><span data-stu-id="05c1a-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05c1a-120">id</span><span class="sxs-lookup"><span data-stu-id="05c1a-120">id</span></span>|<span data-ttu-id="05c1a-121">String</span><span class="sxs-lookup"><span data-stu-id="05c1a-121">String</span></span>|<span data-ttu-id="05c1a-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="05c1a-122">Key of the entity.</span></span>|
|<span data-ttu-id="05c1a-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="05c1a-123">pendingCount</span></span>|<span data-ttu-id="05c1a-124">Int32</span><span class="sxs-lookup"><span data-stu-id="05c1a-124">Int32</span></span>|<span data-ttu-id="05c1a-125">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="05c1a-125">Number of pending devices</span></span>|
|<span data-ttu-id="05c1a-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="05c1a-126">notApplicableCount</span></span>|<span data-ttu-id="05c1a-127">Int32</span><span class="sxs-lookup"><span data-stu-id="05c1a-127">Int32</span></span>|<span data-ttu-id="05c1a-128">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="05c1a-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="05c1a-129">successCount</span><span class="sxs-lookup"><span data-stu-id="05c1a-129">successCount</span></span>|<span data-ttu-id="05c1a-130">Int32</span><span class="sxs-lookup"><span data-stu-id="05c1a-130">Int32</span></span>|<span data-ttu-id="05c1a-131">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="05c1a-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="05c1a-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="05c1a-132">errorCount</span></span>|<span data-ttu-id="05c1a-133">Int32</span><span class="sxs-lookup"><span data-stu-id="05c1a-133">Int32</span></span>|<span data-ttu-id="05c1a-134">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="05c1a-134">Number of error devices</span></span>|
|<span data-ttu-id="05c1a-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="05c1a-135">failedCount</span></span>|<span data-ttu-id="05c1a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="05c1a-136">Int32</span></span>|<span data-ttu-id="05c1a-137">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="05c1a-137">Number of failed devices</span></span>|
|<span data-ttu-id="05c1a-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="05c1a-138">lastUpdateDateTime</span></span>|<span data-ttu-id="05c1a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05c1a-139">DateTimeOffset</span></span>|<span data-ttu-id="05c1a-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="05c1a-140">Last update time</span></span>|
|<span data-ttu-id="05c1a-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="05c1a-141">configurationVersion</span></span>|<span data-ttu-id="05c1a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="05c1a-142">Int32</span></span>|<span data-ttu-id="05c1a-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="05c1a-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="05c1a-144">关系</span><span class="sxs-lookup"><span data-stu-id="05c1a-144">Relationships</span></span>
<span data-ttu-id="05c1a-145">无</span><span class="sxs-lookup"><span data-stu-id="05c1a-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05c1a-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05c1a-146">JSON Representation</span></span>
<span data-ttu-id="05c1a-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05c1a-147">Here is a JSON representation of the resource.</span></span>
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



