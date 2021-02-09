---
title: 更新 managedDeviceEncryptionState
description: 更新 managedDeviceEncryptionState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c56f5de19c483d9d78648278e61e2f84bd1c27dd
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157006"
---
# <a name="update-manageddeviceencryptionstate"></a><span data-ttu-id="9aca1-103">更新 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="9aca1-103">Update managedDeviceEncryptionState</span></span>

<span data-ttu-id="9aca1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9aca1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9aca1-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9aca1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9aca1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9aca1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9aca1-107">更新 [managedDeviceEncryptionState 对象](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="9aca1-107">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9aca1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9aca1-108">Prerequisites</span></span>
<span data-ttu-id="9aca1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9aca1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9aca1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9aca1-111">Permission type</span></span>|<span data-ttu-id="9aca1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9aca1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9aca1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9aca1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9aca1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9aca1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9aca1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9aca1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9aca1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9aca1-116">Not supported.</span></span>|
|<span data-ttu-id="9aca1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9aca1-117">Application</span></span>|<span data-ttu-id="9aca1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9aca1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9aca1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9aca1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="request-headers"></a><span data-ttu-id="9aca1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9aca1-120">Request headers</span></span>
|<span data-ttu-id="9aca1-121">标头</span><span class="sxs-lookup"><span data-stu-id="9aca1-121">Header</span></span>|<span data-ttu-id="9aca1-122">值</span><span class="sxs-lookup"><span data-stu-id="9aca1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9aca1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9aca1-123">Authorization</span></span>|<span data-ttu-id="9aca1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9aca1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9aca1-125">接受</span><span class="sxs-lookup"><span data-stu-id="9aca1-125">Accept</span></span>|<span data-ttu-id="9aca1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9aca1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9aca1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9aca1-127">Request body</span></span>
<span data-ttu-id="9aca1-128">在请求正文中，提供 [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9aca1-128">In the request body, supply a JSON representation for the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

<span data-ttu-id="9aca1-129">下表显示创建 [managedDeviceEncryptionState 时所需的属性](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)。</span><span class="sxs-lookup"><span data-stu-id="9aca1-129">The following table shows the properties that are required when you create the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>

|<span data-ttu-id="9aca1-130">属性</span><span class="sxs-lookup"><span data-stu-id="9aca1-130">Property</span></span>|<span data-ttu-id="9aca1-131">类型</span><span class="sxs-lookup"><span data-stu-id="9aca1-131">Type</span></span>|<span data-ttu-id="9aca1-132">说明</span><span class="sxs-lookup"><span data-stu-id="9aca1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aca1-133">id</span><span class="sxs-lookup"><span data-stu-id="9aca1-133">id</span></span>|<span data-ttu-id="9aca1-134">String</span><span class="sxs-lookup"><span data-stu-id="9aca1-134">String</span></span>|<span data-ttu-id="9aca1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9aca1-135">Key of the entity.</span></span>|
|<span data-ttu-id="9aca1-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9aca1-136">userPrincipalName</span></span>|<span data-ttu-id="9aca1-137">String</span><span class="sxs-lookup"><span data-stu-id="9aca1-137">String</span></span>|<span data-ttu-id="9aca1-138">用户名</span><span class="sxs-lookup"><span data-stu-id="9aca1-138">User name</span></span>|
|<span data-ttu-id="9aca1-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="9aca1-139">deviceType</span></span>|[<span data-ttu-id="9aca1-140">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="9aca1-140">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="9aca1-141">设备平台。</span><span class="sxs-lookup"><span data-stu-id="9aca1-141">Platform of the device.</span></span> <span data-ttu-id="9aca1-142">可能的值是： `desktop` ， ， ， ， ， ， `windowsRT` ， `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` 。</span><span class="sxs-lookup"><span data-stu-id="9aca1-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="9aca1-143">osVersion</span><span class="sxs-lookup"><span data-stu-id="9aca1-143">osVersion</span></span>|<span data-ttu-id="9aca1-144">String</span><span class="sxs-lookup"><span data-stu-id="9aca1-144">String</span></span>|<span data-ttu-id="9aca1-145">设备的操作系统版本</span><span class="sxs-lookup"><span data-stu-id="9aca1-145">Operating system version of the device</span></span>|
|<span data-ttu-id="9aca1-146">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="9aca1-146">tpmSpecificationVersion</span></span>|<span data-ttu-id="9aca1-147">String</span><span class="sxs-lookup"><span data-stu-id="9aca1-147">String</span></span>|<span data-ttu-id="9aca1-148">设备 TPM 版本</span><span class="sxs-lookup"><span data-stu-id="9aca1-148">Device TPM Version</span></span>|
|<span data-ttu-id="9aca1-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="9aca1-149">deviceName</span></span>|<span data-ttu-id="9aca1-150">String</span><span class="sxs-lookup"><span data-stu-id="9aca1-150">String</span></span>|<span data-ttu-id="9aca1-151">设备名称</span><span class="sxs-lookup"><span data-stu-id="9aca1-151">Device name</span></span>|
|<span data-ttu-id="9aca1-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="9aca1-152">encryptionReadinessState</span></span>|[<span data-ttu-id="9aca1-153">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="9aca1-153">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="9aca1-154">加密准备状态。</span><span class="sxs-lookup"><span data-stu-id="9aca1-154">Encryption readiness state.</span></span> <span data-ttu-id="9aca1-155">可取值为：`notReady`、`ready`。</span><span class="sxs-lookup"><span data-stu-id="9aca1-155">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="9aca1-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="9aca1-156">encryptionState</span></span>|[<span data-ttu-id="9aca1-157">encryptionState</span><span class="sxs-lookup"><span data-stu-id="9aca1-157">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="9aca1-158">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="9aca1-158">Device encryption state.</span></span> <span data-ttu-id="9aca1-159">可取值为：`notEncrypted`、`encrypted`。</span><span class="sxs-lookup"><span data-stu-id="9aca1-159">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="9aca1-160">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="9aca1-160">encryptionPolicySettingState</span></span>|[<span data-ttu-id="9aca1-161">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="9aca1-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="9aca1-162">加密策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="9aca1-162">Encryption policy setting state.</span></span> <span data-ttu-id="9aca1-163">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="9aca1-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="9aca1-164">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="9aca1-164">advancedBitLockerStates</span></span>|[<span data-ttu-id="9aca1-165">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="9aca1-165">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="9aca1-166">高级 BitLocker 状态。</span><span class="sxs-lookup"><span data-stu-id="9aca1-166">Advanced BitLocker State.</span></span> <span data-ttu-id="9aca1-167">可能的值是： `success` ， ， ， ， ， ， ， ， `noUserConsent` ， `osVolumeUnprotected` `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeEncryptionMethodMismatch` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` ， `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady` `networkError` ， 。</span><span class="sxs-lookup"><span data-stu-id="9aca1-167">Possible values are: `success`, `noUserConsent`, `osVolumeUnprotected`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeEncryptionMethodMismatch`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="9aca1-168">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="9aca1-168">fileVaultStates</span></span>|[<span data-ttu-id="9aca1-169">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="9aca1-169">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="9aca1-170">FileVault 状态。</span><span class="sxs-lookup"><span data-stu-id="9aca1-170">FileVault State.</span></span> <span data-ttu-id="9aca1-171">可取值为：`success`、`driveEncryptedByUser`、`userDeferredEncryption`、`escrowNotEnabled`。</span><span class="sxs-lookup"><span data-stu-id="9aca1-171">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="9aca1-172">policyDetails</span><span class="sxs-lookup"><span data-stu-id="9aca1-172">policyDetails</span></span>|<span data-ttu-id="9aca1-173">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9aca1-173">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="9aca1-174">策略详细信息</span><span class="sxs-lookup"><span data-stu-id="9aca1-174">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="9aca1-175">响应</span><span class="sxs-lookup"><span data-stu-id="9aca1-175">Response</span></span>
<span data-ttu-id="9aca1-176">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9aca1-176">If successful, this method returns a `200 OK` response code and an updated [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9aca1-177">示例</span><span class="sxs-lookup"><span data-stu-id="9aca1-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="9aca1-178">请求</span><span class="sxs-lookup"><span data-stu-id="9aca1-178">Request</span></span>
<span data-ttu-id="9aca1-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9aca1-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9aca1-180">响应</span><span class="sxs-lookup"><span data-stu-id="9aca1-180">Response</span></span>
<span data-ttu-id="9aca1-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9aca1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




