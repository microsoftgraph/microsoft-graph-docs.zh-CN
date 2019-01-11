---
title: managedDeviceMobileAppConfigurationDeviceSummary 资源类型
description: 包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。
localization_priority: Normal
ms.openlocfilehash: 47a323a074bd42d1e075a2a5ddd6aeb9181c98eb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816343"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="6736e-103">managedDeviceMobileAppConfigurationDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="6736e-103">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="6736e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6736e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6736e-105">包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="6736e-105">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="6736e-106">方法</span><span class="sxs-lookup"><span data-stu-id="6736e-106">Methods</span></span>
|<span data-ttu-id="6736e-107">方法</span><span class="sxs-lookup"><span data-stu-id="6736e-107">Method</span></span>|<span data-ttu-id="6736e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6736e-108">Return Type</span></span>|<span data-ttu-id="6736e-109">说明</span><span class="sxs-lookup"><span data-stu-id="6736e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6736e-110">获取 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6736e-110">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[<span data-ttu-id="6736e-111">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6736e-111">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="6736e-112">读取 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6736e-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="6736e-113">更新 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6736e-113">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[<span data-ttu-id="6736e-114">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6736e-114">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="6736e-115">更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6736e-115">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6736e-116">属性</span><span class="sxs-lookup"><span data-stu-id="6736e-116">Properties</span></span>
|<span data-ttu-id="6736e-117">属性</span><span class="sxs-lookup"><span data-stu-id="6736e-117">Property</span></span>|<span data-ttu-id="6736e-118">类型</span><span class="sxs-lookup"><span data-stu-id="6736e-118">Type</span></span>|<span data-ttu-id="6736e-119">说明</span><span class="sxs-lookup"><span data-stu-id="6736e-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6736e-120">id</span><span class="sxs-lookup"><span data-stu-id="6736e-120">id</span></span>|<span data-ttu-id="6736e-121">String</span><span class="sxs-lookup"><span data-stu-id="6736e-121">String</span></span>|<span data-ttu-id="6736e-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6736e-122">Key of the entity.</span></span>|
|<span data-ttu-id="6736e-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="6736e-123">pendingCount</span></span>|<span data-ttu-id="6736e-124">Int32</span><span class="sxs-lookup"><span data-stu-id="6736e-124">Int32</span></span>|<span data-ttu-id="6736e-125">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="6736e-125">Number of pending devices</span></span>|
|<span data-ttu-id="6736e-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="6736e-126">notApplicableCount</span></span>|<span data-ttu-id="6736e-127">Int32</span><span class="sxs-lookup"><span data-stu-id="6736e-127">Int32</span></span>|<span data-ttu-id="6736e-128">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="6736e-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="6736e-129">successCount</span><span class="sxs-lookup"><span data-stu-id="6736e-129">successCount</span></span>|<span data-ttu-id="6736e-130">Int32</span><span class="sxs-lookup"><span data-stu-id="6736e-130">Int32</span></span>|<span data-ttu-id="6736e-131">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="6736e-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="6736e-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="6736e-132">errorCount</span></span>|<span data-ttu-id="6736e-133">Int32</span><span class="sxs-lookup"><span data-stu-id="6736e-133">Int32</span></span>|<span data-ttu-id="6736e-134">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="6736e-134">Number of error devices</span></span>|
|<span data-ttu-id="6736e-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="6736e-135">failedCount</span></span>|<span data-ttu-id="6736e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6736e-136">Int32</span></span>|<span data-ttu-id="6736e-137">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="6736e-137">Number of failed devices</span></span>|
|<span data-ttu-id="6736e-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="6736e-138">lastUpdateDateTime</span></span>|<span data-ttu-id="6736e-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6736e-139">DateTimeOffset</span></span>|<span data-ttu-id="6736e-140">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="6736e-140">Last update time</span></span>|
|<span data-ttu-id="6736e-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="6736e-141">configurationVersion</span></span>|<span data-ttu-id="6736e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6736e-142">Int32</span></span>|<span data-ttu-id="6736e-143">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="6736e-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="6736e-144">关系</span><span class="sxs-lookup"><span data-stu-id="6736e-144">Relationships</span></span>
<span data-ttu-id="6736e-145">无</span><span class="sxs-lookup"><span data-stu-id="6736e-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6736e-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6736e-146">JSON Representation</span></span>
<span data-ttu-id="6736e-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6736e-147">Here is a JSON representation of the resource.</span></span>
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



