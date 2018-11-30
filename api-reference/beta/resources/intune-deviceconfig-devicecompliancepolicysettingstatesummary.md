---
title: deviceCompliancePolicySettingStateSummary 资源类型
description: 跨帐户的设备合规性策略设置状态摘要。
ms.openlocfilehash: a4707e40ff90649f93cd673a3904caa8b4cd2b9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046525"
---
# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a><span data-ttu-id="6c47f-103">deviceCompliancePolicySettingStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c47f-103">deviceCompliancePolicySettingStateSummary resource type</span></span>

> <span data-ttu-id="6c47f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6c47f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c47f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6c47f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c47f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6c47f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c47f-107">跨帐户的设备合规性策略设置状态摘要。</span><span class="sxs-lookup"><span data-stu-id="6c47f-107">Device Compilance Policy Setting State summary across the account.</span></span>
## <a name="methods"></a><span data-ttu-id="6c47f-108">方法</span><span class="sxs-lookup"><span data-stu-id="6c47f-108">Methods</span></span>
|<span data-ttu-id="6c47f-109">方法</span><span class="sxs-lookup"><span data-stu-id="6c47f-109">Method</span></span>|<span data-ttu-id="6c47f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6c47f-110">Return Type</span></span>|<span data-ttu-id="6c47f-111">说明</span><span class="sxs-lookup"><span data-stu-id="6c47f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c47f-112">列出 deviceCompliancePolicySettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="6c47f-112">List deviceCompliancePolicySettingStateSummaries</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-list.md)|<span data-ttu-id="6c47f-113">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c47f-113">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) collection</span></span>|<span data-ttu-id="6c47f-114">列出 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6c47f-114">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="6c47f-115">获取 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="6c47f-115">Get deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-get.md)|[<span data-ttu-id="6c47f-116">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="6c47f-116">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="6c47f-117">读取 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6c47f-117">Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="6c47f-118">创建 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="6c47f-118">Create deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-create.md)|[<span data-ttu-id="6c47f-119">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="6c47f-119">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="6c47f-120">创建新的 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6c47f-120">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="6c47f-121">删除 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="6c47f-121">Delete deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-delete.md)|<span data-ttu-id="6c47f-122">无</span><span class="sxs-lookup"><span data-stu-id="6c47f-122">None</span></span>|<span data-ttu-id="6c47f-123">删除 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="6c47f-123">Deletes a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>|
|[<span data-ttu-id="6c47f-124">更新 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="6c47f-124">Update deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-update.md)|[<span data-ttu-id="6c47f-125">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="6c47f-125">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="6c47f-126">更新 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6c47f-126">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c47f-127">属性</span><span class="sxs-lookup"><span data-stu-id="6c47f-127">Properties</span></span>
|<span data-ttu-id="6c47f-128">属性</span><span class="sxs-lookup"><span data-stu-id="6c47f-128">Property</span></span>|<span data-ttu-id="6c47f-129">类型</span><span class="sxs-lookup"><span data-stu-id="6c47f-129">Type</span></span>|<span data-ttu-id="6c47f-130">说明</span><span class="sxs-lookup"><span data-stu-id="6c47f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c47f-131">id</span><span class="sxs-lookup"><span data-stu-id="6c47f-131">id</span></span>|<span data-ttu-id="6c47f-132">String</span><span class="sxs-lookup"><span data-stu-id="6c47f-132">String</span></span>|<span data-ttu-id="6c47f-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6c47f-133">Key of the entity.</span></span>|
|<span data-ttu-id="6c47f-134">setting</span><span class="sxs-lookup"><span data-stu-id="6c47f-134">setting</span></span>|<span data-ttu-id="6c47f-135">String</span><span class="sxs-lookup"><span data-stu-id="6c47f-135">String</span></span>|<span data-ttu-id="6c47f-136">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="6c47f-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="6c47f-137">settingName</span><span class="sxs-lookup"><span data-stu-id="6c47f-137">settingName</span></span>|<span data-ttu-id="6c47f-138">String</span><span class="sxs-lookup"><span data-stu-id="6c47f-138">String</span></span>|<span data-ttu-id="6c47f-139">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="6c47f-139">Name of the setting.</span></span>|
|<span data-ttu-id="6c47f-140">platformType</span><span class="sxs-lookup"><span data-stu-id="6c47f-140">platformType</span></span>|[<span data-ttu-id="6c47f-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="6c47f-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="6c47f-142">设置平台。</span><span class="sxs-lookup"><span data-stu-id="6c47f-142">Setting platform.</span></span> <span data-ttu-id="6c47f-143">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="6c47f-143">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="6c47f-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6c47f-144">unknownDeviceCount</span></span>|<span data-ttu-id="6c47f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6c47f-145">Int32</span></span>|<span data-ttu-id="6c47f-146">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="6c47f-146">Number of unknown devices</span></span>|
|<span data-ttu-id="6c47f-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6c47f-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="6c47f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6c47f-148">Int32</span></span>|<span data-ttu-id="6c47f-149">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="6c47f-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="6c47f-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6c47f-150">compliantDeviceCount</span></span>|<span data-ttu-id="6c47f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6c47f-151">Int32</span></span>|<span data-ttu-id="6c47f-152">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="6c47f-152">Number of compliant devices</span></span>|
|<span data-ttu-id="6c47f-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6c47f-153">remediatedDeviceCount</span></span>|<span data-ttu-id="6c47f-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6c47f-154">Int32</span></span>|<span data-ttu-id="6c47f-155">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="6c47f-155">Number of remediated devices</span></span>|
|<span data-ttu-id="6c47f-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6c47f-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="6c47f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6c47f-157">Int32</span></span>|<span data-ttu-id="6c47f-158">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="6c47f-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="6c47f-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6c47f-159">errorDeviceCount</span></span>|<span data-ttu-id="6c47f-160">Int32</span><span class="sxs-lookup"><span data-stu-id="6c47f-160">Int32</span></span>|<span data-ttu-id="6c47f-161">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="6c47f-161">Number of error devices</span></span>|
|<span data-ttu-id="6c47f-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6c47f-162">conflictDeviceCount</span></span>|<span data-ttu-id="6c47f-163">Int32</span><span class="sxs-lookup"><span data-stu-id="6c47f-163">Int32</span></span>|<span data-ttu-id="6c47f-164">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="6c47f-164">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c47f-165">关系</span><span class="sxs-lookup"><span data-stu-id="6c47f-165">Relationships</span></span>
|<span data-ttu-id="6c47f-166">关系</span><span class="sxs-lookup"><span data-stu-id="6c47f-166">Relationship</span></span>|<span data-ttu-id="6c47f-167">类型</span><span class="sxs-lookup"><span data-stu-id="6c47f-167">Type</span></span>|<span data-ttu-id="6c47f-168">说明</span><span class="sxs-lookup"><span data-stu-id="6c47f-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c47f-169">deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="6c47f-169">deviceComplianceSettingStates</span></span>|<span data-ttu-id="6c47f-170">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c47f-170">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="6c47f-171">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6c47f-171">Not yet documented</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c47f-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c47f-172">JSON Representation</span></span>
<span data-ttu-id="6c47f-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c47f-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "platformType": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```





