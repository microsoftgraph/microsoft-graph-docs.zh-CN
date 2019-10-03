---
title: managedDeviceMobileAppConfigurationDeviceSummary 资源类型
description: 包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6aaf2ff42c59a983bf73bd866374fa731cec7b83
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368223"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="a8554-103">managedDeviceMobileAppConfigurationDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8554-103">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="a8554-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a8554-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8554-105">包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="a8554-105">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="a8554-106">方法</span><span class="sxs-lookup"><span data-stu-id="a8554-106">Methods</span></span>
|<span data-ttu-id="a8554-107">方法</span><span class="sxs-lookup"><span data-stu-id="a8554-107">Method</span></span>|<span data-ttu-id="a8554-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a8554-108">Return Type</span></span>|<span data-ttu-id="a8554-109">说明</span><span class="sxs-lookup"><span data-stu-id="a8554-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a8554-110">获取 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a8554-110">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[<span data-ttu-id="a8554-111">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a8554-111">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="a8554-112">读取 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a8554-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="a8554-113">更新 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a8554-113">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[<span data-ttu-id="a8554-114">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a8554-114">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="a8554-115">更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a8554-115">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a8554-116">属性</span><span class="sxs-lookup"><span data-stu-id="a8554-116">Properties</span></span>
|<span data-ttu-id="a8554-117">属性</span><span class="sxs-lookup"><span data-stu-id="a8554-117">Property</span></span>|<span data-ttu-id="a8554-118">类型</span><span class="sxs-lookup"><span data-stu-id="a8554-118">Type</span></span>|<span data-ttu-id="a8554-119">说明</span><span class="sxs-lookup"><span data-stu-id="a8554-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8554-120">id</span><span class="sxs-lookup"><span data-stu-id="a8554-120">id</span></span>|<span data-ttu-id="a8554-121">String</span><span class="sxs-lookup"><span data-stu-id="a8554-121">String</span></span>|<span data-ttu-id="a8554-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a8554-122">Key of the entity.</span></span>|
|<span data-ttu-id="a8554-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="a8554-123">pendingCount</span></span>|<span data-ttu-id="a8554-124">Int32</span><span class="sxs-lookup"><span data-stu-id="a8554-124">Int32</span></span>|<span data-ttu-id="a8554-125">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="a8554-125">Number of pending devices</span></span>|
|<span data-ttu-id="a8554-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="a8554-126">notApplicableCount</span></span>|<span data-ttu-id="a8554-127">Int32</span><span class="sxs-lookup"><span data-stu-id="a8554-127">Int32</span></span>|<span data-ttu-id="a8554-128">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="a8554-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="a8554-129">successCount</span><span class="sxs-lookup"><span data-stu-id="a8554-129">successCount</span></span>|<span data-ttu-id="a8554-130">Int32</span><span class="sxs-lookup"><span data-stu-id="a8554-130">Int32</span></span>|<span data-ttu-id="a8554-131">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="a8554-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="a8554-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="a8554-132">errorCount</span></span>|<span data-ttu-id="a8554-133">Int32</span><span class="sxs-lookup"><span data-stu-id="a8554-133">Int32</span></span>|<span data-ttu-id="a8554-134">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="a8554-134">Number of error devices</span></span>|
|<span data-ttu-id="a8554-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="a8554-135">failedCount</span></span>|<span data-ttu-id="a8554-136">Int32</span><span class="sxs-lookup"><span data-stu-id="a8554-136">Int32</span></span>|<span data-ttu-id="a8554-137">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="a8554-137">Number of failed devices</span></span>|
|<span data-ttu-id="a8554-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a8554-138">lastUpdateDateTime</span></span>|<span data-ttu-id="a8554-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8554-139">DateTimeOffset</span></span>|<span data-ttu-id="a8554-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="a8554-140">Last update time</span></span>|
|<span data-ttu-id="a8554-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="a8554-141">configurationVersion</span></span>|<span data-ttu-id="a8554-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a8554-142">Int32</span></span>|<span data-ttu-id="a8554-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="a8554-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8554-144">关系</span><span class="sxs-lookup"><span data-stu-id="a8554-144">Relationships</span></span>
<span data-ttu-id="a8554-145">无</span><span class="sxs-lookup"><span data-stu-id="a8554-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8554-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8554-146">JSON Representation</span></span>
<span data-ttu-id="a8554-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8554-147">Here is a JSON representation of the resource.</span></span>
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




