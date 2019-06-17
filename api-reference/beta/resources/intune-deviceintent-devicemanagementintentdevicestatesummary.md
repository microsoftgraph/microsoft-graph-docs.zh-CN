---
title: deviceManagementIntentDeviceStateSummary 资源类型
description: 表示意向的设备状态摘要的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72ba65c7b23310a6fb3883bd72579ce838471f4f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964092"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a><span data-ttu-id="9c629-103">deviceManagementIntentDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="9c629-103">deviceManagementIntentDeviceStateSummary resource type</span></span>

> <span data-ttu-id="9c629-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c629-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c629-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c629-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c629-106">表示意向的设备状态摘要的实体</span><span class="sxs-lookup"><span data-stu-id="9c629-106">Entity that represents device state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="9c629-107">方法</span><span class="sxs-lookup"><span data-stu-id="9c629-107">Methods</span></span>
|<span data-ttu-id="9c629-108">方法</span><span class="sxs-lookup"><span data-stu-id="9c629-108">Method</span></span>|<span data-ttu-id="9c629-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9c629-109">Return Type</span></span>|<span data-ttu-id="9c629-110">说明</span><span class="sxs-lookup"><span data-stu-id="9c629-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9c629-111">获取 deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9c629-111">Get deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[<span data-ttu-id="9c629-112">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9c629-112">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="9c629-113">读取[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9c629-113">Read properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="9c629-114">更新 deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9c629-114">Update deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[<span data-ttu-id="9c629-115">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9c629-115">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="9c629-116">更新[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9c629-116">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9c629-117">属性</span><span class="sxs-lookup"><span data-stu-id="9c629-117">Properties</span></span>
|<span data-ttu-id="9c629-118">属性</span><span class="sxs-lookup"><span data-stu-id="9c629-118">Property</span></span>|<span data-ttu-id="9c629-119">类型</span><span class="sxs-lookup"><span data-stu-id="9c629-119">Type</span></span>|<span data-ttu-id="9c629-120">说明</span><span class="sxs-lookup"><span data-stu-id="9c629-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c629-121">id</span><span class="sxs-lookup"><span data-stu-id="9c629-121">id</span></span>|<span data-ttu-id="9c629-122">String</span><span class="sxs-lookup"><span data-stu-id="9c629-122">String</span></span>|<span data-ttu-id="9c629-123">ID</span><span class="sxs-lookup"><span data-stu-id="9c629-123">The ID</span></span>|
|<span data-ttu-id="9c629-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="9c629-124">conflictCount</span></span>|<span data-ttu-id="9c629-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9c629-125">Int32</span></span>|<span data-ttu-id="9c629-126">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="9c629-126">Number of devices in conflict</span></span>|
|<span data-ttu-id="9c629-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="9c629-127">errorCount</span></span>|<span data-ttu-id="9c629-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9c629-128">Int32</span></span>|<span data-ttu-id="9c629-129">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="9c629-129">Number of error devices</span></span>|
|<span data-ttu-id="9c629-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="9c629-130">failedCount</span></span>|<span data-ttu-id="9c629-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9c629-131">Int32</span></span>|<span data-ttu-id="9c629-132">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="9c629-132">Number of failed devices</span></span>|
|<span data-ttu-id="9c629-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="9c629-133">notApplicableCount</span></span>|<span data-ttu-id="9c629-134">Int32</span><span class="sxs-lookup"><span data-stu-id="9c629-134">Int32</span></span>|<span data-ttu-id="9c629-135">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="9c629-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="9c629-136">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="9c629-136">notApplicablePlatformCount</span></span>|<span data-ttu-id="9c629-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9c629-137">Int32</span></span>|<span data-ttu-id="9c629-138">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="9c629-138">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="9c629-139">successCount</span><span class="sxs-lookup"><span data-stu-id="9c629-139">successCount</span></span>|<span data-ttu-id="9c629-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9c629-140">Int32</span></span>|<span data-ttu-id="9c629-141">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="9c629-141">Number of succeeded devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c629-142">关系</span><span class="sxs-lookup"><span data-stu-id="9c629-142">Relationships</span></span>
<span data-ttu-id="9c629-143">无</span><span class="sxs-lookup"><span data-stu-id="9c629-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c629-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c629-144">JSON Representation</span></span>
<span data-ttu-id="9c629-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c629-145">Here is a JSON representation of the resource.</span></span>
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





