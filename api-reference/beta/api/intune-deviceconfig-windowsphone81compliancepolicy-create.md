---
title: 创建 windowsPhone81CompliancePolicy
description: 创建新的 windowsPhone81CompliancePolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f1339d8ced6e5db7566287aca924af5d116cd041
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43334692"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="2f3d1-103">创建 windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2f3d1-103">Create windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="2f3d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f3d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f3d1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f3d1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f3d1-107">创建新的 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-107">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f3d1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f3d1-108">Prerequisites</span></span>
<span data-ttu-id="2f3d1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f3d1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f3d1-111">Permission type</span></span>|<span data-ttu-id="2f3d1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2f3d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f3d1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f3d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f3d1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f3d1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f3d1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f3d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f3d1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-116">Not supported.</span></span>|
|<span data-ttu-id="2f3d1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f3d1-117">Application</span></span>|<span data-ttu-id="2f3d1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f3d1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f3d1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f3d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="2f3d1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f3d1-120">Request headers</span></span>
|<span data-ttu-id="2f3d1-121">标头</span><span class="sxs-lookup"><span data-stu-id="2f3d1-121">Header</span></span>|<span data-ttu-id="2f3d1-122">值</span><span class="sxs-lookup"><span data-stu-id="2f3d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f3d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f3d1-123">Authorization</span></span>|<span data-ttu-id="2f3d1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f3d1-125">接受</span><span class="sxs-lookup"><span data-stu-id="2f3d1-125">Accept</span></span>|<span data-ttu-id="2f3d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f3d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f3d1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f3d1-127">Request body</span></span>
<span data-ttu-id="2f3d1-128">在请求正文中，提供 windowsPhone81CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-128">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="2f3d1-129">下表显示创建 windowsPhone81CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-129">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="2f3d1-130">属性</span><span class="sxs-lookup"><span data-stu-id="2f3d1-130">Property</span></span>|<span data-ttu-id="2f3d1-131">类型</span><span class="sxs-lookup"><span data-stu-id="2f3d1-131">Type</span></span>|<span data-ttu-id="2f3d1-132">说明</span><span class="sxs-lookup"><span data-stu-id="2f3d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f3d1-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f3d1-133">roleScopeTagIds</span></span>|<span data-ttu-id="2f3d1-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="2f3d1-134">String collection</span></span>|<span data-ttu-id="2f3d1-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2f3d1-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f3d1-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f3d1-137">id</span><span class="sxs-lookup"><span data-stu-id="2f3d1-137">id</span></span>|<span data-ttu-id="2f3d1-138">字符串</span><span class="sxs-lookup"><span data-stu-id="2f3d1-138">String</span></span>|<span data-ttu-id="2f3d1-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-139">Key of the entity.</span></span> <span data-ttu-id="2f3d1-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f3d1-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f3d1-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f3d1-141">createdDateTime</span></span>|<span data-ttu-id="2f3d1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f3d1-142">DateTimeOffset</span></span>|<span data-ttu-id="2f3d1-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-143">DateTime the object was created.</span></span> <span data-ttu-id="2f3d1-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f3d1-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f3d1-145">description</span><span class="sxs-lookup"><span data-stu-id="2f3d1-145">description</span></span>|<span data-ttu-id="2f3d1-146">String</span><span class="sxs-lookup"><span data-stu-id="2f3d1-146">String</span></span>|<span data-ttu-id="2f3d1-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f3d1-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f3d1-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f3d1-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f3d1-149">lastModifiedDateTime</span></span>|<span data-ttu-id="2f3d1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f3d1-150">DateTimeOffset</span></span>|<span data-ttu-id="2f3d1-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-151">DateTime the object was last modified.</span></span> <span data-ttu-id="2f3d1-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f3d1-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f3d1-153">displayName</span><span class="sxs-lookup"><span data-stu-id="2f3d1-153">displayName</span></span>|<span data-ttu-id="2f3d1-154">字符串</span><span class="sxs-lookup"><span data-stu-id="2f3d1-154">String</span></span>|<span data-ttu-id="2f3d1-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f3d1-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f3d1-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f3d1-157">version</span><span class="sxs-lookup"><span data-stu-id="2f3d1-157">version</span></span>|<span data-ttu-id="2f3d1-158">Int32</span><span class="sxs-lookup"><span data-stu-id="2f3d1-158">Int32</span></span>|<span data-ttu-id="2f3d1-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-159">Version of the device configuration.</span></span> <span data-ttu-id="2f3d1-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f3d1-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f3d1-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="2f3d1-161">passwordBlockSimple</span></span>|<span data-ttu-id="2f3d1-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f3d1-162">Boolean</span></span>|<span data-ttu-id="2f3d1-163">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="2f3d1-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2f3d1-164">passwordExpirationDays</span></span>|<span data-ttu-id="2f3d1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2f3d1-165">Int32</span></span>|<span data-ttu-id="2f3d1-166">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="2f3d1-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2f3d1-167">passwordMinimumLength</span></span>|<span data-ttu-id="2f3d1-168">Int32</span><span class="sxs-lookup"><span data-stu-id="2f3d1-168">Int32</span></span>|<span data-ttu-id="2f3d1-169">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="2f3d1-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="2f3d1-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="2f3d1-171">Int32</span><span class="sxs-lookup"><span data-stu-id="2f3d1-171">Int32</span></span>|<span data-ttu-id="2f3d1-172">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="2f3d1-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="2f3d1-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="2f3d1-174">Int32</span><span class="sxs-lookup"><span data-stu-id="2f3d1-174">Int32</span></span>|<span data-ttu-id="2f3d1-175">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="2f3d1-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2f3d1-176">passwordRequiredType</span></span>|[<span data-ttu-id="2f3d1-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2f3d1-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="2f3d1-178">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-178">The required password type.</span></span> <span data-ttu-id="2f3d1-179">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="2f3d1-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2f3d1-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2f3d1-181">Int32</span><span class="sxs-lookup"><span data-stu-id="2f3d1-181">Int32</span></span>|<span data-ttu-id="2f3d1-182">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-182">Number of previous passwords to block.</span></span> <span data-ttu-id="2f3d1-183">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="2f3d1-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2f3d1-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="2f3d1-184">passwordRequired</span></span>|<span data-ttu-id="2f3d1-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f3d1-185">Boolean</span></span>|<span data-ttu-id="2f3d1-186">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="2f3d1-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2f3d1-187">osMinimumVersion</span></span>|<span data-ttu-id="2f3d1-188">字符串</span><span class="sxs-lookup"><span data-stu-id="2f3d1-188">String</span></span>|<span data-ttu-id="2f3d1-189">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="2f3d1-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2f3d1-190">osMaximumVersion</span></span>|<span data-ttu-id="2f3d1-191">String</span><span class="sxs-lookup"><span data-stu-id="2f3d1-191">String</span></span>|<span data-ttu-id="2f3d1-192">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="2f3d1-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="2f3d1-193">storageRequireEncryption</span></span>|<span data-ttu-id="2f3d1-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f3d1-194">Boolean</span></span>|<span data-ttu-id="2f3d1-195">要求对 Windows Phone 设备加密。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="2f3d1-196">响应</span><span class="sxs-lookup"><span data-stu-id="2f3d1-196">Response</span></span>
<span data-ttu-id="2f3d1-197">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-197">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f3d1-198">示例</span><span class="sxs-lookup"><span data-stu-id="2f3d1-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f3d1-199">请求</span><span class="sxs-lookup"><span data-stu-id="2f3d1-199">Request</span></span>
<span data-ttu-id="2f3d1-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="2f3d1-201">响应</span><span class="sxs-lookup"><span data-stu-id="2f3d1-201">Response</span></span>
<span data-ttu-id="2f3d1-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f3d1-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



