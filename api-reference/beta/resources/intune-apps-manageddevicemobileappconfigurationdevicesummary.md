---
title: managedDeviceMobileAppConfigurationDeviceSummary 资源类型
description: 包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 64755b1e311f04dc33d41afa8a196a6bb860dfab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052815"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="50b18-103">managedDeviceMobileAppConfigurationDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="50b18-103">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

<span data-ttu-id="50b18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50b18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50b18-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="50b18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50b18-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="50b18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50b18-107">包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="50b18-107">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="50b18-108">方法</span><span class="sxs-lookup"><span data-stu-id="50b18-108">Methods</span></span>
|<span data-ttu-id="50b18-109">方法</span><span class="sxs-lookup"><span data-stu-id="50b18-109">Method</span></span>|<span data-ttu-id="50b18-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="50b18-110">Return Type</span></span>|<span data-ttu-id="50b18-111">说明</span><span class="sxs-lookup"><span data-stu-id="50b18-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="50b18-112">获取 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="50b18-112">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[<span data-ttu-id="50b18-113">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="50b18-113">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="50b18-114">读取 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="50b18-114">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="50b18-115">更新 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="50b18-115">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[<span data-ttu-id="50b18-116">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="50b18-116">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="50b18-117">更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="50b18-117">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="50b18-118">属性</span><span class="sxs-lookup"><span data-stu-id="50b18-118">Properties</span></span>
|<span data-ttu-id="50b18-119">属性</span><span class="sxs-lookup"><span data-stu-id="50b18-119">Property</span></span>|<span data-ttu-id="50b18-120">类型</span><span class="sxs-lookup"><span data-stu-id="50b18-120">Type</span></span>|<span data-ttu-id="50b18-121">说明</span><span class="sxs-lookup"><span data-stu-id="50b18-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50b18-122">id</span><span class="sxs-lookup"><span data-stu-id="50b18-122">id</span></span>|<span data-ttu-id="50b18-123">String</span><span class="sxs-lookup"><span data-stu-id="50b18-123">String</span></span>|<span data-ttu-id="50b18-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="50b18-124">Key of the entity.</span></span>|
|<span data-ttu-id="50b18-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="50b18-125">pendingCount</span></span>|<span data-ttu-id="50b18-126">Int32</span><span class="sxs-lookup"><span data-stu-id="50b18-126">Int32</span></span>|<span data-ttu-id="50b18-127">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="50b18-127">Number of pending devices</span></span>|
|<span data-ttu-id="50b18-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="50b18-128">notApplicableCount</span></span>|<span data-ttu-id="50b18-129">Int32</span><span class="sxs-lookup"><span data-stu-id="50b18-129">Int32</span></span>|<span data-ttu-id="50b18-130">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="50b18-130">Number of not applicable devices</span></span>|
|<span data-ttu-id="50b18-131">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="50b18-131">notApplicablePlatformCount</span></span>|<span data-ttu-id="50b18-132">Int32</span><span class="sxs-lookup"><span data-stu-id="50b18-132">Int32</span></span>|<span data-ttu-id="50b18-133">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="50b18-133">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="50b18-134">successCount</span><span class="sxs-lookup"><span data-stu-id="50b18-134">successCount</span></span>|<span data-ttu-id="50b18-135">Int32</span><span class="sxs-lookup"><span data-stu-id="50b18-135">Int32</span></span>|<span data-ttu-id="50b18-136">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="50b18-136">Number of succeeded devices</span></span>|
|<span data-ttu-id="50b18-137">errorCount</span><span class="sxs-lookup"><span data-stu-id="50b18-137">errorCount</span></span>|<span data-ttu-id="50b18-138">Int32</span><span class="sxs-lookup"><span data-stu-id="50b18-138">Int32</span></span>|<span data-ttu-id="50b18-139">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="50b18-139">Number of error devices</span></span>|
|<span data-ttu-id="50b18-140">failedCount</span><span class="sxs-lookup"><span data-stu-id="50b18-140">failedCount</span></span>|<span data-ttu-id="50b18-141">Int32</span><span class="sxs-lookup"><span data-stu-id="50b18-141">Int32</span></span>|<span data-ttu-id="50b18-142">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="50b18-142">Number of failed devices</span></span>|
|<span data-ttu-id="50b18-143">conflictCount</span><span class="sxs-lookup"><span data-stu-id="50b18-143">conflictCount</span></span>|<span data-ttu-id="50b18-144">Int32</span><span class="sxs-lookup"><span data-stu-id="50b18-144">Int32</span></span>|<span data-ttu-id="50b18-145">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="50b18-145">Number of devices in conflict</span></span>|
|<span data-ttu-id="50b18-146">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="50b18-146">lastUpdateDateTime</span></span>|<span data-ttu-id="50b18-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50b18-147">DateTimeOffset</span></span>|<span data-ttu-id="50b18-148">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="50b18-148">Last update time</span></span>|
|<span data-ttu-id="50b18-149">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="50b18-149">configurationVersion</span></span>|<span data-ttu-id="50b18-150">Int32</span><span class="sxs-lookup"><span data-stu-id="50b18-150">Int32</span></span>|<span data-ttu-id="50b18-151">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="50b18-151">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="50b18-152">关系</span><span class="sxs-lookup"><span data-stu-id="50b18-152">Relationships</span></span>
<span data-ttu-id="50b18-153">无</span><span class="sxs-lookup"><span data-stu-id="50b18-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50b18-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50b18-154">JSON Representation</span></span>
<span data-ttu-id="50b18-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50b18-155">Here is a JSON representation of the resource.</span></span>
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






