---
title: deviceConfigurationDeviceOverview 资源类型
description: 尚未记录
ms.openlocfilehash: 3ed4370b06de330238d426b5c77cfbc94a460a54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045310"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="17fab-103">deviceConfigurationDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="17fab-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="17fab-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="17fab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17fab-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="17fab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17fab-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="17fab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17fab-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="17fab-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="17fab-108">方法</span><span class="sxs-lookup"><span data-stu-id="17fab-108">Methods</span></span>
|<span data-ttu-id="17fab-109">方法</span><span class="sxs-lookup"><span data-stu-id="17fab-109">Method</span></span>|<span data-ttu-id="17fab-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="17fab-110">Return Type</span></span>|<span data-ttu-id="17fab-111">说明</span><span class="sxs-lookup"><span data-stu-id="17fab-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="17fab-112">获取 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="17fab-112">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="17fab-113">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="17fab-113">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="17fab-114">读取 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="17fab-114">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="17fab-115">更新 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="17fab-115">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="17fab-116">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="17fab-116">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="17fab-117">更新 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="17fab-117">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="17fab-118">属性</span><span class="sxs-lookup"><span data-stu-id="17fab-118">Properties</span></span>
|<span data-ttu-id="17fab-119">属性</span><span class="sxs-lookup"><span data-stu-id="17fab-119">Property</span></span>|<span data-ttu-id="17fab-120">类型</span><span class="sxs-lookup"><span data-stu-id="17fab-120">Type</span></span>|<span data-ttu-id="17fab-121">说明</span><span class="sxs-lookup"><span data-stu-id="17fab-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17fab-122">id</span><span class="sxs-lookup"><span data-stu-id="17fab-122">id</span></span>|<span data-ttu-id="17fab-123">String</span><span class="sxs-lookup"><span data-stu-id="17fab-123">String</span></span>|<span data-ttu-id="17fab-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="17fab-124">Key of the entity.</span></span>|
|<span data-ttu-id="17fab-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="17fab-125">pendingCount</span></span>|<span data-ttu-id="17fab-126">Int32</span><span class="sxs-lookup"><span data-stu-id="17fab-126">Int32</span></span>|<span data-ttu-id="17fab-127">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="17fab-127">Number of pending devices</span></span>|
|<span data-ttu-id="17fab-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="17fab-128">notApplicableCount</span></span>|<span data-ttu-id="17fab-129">Int32</span><span class="sxs-lookup"><span data-stu-id="17fab-129">Int32</span></span>|<span data-ttu-id="17fab-130">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="17fab-130">Number of not applicable devices</span></span>|
|<span data-ttu-id="17fab-131">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="17fab-131">notApplicablePlatformCount</span></span>|<span data-ttu-id="17fab-132">Int32</span><span class="sxs-lookup"><span data-stu-id="17fab-132">Int32</span></span>|<span data-ttu-id="17fab-133">由于不匹配平台和策略不适用设备数</span><span class="sxs-lookup"><span data-stu-id="17fab-133">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="17fab-134">successCount</span><span class="sxs-lookup"><span data-stu-id="17fab-134">successCount</span></span>|<span data-ttu-id="17fab-135">Int32</span><span class="sxs-lookup"><span data-stu-id="17fab-135">Int32</span></span>|<span data-ttu-id="17fab-136">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="17fab-136">Number of succeeded devices</span></span>|
|<span data-ttu-id="17fab-137">errorCount</span><span class="sxs-lookup"><span data-stu-id="17fab-137">errorCount</span></span>|<span data-ttu-id="17fab-138">Int32</span><span class="sxs-lookup"><span data-stu-id="17fab-138">Int32</span></span>|<span data-ttu-id="17fab-139">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="17fab-139">Number of error devices</span></span>|
|<span data-ttu-id="17fab-140">failedCount</span><span class="sxs-lookup"><span data-stu-id="17fab-140">failedCount</span></span>|<span data-ttu-id="17fab-141">Int32</span><span class="sxs-lookup"><span data-stu-id="17fab-141">Int32</span></span>|<span data-ttu-id="17fab-142">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="17fab-142">Number of failed devices</span></span>|
|<span data-ttu-id="17fab-143">conflictCount</span><span class="sxs-lookup"><span data-stu-id="17fab-143">conflictCount</span></span>|<span data-ttu-id="17fab-144">Int32</span><span class="sxs-lookup"><span data-stu-id="17fab-144">Int32</span></span>|<span data-ttu-id="17fab-145">存在冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="17fab-145">Number of devices in conflict</span></span>|
|<span data-ttu-id="17fab-146">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="17fab-146">lastUpdateDateTime</span></span>|<span data-ttu-id="17fab-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17fab-147">DateTimeOffset</span></span>|<span data-ttu-id="17fab-148">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="17fab-148">Last update time</span></span>|
|<span data-ttu-id="17fab-149">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="17fab-149">configurationVersion</span></span>|<span data-ttu-id="17fab-150">Int32</span><span class="sxs-lookup"><span data-stu-id="17fab-150">Int32</span></span>|<span data-ttu-id="17fab-151">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="17fab-151">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="17fab-152">关系</span><span class="sxs-lookup"><span data-stu-id="17fab-152">Relationships</span></span>
<span data-ttu-id="17fab-153">无</span><span class="sxs-lookup"><span data-stu-id="17fab-153">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="17fab-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17fab-154">JSON Representation</span></span>
<span data-ttu-id="17fab-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17fab-155">Here is a JSON representation of the resource.</span></span>
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





