---
title: advancedThreatProtectionOnboardingStateSummary 资源类型
description: Windows defender 高级威胁防护在帐户中加入状态摘要。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e4390c765c4f1ed44e034b4554ae2d3137ba121
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175008"
---
# <a name="advancedthreatprotectiononboardingstatesummary-resource-type"></a><span data-ttu-id="94fc6-103">advancedThreatProtectionOnboardingStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="94fc6-103">advancedThreatProtectionOnboardingStateSummary resource type</span></span>

> <span data-ttu-id="94fc6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="94fc6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94fc6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94fc6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94fc6-106">Windows defender 高级威胁防护在帐户中加入状态摘要。</span><span class="sxs-lookup"><span data-stu-id="94fc6-106">Windows defender advanced threat protection onboarding state summary across the account.</span></span>

## <a name="methods"></a><span data-ttu-id="94fc6-107">方法</span><span class="sxs-lookup"><span data-stu-id="94fc6-107">Methods</span></span>
|<span data-ttu-id="94fc6-108">方法</span><span class="sxs-lookup"><span data-stu-id="94fc6-108">Method</span></span>|<span data-ttu-id="94fc6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="94fc6-109">Return Type</span></span>|<span data-ttu-id="94fc6-110">说明</span><span class="sxs-lookup"><span data-stu-id="94fc6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="94fc6-111">获取 advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="94fc6-111">Get advancedThreatProtectionOnboardingStateSummary</span></span>](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-get.md)|[<span data-ttu-id="94fc6-112">advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="94fc6-112">advancedThreatProtectionOnboardingStateSummary</span></span>](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|<span data-ttu-id="94fc6-113">读取[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94fc6-113">Read properties and relationships of the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="94fc6-114">更新 advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="94fc6-114">Update advancedThreatProtectionOnboardingStateSummary</span></span>](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-update.md)|[<span data-ttu-id="94fc6-115">advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="94fc6-115">advancedThreatProtectionOnboardingStateSummary</span></span>](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|<span data-ttu-id="94fc6-116">更新[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94fc6-116">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="94fc6-117">属性</span><span class="sxs-lookup"><span data-stu-id="94fc6-117">Properties</span></span>
|<span data-ttu-id="94fc6-118">属性</span><span class="sxs-lookup"><span data-stu-id="94fc6-118">Property</span></span>|<span data-ttu-id="94fc6-119">类型</span><span class="sxs-lookup"><span data-stu-id="94fc6-119">Type</span></span>|<span data-ttu-id="94fc6-120">说明</span><span class="sxs-lookup"><span data-stu-id="94fc6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94fc6-121">id</span><span class="sxs-lookup"><span data-stu-id="94fc6-121">id</span></span>|<span data-ttu-id="94fc6-122">String</span><span class="sxs-lookup"><span data-stu-id="94fc6-122">String</span></span>|<span data-ttu-id="94fc6-123">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="94fc6-123">Unique Identifier</span></span>|
|<span data-ttu-id="94fc6-124">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94fc6-124">unknownDeviceCount</span></span>|<span data-ttu-id="94fc6-125">Int32</span><span class="sxs-lookup"><span data-stu-id="94fc6-125">Int32</span></span>|<span data-ttu-id="94fc6-126">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="94fc6-126">Number of unknown devices</span></span>|
|<span data-ttu-id="94fc6-127">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94fc6-127">notApplicableDeviceCount</span></span>|<span data-ttu-id="94fc6-128">Int32</span><span class="sxs-lookup"><span data-stu-id="94fc6-128">Int32</span></span>|<span data-ttu-id="94fc6-129">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="94fc6-129">Number of not applicable devices</span></span>|
|<span data-ttu-id="94fc6-130">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94fc6-130">compliantDeviceCount</span></span>|<span data-ttu-id="94fc6-131">Int32</span><span class="sxs-lookup"><span data-stu-id="94fc6-131">Int32</span></span>|<span data-ttu-id="94fc6-132">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="94fc6-132">Number of compliant devices</span></span>|
|<span data-ttu-id="94fc6-133">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94fc6-133">remediatedDeviceCount</span></span>|<span data-ttu-id="94fc6-134">Int32</span><span class="sxs-lookup"><span data-stu-id="94fc6-134">Int32</span></span>|<span data-ttu-id="94fc6-135">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="94fc6-135">Number of remediated devices</span></span>|
|<span data-ttu-id="94fc6-136">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94fc6-136">nonCompliantDeviceCount</span></span>|<span data-ttu-id="94fc6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="94fc6-137">Int32</span></span>|<span data-ttu-id="94fc6-138">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="94fc6-138">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="94fc6-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94fc6-139">errorDeviceCount</span></span>|<span data-ttu-id="94fc6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="94fc6-140">Int32</span></span>|<span data-ttu-id="94fc6-141">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="94fc6-141">Number of error devices</span></span>|
|<span data-ttu-id="94fc6-142">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94fc6-142">conflictDeviceCount</span></span>|<span data-ttu-id="94fc6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="94fc6-143">Int32</span></span>|<span data-ttu-id="94fc6-144">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="94fc6-144">Number of conflict devices</span></span>|
|<span data-ttu-id="94fc6-145">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94fc6-145">notAssignedDeviceCount</span></span>|<span data-ttu-id="94fc6-146">Int32</span><span class="sxs-lookup"><span data-stu-id="94fc6-146">Int32</span></span>|<span data-ttu-id="94fc6-147">未分配设备的数量</span><span class="sxs-lookup"><span data-stu-id="94fc6-147">Number of not assigned devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="94fc6-148">关系</span><span class="sxs-lookup"><span data-stu-id="94fc6-148">Relationships</span></span>
|<span data-ttu-id="94fc6-149">关系</span><span class="sxs-lookup"><span data-stu-id="94fc6-149">Relationship</span></span>|<span data-ttu-id="94fc6-150">类型</span><span class="sxs-lookup"><span data-stu-id="94fc6-150">Type</span></span>|<span data-ttu-id="94fc6-151">说明</span><span class="sxs-lookup"><span data-stu-id="94fc6-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94fc6-152">advancedThreatProtectionOnboardingDeviceSettingStates</span><span class="sxs-lookup"><span data-stu-id="94fc6-152">advancedThreatProtectionOnboardingDeviceSettingStates</span></span>|<span data-ttu-id="94fc6-153">[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="94fc6-153">[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) collection</span></span>|<span data-ttu-id="94fc6-154">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94fc6-154">Not yet documented</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94fc6-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94fc6-155">JSON Representation</span></span>
<span data-ttu-id="94fc6-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94fc6-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.advancedThreatProtectionOnboardingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notAssignedDeviceCount": 1024
}
```




