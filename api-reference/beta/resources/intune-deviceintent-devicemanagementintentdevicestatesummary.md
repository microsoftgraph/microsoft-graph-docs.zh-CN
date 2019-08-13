---
title: deviceManagementIntentDeviceStateSummary 资源类型
description: 表示意向的设备状态摘要的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d4dcbad68d83978d269108b2a9a1b18a246e0039
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371416"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a><span data-ttu-id="3e65e-103">deviceManagementIntentDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e65e-103">deviceManagementIntentDeviceStateSummary resource type</span></span>

> <span data-ttu-id="3e65e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e65e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e65e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e65e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e65e-106">表示意向的设备状态摘要的实体</span><span class="sxs-lookup"><span data-stu-id="3e65e-106">Entity that represents device state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="3e65e-107">方法</span><span class="sxs-lookup"><span data-stu-id="3e65e-107">Methods</span></span>
|<span data-ttu-id="3e65e-108">方法</span><span class="sxs-lookup"><span data-stu-id="3e65e-108">Method</span></span>|<span data-ttu-id="3e65e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3e65e-109">Return Type</span></span>|<span data-ttu-id="3e65e-110">说明</span><span class="sxs-lookup"><span data-stu-id="3e65e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3e65e-111">获取 deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="3e65e-111">Get deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[<span data-ttu-id="3e65e-112">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="3e65e-112">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="3e65e-113">读取[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e65e-113">Read properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="3e65e-114">更新 deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="3e65e-114">Update deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[<span data-ttu-id="3e65e-115">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="3e65e-115">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="3e65e-116">更新[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3e65e-116">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3e65e-117">属性</span><span class="sxs-lookup"><span data-stu-id="3e65e-117">Properties</span></span>
|<span data-ttu-id="3e65e-118">属性</span><span class="sxs-lookup"><span data-stu-id="3e65e-118">Property</span></span>|<span data-ttu-id="3e65e-119">类型</span><span class="sxs-lookup"><span data-stu-id="3e65e-119">Type</span></span>|<span data-ttu-id="3e65e-120">说明</span><span class="sxs-lookup"><span data-stu-id="3e65e-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e65e-121">id</span><span class="sxs-lookup"><span data-stu-id="3e65e-121">id</span></span>|<span data-ttu-id="3e65e-122">String</span><span class="sxs-lookup"><span data-stu-id="3e65e-122">String</span></span>|<span data-ttu-id="3e65e-123">ID</span><span class="sxs-lookup"><span data-stu-id="3e65e-123">The ID</span></span>|
|<span data-ttu-id="3e65e-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="3e65e-124">conflictCount</span></span>|<span data-ttu-id="3e65e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="3e65e-125">Int32</span></span>|<span data-ttu-id="3e65e-126">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="3e65e-126">Number of devices in conflict</span></span>|
|<span data-ttu-id="3e65e-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="3e65e-127">errorCount</span></span>|<span data-ttu-id="3e65e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="3e65e-128">Int32</span></span>|<span data-ttu-id="3e65e-129">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="3e65e-129">Number of error devices</span></span>|
|<span data-ttu-id="3e65e-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="3e65e-130">failedCount</span></span>|<span data-ttu-id="3e65e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="3e65e-131">Int32</span></span>|<span data-ttu-id="3e65e-132">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="3e65e-132">Number of failed devices</span></span>|
|<span data-ttu-id="3e65e-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="3e65e-133">notApplicableCount</span></span>|<span data-ttu-id="3e65e-134">Int32</span><span class="sxs-lookup"><span data-stu-id="3e65e-134">Int32</span></span>|<span data-ttu-id="3e65e-135">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="3e65e-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="3e65e-136">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="3e65e-136">notApplicablePlatformCount</span></span>|<span data-ttu-id="3e65e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3e65e-137">Int32</span></span>|<span data-ttu-id="3e65e-138">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="3e65e-138">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="3e65e-139">successCount</span><span class="sxs-lookup"><span data-stu-id="3e65e-139">successCount</span></span>|<span data-ttu-id="3e65e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3e65e-140">Int32</span></span>|<span data-ttu-id="3e65e-141">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="3e65e-141">Number of succeeded devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e65e-142">关系</span><span class="sxs-lookup"><span data-stu-id="3e65e-142">Relationships</span></span>
<span data-ttu-id="3e65e-143">无</span><span class="sxs-lookup"><span data-stu-id="3e65e-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e65e-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e65e-144">JSON Representation</span></span>
<span data-ttu-id="3e65e-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e65e-145">Here is a JSON representation of the resource.</span></span>
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



