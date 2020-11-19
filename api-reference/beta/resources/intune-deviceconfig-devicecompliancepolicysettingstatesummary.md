---
title: deviceCompliancePolicySettingStateSummary 资源类型
description: 跨帐户的设备合规性策略设置状态摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b7a1e64dc711ae639283b9dbc4f8f3ec937092bd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260325"
---
# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a><span data-ttu-id="f4b0e-103">deviceCompliancePolicySettingStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4b0e-103">deviceCompliancePolicySettingStateSummary resource type</span></span>

<span data-ttu-id="f4b0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4b0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4b0e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4b0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4b0e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4b0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4b0e-107">跨帐户的设备合规性策略设置状态摘要。</span><span class="sxs-lookup"><span data-stu-id="f4b0e-107">Device Compilance Policy Setting State summary across the account.</span></span>

## <a name="methods"></a><span data-ttu-id="f4b0e-108">方法</span><span class="sxs-lookup"><span data-stu-id="f4b0e-108">Methods</span></span>
|<span data-ttu-id="f4b0e-109">方法</span><span class="sxs-lookup"><span data-stu-id="f4b0e-109">Method</span></span>|<span data-ttu-id="f4b0e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f4b0e-110">Return Type</span></span>|<span data-ttu-id="f4b0e-111">说明</span><span class="sxs-lookup"><span data-stu-id="f4b0e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f4b0e-112">列出 deviceCompliancePolicySettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="f4b0e-112">List deviceCompliancePolicySettingStateSummaries</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-list.md)|<span data-ttu-id="f4b0e-113">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4b0e-113">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) collection</span></span>|<span data-ttu-id="f4b0e-114">列出 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4b0e-114">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="f4b0e-115">获取 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="f4b0e-115">Get deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-get.md)|[<span data-ttu-id="f4b0e-116">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="f4b0e-116">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="f4b0e-117">读取 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4b0e-117">Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="f4b0e-118">创建 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="f4b0e-118">Create deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-create.md)|[<span data-ttu-id="f4b0e-119">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="f4b0e-119">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="f4b0e-120">创建新的 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4b0e-120">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="f4b0e-121">删除 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="f4b0e-121">Delete deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-delete.md)|<span data-ttu-id="f4b0e-122">无</span><span class="sxs-lookup"><span data-stu-id="f4b0e-122">None</span></span>|<span data-ttu-id="f4b0e-123">删除 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="f4b0e-123">Deletes a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>|
|[<span data-ttu-id="f4b0e-124">更新 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="f4b0e-124">Update deviceCompliancePolicySettingStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-update.md)|[<span data-ttu-id="f4b0e-125">deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="f4b0e-125">deviceCompliancePolicySettingStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="f4b0e-126">更新 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f4b0e-126">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f4b0e-127">属性</span><span class="sxs-lookup"><span data-stu-id="f4b0e-127">Properties</span></span>
|<span data-ttu-id="f4b0e-128">属性</span><span class="sxs-lookup"><span data-stu-id="f4b0e-128">Property</span></span>|<span data-ttu-id="f4b0e-129">类型</span><span class="sxs-lookup"><span data-stu-id="f4b0e-129">Type</span></span>|<span data-ttu-id="f4b0e-130">说明</span><span class="sxs-lookup"><span data-stu-id="f4b0e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4b0e-131">id</span><span class="sxs-lookup"><span data-stu-id="f4b0e-131">id</span></span>|<span data-ttu-id="f4b0e-132">String</span><span class="sxs-lookup"><span data-stu-id="f4b0e-132">String</span></span>|<span data-ttu-id="f4b0e-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f4b0e-133">Key of the entity.</span></span>|
|<span data-ttu-id="f4b0e-134">setting</span><span class="sxs-lookup"><span data-stu-id="f4b0e-134">setting</span></span>|<span data-ttu-id="f4b0e-135">String</span><span class="sxs-lookup"><span data-stu-id="f4b0e-135">String</span></span>|<span data-ttu-id="f4b0e-136">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="f4b0e-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="f4b0e-137">settingName</span><span class="sxs-lookup"><span data-stu-id="f4b0e-137">settingName</span></span>|<span data-ttu-id="f4b0e-138">String</span><span class="sxs-lookup"><span data-stu-id="f4b0e-138">String</span></span>|<span data-ttu-id="f4b0e-139">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="f4b0e-139">Name of the setting.</span></span>|
|<span data-ttu-id="f4b0e-140">platformType</span><span class="sxs-lookup"><span data-stu-id="f4b0e-140">platformType</span></span>|[<span data-ttu-id="f4b0e-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="f4b0e-141">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="f4b0e-142">设置平台。</span><span class="sxs-lookup"><span data-stu-id="f4b0e-142">Setting platform.</span></span> <span data-ttu-id="f4b0e-143">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="f4b0e-143">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="f4b0e-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f4b0e-144">unknownDeviceCount</span></span>|<span data-ttu-id="f4b0e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f4b0e-145">Int32</span></span>|<span data-ttu-id="f4b0e-146">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="f4b0e-146">Number of unknown devices</span></span>|
|<span data-ttu-id="f4b0e-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f4b0e-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="f4b0e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f4b0e-148">Int32</span></span>|<span data-ttu-id="f4b0e-149">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="f4b0e-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="f4b0e-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f4b0e-150">compliantDeviceCount</span></span>|<span data-ttu-id="f4b0e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f4b0e-151">Int32</span></span>|<span data-ttu-id="f4b0e-152">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="f4b0e-152">Number of compliant devices</span></span>|
|<span data-ttu-id="f4b0e-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f4b0e-153">remediatedDeviceCount</span></span>|<span data-ttu-id="f4b0e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f4b0e-154">Int32</span></span>|<span data-ttu-id="f4b0e-155">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="f4b0e-155">Number of remediated devices</span></span>|
|<span data-ttu-id="f4b0e-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f4b0e-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f4b0e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f4b0e-157">Int32</span></span>|<span data-ttu-id="f4b0e-158">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="f4b0e-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="f4b0e-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f4b0e-159">errorDeviceCount</span></span>|<span data-ttu-id="f4b0e-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f4b0e-160">Int32</span></span>|<span data-ttu-id="f4b0e-161">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="f4b0e-161">Number of error devices</span></span>|
|<span data-ttu-id="f4b0e-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f4b0e-162">conflictDeviceCount</span></span>|<span data-ttu-id="f4b0e-163">Int32</span><span class="sxs-lookup"><span data-stu-id="f4b0e-163">Int32</span></span>|<span data-ttu-id="f4b0e-164">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="f4b0e-164">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4b0e-165">关系</span><span class="sxs-lookup"><span data-stu-id="f4b0e-165">Relationships</span></span>
|<span data-ttu-id="f4b0e-166">关系</span><span class="sxs-lookup"><span data-stu-id="f4b0e-166">Relationship</span></span>|<span data-ttu-id="f4b0e-167">类型</span><span class="sxs-lookup"><span data-stu-id="f4b0e-167">Type</span></span>|<span data-ttu-id="f4b0e-168">描述</span><span class="sxs-lookup"><span data-stu-id="f4b0e-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4b0e-169">deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="f4b0e-169">deviceComplianceSettingStates</span></span>|<span data-ttu-id="f4b0e-170">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4b0e-170">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="f4b0e-171">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f4b0e-171">Not yet documented</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4b0e-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4b0e-172">JSON Representation</span></span>
<span data-ttu-id="f4b0e-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4b0e-173">Here is a JSON representation of the resource.</span></span>
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




