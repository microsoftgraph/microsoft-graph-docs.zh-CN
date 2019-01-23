---
title: advancedThreatProtectionOnboardingStateSummary 资源类型
description: Windows defender 高级的威胁保护入职培训状态摘要跨帐户。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 57aa8aea277cb1cab6f8ed695779a80be763e788
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420085"
---
# <a name="advancedthreatprotectiononboardingstatesummary-resource-type"></a><span data-ttu-id="63390-103">advancedThreatProtectionOnboardingStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="63390-103">advancedThreatProtectionOnboardingStateSummary resource type</span></span>

> <span data-ttu-id="63390-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="63390-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="63390-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="63390-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63390-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63390-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63390-107">Windows defender 高级的威胁保护入职培训状态摘要跨帐户。</span><span class="sxs-lookup"><span data-stu-id="63390-107">Windows defender advanced threat protection onboarding state summary across the account.</span></span>

## <a name="methods"></a><span data-ttu-id="63390-108">方法</span><span class="sxs-lookup"><span data-stu-id="63390-108">Methods</span></span>
|<span data-ttu-id="63390-109">方法</span><span class="sxs-lookup"><span data-stu-id="63390-109">Method</span></span>|<span data-ttu-id="63390-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="63390-110">Return Type</span></span>|<span data-ttu-id="63390-111">说明</span><span class="sxs-lookup"><span data-stu-id="63390-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="63390-112">获取 advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="63390-112">Get advancedThreatProtectionOnboardingStateSummary</span></span>](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-get.md)|[<span data-ttu-id="63390-113">advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="63390-113">advancedThreatProtectionOnboardingStateSummary</span></span>](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|<span data-ttu-id="63390-114">读取属性和[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="63390-114">Read properties and relationships of the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="63390-115">更新 advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="63390-115">Update advancedThreatProtectionOnboardingStateSummary</span></span>](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-update.md)|[<span data-ttu-id="63390-116">advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="63390-116">advancedThreatProtectionOnboardingStateSummary</span></span>](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|<span data-ttu-id="63390-117">更新[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="63390-117">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="63390-118">属性</span><span class="sxs-lookup"><span data-stu-id="63390-118">Properties</span></span>
|<span data-ttu-id="63390-119">属性</span><span class="sxs-lookup"><span data-stu-id="63390-119">Property</span></span>|<span data-ttu-id="63390-120">类型</span><span class="sxs-lookup"><span data-stu-id="63390-120">Type</span></span>|<span data-ttu-id="63390-121">说明</span><span class="sxs-lookup"><span data-stu-id="63390-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63390-122">id</span><span class="sxs-lookup"><span data-stu-id="63390-122">id</span></span>|<span data-ttu-id="63390-123">String</span><span class="sxs-lookup"><span data-stu-id="63390-123">String</span></span>|<span data-ttu-id="63390-124">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="63390-124">Unique Identifier</span></span>|
|<span data-ttu-id="63390-125">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63390-125">unknownDeviceCount</span></span>|<span data-ttu-id="63390-126">Int32</span><span class="sxs-lookup"><span data-stu-id="63390-126">Int32</span></span>|<span data-ttu-id="63390-127">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="63390-127">Number of unknown devices</span></span>|
|<span data-ttu-id="63390-128">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63390-128">notApplicableDeviceCount</span></span>|<span data-ttu-id="63390-129">Int32</span><span class="sxs-lookup"><span data-stu-id="63390-129">Int32</span></span>|<span data-ttu-id="63390-130">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="63390-130">Number of not applicable devices</span></span>|
|<span data-ttu-id="63390-131">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63390-131">compliantDeviceCount</span></span>|<span data-ttu-id="63390-132">Int32</span><span class="sxs-lookup"><span data-stu-id="63390-132">Int32</span></span>|<span data-ttu-id="63390-133">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="63390-133">Number of compliant devices</span></span>|
|<span data-ttu-id="63390-134">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63390-134">remediatedDeviceCount</span></span>|<span data-ttu-id="63390-135">Int32</span><span class="sxs-lookup"><span data-stu-id="63390-135">Int32</span></span>|<span data-ttu-id="63390-136">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="63390-136">Number of remediated devices</span></span>|
|<span data-ttu-id="63390-137">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63390-137">nonCompliantDeviceCount</span></span>|<span data-ttu-id="63390-138">Int32</span><span class="sxs-lookup"><span data-stu-id="63390-138">Int32</span></span>|<span data-ttu-id="63390-139">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="63390-139">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="63390-140">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63390-140">errorDeviceCount</span></span>|<span data-ttu-id="63390-141">Int32</span><span class="sxs-lookup"><span data-stu-id="63390-141">Int32</span></span>|<span data-ttu-id="63390-142">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="63390-142">Number of error devices</span></span>|
|<span data-ttu-id="63390-143">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63390-143">conflictDeviceCount</span></span>|<span data-ttu-id="63390-144">Int32</span><span class="sxs-lookup"><span data-stu-id="63390-144">Int32</span></span>|<span data-ttu-id="63390-145">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="63390-145">Number of conflict devices</span></span>|
|<span data-ttu-id="63390-146">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63390-146">notAssignedDeviceCount</span></span>|<span data-ttu-id="63390-147">Int32</span><span class="sxs-lookup"><span data-stu-id="63390-147">Int32</span></span>|<span data-ttu-id="63390-148">未分配的设备数</span><span class="sxs-lookup"><span data-stu-id="63390-148">Number of not assigned devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="63390-149">关系</span><span class="sxs-lookup"><span data-stu-id="63390-149">Relationships</span></span>
|<span data-ttu-id="63390-150">关系</span><span class="sxs-lookup"><span data-stu-id="63390-150">Relationship</span></span>|<span data-ttu-id="63390-151">类型</span><span class="sxs-lookup"><span data-stu-id="63390-151">Type</span></span>|<span data-ttu-id="63390-152">说明</span><span class="sxs-lookup"><span data-stu-id="63390-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63390-153">advancedThreatProtectionOnboardingDeviceSettingStates</span><span class="sxs-lookup"><span data-stu-id="63390-153">advancedThreatProtectionOnboardingDeviceSettingStates</span></span>|<span data-ttu-id="63390-154">[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="63390-154">[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) collection</span></span>|<span data-ttu-id="63390-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="63390-155">Not yet documented</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63390-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63390-156">JSON Representation</span></span>
<span data-ttu-id="63390-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63390-157">Here is a JSON representation of the resource.</span></span>
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




