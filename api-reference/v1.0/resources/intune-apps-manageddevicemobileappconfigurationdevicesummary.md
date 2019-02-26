---
title: managedDeviceMobileAppConfigurationDeviceSummary 资源类型
description: 包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e62d02b5b702b56d72a0c75f9e5da1f6ad9dbdc3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259638"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="09b89-103">managedDeviceMobileAppConfigurationDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="09b89-103">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="09b89-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09b89-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09b89-105">包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="09b89-105">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="09b89-106">方法</span><span class="sxs-lookup"><span data-stu-id="09b89-106">Methods</span></span>
|<span data-ttu-id="09b89-107">方法</span><span class="sxs-lookup"><span data-stu-id="09b89-107">Method</span></span>|<span data-ttu-id="09b89-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="09b89-108">Return Type</span></span>|<span data-ttu-id="09b89-109">说明</span><span class="sxs-lookup"><span data-stu-id="09b89-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="09b89-110">获取 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="09b89-110">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[<span data-ttu-id="09b89-111">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="09b89-111">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="09b89-112">读取 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="09b89-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="09b89-113">更新 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="09b89-113">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[<span data-ttu-id="09b89-114">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="09b89-114">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="09b89-115">更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="09b89-115">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="09b89-116">属性</span><span class="sxs-lookup"><span data-stu-id="09b89-116">Properties</span></span>
|<span data-ttu-id="09b89-117">属性</span><span class="sxs-lookup"><span data-stu-id="09b89-117">Property</span></span>|<span data-ttu-id="09b89-118">类型</span><span class="sxs-lookup"><span data-stu-id="09b89-118">Type</span></span>|<span data-ttu-id="09b89-119">说明</span><span class="sxs-lookup"><span data-stu-id="09b89-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09b89-120">id</span><span class="sxs-lookup"><span data-stu-id="09b89-120">id</span></span>|<span data-ttu-id="09b89-121">String</span><span class="sxs-lookup"><span data-stu-id="09b89-121">String</span></span>|<span data-ttu-id="09b89-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="09b89-122">Key of the entity.</span></span>|
|<span data-ttu-id="09b89-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="09b89-123">pendingCount</span></span>|<span data-ttu-id="09b89-124">Int32</span><span class="sxs-lookup"><span data-stu-id="09b89-124">Int32</span></span>|<span data-ttu-id="09b89-125">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="09b89-125">Number of pending devices</span></span>|
|<span data-ttu-id="09b89-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="09b89-126">notApplicableCount</span></span>|<span data-ttu-id="09b89-127">Int32</span><span class="sxs-lookup"><span data-stu-id="09b89-127">Int32</span></span>|<span data-ttu-id="09b89-128">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="09b89-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="09b89-129">successCount</span><span class="sxs-lookup"><span data-stu-id="09b89-129">successCount</span></span>|<span data-ttu-id="09b89-130">Int32</span><span class="sxs-lookup"><span data-stu-id="09b89-130">Int32</span></span>|<span data-ttu-id="09b89-131">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="09b89-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="09b89-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="09b89-132">errorCount</span></span>|<span data-ttu-id="09b89-133">Int32</span><span class="sxs-lookup"><span data-stu-id="09b89-133">Int32</span></span>|<span data-ttu-id="09b89-134">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="09b89-134">Number of error devices</span></span>|
|<span data-ttu-id="09b89-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="09b89-135">failedCount</span></span>|<span data-ttu-id="09b89-136">Int32</span><span class="sxs-lookup"><span data-stu-id="09b89-136">Int32</span></span>|<span data-ttu-id="09b89-137">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="09b89-137">Number of failed devices</span></span>|
|<span data-ttu-id="09b89-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="09b89-138">lastUpdateDateTime</span></span>|<span data-ttu-id="09b89-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09b89-139">DateTimeOffset</span></span>|<span data-ttu-id="09b89-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="09b89-140">Last update time</span></span>|
|<span data-ttu-id="09b89-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="09b89-141">configurationVersion</span></span>|<span data-ttu-id="09b89-142">Int32</span><span class="sxs-lookup"><span data-stu-id="09b89-142">Int32</span></span>|<span data-ttu-id="09b89-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="09b89-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="09b89-144">关系</span><span class="sxs-lookup"><span data-stu-id="09b89-144">Relationships</span></span>
<span data-ttu-id="09b89-145">无</span><span class="sxs-lookup"><span data-stu-id="09b89-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09b89-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09b89-146">JSON Representation</span></span>
<span data-ttu-id="09b89-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09b89-147">Here is a JSON representation of the resource.</span></span>
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
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



