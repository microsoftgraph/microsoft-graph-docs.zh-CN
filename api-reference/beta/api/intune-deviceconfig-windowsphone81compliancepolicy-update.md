---
title: 更新 windowsPhone81CompliancePolicy
description: 更新 windowsPhone81CompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 81d09436a7a328763f6a3d6d3c71b4865d8c85e2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49286456"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="2d32a-103">更新 windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2d32a-103">Update windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="2d32a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d32a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d32a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2d32a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d32a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d32a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d32a-107">更新 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2d32a-107">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d32a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2d32a-108">Prerequisites</span></span>
<span data-ttu-id="2d32a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d32a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d32a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d32a-111">Permission type</span></span>|<span data-ttu-id="2d32a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2d32a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d32a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d32a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d32a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d32a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d32a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d32a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d32a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d32a-116">Not supported.</span></span>|
|<span data-ttu-id="2d32a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d32a-117">Application</span></span>|<span data-ttu-id="2d32a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d32a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d32a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d32a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="2d32a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d32a-120">Request headers</span></span>
|<span data-ttu-id="2d32a-121">标头</span><span class="sxs-lookup"><span data-stu-id="2d32a-121">Header</span></span>|<span data-ttu-id="2d32a-122">值</span><span class="sxs-lookup"><span data-stu-id="2d32a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d32a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d32a-123">Authorization</span></span>|<span data-ttu-id="2d32a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2d32a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d32a-125">接受</span><span class="sxs-lookup"><span data-stu-id="2d32a-125">Accept</span></span>|<span data-ttu-id="2d32a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d32a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d32a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d32a-127">Request body</span></span>
<span data-ttu-id="2d32a-128">在请求正文中，提供 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d32a-128">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="2d32a-129">下表显示创建 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2d32a-129">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="2d32a-130">属性</span><span class="sxs-lookup"><span data-stu-id="2d32a-130">Property</span></span>|<span data-ttu-id="2d32a-131">类型</span><span class="sxs-lookup"><span data-stu-id="2d32a-131">Type</span></span>|<span data-ttu-id="2d32a-132">Description</span><span class="sxs-lookup"><span data-stu-id="2d32a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d32a-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2d32a-133">roleScopeTagIds</span></span>|<span data-ttu-id="2d32a-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="2d32a-134">String collection</span></span>|<span data-ttu-id="2d32a-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2d32a-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2d32a-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2d32a-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2d32a-137">id</span><span class="sxs-lookup"><span data-stu-id="2d32a-137">id</span></span>|<span data-ttu-id="2d32a-138">字符串</span><span class="sxs-lookup"><span data-stu-id="2d32a-138">String</span></span>|<span data-ttu-id="2d32a-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2d32a-139">Key of the entity.</span></span> <span data-ttu-id="2d32a-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2d32a-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2d32a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d32a-141">createdDateTime</span></span>|<span data-ttu-id="2d32a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d32a-142">DateTimeOffset</span></span>|<span data-ttu-id="2d32a-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2d32a-143">DateTime the object was created.</span></span> <span data-ttu-id="2d32a-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2d32a-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2d32a-145">description</span><span class="sxs-lookup"><span data-stu-id="2d32a-145">description</span></span>|<span data-ttu-id="2d32a-146">字符串</span><span class="sxs-lookup"><span data-stu-id="2d32a-146">String</span></span>|<span data-ttu-id="2d32a-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2d32a-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2d32a-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2d32a-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2d32a-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d32a-149">lastModifiedDateTime</span></span>|<span data-ttu-id="2d32a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d32a-150">DateTimeOffset</span></span>|<span data-ttu-id="2d32a-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2d32a-151">DateTime the object was last modified.</span></span> <span data-ttu-id="2d32a-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2d32a-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2d32a-153">displayName</span><span class="sxs-lookup"><span data-stu-id="2d32a-153">displayName</span></span>|<span data-ttu-id="2d32a-154">字符串</span><span class="sxs-lookup"><span data-stu-id="2d32a-154">String</span></span>|<span data-ttu-id="2d32a-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2d32a-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2d32a-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2d32a-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2d32a-157">version</span><span class="sxs-lookup"><span data-stu-id="2d32a-157">version</span></span>|<span data-ttu-id="2d32a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="2d32a-158">Int32</span></span>|<span data-ttu-id="2d32a-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2d32a-159">Version of the device configuration.</span></span> <span data-ttu-id="2d32a-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2d32a-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2d32a-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="2d32a-161">passwordBlockSimple</span></span>|<span data-ttu-id="2d32a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d32a-162">Boolean</span></span>|<span data-ttu-id="2d32a-163">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="2d32a-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="2d32a-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2d32a-164">passwordExpirationDays</span></span>|<span data-ttu-id="2d32a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2d32a-165">Int32</span></span>|<span data-ttu-id="2d32a-166">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="2d32a-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="2d32a-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2d32a-167">passwordMinimumLength</span></span>|<span data-ttu-id="2d32a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="2d32a-168">Int32</span></span>|<span data-ttu-id="2d32a-169">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="2d32a-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="2d32a-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="2d32a-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="2d32a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="2d32a-171">Int32</span></span>|<span data-ttu-id="2d32a-172">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="2d32a-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="2d32a-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="2d32a-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="2d32a-174">Int32</span><span class="sxs-lookup"><span data-stu-id="2d32a-174">Int32</span></span>|<span data-ttu-id="2d32a-175">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="2d32a-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="2d32a-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2d32a-176">passwordRequiredType</span></span>|[<span data-ttu-id="2d32a-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2d32a-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="2d32a-178">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="2d32a-178">The required password type.</span></span> <span data-ttu-id="2d32a-179">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="2d32a-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="2d32a-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2d32a-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2d32a-181">Int32</span><span class="sxs-lookup"><span data-stu-id="2d32a-181">Int32</span></span>|<span data-ttu-id="2d32a-182">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="2d32a-182">Number of previous passwords to block.</span></span> <span data-ttu-id="2d32a-183">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="2d32a-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2d32a-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="2d32a-184">passwordRequired</span></span>|<span data-ttu-id="2d32a-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d32a-185">Boolean</span></span>|<span data-ttu-id="2d32a-186">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="2d32a-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="2d32a-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2d32a-187">osMinimumVersion</span></span>|<span data-ttu-id="2d32a-188">String</span><span class="sxs-lookup"><span data-stu-id="2d32a-188">String</span></span>|<span data-ttu-id="2d32a-189">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="2d32a-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="2d32a-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2d32a-190">osMaximumVersion</span></span>|<span data-ttu-id="2d32a-191">String</span><span class="sxs-lookup"><span data-stu-id="2d32a-191">String</span></span>|<span data-ttu-id="2d32a-192">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="2d32a-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="2d32a-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="2d32a-193">storageRequireEncryption</span></span>|<span data-ttu-id="2d32a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d32a-194">Boolean</span></span>|<span data-ttu-id="2d32a-195">要求对 Windows Phone 设备加密。</span><span class="sxs-lookup"><span data-stu-id="2d32a-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="2d32a-196">响应</span><span class="sxs-lookup"><span data-stu-id="2d32a-196">Response</span></span>
<span data-ttu-id="2d32a-197">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2d32a-197">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d32a-198">示例</span><span class="sxs-lookup"><span data-stu-id="2d32a-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d32a-199">请求</span><span class="sxs-lookup"><span data-stu-id="2d32a-199">Request</span></span>
<span data-ttu-id="2d32a-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d32a-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2d32a-201">响应</span><span class="sxs-lookup"><span data-stu-id="2d32a-201">Response</span></span>
<span data-ttu-id="2d32a-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2d32a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




