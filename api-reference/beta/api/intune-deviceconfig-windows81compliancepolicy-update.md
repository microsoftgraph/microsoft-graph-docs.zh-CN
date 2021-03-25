---
title: 更新 windows81CompliancePolicy
description: 更新 windows81CompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 577b216801c67275067211100d03fb9ece1af3ab
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151065"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="b2472-103">更新 windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b2472-103">Update windows81CompliancePolicy</span></span>

<span data-ttu-id="b2472-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2472-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2472-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2472-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2472-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2472-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2472-107">更新 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b2472-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2472-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b2472-108">Prerequisites</span></span>
<span data-ttu-id="b2472-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2472-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2472-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2472-111">Permission type</span></span>|<span data-ttu-id="b2472-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2472-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2472-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2472-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2472-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2472-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2472-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2472-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2472-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2472-116">Not supported.</span></span>|
|<span data-ttu-id="b2472-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2472-117">Application</span></span>|<span data-ttu-id="b2472-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2472-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2472-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2472-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b2472-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2472-120">Request headers</span></span>
|<span data-ttu-id="b2472-121">标头</span><span class="sxs-lookup"><span data-stu-id="b2472-121">Header</span></span>|<span data-ttu-id="b2472-122">值</span><span class="sxs-lookup"><span data-stu-id="b2472-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2472-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2472-123">Authorization</span></span>|<span data-ttu-id="b2472-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b2472-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2472-125">接受</span><span class="sxs-lookup"><span data-stu-id="b2472-125">Accept</span></span>|<span data-ttu-id="b2472-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2472-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2472-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2472-127">Request body</span></span>
<span data-ttu-id="b2472-128">在请求正文中，提供 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2472-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="b2472-129">下表显示创建 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b2472-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="b2472-130">属性</span><span class="sxs-lookup"><span data-stu-id="b2472-130">Property</span></span>|<span data-ttu-id="b2472-131">类型</span><span class="sxs-lookup"><span data-stu-id="b2472-131">Type</span></span>|<span data-ttu-id="b2472-132">说明</span><span class="sxs-lookup"><span data-stu-id="b2472-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2472-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b2472-133">roleScopeTagIds</span></span>|<span data-ttu-id="b2472-134">String collection</span><span class="sxs-lookup"><span data-stu-id="b2472-134">String collection</span></span>|<span data-ttu-id="b2472-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b2472-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b2472-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b2472-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b2472-137">id</span><span class="sxs-lookup"><span data-stu-id="b2472-137">id</span></span>|<span data-ttu-id="b2472-138">String</span><span class="sxs-lookup"><span data-stu-id="b2472-138">String</span></span>|<span data-ttu-id="b2472-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b2472-139">Key of the entity.</span></span> <span data-ttu-id="b2472-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b2472-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b2472-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2472-141">createdDateTime</span></span>|<span data-ttu-id="b2472-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2472-142">DateTimeOffset</span></span>|<span data-ttu-id="b2472-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b2472-143">DateTime the object was created.</span></span> <span data-ttu-id="b2472-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b2472-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b2472-145">说明</span><span class="sxs-lookup"><span data-stu-id="b2472-145">description</span></span>|<span data-ttu-id="b2472-146">String</span><span class="sxs-lookup"><span data-stu-id="b2472-146">String</span></span>|<span data-ttu-id="b2472-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b2472-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b2472-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b2472-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b2472-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2472-149">lastModifiedDateTime</span></span>|<span data-ttu-id="b2472-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2472-150">DateTimeOffset</span></span>|<span data-ttu-id="b2472-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b2472-151">DateTime the object was last modified.</span></span> <span data-ttu-id="b2472-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b2472-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b2472-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b2472-153">displayName</span></span>|<span data-ttu-id="b2472-154">String</span><span class="sxs-lookup"><span data-stu-id="b2472-154">String</span></span>|<span data-ttu-id="b2472-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b2472-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b2472-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b2472-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b2472-157">version</span><span class="sxs-lookup"><span data-stu-id="b2472-157">version</span></span>|<span data-ttu-id="b2472-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b2472-158">Int32</span></span>|<span data-ttu-id="b2472-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b2472-159">Version of the device configuration.</span></span> <span data-ttu-id="b2472-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b2472-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b2472-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b2472-161">passwordRequired</span></span>|<span data-ttu-id="b2472-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2472-162">Boolean</span></span>|<span data-ttu-id="b2472-163">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="b2472-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="b2472-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b2472-164">passwordBlockSimple</span></span>|<span data-ttu-id="b2472-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2472-165">Boolean</span></span>|<span data-ttu-id="b2472-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="b2472-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="b2472-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b2472-167">passwordExpirationDays</span></span>|<span data-ttu-id="b2472-168">Int32</span><span class="sxs-lookup"><span data-stu-id="b2472-168">Int32</span></span>|<span data-ttu-id="b2472-169">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="b2472-169">Password expiration in days.</span></span>|
|<span data-ttu-id="b2472-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b2472-170">passwordMinimumLength</span></span>|<span data-ttu-id="b2472-171">Int32</span><span class="sxs-lookup"><span data-stu-id="b2472-171">Int32</span></span>|<span data-ttu-id="b2472-172">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="b2472-172">The minimum password length.</span></span>|
|<span data-ttu-id="b2472-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b2472-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b2472-174">Int32</span><span class="sxs-lookup"><span data-stu-id="b2472-174">Int32</span></span>|<span data-ttu-id="b2472-175">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b2472-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b2472-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b2472-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b2472-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b2472-177">Int32</span></span>|<span data-ttu-id="b2472-178">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="b2472-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b2472-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b2472-179">passwordRequiredType</span></span>|[<span data-ttu-id="b2472-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b2472-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b2472-181">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="b2472-181">The required password type.</span></span> <span data-ttu-id="b2472-182">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="b2472-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b2472-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b2472-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b2472-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b2472-184">Int32</span></span>|<span data-ttu-id="b2472-185">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="b2472-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="b2472-186">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="b2472-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b2472-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b2472-187">osMinimumVersion</span></span>|<span data-ttu-id="b2472-188">String</span><span class="sxs-lookup"><span data-stu-id="b2472-188">String</span></span>|<span data-ttu-id="b2472-189">最低 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="b2472-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="b2472-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b2472-190">osMaximumVersion</span></span>|<span data-ttu-id="b2472-191">String</span><span class="sxs-lookup"><span data-stu-id="b2472-191">String</span></span>|<span data-ttu-id="b2472-192">最高 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="b2472-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="b2472-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b2472-193">storageRequireEncryption</span></span>|<span data-ttu-id="b2472-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2472-194">Boolean</span></span>|<span data-ttu-id="b2472-195">指示是否要求对 Windows 8.1 设备加密。</span><span class="sxs-lookup"><span data-stu-id="b2472-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="b2472-196">响应</span><span class="sxs-lookup"><span data-stu-id="b2472-196">Response</span></span>
<span data-ttu-id="b2472-197">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2472-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2472-198">示例</span><span class="sxs-lookup"><span data-stu-id="b2472-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2472-199">请求</span><span class="sxs-lookup"><span data-stu-id="b2472-199">Request</span></span>
<span data-ttu-id="b2472-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b2472-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2472-201">响应</span><span class="sxs-lookup"><span data-stu-id="b2472-201">Response</span></span>
<span data-ttu-id="b2472-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2472-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




