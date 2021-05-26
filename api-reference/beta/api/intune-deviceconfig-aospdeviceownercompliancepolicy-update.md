---
title: 更新 aospDeviceOwnerCompliancePolicy
description: 更新 aospDeviceOwnerCompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7a90ab0d19a6dba44a42b653556c71b01e2011c
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665734"
---
# <a name="update-aospdeviceownercompliancepolicy"></a><span data-ttu-id="d83e3-103">更新 aospDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d83e3-103">Update aospDeviceOwnerCompliancePolicy</span></span>

<span data-ttu-id="d83e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d83e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d83e3-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d83e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d83e3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d83e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d83e3-107">更新 [aospDeviceOwnerCompliancePolicy 对象](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="d83e3-107">Update the properties of a [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d83e3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d83e3-108">Prerequisites</span></span>
<span data-ttu-id="d83e3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d83e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d83e3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d83e3-111">Permission type</span></span>|<span data-ttu-id="d83e3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d83e3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d83e3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d83e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d83e3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d83e3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d83e3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d83e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d83e3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d83e3-116">Not supported.</span></span>|
|<span data-ttu-id="d83e3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d83e3-117">Application</span></span>|<span data-ttu-id="d83e3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d83e3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d83e3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d83e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="d83e3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d83e3-120">Request headers</span></span>
|<span data-ttu-id="d83e3-121">标头</span><span class="sxs-lookup"><span data-stu-id="d83e3-121">Header</span></span>|<span data-ttu-id="d83e3-122">值</span><span class="sxs-lookup"><span data-stu-id="d83e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d83e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d83e3-123">Authorization</span></span>|<span data-ttu-id="d83e3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d83e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d83e3-125">接受</span><span class="sxs-lookup"><span data-stu-id="d83e3-125">Accept</span></span>|<span data-ttu-id="d83e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d83e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d83e3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d83e3-127">Request body</span></span>
<span data-ttu-id="d83e3-128">在请求正文中，提供 [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d83e3-128">In the request body, supply a JSON representation for the [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="d83e3-129">下表显示创建 [aospDeviceOwnerCompliancePolicy 时所需的属性](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="d83e3-129">The following table shows the properties that are required when you create the [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="d83e3-130">属性</span><span class="sxs-lookup"><span data-stu-id="d83e3-130">Property</span></span>|<span data-ttu-id="d83e3-131">类型</span><span class="sxs-lookup"><span data-stu-id="d83e3-131">Type</span></span>|<span data-ttu-id="d83e3-132">说明</span><span class="sxs-lookup"><span data-stu-id="d83e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d83e3-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d83e3-133">roleScopeTagIds</span></span>|<span data-ttu-id="d83e3-134">String collection</span><span class="sxs-lookup"><span data-stu-id="d83e3-134">String collection</span></span>|<span data-ttu-id="d83e3-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d83e3-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d83e3-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d83e3-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d83e3-137">id</span><span class="sxs-lookup"><span data-stu-id="d83e3-137">id</span></span>|<span data-ttu-id="d83e3-138">String</span><span class="sxs-lookup"><span data-stu-id="d83e3-138">String</span></span>|<span data-ttu-id="d83e3-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d83e3-139">Key of the entity.</span></span> <span data-ttu-id="d83e3-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d83e3-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d83e3-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d83e3-141">createdDateTime</span></span>|<span data-ttu-id="d83e3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d83e3-142">DateTimeOffset</span></span>|<span data-ttu-id="d83e3-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d83e3-143">DateTime the object was created.</span></span> <span data-ttu-id="d83e3-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d83e3-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d83e3-145">说明</span><span class="sxs-lookup"><span data-stu-id="d83e3-145">description</span></span>|<span data-ttu-id="d83e3-146">String</span><span class="sxs-lookup"><span data-stu-id="d83e3-146">String</span></span>|<span data-ttu-id="d83e3-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d83e3-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d83e3-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d83e3-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d83e3-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d83e3-149">lastModifiedDateTime</span></span>|<span data-ttu-id="d83e3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d83e3-150">DateTimeOffset</span></span>|<span data-ttu-id="d83e3-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d83e3-151">DateTime the object was last modified.</span></span> <span data-ttu-id="d83e3-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d83e3-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d83e3-153">displayName</span><span class="sxs-lookup"><span data-stu-id="d83e3-153">displayName</span></span>|<span data-ttu-id="d83e3-154">String</span><span class="sxs-lookup"><span data-stu-id="d83e3-154">String</span></span>|<span data-ttu-id="d83e3-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d83e3-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d83e3-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d83e3-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d83e3-157">version</span><span class="sxs-lookup"><span data-stu-id="d83e3-157">version</span></span>|<span data-ttu-id="d83e3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d83e3-158">Int32</span></span>|<span data-ttu-id="d83e3-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d83e3-159">Version of the device configuration.</span></span> <span data-ttu-id="d83e3-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d83e3-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d83e3-161">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="d83e3-161">osMinimumVersion</span></span>|<span data-ttu-id="d83e3-162">String</span><span class="sxs-lookup"><span data-stu-id="d83e3-162">String</span></span>|<span data-ttu-id="d83e3-163">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="d83e3-163">Minimum Android version.</span></span>|
|<span data-ttu-id="d83e3-164">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="d83e3-164">osMaximumVersion</span></span>|<span data-ttu-id="d83e3-165">String</span><span class="sxs-lookup"><span data-stu-id="d83e3-165">String</span></span>|<span data-ttu-id="d83e3-166">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="d83e3-166">Maximum Android version.</span></span>|
|<span data-ttu-id="d83e3-167">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="d83e3-167">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="d83e3-168">String</span><span class="sxs-lookup"><span data-stu-id="d83e3-168">String</span></span>|<span data-ttu-id="d83e3-169">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="d83e3-169">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="d83e3-170">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="d83e3-170">passwordRequired</span></span>|<span data-ttu-id="d83e3-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="d83e3-171">Boolean</span></span>|<span data-ttu-id="d83e3-172">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="d83e3-172">Require a password to unlock device.</span></span>|
|<span data-ttu-id="d83e3-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d83e3-173">passwordRequiredType</span></span>|[<span data-ttu-id="d83e3-174">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d83e3-174">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="d83e3-175">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="d83e3-175">Type of characters in password.</span></span> <span data-ttu-id="d83e3-176">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="d83e3-176">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="d83e3-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d83e3-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d83e3-178">Int32</span><span class="sxs-lookup"><span data-stu-id="d83e3-178">Int32</span></span>|<span data-ttu-id="d83e3-179">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="d83e3-179">Minutes of inactivity before a password is required.</span></span> <span data-ttu-id="d83e3-180">有效值为 1 到 8640</span><span class="sxs-lookup"><span data-stu-id="d83e3-180">Valid values 1 to 8640</span></span>|
|<span data-ttu-id="d83e3-181">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d83e3-181">passwordMinimumLength</span></span>|<span data-ttu-id="d83e3-182">Int32</span><span class="sxs-lookup"><span data-stu-id="d83e3-182">Int32</span></span>|<span data-ttu-id="d83e3-183">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="d83e3-183">Minimum password length.</span></span> <span data-ttu-id="d83e3-184">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="d83e3-184">Valid values 4 to 16</span></span>|
|<span data-ttu-id="d83e3-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="d83e3-185">storageRequireEncryption</span></span>|<span data-ttu-id="d83e3-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="d83e3-186">Boolean</span></span>|<span data-ttu-id="d83e3-187">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="d83e3-187">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="d83e3-188">响应</span><span class="sxs-lookup"><span data-stu-id="d83e3-188">Response</span></span>
<span data-ttu-id="d83e3-189">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d83e3-189">If successful, this method returns a `200 OK` response code and an updated [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d83e3-190">示例</span><span class="sxs-lookup"><span data-stu-id="d83e3-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="d83e3-191">请求</span><span class="sxs-lookup"><span data-stu-id="d83e3-191">Request</span></span>
<span data-ttu-id="d83e3-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d83e3-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 593

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumLength": 5,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="d83e3-193">响应</span><span class="sxs-lookup"><span data-stu-id="d83e3-193">Response</span></span>
<span data-ttu-id="d83e3-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d83e3-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 765

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "0837b942-b942-0837-42b9-370842b93708",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumLength": 5,
  "storageRequireEncryption": true
}
```




