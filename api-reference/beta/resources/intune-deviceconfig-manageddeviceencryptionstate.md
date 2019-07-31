---
title: managedDeviceEncryptionState 资源类型
description: 每个设备的加密报告
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb212599c56410b7f66d6f8baa8db1d06d36ba60
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000879"
---
# <a name="manageddeviceencryptionstate-resource-type"></a><span data-ttu-id="a3100-103">managedDeviceEncryptionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3100-103">managedDeviceEncryptionState resource type</span></span>

> <span data-ttu-id="a3100-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a3100-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3100-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3100-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3100-106">每个设备的加密报告</span><span class="sxs-lookup"><span data-stu-id="a3100-106">Encryption report per device</span></span>

## <a name="methods"></a><span data-ttu-id="a3100-107">方法</span><span class="sxs-lookup"><span data-stu-id="a3100-107">Methods</span></span>
|<span data-ttu-id="a3100-108">方法</span><span class="sxs-lookup"><span data-stu-id="a3100-108">Method</span></span>|<span data-ttu-id="a3100-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a3100-109">Return Type</span></span>|<span data-ttu-id="a3100-110">说明</span><span class="sxs-lookup"><span data-stu-id="a3100-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a3100-111">列出 managedDeviceEncryptionStates</span><span class="sxs-lookup"><span data-stu-id="a3100-111">List managedDeviceEncryptionStates</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|<span data-ttu-id="a3100-112">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="a3100-112">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) collection</span></span>|<span data-ttu-id="a3100-113">列出[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a3100-113">List properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects.</span></span>|
|[<span data-ttu-id="a3100-114">获取 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="a3100-114">Get managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[<span data-ttu-id="a3100-115">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="a3100-115">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="a3100-116">读取[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a3100-116">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="a3100-117">创建 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="a3100-117">Create managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[<span data-ttu-id="a3100-118">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="a3100-118">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="a3100-119">创建新的[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a3100-119">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="a3100-120">删除 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="a3100-120">Delete managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|<span data-ttu-id="a3100-121">无</span><span class="sxs-lookup"><span data-stu-id="a3100-121">None</span></span>|<span data-ttu-id="a3100-122">删除[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)。</span><span class="sxs-lookup"><span data-stu-id="a3100-122">Deletes a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>|
|[<span data-ttu-id="a3100-123">更新 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="a3100-123">Update managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[<span data-ttu-id="a3100-124">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="a3100-124">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="a3100-125">更新[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a3100-125">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3100-126">属性</span><span class="sxs-lookup"><span data-stu-id="a3100-126">Properties</span></span>
|<span data-ttu-id="a3100-127">属性</span><span class="sxs-lookup"><span data-stu-id="a3100-127">Property</span></span>|<span data-ttu-id="a3100-128">类型</span><span class="sxs-lookup"><span data-stu-id="a3100-128">Type</span></span>|<span data-ttu-id="a3100-129">说明</span><span class="sxs-lookup"><span data-stu-id="a3100-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3100-130">id</span><span class="sxs-lookup"><span data-stu-id="a3100-130">id</span></span>|<span data-ttu-id="a3100-131">String</span><span class="sxs-lookup"><span data-stu-id="a3100-131">String</span></span>|<span data-ttu-id="a3100-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a3100-132">Key of the entity.</span></span>|
|<span data-ttu-id="a3100-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a3100-133">userPrincipalName</span></span>|<span data-ttu-id="a3100-134">String</span><span class="sxs-lookup"><span data-stu-id="a3100-134">String</span></span>|<span data-ttu-id="a3100-135">用户名</span><span class="sxs-lookup"><span data-stu-id="a3100-135">User name</span></span>|
|<span data-ttu-id="a3100-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="a3100-136">deviceType</span></span>|[<span data-ttu-id="a3100-137">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="a3100-137">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="a3100-138">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="a3100-138">Platform of the device.</span></span> <span data-ttu-id="a3100-139">可能的值为`desktop`: `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a3100-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="a3100-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="a3100-140">osVersion</span></span>|<span data-ttu-id="a3100-141">String</span><span class="sxs-lookup"><span data-stu-id="a3100-141">String</span></span>|<span data-ttu-id="a3100-142">设备的操作系统版本</span><span class="sxs-lookup"><span data-stu-id="a3100-142">Operating system version of the device</span></span>|
|<span data-ttu-id="a3100-143">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="a3100-143">tpmSpecificationVersion</span></span>|<span data-ttu-id="a3100-144">String</span><span class="sxs-lookup"><span data-stu-id="a3100-144">String</span></span>|<span data-ttu-id="a3100-145">设备 TPM 版本</span><span class="sxs-lookup"><span data-stu-id="a3100-145">Device TPM Version</span></span>|
|<span data-ttu-id="a3100-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="a3100-146">deviceName</span></span>|<span data-ttu-id="a3100-147">String</span><span class="sxs-lookup"><span data-stu-id="a3100-147">String</span></span>|<span data-ttu-id="a3100-148">设备名称</span><span class="sxs-lookup"><span data-stu-id="a3100-148">Device name</span></span>|
|<span data-ttu-id="a3100-149">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="a3100-149">encryptionReadinessState</span></span>|[<span data-ttu-id="a3100-150">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="a3100-150">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="a3100-151">加密准备情况状态。</span><span class="sxs-lookup"><span data-stu-id="a3100-151">Encryption readiness state.</span></span> <span data-ttu-id="a3100-152">可取值为：`notReady`、`ready`。</span><span class="sxs-lookup"><span data-stu-id="a3100-152">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="a3100-153">encryptionState</span><span class="sxs-lookup"><span data-stu-id="a3100-153">encryptionState</span></span>|[<span data-ttu-id="a3100-154">encryptionState</span><span class="sxs-lookup"><span data-stu-id="a3100-154">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="a3100-155">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="a3100-155">Device encryption state.</span></span> <span data-ttu-id="a3100-156">可取值为：`notEncrypted`、`encrypted`。</span><span class="sxs-lookup"><span data-stu-id="a3100-156">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="a3100-157">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="a3100-157">encryptionPolicySettingState</span></span>|[<span data-ttu-id="a3100-158">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a3100-158">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a3100-159">加密策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="a3100-159">Encryption policy setting state.</span></span> <span data-ttu-id="a3100-160">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="a3100-160">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a3100-161">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="a3100-161">advancedBitLockerStates</span></span>|[<span data-ttu-id="a3100-162">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="a3100-162">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="a3100-163">高级 BitLocker 状态。</span><span class="sxs-lookup"><span data-stu-id="a3100-163">Advanced BitLocker State.</span></span> <span data-ttu-id="a3100-164">可能的值是`success`: `noUserConsent`、 `osVolumeEncryptionMethodMismatch`、 `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `recoveryKeyBackupFailed` `networkError`、、 `fixedDriveNotEncrypted`、、、、、、、、、、、、。 `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady`</span><span class="sxs-lookup"><span data-stu-id="a3100-164">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="a3100-165">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="a3100-165">fileVaultStates</span></span>|[<span data-ttu-id="a3100-166">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="a3100-166">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="a3100-167">FileVault 状态。</span><span class="sxs-lookup"><span data-stu-id="a3100-167">FileVault State.</span></span> <span data-ttu-id="a3100-168">可取值为：`success`、`driveEncryptedByUser`、`userDeferredEncryption`、`escrowNotEnabled`。</span><span class="sxs-lookup"><span data-stu-id="a3100-168">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="a3100-169">policyDetails</span><span class="sxs-lookup"><span data-stu-id="a3100-169">policyDetails</span></span>|<span data-ttu-id="a3100-170">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)集合</span><span class="sxs-lookup"><span data-stu-id="a3100-170">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="a3100-171">策略详细信息</span><span class="sxs-lookup"><span data-stu-id="a3100-171">Policy Details</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3100-172">关系</span><span class="sxs-lookup"><span data-stu-id="a3100-172">Relationships</span></span>
<span data-ttu-id="a3100-173">无</span><span class="sxs-lookup"><span data-stu-id="a3100-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3100-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3100-174">JSON Representation</span></span>
<span data-ttu-id="a3100-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3100-175">Here is a JSON representation of the resource.</span></span>
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
  "fileVaultStates": "String",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "String",
      "policyName": "String"
    }
  ]
}
```





