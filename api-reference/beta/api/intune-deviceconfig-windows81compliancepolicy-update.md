---
title: 更新 windows81CompliancePolicy
description: 更新 windows81CompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a7b101f91e6791eb480ea8ba1fac056e0095feab
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733482"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="27203-103">更新 windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="27203-103">Update windows81CompliancePolicy</span></span>

<span data-ttu-id="27203-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27203-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27203-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="27203-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27203-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27203-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27203-107">更新 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27203-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27203-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="27203-108">Prerequisites</span></span>
<span data-ttu-id="27203-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27203-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27203-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="27203-111">Permission type</span></span>|<span data-ttu-id="27203-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="27203-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27203-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27203-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27203-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27203-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27203-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27203-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27203-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="27203-116">Not supported.</span></span>|
|<span data-ttu-id="27203-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="27203-117">Application</span></span>|<span data-ttu-id="27203-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27203-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27203-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27203-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="27203-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="27203-120">Request headers</span></span>
|<span data-ttu-id="27203-121">标头</span><span class="sxs-lookup"><span data-stu-id="27203-121">Header</span></span>|<span data-ttu-id="27203-122">值</span><span class="sxs-lookup"><span data-stu-id="27203-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27203-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="27203-123">Authorization</span></span>|<span data-ttu-id="27203-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="27203-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27203-125">接受</span><span class="sxs-lookup"><span data-stu-id="27203-125">Accept</span></span>|<span data-ttu-id="27203-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27203-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27203-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="27203-127">Request body</span></span>
<span data-ttu-id="27203-128">在请求正文中，提供 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27203-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="27203-129">下表显示创建 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="27203-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="27203-130">属性</span><span class="sxs-lookup"><span data-stu-id="27203-130">Property</span></span>|<span data-ttu-id="27203-131">类型</span><span class="sxs-lookup"><span data-stu-id="27203-131">Type</span></span>|<span data-ttu-id="27203-132">说明</span><span class="sxs-lookup"><span data-stu-id="27203-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27203-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="27203-133">roleScopeTagIds</span></span>|<span data-ttu-id="27203-134">String collection</span><span class="sxs-lookup"><span data-stu-id="27203-134">String collection</span></span>|<span data-ttu-id="27203-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="27203-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="27203-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="27203-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="27203-137">id</span><span class="sxs-lookup"><span data-stu-id="27203-137">id</span></span>|<span data-ttu-id="27203-138">String</span><span class="sxs-lookup"><span data-stu-id="27203-138">String</span></span>|<span data-ttu-id="27203-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="27203-139">Key of the entity.</span></span> <span data-ttu-id="27203-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="27203-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="27203-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27203-141">createdDateTime</span></span>|<span data-ttu-id="27203-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27203-142">DateTimeOffset</span></span>|<span data-ttu-id="27203-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="27203-143">DateTime the object was created.</span></span> <span data-ttu-id="27203-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="27203-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="27203-145">说明</span><span class="sxs-lookup"><span data-stu-id="27203-145">description</span></span>|<span data-ttu-id="27203-146">String</span><span class="sxs-lookup"><span data-stu-id="27203-146">String</span></span>|<span data-ttu-id="27203-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="27203-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="27203-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="27203-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="27203-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27203-149">lastModifiedDateTime</span></span>|<span data-ttu-id="27203-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27203-150">DateTimeOffset</span></span>|<span data-ttu-id="27203-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="27203-151">DateTime the object was last modified.</span></span> <span data-ttu-id="27203-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="27203-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="27203-153">displayName</span><span class="sxs-lookup"><span data-stu-id="27203-153">displayName</span></span>|<span data-ttu-id="27203-154">String</span><span class="sxs-lookup"><span data-stu-id="27203-154">String</span></span>|<span data-ttu-id="27203-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="27203-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="27203-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="27203-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="27203-157">version</span><span class="sxs-lookup"><span data-stu-id="27203-157">version</span></span>|<span data-ttu-id="27203-158">Int32</span><span class="sxs-lookup"><span data-stu-id="27203-158">Int32</span></span>|<span data-ttu-id="27203-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="27203-159">Version of the device configuration.</span></span> <span data-ttu-id="27203-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="27203-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="27203-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="27203-161">passwordRequired</span></span>|<span data-ttu-id="27203-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="27203-162">Boolean</span></span>|<span data-ttu-id="27203-163">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="27203-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="27203-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="27203-164">passwordBlockSimple</span></span>|<span data-ttu-id="27203-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="27203-165">Boolean</span></span>|<span data-ttu-id="27203-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="27203-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="27203-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="27203-167">passwordExpirationDays</span></span>|<span data-ttu-id="27203-168">Int32</span><span class="sxs-lookup"><span data-stu-id="27203-168">Int32</span></span>|<span data-ttu-id="27203-169">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="27203-169">Password expiration in days.</span></span>|
|<span data-ttu-id="27203-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="27203-170">passwordMinimumLength</span></span>|<span data-ttu-id="27203-171">Int32</span><span class="sxs-lookup"><span data-stu-id="27203-171">Int32</span></span>|<span data-ttu-id="27203-172">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="27203-172">The minimum password length.</span></span>|
|<span data-ttu-id="27203-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="27203-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="27203-174">Int32</span><span class="sxs-lookup"><span data-stu-id="27203-174">Int32</span></span>|<span data-ttu-id="27203-175">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="27203-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="27203-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="27203-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="27203-177">Int32</span><span class="sxs-lookup"><span data-stu-id="27203-177">Int32</span></span>|<span data-ttu-id="27203-178">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="27203-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="27203-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="27203-179">passwordRequiredType</span></span>|[<span data-ttu-id="27203-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="27203-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="27203-181">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="27203-181">The required password type.</span></span> <span data-ttu-id="27203-182">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="27203-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="27203-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="27203-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="27203-184">Int32</span><span class="sxs-lookup"><span data-stu-id="27203-184">Int32</span></span>|<span data-ttu-id="27203-185">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="27203-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="27203-186">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="27203-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="27203-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="27203-187">osMinimumVersion</span></span>|<span data-ttu-id="27203-188">String</span><span class="sxs-lookup"><span data-stu-id="27203-188">String</span></span>|<span data-ttu-id="27203-189">最低 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="27203-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="27203-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="27203-190">osMaximumVersion</span></span>|<span data-ttu-id="27203-191">String</span><span class="sxs-lookup"><span data-stu-id="27203-191">String</span></span>|<span data-ttu-id="27203-192">最高 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="27203-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="27203-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="27203-193">storageRequireEncryption</span></span>|<span data-ttu-id="27203-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="27203-194">Boolean</span></span>|<span data-ttu-id="27203-195">指示是否要求对 Windows 8.1 设备加密。</span><span class="sxs-lookup"><span data-stu-id="27203-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="27203-196">响应</span><span class="sxs-lookup"><span data-stu-id="27203-196">Response</span></span>
<span data-ttu-id="27203-197">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="27203-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27203-198">示例</span><span class="sxs-lookup"><span data-stu-id="27203-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="27203-199">请求</span><span class="sxs-lookup"><span data-stu-id="27203-199">Request</span></span>
<span data-ttu-id="27203-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27203-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 664

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="27203-201">响应</span><span class="sxs-lookup"><span data-stu-id="27203-201">Response</span></span>
<span data-ttu-id="27203-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27203-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 836

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```





