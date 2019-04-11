---
title: deviceManagementIntentDeviceStateSummary 资源类型
description: 表示意向的设备状态摘要的实体
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f78f35a11241b5bf0376816827e79c6b1cc3e7bf
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805857"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a><span data-ttu-id="c2f86-103">deviceManagementIntentDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2f86-103">deviceManagementIntentDeviceStateSummary resource type</span></span>

> <span data-ttu-id="c2f86-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c2f86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2f86-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c2f86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2f86-106">表示意向的设备状态摘要的实体</span><span class="sxs-lookup"><span data-stu-id="c2f86-106">Entity that represents device state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="c2f86-107">方法</span><span class="sxs-lookup"><span data-stu-id="c2f86-107">Methods</span></span>
|<span data-ttu-id="c2f86-108">方法</span><span class="sxs-lookup"><span data-stu-id="c2f86-108">Method</span></span>|<span data-ttu-id="c2f86-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c2f86-109">Return Type</span></span>|<span data-ttu-id="c2f86-110">说明</span><span class="sxs-lookup"><span data-stu-id="c2f86-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c2f86-111">获取 deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c2f86-111">Get deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[<span data-ttu-id="c2f86-112">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c2f86-112">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="c2f86-113">读取[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c2f86-113">Read properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="c2f86-114">更新 deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c2f86-114">Update deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[<span data-ttu-id="c2f86-115">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c2f86-115">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="c2f86-116">更新[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c2f86-116">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c2f86-117">属性</span><span class="sxs-lookup"><span data-stu-id="c2f86-117">Properties</span></span>
|<span data-ttu-id="c2f86-118">属性</span><span class="sxs-lookup"><span data-stu-id="c2f86-118">Property</span></span>|<span data-ttu-id="c2f86-119">类型</span><span class="sxs-lookup"><span data-stu-id="c2f86-119">Type</span></span>|<span data-ttu-id="c2f86-120">说明</span><span class="sxs-lookup"><span data-stu-id="c2f86-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2f86-121">id</span><span class="sxs-lookup"><span data-stu-id="c2f86-121">id</span></span>|<span data-ttu-id="c2f86-122">String</span><span class="sxs-lookup"><span data-stu-id="c2f86-122">String</span></span>|<span data-ttu-id="c2f86-123">ID</span><span class="sxs-lookup"><span data-stu-id="c2f86-123">The ID</span></span>|
|<span data-ttu-id="c2f86-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="c2f86-124">conflictCount</span></span>|<span data-ttu-id="c2f86-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c2f86-125">Int32</span></span>|<span data-ttu-id="c2f86-126">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="c2f86-126">Number of devices in conflict</span></span>|
|<span data-ttu-id="c2f86-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="c2f86-127">errorCount</span></span>|<span data-ttu-id="c2f86-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c2f86-128">Int32</span></span>|<span data-ttu-id="c2f86-129">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="c2f86-129">Number of error devices</span></span>|
|<span data-ttu-id="c2f86-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="c2f86-130">failedCount</span></span>|<span data-ttu-id="c2f86-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c2f86-131">Int32</span></span>|<span data-ttu-id="c2f86-132">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="c2f86-132">Number of failed devices</span></span>|
|<span data-ttu-id="c2f86-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="c2f86-133">notApplicableCount</span></span>|<span data-ttu-id="c2f86-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c2f86-134">Int32</span></span>|<span data-ttu-id="c2f86-135">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="c2f86-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="c2f86-136">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="c2f86-136">notApplicablePlatformCount</span></span>|<span data-ttu-id="c2f86-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c2f86-137">Int32</span></span>|<span data-ttu-id="c2f86-138">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="c2f86-138">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="c2f86-139">successCount</span><span class="sxs-lookup"><span data-stu-id="c2f86-139">successCount</span></span>|<span data-ttu-id="c2f86-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c2f86-140">Int32</span></span>|<span data-ttu-id="c2f86-141">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="c2f86-141">Number of succeeded devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2f86-142">关系</span><span class="sxs-lookup"><span data-stu-id="c2f86-142">Relationships</span></span>
<span data-ttu-id="c2f86-143">无</span><span class="sxs-lookup"><span data-stu-id="c2f86-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2f86-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2f86-144">JSON Representation</span></span>
<span data-ttu-id="c2f86-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2f86-145">Here is a JSON representation of the resource.</span></span>
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





