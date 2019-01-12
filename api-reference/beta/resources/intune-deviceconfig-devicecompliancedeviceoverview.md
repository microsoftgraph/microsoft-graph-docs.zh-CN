---
title: deviceComplianceDeviceOverview 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 831fe9241b23758ee868053e59e93b427fbfc2dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950751"
---
# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="47361-103">deviceComplianceDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="47361-103">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="47361-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="47361-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47361-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="47361-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47361-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="47361-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47361-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="47361-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="47361-108">方法</span><span class="sxs-lookup"><span data-stu-id="47361-108">Methods</span></span>
|<span data-ttu-id="47361-109">方法</span><span class="sxs-lookup"><span data-stu-id="47361-109">Method</span></span>|<span data-ttu-id="47361-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="47361-110">Return Type</span></span>|<span data-ttu-id="47361-111">说明</span><span class="sxs-lookup"><span data-stu-id="47361-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="47361-112">获取 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="47361-112">Get deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-get.md)|[<span data-ttu-id="47361-113">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="47361-113">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="47361-114">读取 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="47361-114">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="47361-115">更新 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="47361-115">Update deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-update.md)|[<span data-ttu-id="47361-116">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="47361-116">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="47361-117">更新 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="47361-117">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="47361-118">属性</span><span class="sxs-lookup"><span data-stu-id="47361-118">Properties</span></span>
|<span data-ttu-id="47361-119">属性</span><span class="sxs-lookup"><span data-stu-id="47361-119">Property</span></span>|<span data-ttu-id="47361-120">类型</span><span class="sxs-lookup"><span data-stu-id="47361-120">Type</span></span>|<span data-ttu-id="47361-121">说明</span><span class="sxs-lookup"><span data-stu-id="47361-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47361-122">id</span><span class="sxs-lookup"><span data-stu-id="47361-122">id</span></span>|<span data-ttu-id="47361-123">String</span><span class="sxs-lookup"><span data-stu-id="47361-123">String</span></span>|<span data-ttu-id="47361-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="47361-124">Key of the entity.</span></span>|
|<span data-ttu-id="47361-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="47361-125">pendingCount</span></span>|<span data-ttu-id="47361-126">Int32</span><span class="sxs-lookup"><span data-stu-id="47361-126">Int32</span></span>|<span data-ttu-id="47361-127">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="47361-127">Number of pending devices</span></span>|
|<span data-ttu-id="47361-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="47361-128">notApplicableCount</span></span>|<span data-ttu-id="47361-129">Int32</span><span class="sxs-lookup"><span data-stu-id="47361-129">Int32</span></span>|<span data-ttu-id="47361-130">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="47361-130">Number of not applicable devices</span></span>|
|<span data-ttu-id="47361-131">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="47361-131">notApplicablePlatformCount</span></span>|<span data-ttu-id="47361-132">Int32</span><span class="sxs-lookup"><span data-stu-id="47361-132">Int32</span></span>|<span data-ttu-id="47361-133">由于不匹配平台和策略不适用设备数</span><span class="sxs-lookup"><span data-stu-id="47361-133">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="47361-134">successCount</span><span class="sxs-lookup"><span data-stu-id="47361-134">successCount</span></span>|<span data-ttu-id="47361-135">Int32</span><span class="sxs-lookup"><span data-stu-id="47361-135">Int32</span></span>|<span data-ttu-id="47361-136">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="47361-136">Number of succeeded devices</span></span>|
|<span data-ttu-id="47361-137">errorCount</span><span class="sxs-lookup"><span data-stu-id="47361-137">errorCount</span></span>|<span data-ttu-id="47361-138">Int32</span><span class="sxs-lookup"><span data-stu-id="47361-138">Int32</span></span>|<span data-ttu-id="47361-139">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="47361-139">Number of error devices</span></span>|
|<span data-ttu-id="47361-140">failedCount</span><span class="sxs-lookup"><span data-stu-id="47361-140">failedCount</span></span>|<span data-ttu-id="47361-141">Int32</span><span class="sxs-lookup"><span data-stu-id="47361-141">Int32</span></span>|<span data-ttu-id="47361-142">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="47361-142">Number of failed devices</span></span>|
|<span data-ttu-id="47361-143">conflictCount</span><span class="sxs-lookup"><span data-stu-id="47361-143">conflictCount</span></span>|<span data-ttu-id="47361-144">Int32</span><span class="sxs-lookup"><span data-stu-id="47361-144">Int32</span></span>|<span data-ttu-id="47361-145">存在冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="47361-145">Number of devices in conflict</span></span>|
|<span data-ttu-id="47361-146">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="47361-146">lastUpdateDateTime</span></span>|<span data-ttu-id="47361-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47361-147">DateTimeOffset</span></span>|<span data-ttu-id="47361-148">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="47361-148">Last update time</span></span>|
|<span data-ttu-id="47361-149">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="47361-149">configurationVersion</span></span>|<span data-ttu-id="47361-150">Int32</span><span class="sxs-lookup"><span data-stu-id="47361-150">Int32</span></span>|<span data-ttu-id="47361-151">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="47361-151">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="47361-152">关系</span><span class="sxs-lookup"><span data-stu-id="47361-152">Relationships</span></span>
<span data-ttu-id="47361-153">无</span><span class="sxs-lookup"><span data-stu-id="47361-153">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47361-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47361-154">JSON Representation</span></span>
<span data-ttu-id="47361-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47361-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
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





