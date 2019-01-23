---
title: 更新 windows81CompliancePolicy
description: 更新 windows81CompliancePolicy 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 77b744aa62fddf7427496855a2e8a20239ff53ee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413575"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="8bade-103">更新 windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8bade-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="8bade-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="8bade-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8bade-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8bade-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8bade-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8bade-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bade-107">更新 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8bade-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bade-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8bade-108">Prerequisites</span></span>
<span data-ttu-id="8bade-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8bade-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8bade-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8bade-111">Permission type</span></span>|<span data-ttu-id="8bade-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8bade-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bade-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8bade-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8bade-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bade-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8bade-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8bade-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bade-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8bade-116">Not supported.</span></span>|
|<span data-ttu-id="8bade-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8bade-117">Application</span></span>|<span data-ttu-id="8bade-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8bade-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bade-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8bade-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="8bade-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8bade-120">Request headers</span></span>
|<span data-ttu-id="8bade-121">标头</span><span class="sxs-lookup"><span data-stu-id="8bade-121">Header</span></span>|<span data-ttu-id="8bade-122">值</span><span class="sxs-lookup"><span data-stu-id="8bade-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bade-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bade-123">Authorization</span></span>|<span data-ttu-id="8bade-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8bade-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bade-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8bade-125">Accept</span></span>|<span data-ttu-id="8bade-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8bade-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bade-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8bade-127">Request body</span></span>
<span data-ttu-id="8bade-128">在请求正文中，提供 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8bade-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="8bade-129">下表显示创建 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8bade-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="8bade-130">属性</span><span class="sxs-lookup"><span data-stu-id="8bade-130">Property</span></span>|<span data-ttu-id="8bade-131">类型</span><span class="sxs-lookup"><span data-stu-id="8bade-131">Type</span></span>|<span data-ttu-id="8bade-132">说明</span><span class="sxs-lookup"><span data-stu-id="8bade-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bade-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8bade-133">roleScopeTagIds</span></span>|<span data-ttu-id="8bade-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="8bade-134">String collection</span></span>|<span data-ttu-id="8bade-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="8bade-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8bade-136">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8bade-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8bade-137">id</span><span class="sxs-lookup"><span data-stu-id="8bade-137">id</span></span>|<span data-ttu-id="8bade-138">String</span><span class="sxs-lookup"><span data-stu-id="8bade-138">String</span></span>|<span data-ttu-id="8bade-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8bade-139">Key of the entity.</span></span> <span data-ttu-id="8bade-140">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8bade-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8bade-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8bade-141">createdDateTime</span></span>|<span data-ttu-id="8bade-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bade-142">DateTimeOffset</span></span>|<span data-ttu-id="8bade-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8bade-143">DateTime the object was created.</span></span> <span data-ttu-id="8bade-144">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8bade-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8bade-145">description</span><span class="sxs-lookup"><span data-stu-id="8bade-145">description</span></span>|<span data-ttu-id="8bade-146">String</span><span class="sxs-lookup"><span data-stu-id="8bade-146">String</span></span>|<span data-ttu-id="8bade-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8bade-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8bade-148">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8bade-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8bade-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bade-149">lastModifiedDateTime</span></span>|<span data-ttu-id="8bade-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bade-150">DateTimeOffset</span></span>|<span data-ttu-id="8bade-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8bade-151">DateTime the object was last modified.</span></span> <span data-ttu-id="8bade-152">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8bade-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8bade-153">displayName</span><span class="sxs-lookup"><span data-stu-id="8bade-153">displayName</span></span>|<span data-ttu-id="8bade-154">String</span><span class="sxs-lookup"><span data-stu-id="8bade-154">String</span></span>|<span data-ttu-id="8bade-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8bade-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8bade-156">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8bade-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8bade-157">version</span><span class="sxs-lookup"><span data-stu-id="8bade-157">version</span></span>|<span data-ttu-id="8bade-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8bade-158">Int32</span></span>|<span data-ttu-id="8bade-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8bade-159">Version of the device configuration.</span></span> <span data-ttu-id="8bade-160">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8bade-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8bade-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8bade-161">passwordRequired</span></span>|<span data-ttu-id="8bade-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bade-162">Boolean</span></span>|<span data-ttu-id="8bade-163">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="8bade-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="8bade-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="8bade-164">passwordBlockSimple</span></span>|<span data-ttu-id="8bade-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bade-165">Boolean</span></span>|<span data-ttu-id="8bade-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="8bade-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="8bade-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8bade-167">passwordExpirationDays</span></span>|<span data-ttu-id="8bade-168">Int32</span><span class="sxs-lookup"><span data-stu-id="8bade-168">Int32</span></span>|<span data-ttu-id="8bade-169">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="8bade-169">Password expiration in days.</span></span>|
|<span data-ttu-id="8bade-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8bade-170">passwordMinimumLength</span></span>|<span data-ttu-id="8bade-171">Int32</span><span class="sxs-lookup"><span data-stu-id="8bade-171">Int32</span></span>|<span data-ttu-id="8bade-172">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="8bade-172">The minimum password length.</span></span>|
|<span data-ttu-id="8bade-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8bade-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8bade-174">Int32</span><span class="sxs-lookup"><span data-stu-id="8bade-174">Int32</span></span>|<span data-ttu-id="8bade-175">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="8bade-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="8bade-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8bade-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8bade-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8bade-177">Int32</span></span>|<span data-ttu-id="8bade-178">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="8bade-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8bade-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8bade-179">passwordRequiredType</span></span>|[<span data-ttu-id="8bade-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8bade-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="8bade-181">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="8bade-181">The required password type.</span></span> <span data-ttu-id="8bade-182">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="8bade-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8bade-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8bade-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8bade-184">Int32</span><span class="sxs-lookup"><span data-stu-id="8bade-184">Int32</span></span>|<span data-ttu-id="8bade-185">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="8bade-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="8bade-186">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="8bade-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8bade-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8bade-187">osMinimumVersion</span></span>|<span data-ttu-id="8bade-188">String</span><span class="sxs-lookup"><span data-stu-id="8bade-188">String</span></span>|<span data-ttu-id="8bade-189">最低 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="8bade-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="8bade-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8bade-190">osMaximumVersion</span></span>|<span data-ttu-id="8bade-191">String</span><span class="sxs-lookup"><span data-stu-id="8bade-191">String</span></span>|<span data-ttu-id="8bade-192">最高 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="8bade-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="8bade-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="8bade-193">storageRequireEncryption</span></span>|<span data-ttu-id="8bade-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bade-194">Boolean</span></span>|<span data-ttu-id="8bade-195">指示是否要求对 Windows 8.1 设备加密。</span><span class="sxs-lookup"><span data-stu-id="8bade-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="8bade-196">响应</span><span class="sxs-lookup"><span data-stu-id="8bade-196">Response</span></span>
<span data-ttu-id="8bade-197">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8bade-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bade-198">示例</span><span class="sxs-lookup"><span data-stu-id="8bade-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bade-199">请求</span><span class="sxs-lookup"><span data-stu-id="8bade-199">Request</span></span>
<span data-ttu-id="8bade-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8bade-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8bade-201">响应</span><span class="sxs-lookup"><span data-stu-id="8bade-201">Response</span></span>
<span data-ttu-id="8bade-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8bade-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




