---
title: 创建 windows81CompliancePolicy
description: 创建新的 windows81CompliancePolicy 对象。
ms.openlocfilehash: c7366204a6b3985892f6da51efb5611901286d2a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047788"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="870c5-103">创建 windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="870c5-103">Create windows81CompliancePolicy</span></span>

> <span data-ttu-id="870c5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="870c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="870c5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="870c5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="870c5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="870c5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="870c5-107">创建新的 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="870c5-107">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="870c5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="870c5-108">Prerequisites</span></span>
<span data-ttu-id="870c5-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="870c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="870c5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="870c5-111">Permission type</span></span>|<span data-ttu-id="870c5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="870c5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="870c5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="870c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="870c5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="870c5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="870c5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="870c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="870c5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="870c5-116">Not supported.</span></span>|
|<span data-ttu-id="870c5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="870c5-117">Application</span></span>|<span data-ttu-id="870c5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="870c5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="870c5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="870c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="870c5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="870c5-120">Request headers</span></span>
|<span data-ttu-id="870c5-121">标头</span><span class="sxs-lookup"><span data-stu-id="870c5-121">Header</span></span>|<span data-ttu-id="870c5-122">值</span><span class="sxs-lookup"><span data-stu-id="870c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="870c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="870c5-123">Authorization</span></span>|<span data-ttu-id="870c5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="870c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="870c5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="870c5-125">Accept</span></span>|<span data-ttu-id="870c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="870c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="870c5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="870c5-127">Request body</span></span>
<span data-ttu-id="870c5-128">在请求正文中，提供 windows81CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="870c5-128">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="870c5-129">下表显示创建 windows81CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="870c5-129">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="870c5-130">属性</span><span class="sxs-lookup"><span data-stu-id="870c5-130">Property</span></span>|<span data-ttu-id="870c5-131">类型</span><span class="sxs-lookup"><span data-stu-id="870c5-131">Type</span></span>|<span data-ttu-id="870c5-132">说明</span><span class="sxs-lookup"><span data-stu-id="870c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="870c5-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="870c5-133">roleScopeTagIds</span></span>|<span data-ttu-id="870c5-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="870c5-134">String collection</span></span>|<span data-ttu-id="870c5-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="870c5-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="870c5-136">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="870c5-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="870c5-137">id</span><span class="sxs-lookup"><span data-stu-id="870c5-137">id</span></span>|<span data-ttu-id="870c5-138">String</span><span class="sxs-lookup"><span data-stu-id="870c5-138">String</span></span>|<span data-ttu-id="870c5-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="870c5-139">Key of the entity.</span></span> <span data-ttu-id="870c5-140">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="870c5-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="870c5-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="870c5-141">createdDateTime</span></span>|<span data-ttu-id="870c5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="870c5-142">DateTimeOffset</span></span>|<span data-ttu-id="870c5-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="870c5-143">DateTime the object was created.</span></span> <span data-ttu-id="870c5-144">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="870c5-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="870c5-145">description</span><span class="sxs-lookup"><span data-stu-id="870c5-145">description</span></span>|<span data-ttu-id="870c5-146">String</span><span class="sxs-lookup"><span data-stu-id="870c5-146">String</span></span>|<span data-ttu-id="870c5-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="870c5-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="870c5-148">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="870c5-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="870c5-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="870c5-149">lastModifiedDateTime</span></span>|<span data-ttu-id="870c5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="870c5-150">DateTimeOffset</span></span>|<span data-ttu-id="870c5-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="870c5-151">DateTime the object was last modified.</span></span> <span data-ttu-id="870c5-152">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="870c5-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="870c5-153">displayName</span><span class="sxs-lookup"><span data-stu-id="870c5-153">displayName</span></span>|<span data-ttu-id="870c5-154">String</span><span class="sxs-lookup"><span data-stu-id="870c5-154">String</span></span>|<span data-ttu-id="870c5-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="870c5-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="870c5-156">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="870c5-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="870c5-157">version</span><span class="sxs-lookup"><span data-stu-id="870c5-157">version</span></span>|<span data-ttu-id="870c5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="870c5-158">Int32</span></span>|<span data-ttu-id="870c5-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="870c5-159">Version of the device configuration.</span></span> <span data-ttu-id="870c5-160">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="870c5-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="870c5-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="870c5-161">passwordRequired</span></span>|<span data-ttu-id="870c5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="870c5-162">Boolean</span></span>|<span data-ttu-id="870c5-163">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="870c5-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="870c5-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="870c5-164">passwordBlockSimple</span></span>|<span data-ttu-id="870c5-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="870c5-165">Boolean</span></span>|<span data-ttu-id="870c5-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="870c5-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="870c5-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="870c5-167">passwordExpirationDays</span></span>|<span data-ttu-id="870c5-168">Int32</span><span class="sxs-lookup"><span data-stu-id="870c5-168">Int32</span></span>|<span data-ttu-id="870c5-169">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="870c5-169">Password expiration in days.</span></span>|
|<span data-ttu-id="870c5-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="870c5-170">passwordMinimumLength</span></span>|<span data-ttu-id="870c5-171">Int32</span><span class="sxs-lookup"><span data-stu-id="870c5-171">Int32</span></span>|<span data-ttu-id="870c5-172">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="870c5-172">The minimum password length.</span></span>|
|<span data-ttu-id="870c5-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="870c5-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="870c5-174">Int32</span><span class="sxs-lookup"><span data-stu-id="870c5-174">Int32</span></span>|<span data-ttu-id="870c5-175">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="870c5-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="870c5-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="870c5-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="870c5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="870c5-177">Int32</span></span>|<span data-ttu-id="870c5-178">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="870c5-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="870c5-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="870c5-179">passwordRequiredType</span></span>|[<span data-ttu-id="870c5-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="870c5-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="870c5-181">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="870c5-181">The required password type.</span></span> <span data-ttu-id="870c5-182">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="870c5-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="870c5-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="870c5-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="870c5-184">Int32</span><span class="sxs-lookup"><span data-stu-id="870c5-184">Int32</span></span>|<span data-ttu-id="870c5-185">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="870c5-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="870c5-186">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="870c5-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="870c5-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="870c5-187">osMinimumVersion</span></span>|<span data-ttu-id="870c5-188">String</span><span class="sxs-lookup"><span data-stu-id="870c5-188">String</span></span>|<span data-ttu-id="870c5-189">最低 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="870c5-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="870c5-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="870c5-190">osMaximumVersion</span></span>|<span data-ttu-id="870c5-191">String</span><span class="sxs-lookup"><span data-stu-id="870c5-191">String</span></span>|<span data-ttu-id="870c5-192">最高 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="870c5-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="870c5-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="870c5-193">storageRequireEncryption</span></span>|<span data-ttu-id="870c5-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="870c5-194">Boolean</span></span>|<span data-ttu-id="870c5-195">指示是否要求对 Windows 8.1 设备加密。</span><span class="sxs-lookup"><span data-stu-id="870c5-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="870c5-196">响应</span><span class="sxs-lookup"><span data-stu-id="870c5-196">Response</span></span>
<span data-ttu-id="870c5-197">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="870c5-197">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="870c5-198">示例</span><span class="sxs-lookup"><span data-stu-id="870c5-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="870c5-199">请求</span><span class="sxs-lookup"><span data-stu-id="870c5-199">Request</span></span>
<span data-ttu-id="870c5-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="870c5-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 728

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="870c5-201">响应</span><span class="sxs-lookup"><span data-stu-id="870c5-201">Response</span></span>
<span data-ttu-id="870c5-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="870c5-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





