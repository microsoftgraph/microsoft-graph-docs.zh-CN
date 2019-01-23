---
title: deviceComplianceDeviceOverview 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0cf618cb0d78093bf9eb08fc82ef4bc17f8fe836
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402557"
---
# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="06835-103">deviceComplianceDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="06835-103">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="06835-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="06835-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="06835-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="06835-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06835-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06835-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06835-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="06835-107">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="06835-108">方法</span><span class="sxs-lookup"><span data-stu-id="06835-108">Methods</span></span>
|<span data-ttu-id="06835-109">方法</span><span class="sxs-lookup"><span data-stu-id="06835-109">Method</span></span>|<span data-ttu-id="06835-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="06835-110">Return Type</span></span>|<span data-ttu-id="06835-111">说明</span><span class="sxs-lookup"><span data-stu-id="06835-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06835-112">获取 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="06835-112">Get deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-get.md)|[<span data-ttu-id="06835-113">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="06835-113">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="06835-114">读取 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06835-114">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="06835-115">更新 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="06835-115">Update deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-update.md)|[<span data-ttu-id="06835-116">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="06835-116">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="06835-117">更新 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="06835-117">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06835-118">属性</span><span class="sxs-lookup"><span data-stu-id="06835-118">Properties</span></span>
|<span data-ttu-id="06835-119">属性</span><span class="sxs-lookup"><span data-stu-id="06835-119">Property</span></span>|<span data-ttu-id="06835-120">类型</span><span class="sxs-lookup"><span data-stu-id="06835-120">Type</span></span>|<span data-ttu-id="06835-121">说明</span><span class="sxs-lookup"><span data-stu-id="06835-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06835-122">id</span><span class="sxs-lookup"><span data-stu-id="06835-122">id</span></span>|<span data-ttu-id="06835-123">String</span><span class="sxs-lookup"><span data-stu-id="06835-123">String</span></span>|<span data-ttu-id="06835-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="06835-124">Key of the entity.</span></span>|
|<span data-ttu-id="06835-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="06835-125">pendingCount</span></span>|<span data-ttu-id="06835-126">Int32</span><span class="sxs-lookup"><span data-stu-id="06835-126">Int32</span></span>|<span data-ttu-id="06835-127">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="06835-127">Number of pending devices</span></span>|
|<span data-ttu-id="06835-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="06835-128">notApplicableCount</span></span>|<span data-ttu-id="06835-129">Int32</span><span class="sxs-lookup"><span data-stu-id="06835-129">Int32</span></span>|<span data-ttu-id="06835-130">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="06835-130">Number of not applicable devices</span></span>|
|<span data-ttu-id="06835-131">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="06835-131">notApplicablePlatformCount</span></span>|<span data-ttu-id="06835-132">Int32</span><span class="sxs-lookup"><span data-stu-id="06835-132">Int32</span></span>|<span data-ttu-id="06835-133">由于不匹配平台和策略不适用设备数</span><span class="sxs-lookup"><span data-stu-id="06835-133">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="06835-134">successCount</span><span class="sxs-lookup"><span data-stu-id="06835-134">successCount</span></span>|<span data-ttu-id="06835-135">Int32</span><span class="sxs-lookup"><span data-stu-id="06835-135">Int32</span></span>|<span data-ttu-id="06835-136">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="06835-136">Number of succeeded devices</span></span>|
|<span data-ttu-id="06835-137">errorCount</span><span class="sxs-lookup"><span data-stu-id="06835-137">errorCount</span></span>|<span data-ttu-id="06835-138">Int32</span><span class="sxs-lookup"><span data-stu-id="06835-138">Int32</span></span>|<span data-ttu-id="06835-139">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="06835-139">Number of error devices</span></span>|
|<span data-ttu-id="06835-140">failedCount</span><span class="sxs-lookup"><span data-stu-id="06835-140">failedCount</span></span>|<span data-ttu-id="06835-141">Int32</span><span class="sxs-lookup"><span data-stu-id="06835-141">Int32</span></span>|<span data-ttu-id="06835-142">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="06835-142">Number of failed devices</span></span>|
|<span data-ttu-id="06835-143">conflictCount</span><span class="sxs-lookup"><span data-stu-id="06835-143">conflictCount</span></span>|<span data-ttu-id="06835-144">Int32</span><span class="sxs-lookup"><span data-stu-id="06835-144">Int32</span></span>|<span data-ttu-id="06835-145">存在冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="06835-145">Number of devices in conflict</span></span>|
|<span data-ttu-id="06835-146">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="06835-146">lastUpdateDateTime</span></span>|<span data-ttu-id="06835-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06835-147">DateTimeOffset</span></span>|<span data-ttu-id="06835-148">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="06835-148">Last update time</span></span>|
|<span data-ttu-id="06835-149">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="06835-149">configurationVersion</span></span>|<span data-ttu-id="06835-150">Int32</span><span class="sxs-lookup"><span data-stu-id="06835-150">Int32</span></span>|<span data-ttu-id="06835-151">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="06835-151">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="06835-152">关系</span><span class="sxs-lookup"><span data-stu-id="06835-152">Relationships</span></span>
<span data-ttu-id="06835-153">无</span><span class="sxs-lookup"><span data-stu-id="06835-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06835-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06835-154">JSON Representation</span></span>
<span data-ttu-id="06835-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06835-155">Here is a JSON representation of the resource.</span></span>
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




