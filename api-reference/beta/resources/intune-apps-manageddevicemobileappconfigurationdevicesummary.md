---
title: managedDeviceMobileAppConfigurationDeviceSummary 资源类型
description: 包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 361ac12dc78e87490c227a6720e2ec7e0d5de3b6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42492402"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="06c02-103">managedDeviceMobileAppConfigurationDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="06c02-103">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

<span data-ttu-id="06c02-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="06c02-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06c02-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="06c02-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06c02-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06c02-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06c02-107">包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="06c02-107">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="06c02-108">方法</span><span class="sxs-lookup"><span data-stu-id="06c02-108">Methods</span></span>
|<span data-ttu-id="06c02-109">方法</span><span class="sxs-lookup"><span data-stu-id="06c02-109">Method</span></span>|<span data-ttu-id="06c02-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="06c02-110">Return Type</span></span>|<span data-ttu-id="06c02-111">说明</span><span class="sxs-lookup"><span data-stu-id="06c02-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06c02-112">获取 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="06c02-112">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[<span data-ttu-id="06c02-113">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="06c02-113">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="06c02-114">读取 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06c02-114">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="06c02-115">更新 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="06c02-115">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[<span data-ttu-id="06c02-116">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="06c02-116">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="06c02-117">更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="06c02-117">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06c02-118">属性</span><span class="sxs-lookup"><span data-stu-id="06c02-118">Properties</span></span>
|<span data-ttu-id="06c02-119">属性</span><span class="sxs-lookup"><span data-stu-id="06c02-119">Property</span></span>|<span data-ttu-id="06c02-120">类型</span><span class="sxs-lookup"><span data-stu-id="06c02-120">Type</span></span>|<span data-ttu-id="06c02-121">说明</span><span class="sxs-lookup"><span data-stu-id="06c02-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06c02-122">id</span><span class="sxs-lookup"><span data-stu-id="06c02-122">id</span></span>|<span data-ttu-id="06c02-123">String</span><span class="sxs-lookup"><span data-stu-id="06c02-123">String</span></span>|<span data-ttu-id="06c02-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="06c02-124">Key of the entity.</span></span>|
|<span data-ttu-id="06c02-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="06c02-125">pendingCount</span></span>|<span data-ttu-id="06c02-126">Int32</span><span class="sxs-lookup"><span data-stu-id="06c02-126">Int32</span></span>|<span data-ttu-id="06c02-127">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="06c02-127">Number of pending devices</span></span>|
|<span data-ttu-id="06c02-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="06c02-128">notApplicableCount</span></span>|<span data-ttu-id="06c02-129">Int32</span><span class="sxs-lookup"><span data-stu-id="06c02-129">Int32</span></span>|<span data-ttu-id="06c02-130">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="06c02-130">Number of not applicable devices</span></span>|
|<span data-ttu-id="06c02-131">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="06c02-131">notApplicablePlatformCount</span></span>|<span data-ttu-id="06c02-132">Int32</span><span class="sxs-lookup"><span data-stu-id="06c02-132">Int32</span></span>|<span data-ttu-id="06c02-133">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="06c02-133">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="06c02-134">successCount</span><span class="sxs-lookup"><span data-stu-id="06c02-134">successCount</span></span>|<span data-ttu-id="06c02-135">Int32</span><span class="sxs-lookup"><span data-stu-id="06c02-135">Int32</span></span>|<span data-ttu-id="06c02-136">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="06c02-136">Number of succeeded devices</span></span>|
|<span data-ttu-id="06c02-137">errorCount</span><span class="sxs-lookup"><span data-stu-id="06c02-137">errorCount</span></span>|<span data-ttu-id="06c02-138">Int32</span><span class="sxs-lookup"><span data-stu-id="06c02-138">Int32</span></span>|<span data-ttu-id="06c02-139">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="06c02-139">Number of error devices</span></span>|
|<span data-ttu-id="06c02-140">failedCount</span><span class="sxs-lookup"><span data-stu-id="06c02-140">failedCount</span></span>|<span data-ttu-id="06c02-141">Int32</span><span class="sxs-lookup"><span data-stu-id="06c02-141">Int32</span></span>|<span data-ttu-id="06c02-142">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="06c02-142">Number of failed devices</span></span>|
|<span data-ttu-id="06c02-143">conflictCount</span><span class="sxs-lookup"><span data-stu-id="06c02-143">conflictCount</span></span>|<span data-ttu-id="06c02-144">Int32</span><span class="sxs-lookup"><span data-stu-id="06c02-144">Int32</span></span>|<span data-ttu-id="06c02-145">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="06c02-145">Number of devices in conflict</span></span>|
|<span data-ttu-id="06c02-146">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="06c02-146">lastUpdateDateTime</span></span>|<span data-ttu-id="06c02-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06c02-147">DateTimeOffset</span></span>|<span data-ttu-id="06c02-148">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="06c02-148">Last update time</span></span>|
|<span data-ttu-id="06c02-149">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="06c02-149">configurationVersion</span></span>|<span data-ttu-id="06c02-150">Int32</span><span class="sxs-lookup"><span data-stu-id="06c02-150">Int32</span></span>|<span data-ttu-id="06c02-151">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="06c02-151">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="06c02-152">关系</span><span class="sxs-lookup"><span data-stu-id="06c02-152">Relationships</span></span>
<span data-ttu-id="06c02-153">无</span><span class="sxs-lookup"><span data-stu-id="06c02-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06c02-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06c02-154">JSON Representation</span></span>
<span data-ttu-id="06c02-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06c02-155">Here is a JSON representation of the resource.</span></span>
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



