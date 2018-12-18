---
title: deviceConfigurationDeviceOverview 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 32011d2c354486a3ea9d029970cf57d76843bff3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332345"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="deb8b-103">deviceConfigurationDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="deb8b-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="deb8b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="deb8b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="deb8b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="deb8b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="deb8b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="deb8b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="deb8b-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="deb8b-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="deb8b-108">方法</span><span class="sxs-lookup"><span data-stu-id="deb8b-108">Methods</span></span>
|<span data-ttu-id="deb8b-109">方法</span><span class="sxs-lookup"><span data-stu-id="deb8b-109">Method</span></span>|<span data-ttu-id="deb8b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="deb8b-110">Return Type</span></span>|<span data-ttu-id="deb8b-111">说明</span><span class="sxs-lookup"><span data-stu-id="deb8b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="deb8b-112">获取 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="deb8b-112">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="deb8b-113">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="deb8b-113">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="deb8b-114">读取 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="deb8b-114">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="deb8b-115">更新 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="deb8b-115">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="deb8b-116">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="deb8b-116">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="deb8b-117">更新 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="deb8b-117">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="deb8b-118">属性</span><span class="sxs-lookup"><span data-stu-id="deb8b-118">Properties</span></span>
|<span data-ttu-id="deb8b-119">属性</span><span class="sxs-lookup"><span data-stu-id="deb8b-119">Property</span></span>|<span data-ttu-id="deb8b-120">类型</span><span class="sxs-lookup"><span data-stu-id="deb8b-120">Type</span></span>|<span data-ttu-id="deb8b-121">说明</span><span class="sxs-lookup"><span data-stu-id="deb8b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="deb8b-122">id</span><span class="sxs-lookup"><span data-stu-id="deb8b-122">id</span></span>|<span data-ttu-id="deb8b-123">String</span><span class="sxs-lookup"><span data-stu-id="deb8b-123">String</span></span>|<span data-ttu-id="deb8b-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="deb8b-124">Key of the entity.</span></span>|
|<span data-ttu-id="deb8b-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="deb8b-125">pendingCount</span></span>|<span data-ttu-id="deb8b-126">Int32</span><span class="sxs-lookup"><span data-stu-id="deb8b-126">Int32</span></span>|<span data-ttu-id="deb8b-127">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="deb8b-127">Number of pending devices</span></span>|
|<span data-ttu-id="deb8b-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="deb8b-128">notApplicableCount</span></span>|<span data-ttu-id="deb8b-129">Int32</span><span class="sxs-lookup"><span data-stu-id="deb8b-129">Int32</span></span>|<span data-ttu-id="deb8b-130">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="deb8b-130">Number of not applicable devices</span></span>|
|<span data-ttu-id="deb8b-131">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="deb8b-131">notApplicablePlatformCount</span></span>|<span data-ttu-id="deb8b-132">Int32</span><span class="sxs-lookup"><span data-stu-id="deb8b-132">Int32</span></span>|<span data-ttu-id="deb8b-133">由于不匹配平台和策略不适用设备数</span><span class="sxs-lookup"><span data-stu-id="deb8b-133">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="deb8b-134">successCount</span><span class="sxs-lookup"><span data-stu-id="deb8b-134">successCount</span></span>|<span data-ttu-id="deb8b-135">Int32</span><span class="sxs-lookup"><span data-stu-id="deb8b-135">Int32</span></span>|<span data-ttu-id="deb8b-136">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="deb8b-136">Number of succeeded devices</span></span>|
|<span data-ttu-id="deb8b-137">errorCount</span><span class="sxs-lookup"><span data-stu-id="deb8b-137">errorCount</span></span>|<span data-ttu-id="deb8b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="deb8b-138">Int32</span></span>|<span data-ttu-id="deb8b-139">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="deb8b-139">Number of error devices</span></span>|
|<span data-ttu-id="deb8b-140">failedCount</span><span class="sxs-lookup"><span data-stu-id="deb8b-140">failedCount</span></span>|<span data-ttu-id="deb8b-141">Int32</span><span class="sxs-lookup"><span data-stu-id="deb8b-141">Int32</span></span>|<span data-ttu-id="deb8b-142">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="deb8b-142">Number of failed devices</span></span>|
|<span data-ttu-id="deb8b-143">conflictCount</span><span class="sxs-lookup"><span data-stu-id="deb8b-143">conflictCount</span></span>|<span data-ttu-id="deb8b-144">Int32</span><span class="sxs-lookup"><span data-stu-id="deb8b-144">Int32</span></span>|<span data-ttu-id="deb8b-145">存在冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="deb8b-145">Number of devices in conflict</span></span>|
|<span data-ttu-id="deb8b-146">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="deb8b-146">lastUpdateDateTime</span></span>|<span data-ttu-id="deb8b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="deb8b-147">DateTimeOffset</span></span>|<span data-ttu-id="deb8b-148">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="deb8b-148">Last update time</span></span>|
|<span data-ttu-id="deb8b-149">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="deb8b-149">configurationVersion</span></span>|<span data-ttu-id="deb8b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="deb8b-150">Int32</span></span>|<span data-ttu-id="deb8b-151">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="deb8b-151">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="deb8b-152">关系</span><span class="sxs-lookup"><span data-stu-id="deb8b-152">Relationships</span></span>
<span data-ttu-id="deb8b-153">无</span><span class="sxs-lookup"><span data-stu-id="deb8b-153">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="deb8b-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="deb8b-154">JSON Representation</span></span>
<span data-ttu-id="deb8b-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="deb8b-155">Here is a JSON representation of the resource.</span></span>
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





