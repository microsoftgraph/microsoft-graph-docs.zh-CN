---
title: 创建 managedDeviceEncryptionState
description: 创建新的 managedDeviceEncryptionState 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e07632944ff5ba2230b25214dd767aed94d47f05
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43431970"
---
# <a name="create-manageddeviceencryptionstate"></a><span data-ttu-id="2867c-103">创建 managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="2867c-103">Create managedDeviceEncryptionState</span></span>

<span data-ttu-id="2867c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2867c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2867c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2867c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2867c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2867c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2867c-107">创建新的[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2867c-107">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2867c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2867c-108">Prerequisites</span></span>
<span data-ttu-id="2867c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2867c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2867c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2867c-111">Permission type</span></span>|<span data-ttu-id="2867c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2867c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2867c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2867c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2867c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2867c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2867c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2867c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2867c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2867c-116">Not supported.</span></span>|
|<span data-ttu-id="2867c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2867c-117">Application</span></span>|<span data-ttu-id="2867c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2867c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2867c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2867c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a><span data-ttu-id="2867c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2867c-120">Request headers</span></span>
|<span data-ttu-id="2867c-121">标头</span><span class="sxs-lookup"><span data-stu-id="2867c-121">Header</span></span>|<span data-ttu-id="2867c-122">值</span><span class="sxs-lookup"><span data-stu-id="2867c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2867c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2867c-123">Authorization</span></span>|<span data-ttu-id="2867c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2867c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2867c-125">接受</span><span class="sxs-lookup"><span data-stu-id="2867c-125">Accept</span></span>|<span data-ttu-id="2867c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2867c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2867c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2867c-127">Request body</span></span>
<span data-ttu-id="2867c-128">在请求正文中，提供 managedDeviceEncryptionState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2867c-128">In the request body, supply a JSON representation for the managedDeviceEncryptionState object.</span></span>

<span data-ttu-id="2867c-129">下表显示创建 managedDeviceEncryptionState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2867c-129">The following table shows the properties that are required when you create the managedDeviceEncryptionState.</span></span>

|<span data-ttu-id="2867c-130">属性</span><span class="sxs-lookup"><span data-stu-id="2867c-130">Property</span></span>|<span data-ttu-id="2867c-131">类型</span><span class="sxs-lookup"><span data-stu-id="2867c-131">Type</span></span>|<span data-ttu-id="2867c-132">说明</span><span class="sxs-lookup"><span data-stu-id="2867c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2867c-133">id</span><span class="sxs-lookup"><span data-stu-id="2867c-133">id</span></span>|<span data-ttu-id="2867c-134">String</span><span class="sxs-lookup"><span data-stu-id="2867c-134">String</span></span>|<span data-ttu-id="2867c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2867c-135">Key of the entity.</span></span>|
|<span data-ttu-id="2867c-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2867c-136">userPrincipalName</span></span>|<span data-ttu-id="2867c-137">String</span><span class="sxs-lookup"><span data-stu-id="2867c-137">String</span></span>|<span data-ttu-id="2867c-138">用户名</span><span class="sxs-lookup"><span data-stu-id="2867c-138">User name</span></span>|
|<span data-ttu-id="2867c-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="2867c-139">deviceType</span></span>|[<span data-ttu-id="2867c-140">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="2867c-140">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="2867c-141">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="2867c-141">Platform of the device.</span></span> <span data-ttu-id="2867c-142">可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `palm` `unknown`、、、、、、、、、、、、、、、、、、、。 `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry`</span><span class="sxs-lookup"><span data-stu-id="2867c-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="2867c-143">osVersion</span><span class="sxs-lookup"><span data-stu-id="2867c-143">osVersion</span></span>|<span data-ttu-id="2867c-144">String</span><span class="sxs-lookup"><span data-stu-id="2867c-144">String</span></span>|<span data-ttu-id="2867c-145">设备的操作系统版本</span><span class="sxs-lookup"><span data-stu-id="2867c-145">Operating system version of the device</span></span>|
|<span data-ttu-id="2867c-146">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="2867c-146">tpmSpecificationVersion</span></span>|<span data-ttu-id="2867c-147">String</span><span class="sxs-lookup"><span data-stu-id="2867c-147">String</span></span>|<span data-ttu-id="2867c-148">设备 TPM 版本</span><span class="sxs-lookup"><span data-stu-id="2867c-148">Device TPM Version</span></span>|
|<span data-ttu-id="2867c-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="2867c-149">deviceName</span></span>|<span data-ttu-id="2867c-150">String</span><span class="sxs-lookup"><span data-stu-id="2867c-150">String</span></span>|<span data-ttu-id="2867c-151">设备名称</span><span class="sxs-lookup"><span data-stu-id="2867c-151">Device name</span></span>|
|<span data-ttu-id="2867c-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="2867c-152">encryptionReadinessState</span></span>|[<span data-ttu-id="2867c-153">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="2867c-153">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="2867c-154">加密准备情况状态。</span><span class="sxs-lookup"><span data-stu-id="2867c-154">Encryption readiness state.</span></span> <span data-ttu-id="2867c-155">可取值为：`notReady`、`ready`。</span><span class="sxs-lookup"><span data-stu-id="2867c-155">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="2867c-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="2867c-156">encryptionState</span></span>|[<span data-ttu-id="2867c-157">encryptionState</span><span class="sxs-lookup"><span data-stu-id="2867c-157">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="2867c-158">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="2867c-158">Device encryption state.</span></span> <span data-ttu-id="2867c-159">可取值为：`notEncrypted`、`encrypted`。</span><span class="sxs-lookup"><span data-stu-id="2867c-159">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="2867c-160">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="2867c-160">encryptionPolicySettingState</span></span>|[<span data-ttu-id="2867c-161">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2867c-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2867c-162">加密策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="2867c-162">Encryption policy setting state.</span></span> <span data-ttu-id="2867c-163">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="2867c-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2867c-164">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="2867c-164">advancedBitLockerStates</span></span>|[<span data-ttu-id="2867c-165">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="2867c-165">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="2867c-166">高级 BitLocker 状态。</span><span class="sxs-lookup"><span data-stu-id="2867c-166">Advanced BitLocker State.</span></span> <span data-ttu-id="2867c-167">可能的值是`success`： `noUserConsent`、 `osVolumeEncryptionMethodMismatch`、 `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `recoveryKeyBackupFailed` `networkError`、、 `fixedDriveNotEncrypted`、、、、、、、、、、、、。 `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady`</span><span class="sxs-lookup"><span data-stu-id="2867c-167">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="2867c-168">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="2867c-168">fileVaultStates</span></span>|[<span data-ttu-id="2867c-169">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="2867c-169">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="2867c-170">FileVault 状态。</span><span class="sxs-lookup"><span data-stu-id="2867c-170">FileVault State.</span></span> <span data-ttu-id="2867c-171">可取值为：`success`、`driveEncryptedByUser`、`userDeferredEncryption`、`escrowNotEnabled`。</span><span class="sxs-lookup"><span data-stu-id="2867c-171">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="2867c-172">policyDetails</span><span class="sxs-lookup"><span data-stu-id="2867c-172">policyDetails</span></span>|<span data-ttu-id="2867c-173">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)集合</span><span class="sxs-lookup"><span data-stu-id="2867c-173">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="2867c-174">策略详细信息</span><span class="sxs-lookup"><span data-stu-id="2867c-174">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="2867c-175">响应</span><span class="sxs-lookup"><span data-stu-id="2867c-175">Response</span></span>
<span data-ttu-id="2867c-176">如果成功，此方法在响应`201 Created`正文中返回响应代码和[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2867c-176">If successful, this method returns a `201 Created` response code and a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2867c-177">示例</span><span class="sxs-lookup"><span data-stu-id="2867c-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="2867c-178">请求</span><span class="sxs-lookup"><span data-stu-id="2867c-178">Request</span></span>
<span data-ttu-id="2867c-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2867c-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates
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

### <a name="response"></a><span data-ttu-id="2867c-180">响应</span><span class="sxs-lookup"><span data-stu-id="2867c-180">Response</span></span>
<span data-ttu-id="2867c-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2867c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



