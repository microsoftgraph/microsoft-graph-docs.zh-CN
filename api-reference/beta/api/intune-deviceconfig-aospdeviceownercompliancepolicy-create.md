---
title: 创建 aospDeviceOwnerCompliancePolicy
description: 创建新的 aospDeviceOwnerCompliancePolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02e80fa9e55b7b44751fb426cc12f8360045c80d
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665741"
---
# <a name="create-aospdeviceownercompliancepolicy"></a><span data-ttu-id="e2b09-103">创建 aospDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e2b09-103">Create aospDeviceOwnerCompliancePolicy</span></span>

<span data-ttu-id="e2b09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2b09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2b09-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e2b09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2b09-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2b09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2b09-107">创建新的 [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2b09-107">Create a new [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2b09-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e2b09-108">Prerequisites</span></span>
<span data-ttu-id="e2b09-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2b09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2b09-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2b09-111">Permission type</span></span>|<span data-ttu-id="e2b09-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2b09-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2b09-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2b09-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2b09-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2b09-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2b09-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2b09-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2b09-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2b09-116">Not supported.</span></span>|
|<span data-ttu-id="e2b09-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2b09-117">Application</span></span>|<span data-ttu-id="e2b09-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2b09-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2b09-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2b09-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e2b09-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2b09-120">Request headers</span></span>
|<span data-ttu-id="e2b09-121">标头</span><span class="sxs-lookup"><span data-stu-id="e2b09-121">Header</span></span>|<span data-ttu-id="e2b09-122">值</span><span class="sxs-lookup"><span data-stu-id="e2b09-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2b09-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2b09-123">Authorization</span></span>|<span data-ttu-id="e2b09-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e2b09-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2b09-125">接受</span><span class="sxs-lookup"><span data-stu-id="e2b09-125">Accept</span></span>|<span data-ttu-id="e2b09-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2b09-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2b09-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2b09-127">Request body</span></span>
<span data-ttu-id="e2b09-128">在请求正文中，提供 aospDeviceOwnerCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2b09-128">In the request body, supply a JSON representation for the aospDeviceOwnerCompliancePolicy object.</span></span>

<span data-ttu-id="e2b09-129">下表显示创建 aospDeviceOwnerCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e2b09-129">The following table shows the properties that are required when you create the aospDeviceOwnerCompliancePolicy.</span></span>

|<span data-ttu-id="e2b09-130">属性</span><span class="sxs-lookup"><span data-stu-id="e2b09-130">Property</span></span>|<span data-ttu-id="e2b09-131">类型</span><span class="sxs-lookup"><span data-stu-id="e2b09-131">Type</span></span>|<span data-ttu-id="e2b09-132">说明</span><span class="sxs-lookup"><span data-stu-id="e2b09-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2b09-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e2b09-133">roleScopeTagIds</span></span>|<span data-ttu-id="e2b09-134">String collection</span><span class="sxs-lookup"><span data-stu-id="e2b09-134">String collection</span></span>|<span data-ttu-id="e2b09-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e2b09-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e2b09-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e2b09-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e2b09-137">id</span><span class="sxs-lookup"><span data-stu-id="e2b09-137">id</span></span>|<span data-ttu-id="e2b09-138">String</span><span class="sxs-lookup"><span data-stu-id="e2b09-138">String</span></span>|<span data-ttu-id="e2b09-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e2b09-139">Key of the entity.</span></span> <span data-ttu-id="e2b09-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e2b09-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e2b09-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2b09-141">createdDateTime</span></span>|<span data-ttu-id="e2b09-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2b09-142">DateTimeOffset</span></span>|<span data-ttu-id="e2b09-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e2b09-143">DateTime the object was created.</span></span> <span data-ttu-id="e2b09-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e2b09-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e2b09-145">说明</span><span class="sxs-lookup"><span data-stu-id="e2b09-145">description</span></span>|<span data-ttu-id="e2b09-146">String</span><span class="sxs-lookup"><span data-stu-id="e2b09-146">String</span></span>|<span data-ttu-id="e2b09-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e2b09-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e2b09-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e2b09-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e2b09-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2b09-149">lastModifiedDateTime</span></span>|<span data-ttu-id="e2b09-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2b09-150">DateTimeOffset</span></span>|<span data-ttu-id="e2b09-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e2b09-151">DateTime the object was last modified.</span></span> <span data-ttu-id="e2b09-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e2b09-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e2b09-153">displayName</span><span class="sxs-lookup"><span data-stu-id="e2b09-153">displayName</span></span>|<span data-ttu-id="e2b09-154">String</span><span class="sxs-lookup"><span data-stu-id="e2b09-154">String</span></span>|<span data-ttu-id="e2b09-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e2b09-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e2b09-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e2b09-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e2b09-157">version</span><span class="sxs-lookup"><span data-stu-id="e2b09-157">version</span></span>|<span data-ttu-id="e2b09-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e2b09-158">Int32</span></span>|<span data-ttu-id="e2b09-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e2b09-159">Version of the device configuration.</span></span> <span data-ttu-id="e2b09-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e2b09-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e2b09-161">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e2b09-161">osMinimumVersion</span></span>|<span data-ttu-id="e2b09-162">String</span><span class="sxs-lookup"><span data-stu-id="e2b09-162">String</span></span>|<span data-ttu-id="e2b09-163">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="e2b09-163">Minimum Android version.</span></span>|
|<span data-ttu-id="e2b09-164">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e2b09-164">osMaximumVersion</span></span>|<span data-ttu-id="e2b09-165">String</span><span class="sxs-lookup"><span data-stu-id="e2b09-165">String</span></span>|<span data-ttu-id="e2b09-166">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="e2b09-166">Maximum Android version.</span></span>|
|<span data-ttu-id="e2b09-167">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="e2b09-167">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="e2b09-168">String</span><span class="sxs-lookup"><span data-stu-id="e2b09-168">String</span></span>|<span data-ttu-id="e2b09-169">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="e2b09-169">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="e2b09-170">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e2b09-170">passwordRequired</span></span>|<span data-ttu-id="e2b09-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b09-171">Boolean</span></span>|<span data-ttu-id="e2b09-172">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="e2b09-172">Require a password to unlock device.</span></span>|
|<span data-ttu-id="e2b09-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e2b09-173">passwordRequiredType</span></span>|[<span data-ttu-id="e2b09-174">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e2b09-174">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="e2b09-175">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="e2b09-175">Type of characters in password.</span></span> <span data-ttu-id="e2b09-176">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="e2b09-176">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="e2b09-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e2b09-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e2b09-178">Int32</span><span class="sxs-lookup"><span data-stu-id="e2b09-178">Int32</span></span>|<span data-ttu-id="e2b09-179">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="e2b09-179">Minutes of inactivity before a password is required.</span></span> <span data-ttu-id="e2b09-180">有效值为 1 到 8640</span><span class="sxs-lookup"><span data-stu-id="e2b09-180">Valid values 1 to 8640</span></span>|
|<span data-ttu-id="e2b09-181">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e2b09-181">passwordMinimumLength</span></span>|<span data-ttu-id="e2b09-182">Int32</span><span class="sxs-lookup"><span data-stu-id="e2b09-182">Int32</span></span>|<span data-ttu-id="e2b09-183">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="e2b09-183">Minimum password length.</span></span> <span data-ttu-id="e2b09-184">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="e2b09-184">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e2b09-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e2b09-185">storageRequireEncryption</span></span>|<span data-ttu-id="e2b09-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b09-186">Boolean</span></span>|<span data-ttu-id="e2b09-187">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="e2b09-187">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="e2b09-188">响应</span><span class="sxs-lookup"><span data-stu-id="e2b09-188">Response</span></span>
<span data-ttu-id="e2b09-189">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2b09-189">If successful, this method returns a `201 Created` response code and a [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2b09-190">示例</span><span class="sxs-lookup"><span data-stu-id="e2b09-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2b09-191">请求</span><span class="sxs-lookup"><span data-stu-id="e2b09-191">Request</span></span>
<span data-ttu-id="e2b09-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2b09-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="e2b09-193">响应</span><span class="sxs-lookup"><span data-stu-id="e2b09-193">Response</span></span>
<span data-ttu-id="e2b09-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e2b09-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




