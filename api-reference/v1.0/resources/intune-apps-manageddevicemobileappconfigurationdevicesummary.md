---
title: managedDeviceMobileAppConfigurationDeviceSummary 资源类型
description: 包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: baa3804fe4a26a0f1ce349c59918a981c819c56a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752236"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="71618-103">managedDeviceMobileAppConfigurationDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="71618-103">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

<span data-ttu-id="71618-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71618-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71618-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71618-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71618-106">包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="71618-106">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="71618-107">Methods</span><span class="sxs-lookup"><span data-stu-id="71618-107">Methods</span></span>
|<span data-ttu-id="71618-108">方法</span><span class="sxs-lookup"><span data-stu-id="71618-108">Method</span></span>|<span data-ttu-id="71618-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="71618-109">Return Type</span></span>|<span data-ttu-id="71618-110">Description</span><span class="sxs-lookup"><span data-stu-id="71618-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="71618-111">获取 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="71618-111">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[<span data-ttu-id="71618-112">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="71618-112">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="71618-113">读取 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71618-113">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="71618-114">更新 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="71618-114">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[<span data-ttu-id="71618-115">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="71618-115">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="71618-116">更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="71618-116">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="71618-117">属性</span><span class="sxs-lookup"><span data-stu-id="71618-117">Properties</span></span>
|<span data-ttu-id="71618-118">属性</span><span class="sxs-lookup"><span data-stu-id="71618-118">Property</span></span>|<span data-ttu-id="71618-119">类型</span><span class="sxs-lookup"><span data-stu-id="71618-119">Type</span></span>|<span data-ttu-id="71618-120">说明</span><span class="sxs-lookup"><span data-stu-id="71618-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71618-121">id</span><span class="sxs-lookup"><span data-stu-id="71618-121">id</span></span>|<span data-ttu-id="71618-122">String</span><span class="sxs-lookup"><span data-stu-id="71618-122">String</span></span>|<span data-ttu-id="71618-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="71618-123">Key of the entity.</span></span>|
|<span data-ttu-id="71618-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="71618-124">pendingCount</span></span>|<span data-ttu-id="71618-125">Int32</span><span class="sxs-lookup"><span data-stu-id="71618-125">Int32</span></span>|<span data-ttu-id="71618-126">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="71618-126">Number of pending devices</span></span>|
|<span data-ttu-id="71618-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="71618-127">notApplicableCount</span></span>|<span data-ttu-id="71618-128">Int32</span><span class="sxs-lookup"><span data-stu-id="71618-128">Int32</span></span>|<span data-ttu-id="71618-129">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="71618-129">Number of not applicable devices</span></span>|
|<span data-ttu-id="71618-130">successCount</span><span class="sxs-lookup"><span data-stu-id="71618-130">successCount</span></span>|<span data-ttu-id="71618-131">Int32</span><span class="sxs-lookup"><span data-stu-id="71618-131">Int32</span></span>|<span data-ttu-id="71618-132">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="71618-132">Number of succeeded devices</span></span>|
|<span data-ttu-id="71618-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="71618-133">errorCount</span></span>|<span data-ttu-id="71618-134">Int32</span><span class="sxs-lookup"><span data-stu-id="71618-134">Int32</span></span>|<span data-ttu-id="71618-135">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="71618-135">Number of error devices</span></span>|
|<span data-ttu-id="71618-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="71618-136">failedCount</span></span>|<span data-ttu-id="71618-137">Int32</span><span class="sxs-lookup"><span data-stu-id="71618-137">Int32</span></span>|<span data-ttu-id="71618-138">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="71618-138">Number of failed devices</span></span>|
|<span data-ttu-id="71618-139">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="71618-139">lastUpdateDateTime</span></span>|<span data-ttu-id="71618-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71618-140">DateTimeOffset</span></span>|<span data-ttu-id="71618-141">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="71618-141">Last update time</span></span>|
|<span data-ttu-id="71618-142">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="71618-142">configurationVersion</span></span>|<span data-ttu-id="71618-143">Int32</span><span class="sxs-lookup"><span data-stu-id="71618-143">Int32</span></span>|<span data-ttu-id="71618-144">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="71618-144">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="71618-145">关系</span><span class="sxs-lookup"><span data-stu-id="71618-145">Relationships</span></span>
<span data-ttu-id="71618-146">无</span><span class="sxs-lookup"><span data-stu-id="71618-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71618-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71618-147">JSON Representation</span></span>
<span data-ttu-id="71618-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71618-148">Here is a JSON representation of the resource.</span></span>
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




