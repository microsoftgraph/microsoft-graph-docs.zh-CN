---
title: managedDeviceEncryptionState 资源类型
description: 每个设备的加密报告
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a6c9e601efc8d68e3c3794c4d6dacc988753ef3c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437303"
---
# <a name="manageddeviceencryptionstate-resource-type"></a><span data-ttu-id="79cb1-103">managedDeviceEncryptionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="79cb1-103">managedDeviceEncryptionState resource type</span></span>

<span data-ttu-id="79cb1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79cb1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79cb1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="79cb1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79cb1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79cb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79cb1-107">每个设备的加密报告</span><span class="sxs-lookup"><span data-stu-id="79cb1-107">Encryption report per device</span></span>

## <a name="methods"></a><span data-ttu-id="79cb1-108">方法</span><span class="sxs-lookup"><span data-stu-id="79cb1-108">Methods</span></span>
|<span data-ttu-id="79cb1-109">方法</span><span class="sxs-lookup"><span data-stu-id="79cb1-109">Method</span></span>|<span data-ttu-id="79cb1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="79cb1-110">Return Type</span></span>|<span data-ttu-id="79cb1-111">说明</span><span class="sxs-lookup"><span data-stu-id="79cb1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="79cb1-112">列出 managedDeviceEncryptionStates</span><span class="sxs-lookup"><span data-stu-id="79cb1-112">List managedDeviceEncryptionStates</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|<span data-ttu-id="79cb1-113">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="79cb1-113">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) collection</span></span>|<span data-ttu-id="79cb1-114">列出[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="79cb1-114">List properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects.</span></span>|
|[<span data-ttu-id="79cb1-115">获取 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="79cb1-115">Get managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[<span data-ttu-id="79cb1-116">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="79cb1-116">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="79cb1-117">读取[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="79cb1-117">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="79cb1-118">创建 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="79cb1-118">Create managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[<span data-ttu-id="79cb1-119">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="79cb1-119">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="79cb1-120">创建新的[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="79cb1-120">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="79cb1-121">删除 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="79cb1-121">Delete managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|<span data-ttu-id="79cb1-122">无</span><span class="sxs-lookup"><span data-stu-id="79cb1-122">None</span></span>|<span data-ttu-id="79cb1-123">删除[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)。</span><span class="sxs-lookup"><span data-stu-id="79cb1-123">Deletes a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>|
|[<span data-ttu-id="79cb1-124">更新 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="79cb1-124">Update managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[<span data-ttu-id="79cb1-125">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="79cb1-125">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="79cb1-126">更新[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="79cb1-126">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="79cb1-127">属性</span><span class="sxs-lookup"><span data-stu-id="79cb1-127">Properties</span></span>
|<span data-ttu-id="79cb1-128">属性</span><span class="sxs-lookup"><span data-stu-id="79cb1-128">Property</span></span>|<span data-ttu-id="79cb1-129">类型</span><span class="sxs-lookup"><span data-stu-id="79cb1-129">Type</span></span>|<span data-ttu-id="79cb1-130">说明</span><span class="sxs-lookup"><span data-stu-id="79cb1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79cb1-131">id</span><span class="sxs-lookup"><span data-stu-id="79cb1-131">id</span></span>|<span data-ttu-id="79cb1-132">String</span><span class="sxs-lookup"><span data-stu-id="79cb1-132">String</span></span>|<span data-ttu-id="79cb1-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="79cb1-133">Key of the entity.</span></span>|
|<span data-ttu-id="79cb1-134">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="79cb1-134">userPrincipalName</span></span>|<span data-ttu-id="79cb1-135">String</span><span class="sxs-lookup"><span data-stu-id="79cb1-135">String</span></span>|<span data-ttu-id="79cb1-136">用户名</span><span class="sxs-lookup"><span data-stu-id="79cb1-136">User name</span></span>|
|<span data-ttu-id="79cb1-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="79cb1-137">deviceType</span></span>|[<span data-ttu-id="79cb1-138">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="79cb1-138">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="79cb1-139">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="79cb1-139">Platform of the device.</span></span> <span data-ttu-id="79cb1-140">可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `palm` `unknown`、、、、、、、、、、、、、、、、、、、。 `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry`</span><span class="sxs-lookup"><span data-stu-id="79cb1-140">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="79cb1-141">osVersion</span><span class="sxs-lookup"><span data-stu-id="79cb1-141">osVersion</span></span>|<span data-ttu-id="79cb1-142">String</span><span class="sxs-lookup"><span data-stu-id="79cb1-142">String</span></span>|<span data-ttu-id="79cb1-143">设备的操作系统版本</span><span class="sxs-lookup"><span data-stu-id="79cb1-143">Operating system version of the device</span></span>|
|<span data-ttu-id="79cb1-144">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="79cb1-144">tpmSpecificationVersion</span></span>|<span data-ttu-id="79cb1-145">String</span><span class="sxs-lookup"><span data-stu-id="79cb1-145">String</span></span>|<span data-ttu-id="79cb1-146">设备 TPM 版本</span><span class="sxs-lookup"><span data-stu-id="79cb1-146">Device TPM Version</span></span>|
|<span data-ttu-id="79cb1-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="79cb1-147">deviceName</span></span>|<span data-ttu-id="79cb1-148">String</span><span class="sxs-lookup"><span data-stu-id="79cb1-148">String</span></span>|<span data-ttu-id="79cb1-149">设备名称</span><span class="sxs-lookup"><span data-stu-id="79cb1-149">Device name</span></span>|
|<span data-ttu-id="79cb1-150">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="79cb1-150">encryptionReadinessState</span></span>|[<span data-ttu-id="79cb1-151">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="79cb1-151">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="79cb1-152">加密准备情况状态。</span><span class="sxs-lookup"><span data-stu-id="79cb1-152">Encryption readiness state.</span></span> <span data-ttu-id="79cb1-153">可取值为：`notReady`、`ready`。</span><span class="sxs-lookup"><span data-stu-id="79cb1-153">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="79cb1-154">encryptionState</span><span class="sxs-lookup"><span data-stu-id="79cb1-154">encryptionState</span></span>|[<span data-ttu-id="79cb1-155">encryptionState</span><span class="sxs-lookup"><span data-stu-id="79cb1-155">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="79cb1-156">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="79cb1-156">Device encryption state.</span></span> <span data-ttu-id="79cb1-157">可取值为：`notEncrypted`、`encrypted`。</span><span class="sxs-lookup"><span data-stu-id="79cb1-157">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="79cb1-158">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="79cb1-158">encryptionPolicySettingState</span></span>|[<span data-ttu-id="79cb1-159">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="79cb1-159">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="79cb1-160">加密策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="79cb1-160">Encryption policy setting state.</span></span> <span data-ttu-id="79cb1-161">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="79cb1-161">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="79cb1-162">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="79cb1-162">advancedBitLockerStates</span></span>|[<span data-ttu-id="79cb1-163">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="79cb1-163">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="79cb1-164">高级 BitLocker 状态。</span><span class="sxs-lookup"><span data-stu-id="79cb1-164">Advanced BitLocker State.</span></span> <span data-ttu-id="79cb1-165">可能的值是`success`： `noUserConsent`、 `osVolumeEncryptionMethodMismatch`、 `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `recoveryKeyBackupFailed` `networkError`、、 `fixedDriveNotEncrypted`、、、、、、、、、、、、。 `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady`</span><span class="sxs-lookup"><span data-stu-id="79cb1-165">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="79cb1-166">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="79cb1-166">fileVaultStates</span></span>|[<span data-ttu-id="79cb1-167">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="79cb1-167">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="79cb1-168">FileVault 状态。</span><span class="sxs-lookup"><span data-stu-id="79cb1-168">FileVault State.</span></span> <span data-ttu-id="79cb1-169">可取值为：`success`、`driveEncryptedByUser`、`userDeferredEncryption`、`escrowNotEnabled`。</span><span class="sxs-lookup"><span data-stu-id="79cb1-169">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="79cb1-170">policyDetails</span><span class="sxs-lookup"><span data-stu-id="79cb1-170">policyDetails</span></span>|<span data-ttu-id="79cb1-171">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)集合</span><span class="sxs-lookup"><span data-stu-id="79cb1-171">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="79cb1-172">策略详细信息</span><span class="sxs-lookup"><span data-stu-id="79cb1-172">Policy Details</span></span>|

## <a name="relationships"></a><span data-ttu-id="79cb1-173">关系</span><span class="sxs-lookup"><span data-stu-id="79cb1-173">Relationships</span></span>
<span data-ttu-id="79cb1-174">无</span><span class="sxs-lookup"><span data-stu-id="79cb1-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79cb1-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79cb1-175">JSON Representation</span></span>
<span data-ttu-id="79cb1-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79cb1-176">Here is a JSON representation of the resource.</span></span>
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



