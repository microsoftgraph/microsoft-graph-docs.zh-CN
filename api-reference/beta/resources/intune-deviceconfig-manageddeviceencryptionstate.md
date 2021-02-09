---
title: managedDeviceEncryptionState 资源类型
description: 每个设备的加密报告
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9fb45813f19ef2ef33653902c4468cedf7aed3e7
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154255"
---
# <a name="manageddeviceencryptionstate-resource-type"></a><span data-ttu-id="9759d-103">managedDeviceEncryptionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="9759d-103">managedDeviceEncryptionState resource type</span></span>

<span data-ttu-id="9759d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9759d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9759d-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9759d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9759d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9759d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9759d-107">每个设备的加密报告</span><span class="sxs-lookup"><span data-stu-id="9759d-107">Encryption report per device</span></span>

## <a name="methods"></a><span data-ttu-id="9759d-108">方法</span><span class="sxs-lookup"><span data-stu-id="9759d-108">Methods</span></span>
|<span data-ttu-id="9759d-109">方法</span><span class="sxs-lookup"><span data-stu-id="9759d-109">Method</span></span>|<span data-ttu-id="9759d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9759d-110">Return Type</span></span>|<span data-ttu-id="9759d-111">说明</span><span class="sxs-lookup"><span data-stu-id="9759d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9759d-112">列出 managedDeviceEncryptionStates</span><span class="sxs-lookup"><span data-stu-id="9759d-112">List managedDeviceEncryptionStates</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|<span data-ttu-id="9759d-113">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9759d-113">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) collection</span></span>|<span data-ttu-id="9759d-114">列出 [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9759d-114">List properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects.</span></span>|
|[<span data-ttu-id="9759d-115">获取 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="9759d-115">Get managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[<span data-ttu-id="9759d-116">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="9759d-116">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="9759d-117">读取 [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9759d-117">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="9759d-118">创建 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="9759d-118">Create managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[<span data-ttu-id="9759d-119">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="9759d-119">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="9759d-120">创建新的 [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9759d-120">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="9759d-121">删除 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="9759d-121">Delete managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|<span data-ttu-id="9759d-122">无</span><span class="sxs-lookup"><span data-stu-id="9759d-122">None</span></span>|<span data-ttu-id="9759d-123">删除 [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)。</span><span class="sxs-lookup"><span data-stu-id="9759d-123">Deletes a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>|
|[<span data-ttu-id="9759d-124">更新 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="9759d-124">Update managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[<span data-ttu-id="9759d-125">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="9759d-125">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="9759d-126">更新 [managedDeviceEncryptionState 对象](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="9759d-126">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9759d-127">属性</span><span class="sxs-lookup"><span data-stu-id="9759d-127">Properties</span></span>
|<span data-ttu-id="9759d-128">属性</span><span class="sxs-lookup"><span data-stu-id="9759d-128">Property</span></span>|<span data-ttu-id="9759d-129">类型</span><span class="sxs-lookup"><span data-stu-id="9759d-129">Type</span></span>|<span data-ttu-id="9759d-130">说明</span><span class="sxs-lookup"><span data-stu-id="9759d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9759d-131">id</span><span class="sxs-lookup"><span data-stu-id="9759d-131">id</span></span>|<span data-ttu-id="9759d-132">String</span><span class="sxs-lookup"><span data-stu-id="9759d-132">String</span></span>|<span data-ttu-id="9759d-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9759d-133">Key of the entity.</span></span>|
|<span data-ttu-id="9759d-134">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9759d-134">userPrincipalName</span></span>|<span data-ttu-id="9759d-135">String</span><span class="sxs-lookup"><span data-stu-id="9759d-135">String</span></span>|<span data-ttu-id="9759d-136">用户名</span><span class="sxs-lookup"><span data-stu-id="9759d-136">User name</span></span>|
|<span data-ttu-id="9759d-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="9759d-137">deviceType</span></span>|[<span data-ttu-id="9759d-138">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="9759d-138">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="9759d-139">设备平台。</span><span class="sxs-lookup"><span data-stu-id="9759d-139">Platform of the device.</span></span> <span data-ttu-id="9759d-140">可能的值是： `desktop` ， ， ， ， ， ， `windowsRT` ， `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` 。</span><span class="sxs-lookup"><span data-stu-id="9759d-140">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="9759d-141">osVersion</span><span class="sxs-lookup"><span data-stu-id="9759d-141">osVersion</span></span>|<span data-ttu-id="9759d-142">String</span><span class="sxs-lookup"><span data-stu-id="9759d-142">String</span></span>|<span data-ttu-id="9759d-143">设备的操作系统版本</span><span class="sxs-lookup"><span data-stu-id="9759d-143">Operating system version of the device</span></span>|
|<span data-ttu-id="9759d-144">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="9759d-144">tpmSpecificationVersion</span></span>|<span data-ttu-id="9759d-145">String</span><span class="sxs-lookup"><span data-stu-id="9759d-145">String</span></span>|<span data-ttu-id="9759d-146">设备 TPM 版本</span><span class="sxs-lookup"><span data-stu-id="9759d-146">Device TPM Version</span></span>|
|<span data-ttu-id="9759d-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="9759d-147">deviceName</span></span>|<span data-ttu-id="9759d-148">String</span><span class="sxs-lookup"><span data-stu-id="9759d-148">String</span></span>|<span data-ttu-id="9759d-149">设备名称</span><span class="sxs-lookup"><span data-stu-id="9759d-149">Device name</span></span>|
|<span data-ttu-id="9759d-150">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="9759d-150">encryptionReadinessState</span></span>|[<span data-ttu-id="9759d-151">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="9759d-151">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="9759d-152">加密准备状态。</span><span class="sxs-lookup"><span data-stu-id="9759d-152">Encryption readiness state.</span></span> <span data-ttu-id="9759d-153">可取值为：`notReady`、`ready`。</span><span class="sxs-lookup"><span data-stu-id="9759d-153">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="9759d-154">encryptionState</span><span class="sxs-lookup"><span data-stu-id="9759d-154">encryptionState</span></span>|[<span data-ttu-id="9759d-155">encryptionState</span><span class="sxs-lookup"><span data-stu-id="9759d-155">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="9759d-156">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="9759d-156">Device encryption state.</span></span> <span data-ttu-id="9759d-157">可取值为：`notEncrypted`、`encrypted`。</span><span class="sxs-lookup"><span data-stu-id="9759d-157">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="9759d-158">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="9759d-158">encryptionPolicySettingState</span></span>|[<span data-ttu-id="9759d-159">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="9759d-159">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="9759d-160">加密策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="9759d-160">Encryption policy setting state.</span></span> <span data-ttu-id="9759d-161">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="9759d-161">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="9759d-162">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="9759d-162">advancedBitLockerStates</span></span>|[<span data-ttu-id="9759d-163">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="9759d-163">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="9759d-164">高级 BitLocker 状态。</span><span class="sxs-lookup"><span data-stu-id="9759d-164">Advanced BitLocker State.</span></span> <span data-ttu-id="9759d-165">可能的值是： `success` ， ， ， ， ， ， ， ， `noUserConsent` ， `osVolumeUnprotected` `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeEncryptionMethodMismatch` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` ， `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady` `networkError` ， 。</span><span class="sxs-lookup"><span data-stu-id="9759d-165">Possible values are: `success`, `noUserConsent`, `osVolumeUnprotected`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeEncryptionMethodMismatch`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="9759d-166">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="9759d-166">fileVaultStates</span></span>|[<span data-ttu-id="9759d-167">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="9759d-167">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="9759d-168">FileVault 状态。</span><span class="sxs-lookup"><span data-stu-id="9759d-168">FileVault State.</span></span> <span data-ttu-id="9759d-169">可取值为：`success`、`driveEncryptedByUser`、`userDeferredEncryption`、`escrowNotEnabled`。</span><span class="sxs-lookup"><span data-stu-id="9759d-169">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="9759d-170">policyDetails</span><span class="sxs-lookup"><span data-stu-id="9759d-170">policyDetails</span></span>|<span data-ttu-id="9759d-171">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9759d-171">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="9759d-172">策略详细信息</span><span class="sxs-lookup"><span data-stu-id="9759d-172">Policy Details</span></span>|

## <a name="relationships"></a><span data-ttu-id="9759d-173">关系</span><span class="sxs-lookup"><span data-stu-id="9759d-173">Relationships</span></span>
<span data-ttu-id="9759d-174">无</span><span class="sxs-lookup"><span data-stu-id="9759d-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9759d-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9759d-175">JSON Representation</span></span>
<span data-ttu-id="9759d-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9759d-176">Here is a JSON representation of the resource.</span></span>
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




