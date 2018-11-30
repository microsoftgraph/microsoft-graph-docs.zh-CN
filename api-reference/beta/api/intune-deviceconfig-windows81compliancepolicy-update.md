---
title: 更新 windows81CompliancePolicy
description: 更新 windows81CompliancePolicy 对象的属性。
ms.openlocfilehash: 238d1f063e5c41f7f7622ef56bff69db29559631
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046282"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="65220-103">更新 windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="65220-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="65220-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="65220-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65220-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="65220-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65220-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="65220-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65220-107">更新 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="65220-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="65220-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="65220-108">Prerequisites</span></span>
<span data-ttu-id="65220-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="65220-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65220-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="65220-111">Permission type</span></span>|<span data-ttu-id="65220-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65220-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65220-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65220-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65220-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65220-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65220-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65220-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65220-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="65220-116">Not supported.</span></span>|
|<span data-ttu-id="65220-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="65220-117">Application</span></span>|<span data-ttu-id="65220-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="65220-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65220-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65220-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="65220-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="65220-120">Request headers</span></span>
|<span data-ttu-id="65220-121">标头</span><span class="sxs-lookup"><span data-stu-id="65220-121">Header</span></span>|<span data-ttu-id="65220-122">值</span><span class="sxs-lookup"><span data-stu-id="65220-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65220-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65220-123">Authorization</span></span>|<span data-ttu-id="65220-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65220-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65220-125">Accept</span><span class="sxs-lookup"><span data-stu-id="65220-125">Accept</span></span>|<span data-ttu-id="65220-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65220-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65220-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="65220-127">Request body</span></span>
<span data-ttu-id="65220-128">在请求正文中，提供 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65220-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="65220-129">下表显示创建 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="65220-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="65220-130">属性</span><span class="sxs-lookup"><span data-stu-id="65220-130">Property</span></span>|<span data-ttu-id="65220-131">类型</span><span class="sxs-lookup"><span data-stu-id="65220-131">Type</span></span>|<span data-ttu-id="65220-132">说明</span><span class="sxs-lookup"><span data-stu-id="65220-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65220-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="65220-133">roleScopeTagIds</span></span>|<span data-ttu-id="65220-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="65220-134">String collection</span></span>|<span data-ttu-id="65220-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="65220-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="65220-136">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65220-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="65220-137">id</span><span class="sxs-lookup"><span data-stu-id="65220-137">id</span></span>|<span data-ttu-id="65220-138">String</span><span class="sxs-lookup"><span data-stu-id="65220-138">String</span></span>|<span data-ttu-id="65220-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="65220-139">Key of the entity.</span></span> <span data-ttu-id="65220-140">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65220-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="65220-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65220-141">createdDateTime</span></span>|<span data-ttu-id="65220-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65220-142">DateTimeOffset</span></span>|<span data-ttu-id="65220-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="65220-143">DateTime the object was created.</span></span> <span data-ttu-id="65220-144">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65220-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="65220-145">description</span><span class="sxs-lookup"><span data-stu-id="65220-145">description</span></span>|<span data-ttu-id="65220-146">String</span><span class="sxs-lookup"><span data-stu-id="65220-146">String</span></span>|<span data-ttu-id="65220-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="65220-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="65220-148">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65220-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="65220-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65220-149">lastModifiedDateTime</span></span>|<span data-ttu-id="65220-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65220-150">DateTimeOffset</span></span>|<span data-ttu-id="65220-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="65220-151">DateTime the object was last modified.</span></span> <span data-ttu-id="65220-152">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65220-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="65220-153">displayName</span><span class="sxs-lookup"><span data-stu-id="65220-153">displayName</span></span>|<span data-ttu-id="65220-154">String</span><span class="sxs-lookup"><span data-stu-id="65220-154">String</span></span>|<span data-ttu-id="65220-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="65220-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="65220-156">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65220-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="65220-157">version</span><span class="sxs-lookup"><span data-stu-id="65220-157">version</span></span>|<span data-ttu-id="65220-158">Int32</span><span class="sxs-lookup"><span data-stu-id="65220-158">Int32</span></span>|<span data-ttu-id="65220-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="65220-159">Version of the device configuration.</span></span> <span data-ttu-id="65220-160">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65220-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="65220-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="65220-161">passwordRequired</span></span>|<span data-ttu-id="65220-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="65220-162">Boolean</span></span>|<span data-ttu-id="65220-163">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="65220-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="65220-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="65220-164">passwordBlockSimple</span></span>|<span data-ttu-id="65220-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="65220-165">Boolean</span></span>|<span data-ttu-id="65220-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="65220-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="65220-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="65220-167">passwordExpirationDays</span></span>|<span data-ttu-id="65220-168">Int32</span><span class="sxs-lookup"><span data-stu-id="65220-168">Int32</span></span>|<span data-ttu-id="65220-169">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="65220-169">Password expiration in days.</span></span>|
|<span data-ttu-id="65220-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="65220-170">passwordMinimumLength</span></span>|<span data-ttu-id="65220-171">Int32</span><span class="sxs-lookup"><span data-stu-id="65220-171">Int32</span></span>|<span data-ttu-id="65220-172">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="65220-172">The minimum password length.</span></span>|
|<span data-ttu-id="65220-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="65220-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="65220-174">Int32</span><span class="sxs-lookup"><span data-stu-id="65220-174">Int32</span></span>|<span data-ttu-id="65220-175">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="65220-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="65220-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="65220-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="65220-177">Int32</span><span class="sxs-lookup"><span data-stu-id="65220-177">Int32</span></span>|<span data-ttu-id="65220-178">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="65220-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="65220-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="65220-179">passwordRequiredType</span></span>|[<span data-ttu-id="65220-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="65220-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="65220-181">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="65220-181">The required password type.</span></span> <span data-ttu-id="65220-182">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="65220-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="65220-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="65220-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="65220-184">Int32</span><span class="sxs-lookup"><span data-stu-id="65220-184">Int32</span></span>|<span data-ttu-id="65220-185">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="65220-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="65220-186">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="65220-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="65220-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="65220-187">osMinimumVersion</span></span>|<span data-ttu-id="65220-188">String</span><span class="sxs-lookup"><span data-stu-id="65220-188">String</span></span>|<span data-ttu-id="65220-189">最低 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="65220-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="65220-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="65220-190">osMaximumVersion</span></span>|<span data-ttu-id="65220-191">String</span><span class="sxs-lookup"><span data-stu-id="65220-191">String</span></span>|<span data-ttu-id="65220-192">最高 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="65220-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="65220-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="65220-193">storageRequireEncryption</span></span>|<span data-ttu-id="65220-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="65220-194">Boolean</span></span>|<span data-ttu-id="65220-195">指示是否要求对 Windows 8.1 设备加密。</span><span class="sxs-lookup"><span data-stu-id="65220-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="65220-196">响应</span><span class="sxs-lookup"><span data-stu-id="65220-196">Response</span></span>
<span data-ttu-id="65220-197">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65220-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65220-198">示例</span><span class="sxs-lookup"><span data-stu-id="65220-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="65220-199">请求</span><span class="sxs-lookup"><span data-stu-id="65220-199">Request</span></span>
<span data-ttu-id="65220-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65220-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 664

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="65220-201">响应</span><span class="sxs-lookup"><span data-stu-id="65220-201">Response</span></span>
<span data-ttu-id="65220-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65220-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





