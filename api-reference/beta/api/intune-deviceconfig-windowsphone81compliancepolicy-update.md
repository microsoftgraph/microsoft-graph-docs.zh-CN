---
title: 更新 windowsPhone81CompliancePolicy
description: 更新 windowsPhone81CompliancePolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 804fdb19f5f9ba17afb3b8880f7b3ed602cdf197
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32513277"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="c7d05-103">更新 windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c7d05-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="c7d05-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7d05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7d05-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7d05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7d05-106">更新 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c7d05-106">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7d05-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c7d05-107">Prerequisites</span></span>
<span data-ttu-id="c7d05-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7d05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7d05-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7d05-110">Permission type</span></span>|<span data-ttu-id="c7d05-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c7d05-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7d05-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7d05-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7d05-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7d05-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7d05-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7d05-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7d05-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7d05-115">Not supported.</span></span>|
|<span data-ttu-id="c7d05-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7d05-116">Application</span></span>|<span data-ttu-id="c7d05-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7d05-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7d05-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7d05-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="c7d05-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7d05-119">Request headers</span></span>
|<span data-ttu-id="c7d05-120">标头</span><span class="sxs-lookup"><span data-stu-id="c7d05-120">Header</span></span>|<span data-ttu-id="c7d05-121">值</span><span class="sxs-lookup"><span data-stu-id="c7d05-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7d05-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7d05-122">Authorization</span></span>|<span data-ttu-id="c7d05-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c7d05-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7d05-124">接受</span><span class="sxs-lookup"><span data-stu-id="c7d05-124">Accept</span></span>|<span data-ttu-id="c7d05-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c7d05-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7d05-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7d05-126">Request body</span></span>
<span data-ttu-id="c7d05-127">在请求正文中，提供 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7d05-127">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="c7d05-128">下表显示创建 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c7d05-128">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="c7d05-129">属性</span><span class="sxs-lookup"><span data-stu-id="c7d05-129">Property</span></span>|<span data-ttu-id="c7d05-130">类型</span><span class="sxs-lookup"><span data-stu-id="c7d05-130">Type</span></span>|<span data-ttu-id="c7d05-131">说明</span><span class="sxs-lookup"><span data-stu-id="c7d05-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7d05-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c7d05-132">roleScopeTagIds</span></span>|<span data-ttu-id="c7d05-133">String collection</span><span class="sxs-lookup"><span data-stu-id="c7d05-133">String collection</span></span>|<span data-ttu-id="c7d05-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c7d05-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c7d05-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c7d05-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7d05-136">id</span><span class="sxs-lookup"><span data-stu-id="c7d05-136">id</span></span>|<span data-ttu-id="c7d05-137">String</span><span class="sxs-lookup"><span data-stu-id="c7d05-137">String</span></span>|<span data-ttu-id="c7d05-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c7d05-138">Key of the entity.</span></span> <span data-ttu-id="c7d05-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c7d05-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7d05-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7d05-140">createdDateTime</span></span>|<span data-ttu-id="c7d05-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7d05-141">DateTimeOffset</span></span>|<span data-ttu-id="c7d05-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c7d05-142">DateTime the object was created.</span></span> <span data-ttu-id="c7d05-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c7d05-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7d05-144">description</span><span class="sxs-lookup"><span data-stu-id="c7d05-144">description</span></span>|<span data-ttu-id="c7d05-145">字符串</span><span class="sxs-lookup"><span data-stu-id="c7d05-145">String</span></span>|<span data-ttu-id="c7d05-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c7d05-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c7d05-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c7d05-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7d05-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7d05-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c7d05-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7d05-149">DateTimeOffset</span></span>|<span data-ttu-id="c7d05-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c7d05-150">DateTime the object was last modified.</span></span> <span data-ttu-id="c7d05-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c7d05-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7d05-152">displayName</span><span class="sxs-lookup"><span data-stu-id="c7d05-152">displayName</span></span>|<span data-ttu-id="c7d05-153">字符串</span><span class="sxs-lookup"><span data-stu-id="c7d05-153">String</span></span>|<span data-ttu-id="c7d05-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c7d05-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c7d05-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c7d05-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7d05-156">version</span><span class="sxs-lookup"><span data-stu-id="c7d05-156">version</span></span>|<span data-ttu-id="c7d05-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d05-157">Int32</span></span>|<span data-ttu-id="c7d05-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c7d05-158">Version of the device configuration.</span></span> <span data-ttu-id="c7d05-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c7d05-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7d05-160">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c7d05-160">passwordBlockSimple</span></span>|<span data-ttu-id="c7d05-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7d05-161">Boolean</span></span>|<span data-ttu-id="c7d05-162">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="c7d05-162">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="c7d05-163">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c7d05-163">passwordExpirationDays</span></span>|<span data-ttu-id="c7d05-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d05-164">Int32</span></span>|<span data-ttu-id="c7d05-165">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="c7d05-165">Number of days before the password expires.</span></span>|
|<span data-ttu-id="c7d05-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c7d05-166">passwordMinimumLength</span></span>|<span data-ttu-id="c7d05-167">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d05-167">Int32</span></span>|<span data-ttu-id="c7d05-168">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="c7d05-168">Minimum length of passwords.</span></span>|
|<span data-ttu-id="c7d05-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c7d05-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c7d05-170">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d05-170">Int32</span></span>|<span data-ttu-id="c7d05-171">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c7d05-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c7d05-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c7d05-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c7d05-173">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d05-173">Int32</span></span>|<span data-ttu-id="c7d05-174">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="c7d05-174">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c7d05-175">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c7d05-175">passwordRequiredType</span></span>|[<span data-ttu-id="c7d05-176">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c7d05-176">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c7d05-177">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="c7d05-177">The required password type.</span></span> <span data-ttu-id="c7d05-178">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="c7d05-178">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c7d05-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c7d05-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c7d05-180">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d05-180">Int32</span></span>|<span data-ttu-id="c7d05-181">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="c7d05-181">Number of previous passwords to block.</span></span> <span data-ttu-id="c7d05-182">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="c7d05-182">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c7d05-183">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c7d05-183">passwordRequired</span></span>|<span data-ttu-id="c7d05-184">布尔</span><span class="sxs-lookup"><span data-stu-id="c7d05-184">Boolean</span></span>|<span data-ttu-id="c7d05-185">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="c7d05-185">Whether or not to require a password.</span></span>|
|<span data-ttu-id="c7d05-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c7d05-186">osMinimumVersion</span></span>|<span data-ttu-id="c7d05-187">字符串</span><span class="sxs-lookup"><span data-stu-id="c7d05-187">String</span></span>|<span data-ttu-id="c7d05-188">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="c7d05-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="c7d05-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c7d05-189">osMaximumVersion</span></span>|<span data-ttu-id="c7d05-190">String</span><span class="sxs-lookup"><span data-stu-id="c7d05-190">String</span></span>|<span data-ttu-id="c7d05-191">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="c7d05-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="c7d05-192">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c7d05-192">storageRequireEncryption</span></span>|<span data-ttu-id="c7d05-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7d05-193">Boolean</span></span>|<span data-ttu-id="c7d05-194">要求对 Windows Phone 设备加密。</span><span class="sxs-lookup"><span data-stu-id="c7d05-194">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="c7d05-195">响应</span><span class="sxs-lookup"><span data-stu-id="c7d05-195">Response</span></span>
<span data-ttu-id="c7d05-196">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7d05-196">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7d05-197">示例</span><span class="sxs-lookup"><span data-stu-id="c7d05-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7d05-198">请求</span><span class="sxs-lookup"><span data-stu-id="c7d05-198">Request</span></span>
<span data-ttu-id="c7d05-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7d05-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 669

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="c7d05-200">响应</span><span class="sxs-lookup"><span data-stu-id="c7d05-200">Response</span></span>
<span data-ttu-id="c7d05-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7d05-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 841

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```





