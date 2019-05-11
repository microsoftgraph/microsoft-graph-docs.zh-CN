---
title: managedDeviceMobileAppConfigurationDeviceSummary 资源类型
description: 包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ed6550cf071d04b72f1b5d2ba9ad97233d7289b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950128"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="ac607-103">managedDeviceMobileAppConfigurationDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac607-103">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="ac607-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ac607-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac607-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ac607-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac607-106">包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="ac607-106">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="ac607-107">方法</span><span class="sxs-lookup"><span data-stu-id="ac607-107">Methods</span></span>
|<span data-ttu-id="ac607-108">方法</span><span class="sxs-lookup"><span data-stu-id="ac607-108">Method</span></span>|<span data-ttu-id="ac607-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ac607-109">Return Type</span></span>|<span data-ttu-id="ac607-110">说明</span><span class="sxs-lookup"><span data-stu-id="ac607-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ac607-111">获取 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="ac607-111">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[<span data-ttu-id="ac607-112">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="ac607-112">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="ac607-113">读取 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ac607-113">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="ac607-114">更新 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="ac607-114">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[<span data-ttu-id="ac607-115">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="ac607-115">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="ac607-116">更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ac607-116">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac607-117">属性</span><span class="sxs-lookup"><span data-stu-id="ac607-117">Properties</span></span>
|<span data-ttu-id="ac607-118">属性</span><span class="sxs-lookup"><span data-stu-id="ac607-118">Property</span></span>|<span data-ttu-id="ac607-119">类型</span><span class="sxs-lookup"><span data-stu-id="ac607-119">Type</span></span>|<span data-ttu-id="ac607-120">说明</span><span class="sxs-lookup"><span data-stu-id="ac607-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac607-121">id</span><span class="sxs-lookup"><span data-stu-id="ac607-121">id</span></span>|<span data-ttu-id="ac607-122">String</span><span class="sxs-lookup"><span data-stu-id="ac607-122">String</span></span>|<span data-ttu-id="ac607-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ac607-123">Key of the entity.</span></span>|
|<span data-ttu-id="ac607-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="ac607-124">pendingCount</span></span>|<span data-ttu-id="ac607-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ac607-125">Int32</span></span>|<span data-ttu-id="ac607-126">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="ac607-126">Number of pending devices</span></span>|
|<span data-ttu-id="ac607-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="ac607-127">notApplicableCount</span></span>|<span data-ttu-id="ac607-128">Int32</span><span class="sxs-lookup"><span data-stu-id="ac607-128">Int32</span></span>|<span data-ttu-id="ac607-129">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="ac607-129">Number of not applicable devices</span></span>|
|<span data-ttu-id="ac607-130">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="ac607-130">notApplicablePlatformCount</span></span>|<span data-ttu-id="ac607-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ac607-131">Int32</span></span>|<span data-ttu-id="ac607-132">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="ac607-132">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="ac607-133">successCount</span><span class="sxs-lookup"><span data-stu-id="ac607-133">successCount</span></span>|<span data-ttu-id="ac607-134">Int32</span><span class="sxs-lookup"><span data-stu-id="ac607-134">Int32</span></span>|<span data-ttu-id="ac607-135">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="ac607-135">Number of succeeded devices</span></span>|
|<span data-ttu-id="ac607-136">errorCount</span><span class="sxs-lookup"><span data-stu-id="ac607-136">errorCount</span></span>|<span data-ttu-id="ac607-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ac607-137">Int32</span></span>|<span data-ttu-id="ac607-138">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="ac607-138">Number of error devices</span></span>|
|<span data-ttu-id="ac607-139">failedCount</span><span class="sxs-lookup"><span data-stu-id="ac607-139">failedCount</span></span>|<span data-ttu-id="ac607-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ac607-140">Int32</span></span>|<span data-ttu-id="ac607-141">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="ac607-141">Number of failed devices</span></span>|
|<span data-ttu-id="ac607-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="ac607-142">conflictCount</span></span>|<span data-ttu-id="ac607-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ac607-143">Int32</span></span>|<span data-ttu-id="ac607-144">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="ac607-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="ac607-145">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="ac607-145">lastUpdateDateTime</span></span>|<span data-ttu-id="ac607-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac607-146">DateTimeOffset</span></span>|<span data-ttu-id="ac607-147">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="ac607-147">Last update time</span></span>|
|<span data-ttu-id="ac607-148">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="ac607-148">configurationVersion</span></span>|<span data-ttu-id="ac607-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ac607-149">Int32</span></span>|<span data-ttu-id="ac607-150">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="ac607-150">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac607-151">关系</span><span class="sxs-lookup"><span data-stu-id="ac607-151">Relationships</span></span>
<span data-ttu-id="ac607-152">无</span><span class="sxs-lookup"><span data-stu-id="ac607-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac607-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac607-153">JSON Representation</span></span>
<span data-ttu-id="ac607-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac607-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
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




