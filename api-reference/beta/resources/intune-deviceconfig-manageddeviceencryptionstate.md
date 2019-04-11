---
title: managedDeviceEncryptionState 资源类型
description: 每个设备的加密报告
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9193c795f9c488b5f157014c81d00a4b5118d149
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779872"
---
# <a name="manageddeviceencryptionstate-resource-type"></a><span data-ttu-id="6053e-103">managedDeviceEncryptionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="6053e-103">managedDeviceEncryptionState resource type</span></span>

> <span data-ttu-id="6053e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6053e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6053e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6053e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6053e-106">每个设备的加密报告</span><span class="sxs-lookup"><span data-stu-id="6053e-106">Encryption report per device</span></span>

## <a name="methods"></a><span data-ttu-id="6053e-107">方法</span><span class="sxs-lookup"><span data-stu-id="6053e-107">Methods</span></span>
|<span data-ttu-id="6053e-108">方法</span><span class="sxs-lookup"><span data-stu-id="6053e-108">Method</span></span>|<span data-ttu-id="6053e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="6053e-109">Return Type</span></span>|<span data-ttu-id="6053e-110">说明</span><span class="sxs-lookup"><span data-stu-id="6053e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6053e-111">列出 managedDeviceEncryptionStates</span><span class="sxs-lookup"><span data-stu-id="6053e-111">List managedDeviceEncryptionStates</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|<span data-ttu-id="6053e-112">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="6053e-112">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) collection</span></span>|<span data-ttu-id="6053e-113">列出[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6053e-113">List properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects.</span></span>|
|[<span data-ttu-id="6053e-114">获取 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="6053e-114">Get managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[<span data-ttu-id="6053e-115">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="6053e-115">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="6053e-116">读取[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6053e-116">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="6053e-117">创建 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="6053e-117">Create managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[<span data-ttu-id="6053e-118">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="6053e-118">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="6053e-119">创建新的[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6053e-119">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="6053e-120">删除 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="6053e-120">Delete managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|<span data-ttu-id="6053e-121">无</span><span class="sxs-lookup"><span data-stu-id="6053e-121">None</span></span>|<span data-ttu-id="6053e-122">删除[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)。</span><span class="sxs-lookup"><span data-stu-id="6053e-122">Deletes a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>|
|[<span data-ttu-id="6053e-123">更新 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="6053e-123">Update managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[<span data-ttu-id="6053e-124">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="6053e-124">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="6053e-125">更新[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6053e-125">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6053e-126">属性</span><span class="sxs-lookup"><span data-stu-id="6053e-126">Properties</span></span>
|<span data-ttu-id="6053e-127">属性</span><span class="sxs-lookup"><span data-stu-id="6053e-127">Property</span></span>|<span data-ttu-id="6053e-128">类型</span><span class="sxs-lookup"><span data-stu-id="6053e-128">Type</span></span>|<span data-ttu-id="6053e-129">说明</span><span class="sxs-lookup"><span data-stu-id="6053e-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6053e-130">id</span><span class="sxs-lookup"><span data-stu-id="6053e-130">id</span></span>|<span data-ttu-id="6053e-131">String</span><span class="sxs-lookup"><span data-stu-id="6053e-131">String</span></span>|<span data-ttu-id="6053e-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6053e-132">Key of the entity.</span></span>|
|<span data-ttu-id="6053e-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6053e-133">userPrincipalName</span></span>|<span data-ttu-id="6053e-134">String</span><span class="sxs-lookup"><span data-stu-id="6053e-134">String</span></span>|<span data-ttu-id="6053e-135">用户名</span><span class="sxs-lookup"><span data-stu-id="6053e-135">User name</span></span>|
|<span data-ttu-id="6053e-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="6053e-136">deviceType</span></span>|[<span data-ttu-id="6053e-137">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="6053e-137">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="6053e-138">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="6053e-138">Platform of the device.</span></span> <span data-ttu-id="6053e-139">可能的值为`desktop`: `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="6053e-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="6053e-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="6053e-140">osVersion</span></span>|<span data-ttu-id="6053e-141">String</span><span class="sxs-lookup"><span data-stu-id="6053e-141">String</span></span>|<span data-ttu-id="6053e-142">设备的操作系统版本</span><span class="sxs-lookup"><span data-stu-id="6053e-142">Operating system version of the device</span></span>|
|<span data-ttu-id="6053e-143">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="6053e-143">tpmSpecificationVersion</span></span>|<span data-ttu-id="6053e-144">String</span><span class="sxs-lookup"><span data-stu-id="6053e-144">String</span></span>|<span data-ttu-id="6053e-145">设备 TPM 版本</span><span class="sxs-lookup"><span data-stu-id="6053e-145">Device TPM Version</span></span>|
|<span data-ttu-id="6053e-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="6053e-146">deviceName</span></span>|<span data-ttu-id="6053e-147">String</span><span class="sxs-lookup"><span data-stu-id="6053e-147">String</span></span>|<span data-ttu-id="6053e-148">设备名称</span><span class="sxs-lookup"><span data-stu-id="6053e-148">Device name</span></span>|
|<span data-ttu-id="6053e-149">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="6053e-149">encryptionReadinessState</span></span>|[<span data-ttu-id="6053e-150">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="6053e-150">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="6053e-151">加密准备情况状态。</span><span class="sxs-lookup"><span data-stu-id="6053e-151">Encryption readiness state.</span></span> <span data-ttu-id="6053e-152">可取值为：`notReady`、`ready`。</span><span class="sxs-lookup"><span data-stu-id="6053e-152">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="6053e-153">encryptionState</span><span class="sxs-lookup"><span data-stu-id="6053e-153">encryptionState</span></span>|[<span data-ttu-id="6053e-154">encryptionState</span><span class="sxs-lookup"><span data-stu-id="6053e-154">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="6053e-155">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="6053e-155">Device encryption state.</span></span> <span data-ttu-id="6053e-156">可取值为：`notEncrypted`、`encrypted`。</span><span class="sxs-lookup"><span data-stu-id="6053e-156">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="6053e-157">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="6053e-157">encryptionPolicySettingState</span></span>|[<span data-ttu-id="6053e-158">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="6053e-158">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6053e-159">加密策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="6053e-159">Encryption policy setting state.</span></span> <span data-ttu-id="6053e-160">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="6053e-160">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6053e-161">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="6053e-161">advancedBitLockerStates</span></span>|[<span data-ttu-id="6053e-162">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="6053e-162">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="6053e-163">高级 BitLocker 状态。</span><span class="sxs-lookup"><span data-stu-id="6053e-163">Advanced BitLocker State.</span></span> <span data-ttu-id="6053e-164">可能的值是`success`: `noUserConsent`、 `osVolumeEncryptionMethodMismatch`、 `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `recoveryKeyBackupFailed` `networkError`、、 `fixedDriveNotEncrypted`、、、、、、、、、、、、。 `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady`</span><span class="sxs-lookup"><span data-stu-id="6053e-164">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="6053e-165">policyDetails</span><span class="sxs-lookup"><span data-stu-id="6053e-165">policyDetails</span></span>|<span data-ttu-id="6053e-166">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)集合</span><span class="sxs-lookup"><span data-stu-id="6053e-166">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="6053e-167">策略详细信息</span><span class="sxs-lookup"><span data-stu-id="6053e-167">Policy Details</span></span>|

## <a name="relationships"></a><span data-ttu-id="6053e-168">关系</span><span class="sxs-lookup"><span data-stu-id="6053e-168">Relationships</span></span>
<span data-ttu-id="6053e-169">无</span><span class="sxs-lookup"><span data-stu-id="6053e-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6053e-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6053e-170">JSON Representation</span></span>
<span data-ttu-id="6053e-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6053e-171">Here is a JSON representation of the resource.</span></span>
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





