---
title: deviceManagementIntentDeviceStateSummary 资源类型
description: 表示意向的设备状态摘要的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b0b8fda6e7c61d3782374450dc884e2853d9e141
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275795"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a><span data-ttu-id="9da53-103">deviceManagementIntentDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="9da53-103">deviceManagementIntentDeviceStateSummary resource type</span></span>

<span data-ttu-id="9da53-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9da53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9da53-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9da53-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9da53-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9da53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9da53-107">表示意向的设备状态摘要的实体</span><span class="sxs-lookup"><span data-stu-id="9da53-107">Entity that represents device state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="9da53-108">方法</span><span class="sxs-lookup"><span data-stu-id="9da53-108">Methods</span></span>
|<span data-ttu-id="9da53-109">方法</span><span class="sxs-lookup"><span data-stu-id="9da53-109">Method</span></span>|<span data-ttu-id="9da53-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9da53-110">Return Type</span></span>|<span data-ttu-id="9da53-111">说明</span><span class="sxs-lookup"><span data-stu-id="9da53-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9da53-112">获取 deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9da53-112">Get deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[<span data-ttu-id="9da53-113">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9da53-113">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="9da53-114">读取 [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9da53-114">Read properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="9da53-115">更新 deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9da53-115">Update deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[<span data-ttu-id="9da53-116">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9da53-116">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="9da53-117">更新 [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9da53-117">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9da53-118">属性</span><span class="sxs-lookup"><span data-stu-id="9da53-118">Properties</span></span>
|<span data-ttu-id="9da53-119">属性</span><span class="sxs-lookup"><span data-stu-id="9da53-119">Property</span></span>|<span data-ttu-id="9da53-120">类型</span><span class="sxs-lookup"><span data-stu-id="9da53-120">Type</span></span>|<span data-ttu-id="9da53-121">说明</span><span class="sxs-lookup"><span data-stu-id="9da53-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9da53-122">id</span><span class="sxs-lookup"><span data-stu-id="9da53-122">id</span></span>|<span data-ttu-id="9da53-123">字符串</span><span class="sxs-lookup"><span data-stu-id="9da53-123">String</span></span>|<span data-ttu-id="9da53-124">ID</span><span class="sxs-lookup"><span data-stu-id="9da53-124">The ID</span></span>|
|<span data-ttu-id="9da53-125">conflictCount</span><span class="sxs-lookup"><span data-stu-id="9da53-125">conflictCount</span></span>|<span data-ttu-id="9da53-126">Int32</span><span class="sxs-lookup"><span data-stu-id="9da53-126">Int32</span></span>|<span data-ttu-id="9da53-127">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="9da53-127">Number of devices in conflict</span></span>|
|<span data-ttu-id="9da53-128">errorCount</span><span class="sxs-lookup"><span data-stu-id="9da53-128">errorCount</span></span>|<span data-ttu-id="9da53-129">Int32</span><span class="sxs-lookup"><span data-stu-id="9da53-129">Int32</span></span>|<span data-ttu-id="9da53-130">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="9da53-130">Number of error devices</span></span>|
|<span data-ttu-id="9da53-131">failedCount</span><span class="sxs-lookup"><span data-stu-id="9da53-131">failedCount</span></span>|<span data-ttu-id="9da53-132">Int32</span><span class="sxs-lookup"><span data-stu-id="9da53-132">Int32</span></span>|<span data-ttu-id="9da53-133">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="9da53-133">Number of failed devices</span></span>|
|<span data-ttu-id="9da53-134">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="9da53-134">notApplicableCount</span></span>|<span data-ttu-id="9da53-135">Int32</span><span class="sxs-lookup"><span data-stu-id="9da53-135">Int32</span></span>|<span data-ttu-id="9da53-136">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="9da53-136">Number of not applicable devices</span></span>|
|<span data-ttu-id="9da53-137">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="9da53-137">notApplicablePlatformCount</span></span>|<span data-ttu-id="9da53-138">Int32</span><span class="sxs-lookup"><span data-stu-id="9da53-138">Int32</span></span>|<span data-ttu-id="9da53-139">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="9da53-139">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="9da53-140">successCount</span><span class="sxs-lookup"><span data-stu-id="9da53-140">successCount</span></span>|<span data-ttu-id="9da53-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9da53-141">Int32</span></span>|<span data-ttu-id="9da53-142">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="9da53-142">Number of succeeded devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="9da53-143">关系</span><span class="sxs-lookup"><span data-stu-id="9da53-143">Relationships</span></span>
<span data-ttu-id="9da53-144">无</span><span class="sxs-lookup"><span data-stu-id="9da53-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9da53-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9da53-145">JSON Representation</span></span>
<span data-ttu-id="9da53-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9da53-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024
}
```




