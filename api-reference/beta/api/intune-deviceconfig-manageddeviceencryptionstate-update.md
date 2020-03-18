---
title: 更新 managedDeviceEncryptionState
description: 更新 managedDeviceEncryptionState 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6109a11d366aece7a1df1b86f4aae2459d696019
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42742979"
---
# <a name="update-manageddeviceencryptionstate"></a><span data-ttu-id="d1472-103">更新 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="d1472-103">Update managedDeviceEncryptionState</span></span>

> <span data-ttu-id="d1472-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1472-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1472-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1472-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1472-106">更新[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d1472-106">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1472-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d1472-107">Prerequisites</span></span>
<span data-ttu-id="d1472-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1472-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1472-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1472-110">Permission type</span></span>|<span data-ttu-id="d1472-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d1472-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1472-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1472-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1472-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1472-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1472-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1472-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1472-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1472-115">Not supported.</span></span>|
|<span data-ttu-id="d1472-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1472-116">Application</span></span>|<span data-ttu-id="d1472-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1472-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1472-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1472-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="request-headers"></a><span data-ttu-id="d1472-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1472-119">Request headers</span></span>
|<span data-ttu-id="d1472-120">标头</span><span class="sxs-lookup"><span data-stu-id="d1472-120">Header</span></span>|<span data-ttu-id="d1472-121">值</span><span class="sxs-lookup"><span data-stu-id="d1472-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1472-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1472-122">Authorization</span></span>|<span data-ttu-id="d1472-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d1472-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1472-124">接受</span><span class="sxs-lookup"><span data-stu-id="d1472-124">Accept</span></span>|<span data-ttu-id="d1472-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d1472-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1472-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1472-126">Request body</span></span>
<span data-ttu-id="d1472-127">在请求正文中，提供[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1472-127">In the request body, supply a JSON representation for the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

<span data-ttu-id="d1472-128">下表显示创建[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d1472-128">The following table shows the properties that are required when you create the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>

|<span data-ttu-id="d1472-129">属性</span><span class="sxs-lookup"><span data-stu-id="d1472-129">Property</span></span>|<span data-ttu-id="d1472-130">类型</span><span class="sxs-lookup"><span data-stu-id="d1472-130">Type</span></span>|<span data-ttu-id="d1472-131">说明</span><span class="sxs-lookup"><span data-stu-id="d1472-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1472-132">id</span><span class="sxs-lookup"><span data-stu-id="d1472-132">id</span></span>|<span data-ttu-id="d1472-133">String</span><span class="sxs-lookup"><span data-stu-id="d1472-133">String</span></span>|<span data-ttu-id="d1472-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d1472-134">Key of the entity.</span></span>|
|<span data-ttu-id="d1472-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d1472-135">userPrincipalName</span></span>|<span data-ttu-id="d1472-136">String</span><span class="sxs-lookup"><span data-stu-id="d1472-136">String</span></span>|<span data-ttu-id="d1472-137">用户名</span><span class="sxs-lookup"><span data-stu-id="d1472-137">User name</span></span>|
|<span data-ttu-id="d1472-138">deviceType</span><span class="sxs-lookup"><span data-stu-id="d1472-138">deviceType</span></span>|[<span data-ttu-id="d1472-139">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="d1472-139">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="d1472-140">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="d1472-140">Platform of the device.</span></span> <span data-ttu-id="d1472-141">可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `palm` `unknown`、、、、、、、、、、、、、、、、、、、。 `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry`</span><span class="sxs-lookup"><span data-stu-id="d1472-141">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="d1472-142">osVersion</span><span class="sxs-lookup"><span data-stu-id="d1472-142">osVersion</span></span>|<span data-ttu-id="d1472-143">String</span><span class="sxs-lookup"><span data-stu-id="d1472-143">String</span></span>|<span data-ttu-id="d1472-144">设备的操作系统版本</span><span class="sxs-lookup"><span data-stu-id="d1472-144">Operating system version of the device</span></span>|
|<span data-ttu-id="d1472-145">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="d1472-145">tpmSpecificationVersion</span></span>|<span data-ttu-id="d1472-146">String</span><span class="sxs-lookup"><span data-stu-id="d1472-146">String</span></span>|<span data-ttu-id="d1472-147">设备 TPM 版本</span><span class="sxs-lookup"><span data-stu-id="d1472-147">Device TPM Version</span></span>|
|<span data-ttu-id="d1472-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="d1472-148">deviceName</span></span>|<span data-ttu-id="d1472-149">String</span><span class="sxs-lookup"><span data-stu-id="d1472-149">String</span></span>|<span data-ttu-id="d1472-150">设备名称</span><span class="sxs-lookup"><span data-stu-id="d1472-150">Device name</span></span>|
|<span data-ttu-id="d1472-151">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="d1472-151">encryptionReadinessState</span></span>|[<span data-ttu-id="d1472-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="d1472-152">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="d1472-153">加密准备情况状态。</span><span class="sxs-lookup"><span data-stu-id="d1472-153">Encryption readiness state.</span></span> <span data-ttu-id="d1472-154">可取值为：`notReady`、`ready`。</span><span class="sxs-lookup"><span data-stu-id="d1472-154">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="d1472-155">encryptionState</span><span class="sxs-lookup"><span data-stu-id="d1472-155">encryptionState</span></span>|[<span data-ttu-id="d1472-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="d1472-156">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="d1472-157">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="d1472-157">Device encryption state.</span></span> <span data-ttu-id="d1472-158">可取值为：`notEncrypted`、`encrypted`。</span><span class="sxs-lookup"><span data-stu-id="d1472-158">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="d1472-159">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="d1472-159">encryptionPolicySettingState</span></span>|[<span data-ttu-id="d1472-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d1472-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d1472-161">加密策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="d1472-161">Encryption policy setting state.</span></span> <span data-ttu-id="d1472-162">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="d1472-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d1472-163">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="d1472-163">advancedBitLockerStates</span></span>|[<span data-ttu-id="d1472-164">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="d1472-164">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="d1472-165">高级 BitLocker 状态。</span><span class="sxs-lookup"><span data-stu-id="d1472-165">Advanced BitLocker State.</span></span> <span data-ttu-id="d1472-166">可能的值是`success`： `noUserConsent`、 `osVolumeEncryptionMethodMismatch`、 `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `recoveryKeyBackupFailed` `networkError`、、 `fixedDriveNotEncrypted`、、、、、、、、、、、、。 `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady`</span><span class="sxs-lookup"><span data-stu-id="d1472-166">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="d1472-167">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="d1472-167">fileVaultStates</span></span>|[<span data-ttu-id="d1472-168">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="d1472-168">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="d1472-169">FileVault 状态。</span><span class="sxs-lookup"><span data-stu-id="d1472-169">FileVault State.</span></span> <span data-ttu-id="d1472-170">可取值为：`success`、`driveEncryptedByUser`、`userDeferredEncryption`、`escrowNotEnabled`。</span><span class="sxs-lookup"><span data-stu-id="d1472-170">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="d1472-171">policyDetails</span><span class="sxs-lookup"><span data-stu-id="d1472-171">policyDetails</span></span>|<span data-ttu-id="d1472-172">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)集合</span><span class="sxs-lookup"><span data-stu-id="d1472-172">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="d1472-173">策略详细信息</span><span class="sxs-lookup"><span data-stu-id="d1472-173">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="d1472-174">响应</span><span class="sxs-lookup"><span data-stu-id="d1472-174">Response</span></span>
<span data-ttu-id="d1472-175">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d1472-175">If successful, this method returns a `200 OK` response code and an updated [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1472-176">示例</span><span class="sxs-lookup"><span data-stu-id="d1472-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1472-177">请求</span><span class="sxs-lookup"><span data-stu-id="d1472-177">Request</span></span>
<span data-ttu-id="d1472-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1472-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
Content-type: application/json
Content-length: 704

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "userPrincipalName": "User Principal Name value",
  "deviceType": "windowsRT",
  "osVersion": "Os Version value",
  "tpmSpecificationVersion": "Tpm Specification Version value",
  "deviceName": "Device Name value",
  "encryptionReadinessState": "ready",
  "encryptionState": "encrypted",
  "encryptionPolicySettingState": "notApplicable",
  "advancedBitLockerStates": "noUserConsent",
  "fileVaultStates": "driveEncryptedByUser",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d1472-179">响应</span><span class="sxs-lookup"><span data-stu-id="d1472-179">Response</span></span>
<span data-ttu-id="d1472-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d1472-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 753

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "f09b4ab6-4ab6-f09b-b64a-9bf0b64a9bf0",
  "userPrincipalName": "User Principal Name value",
  "deviceType": "windowsRT",
  "osVersion": "Os Version value",
  "tpmSpecificationVersion": "Tpm Specification Version value",
  "deviceName": "Device Name value",
  "encryptionReadinessState": "ready",
  "encryptionState": "encrypted",
  "encryptionPolicySettingState": "notApplicable",
  "advancedBitLockerStates": "noUserConsent",
  "fileVaultStates": "driveEncryptedByUser",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```




