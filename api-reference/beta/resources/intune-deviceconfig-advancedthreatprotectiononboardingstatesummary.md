---
title: advancedThreatProtectionOnboardingStateSummary 资源类型
description: Windows defender 高级的威胁保护入职培训状态摘要跨帐户。
author: tfitzmac
ms.openlocfilehash: 3a31d489374b87469d2ed6fb87bb70f8d89d710c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359169"
---
# <a name="advancedthreatprotectiononboardingstatesummary-resource-type"></a><span data-ttu-id="febbe-103">advancedThreatProtectionOnboardingStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="febbe-103">advancedThreatProtectionOnboardingStateSummary resource type</span></span>

> <span data-ttu-id="febbe-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="febbe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="febbe-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="febbe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="febbe-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="febbe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="febbe-107">Windows defender 高级的威胁保护入职培训状态摘要跨帐户。</span><span class="sxs-lookup"><span data-stu-id="febbe-107">Windows defender advanced threat protection onboarding state summary across the account.</span></span>
## <a name="methods"></a><span data-ttu-id="febbe-108">方法</span><span class="sxs-lookup"><span data-stu-id="febbe-108">Methods</span></span>
|<span data-ttu-id="febbe-109">方法</span><span class="sxs-lookup"><span data-stu-id="febbe-109">Method</span></span>|<span data-ttu-id="febbe-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="febbe-110">Return Type</span></span>|<span data-ttu-id="febbe-111">说明</span><span class="sxs-lookup"><span data-stu-id="febbe-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="febbe-112">获取 advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="febbe-112">Get advancedThreatProtectionOnboardingStateSummary</span></span>](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-get.md)|[<span data-ttu-id="febbe-113">advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="febbe-113">advancedThreatProtectionOnboardingStateSummary</span></span>](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|<span data-ttu-id="febbe-114">读取属性和[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="febbe-114">Read properties and relationships of the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="febbe-115">更新 advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="febbe-115">Update advancedThreatProtectionOnboardingStateSummary</span></span>](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-update.md)|[<span data-ttu-id="febbe-116">advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="febbe-116">advancedThreatProtectionOnboardingStateSummary</span></span>](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|<span data-ttu-id="febbe-117">更新[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="febbe-117">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="febbe-118">属性</span><span class="sxs-lookup"><span data-stu-id="febbe-118">Properties</span></span>
|<span data-ttu-id="febbe-119">属性</span><span class="sxs-lookup"><span data-stu-id="febbe-119">Property</span></span>|<span data-ttu-id="febbe-120">类型</span><span class="sxs-lookup"><span data-stu-id="febbe-120">Type</span></span>|<span data-ttu-id="febbe-121">说明</span><span class="sxs-lookup"><span data-stu-id="febbe-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="febbe-122">id</span><span class="sxs-lookup"><span data-stu-id="febbe-122">id</span></span>|<span data-ttu-id="febbe-123">String</span><span class="sxs-lookup"><span data-stu-id="febbe-123">String</span></span>|<span data-ttu-id="febbe-124">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="febbe-124">Unique Identifier</span></span>|
|<span data-ttu-id="febbe-125">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="febbe-125">unknownDeviceCount</span></span>|<span data-ttu-id="febbe-126">Int32</span><span class="sxs-lookup"><span data-stu-id="febbe-126">Int32</span></span>|<span data-ttu-id="febbe-127">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="febbe-127">Number of unknown devices</span></span>|
|<span data-ttu-id="febbe-128">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="febbe-128">notApplicableDeviceCount</span></span>|<span data-ttu-id="febbe-129">Int32</span><span class="sxs-lookup"><span data-stu-id="febbe-129">Int32</span></span>|<span data-ttu-id="febbe-130">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="febbe-130">Number of not applicable devices</span></span>|
|<span data-ttu-id="febbe-131">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="febbe-131">compliantDeviceCount</span></span>|<span data-ttu-id="febbe-132">Int32</span><span class="sxs-lookup"><span data-stu-id="febbe-132">Int32</span></span>|<span data-ttu-id="febbe-133">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="febbe-133">Number of compliant devices</span></span>|
|<span data-ttu-id="febbe-134">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="febbe-134">remediatedDeviceCount</span></span>|<span data-ttu-id="febbe-135">Int32</span><span class="sxs-lookup"><span data-stu-id="febbe-135">Int32</span></span>|<span data-ttu-id="febbe-136">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="febbe-136">Number of remediated devices</span></span>|
|<span data-ttu-id="febbe-137">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="febbe-137">nonCompliantDeviceCount</span></span>|<span data-ttu-id="febbe-138">Int32</span><span class="sxs-lookup"><span data-stu-id="febbe-138">Int32</span></span>|<span data-ttu-id="febbe-139">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="febbe-139">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="febbe-140">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="febbe-140">errorDeviceCount</span></span>|<span data-ttu-id="febbe-141">Int32</span><span class="sxs-lookup"><span data-stu-id="febbe-141">Int32</span></span>|<span data-ttu-id="febbe-142">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="febbe-142">Number of error devices</span></span>|
|<span data-ttu-id="febbe-143">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="febbe-143">conflictDeviceCount</span></span>|<span data-ttu-id="febbe-144">Int32</span><span class="sxs-lookup"><span data-stu-id="febbe-144">Int32</span></span>|<span data-ttu-id="febbe-145">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="febbe-145">Number of conflict devices</span></span>|
|<span data-ttu-id="febbe-146">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="febbe-146">notAssignedDeviceCount</span></span>|<span data-ttu-id="febbe-147">Int32</span><span class="sxs-lookup"><span data-stu-id="febbe-147">Int32</span></span>|<span data-ttu-id="febbe-148">未分配的设备数</span><span class="sxs-lookup"><span data-stu-id="febbe-148">Number of not assigned devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="febbe-149">Relationships</span><span class="sxs-lookup"><span data-stu-id="febbe-149">Relationships</span></span>
|<span data-ttu-id="febbe-150">关系</span><span class="sxs-lookup"><span data-stu-id="febbe-150">Relationship</span></span>|<span data-ttu-id="febbe-151">类型</span><span class="sxs-lookup"><span data-stu-id="febbe-151">Type</span></span>|<span data-ttu-id="febbe-152">说明</span><span class="sxs-lookup"><span data-stu-id="febbe-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="febbe-153">advancedThreatProtectionOnboardingDeviceSettingStates</span><span class="sxs-lookup"><span data-stu-id="febbe-153">advancedThreatProtectionOnboardingDeviceSettingStates</span></span>|<span data-ttu-id="febbe-154">[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="febbe-154">[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) collection</span></span>|<span data-ttu-id="febbe-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="febbe-155">Not yet documented</span></span>|

## <a name="json-representation"></a><span data-ttu-id="febbe-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="febbe-156">JSON Representation</span></span>
<span data-ttu-id="febbe-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="febbe-157">Here is a JSON representation of the resource.</span></span>
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





