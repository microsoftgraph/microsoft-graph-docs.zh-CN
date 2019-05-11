---
title: managedDeviceEncryptionState 资源类型
description: 每个设备的加密报告
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6816e8bc0bb71f4f81b3fc213db622d38ed83816
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944934"
---
# <a name="manageddeviceencryptionstate-resource-type"></a><span data-ttu-id="c5b9f-103">managedDeviceEncryptionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5b9f-103">managedDeviceEncryptionState resource type</span></span>

> <span data-ttu-id="c5b9f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5b9f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5b9f-106">每个设备的加密报告</span><span class="sxs-lookup"><span data-stu-id="c5b9f-106">Encryption report per device</span></span>

## <a name="methods"></a><span data-ttu-id="c5b9f-107">方法</span><span class="sxs-lookup"><span data-stu-id="c5b9f-107">Methods</span></span>
|<span data-ttu-id="c5b9f-108">方法</span><span class="sxs-lookup"><span data-stu-id="c5b9f-108">Method</span></span>|<span data-ttu-id="c5b9f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c5b9f-109">Return Type</span></span>|<span data-ttu-id="c5b9f-110">说明</span><span class="sxs-lookup"><span data-stu-id="c5b9f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c5b9f-111">列出 managedDeviceEncryptionStates</span><span class="sxs-lookup"><span data-stu-id="c5b9f-111">List managedDeviceEncryptionStates</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|<span data-ttu-id="c5b9f-112">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="c5b9f-112">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) collection</span></span>|<span data-ttu-id="c5b9f-113">列出[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-113">List properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects.</span></span>|
|[<span data-ttu-id="c5b9f-114">获取 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="c5b9f-114">Get managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[<span data-ttu-id="c5b9f-115">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="c5b9f-115">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="c5b9f-116">读取[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-116">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="c5b9f-117">创建 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="c5b9f-117">Create managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[<span data-ttu-id="c5b9f-118">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="c5b9f-118">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="c5b9f-119">创建新的[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-119">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="c5b9f-120">删除 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="c5b9f-120">Delete managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|<span data-ttu-id="c5b9f-121">无</span><span class="sxs-lookup"><span data-stu-id="c5b9f-121">None</span></span>|<span data-ttu-id="c5b9f-122">删除[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-122">Deletes a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>|
|[<span data-ttu-id="c5b9f-123">更新 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="c5b9f-123">Update managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[<span data-ttu-id="c5b9f-124">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="c5b9f-124">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="c5b9f-125">更新[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-125">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5b9f-126">属性</span><span class="sxs-lookup"><span data-stu-id="c5b9f-126">Properties</span></span>
|<span data-ttu-id="c5b9f-127">属性</span><span class="sxs-lookup"><span data-stu-id="c5b9f-127">Property</span></span>|<span data-ttu-id="c5b9f-128">类型</span><span class="sxs-lookup"><span data-stu-id="c5b9f-128">Type</span></span>|<span data-ttu-id="c5b9f-129">说明</span><span class="sxs-lookup"><span data-stu-id="c5b9f-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5b9f-130">id</span><span class="sxs-lookup"><span data-stu-id="c5b9f-130">id</span></span>|<span data-ttu-id="c5b9f-131">String</span><span class="sxs-lookup"><span data-stu-id="c5b9f-131">String</span></span>|<span data-ttu-id="c5b9f-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-132">Key of the entity.</span></span>|
|<span data-ttu-id="c5b9f-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c5b9f-133">userPrincipalName</span></span>|<span data-ttu-id="c5b9f-134">String</span><span class="sxs-lookup"><span data-stu-id="c5b9f-134">String</span></span>|<span data-ttu-id="c5b9f-135">用户名</span><span class="sxs-lookup"><span data-stu-id="c5b9f-135">User name</span></span>|
|<span data-ttu-id="c5b9f-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="c5b9f-136">deviceType</span></span>|[<span data-ttu-id="c5b9f-137">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="c5b9f-137">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="c5b9f-138">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-138">Platform of the device.</span></span> <span data-ttu-id="c5b9f-139">可能的值为`desktop`: `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c5b9f-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="c5b9f-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="c5b9f-140">osVersion</span></span>|<span data-ttu-id="c5b9f-141">String</span><span class="sxs-lookup"><span data-stu-id="c5b9f-141">String</span></span>|<span data-ttu-id="c5b9f-142">设备的操作系统版本</span><span class="sxs-lookup"><span data-stu-id="c5b9f-142">Operating system version of the device</span></span>|
|<span data-ttu-id="c5b9f-143">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="c5b9f-143">tpmSpecificationVersion</span></span>|<span data-ttu-id="c5b9f-144">String</span><span class="sxs-lookup"><span data-stu-id="c5b9f-144">String</span></span>|<span data-ttu-id="c5b9f-145">设备 TPM 版本</span><span class="sxs-lookup"><span data-stu-id="c5b9f-145">Device TPM Version</span></span>|
|<span data-ttu-id="c5b9f-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="c5b9f-146">deviceName</span></span>|<span data-ttu-id="c5b9f-147">String</span><span class="sxs-lookup"><span data-stu-id="c5b9f-147">String</span></span>|<span data-ttu-id="c5b9f-148">设备名称</span><span class="sxs-lookup"><span data-stu-id="c5b9f-148">Device name</span></span>|
|<span data-ttu-id="c5b9f-149">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="c5b9f-149">encryptionReadinessState</span></span>|[<span data-ttu-id="c5b9f-150">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="c5b9f-150">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="c5b9f-151">加密准备情况状态。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-151">Encryption readiness state.</span></span> <span data-ttu-id="c5b9f-152">可取值为：`notReady`、`ready`。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-152">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="c5b9f-153">encryptionState</span><span class="sxs-lookup"><span data-stu-id="c5b9f-153">encryptionState</span></span>|[<span data-ttu-id="c5b9f-154">encryptionState</span><span class="sxs-lookup"><span data-stu-id="c5b9f-154">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="c5b9f-155">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-155">Device encryption state.</span></span> <span data-ttu-id="c5b9f-156">可取值为：`notEncrypted`、`encrypted`。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-156">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="c5b9f-157">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="c5b9f-157">encryptionPolicySettingState</span></span>|[<span data-ttu-id="c5b9f-158">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c5b9f-158">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c5b9f-159">加密策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-159">Encryption policy setting state.</span></span> <span data-ttu-id="c5b9f-160">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-160">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c5b9f-161">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="c5b9f-161">advancedBitLockerStates</span></span>|[<span data-ttu-id="c5b9f-162">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="c5b9f-162">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="c5b9f-163">高级 BitLocker 状态。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-163">Advanced BitLocker State.</span></span> <span data-ttu-id="c5b9f-164">可能的值是`success`: `noUserConsent`、 `osVolumeEncryptionMethodMismatch`、 `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `recoveryKeyBackupFailed` `networkError`、、 `fixedDriveNotEncrypted`、、、、、、、、、、、、。 `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady`</span><span class="sxs-lookup"><span data-stu-id="c5b9f-164">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="c5b9f-165">policyDetails</span><span class="sxs-lookup"><span data-stu-id="c5b9f-165">policyDetails</span></span>|<span data-ttu-id="c5b9f-166">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)集合</span><span class="sxs-lookup"><span data-stu-id="c5b9f-166">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="c5b9f-167">策略详细信息</span><span class="sxs-lookup"><span data-stu-id="c5b9f-167">Policy Details</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5b9f-168">关系</span><span class="sxs-lookup"><span data-stu-id="c5b9f-168">Relationships</span></span>
<span data-ttu-id="c5b9f-169">无</span><span class="sxs-lookup"><span data-stu-id="c5b9f-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5b9f-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5b9f-170">JSON Representation</span></span>
<span data-ttu-id="c5b9f-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5b9f-171">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceEncryptionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "deviceType": "String",
  "osVersion": "String",
  "tpmSpecificationVersion": "String",
  "deviceName": "String",
  "encryptionReadinessState": "String",
  "encryptionState": "String",
  "encryptionPolicySettingState": "String",
  "advancedBitLockerStates": "String",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "String",
      "policyName": "String"
    }
  ]
}
```




