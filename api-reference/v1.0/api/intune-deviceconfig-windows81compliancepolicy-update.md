---
title: 更新 windows81CompliancePolicy
description: 更新 windows81CompliancePolicy 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e137b310c38da7d19bc1f03c4aa2359c917abdf9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365129"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="b1a6f-103">更新 windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b1a6f-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="b1a6f-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1a6f-105">更新 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-105">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1a6f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b1a6f-106">Prerequisites</span></span>
<span data-ttu-id="b1a6f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1a6f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1a6f-109">Permission type</span></span>|<span data-ttu-id="b1a6f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b1a6f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1a6f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1a6f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b1a6f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1a6f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1a6f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1a6f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1a6f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-114">Not supported.</span></span>|
|<span data-ttu-id="b1a6f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1a6f-115">Application</span></span>|<span data-ttu-id="b1a6f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1a6f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1a6f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b1a6f-118">请求头</span><span class="sxs-lookup"><span data-stu-id="b1a6f-118">Request headers</span></span>
|<span data-ttu-id="b1a6f-119">标头</span><span class="sxs-lookup"><span data-stu-id="b1a6f-119">Header</span></span>|<span data-ttu-id="b1a6f-120">值</span><span class="sxs-lookup"><span data-stu-id="b1a6f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1a6f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1a6f-121">Authorization</span></span>|<span data-ttu-id="b1a6f-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1a6f-123">接受</span><span class="sxs-lookup"><span data-stu-id="b1a6f-123">Accept</span></span>|<span data-ttu-id="b1a6f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b1a6f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1a6f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1a6f-125">Request body</span></span>
<span data-ttu-id="b1a6f-126">在请求正文中，提供 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-126">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="b1a6f-127">下表显示创建 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-127">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="b1a6f-128">属性</span><span class="sxs-lookup"><span data-stu-id="b1a6f-128">Property</span></span>|<span data-ttu-id="b1a6f-129">类型</span><span class="sxs-lookup"><span data-stu-id="b1a6f-129">Type</span></span>|<span data-ttu-id="b1a6f-130">说明</span><span class="sxs-lookup"><span data-stu-id="b1a6f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1a6f-131">id</span><span class="sxs-lookup"><span data-stu-id="b1a6f-131">id</span></span>|<span data-ttu-id="b1a6f-132">字符串</span><span class="sxs-lookup"><span data-stu-id="b1a6f-132">String</span></span>|<span data-ttu-id="b1a6f-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-133">Key of the entity.</span></span> <span data-ttu-id="b1a6f-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1a6f-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1a6f-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1a6f-135">createdDateTime</span></span>|<span data-ttu-id="b1a6f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1a6f-136">DateTimeOffset</span></span>|<span data-ttu-id="b1a6f-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-137">DateTime the object was created.</span></span> <span data-ttu-id="b1a6f-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1a6f-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1a6f-139">说明</span><span class="sxs-lookup"><span data-stu-id="b1a6f-139">description</span></span>|<span data-ttu-id="b1a6f-140">String</span><span class="sxs-lookup"><span data-stu-id="b1a6f-140">String</span></span>|<span data-ttu-id="b1a6f-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b1a6f-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1a6f-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1a6f-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1a6f-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b1a6f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1a6f-144">DateTimeOffset</span></span>|<span data-ttu-id="b1a6f-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-145">DateTime the object was last modified.</span></span> <span data-ttu-id="b1a6f-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1a6f-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1a6f-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b1a6f-147">displayName</span></span>|<span data-ttu-id="b1a6f-148">字符串</span><span class="sxs-lookup"><span data-stu-id="b1a6f-148">String</span></span>|<span data-ttu-id="b1a6f-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b1a6f-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1a6f-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1a6f-151">version</span><span class="sxs-lookup"><span data-stu-id="b1a6f-151">version</span></span>|<span data-ttu-id="b1a6f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b1a6f-152">Int32</span></span>|<span data-ttu-id="b1a6f-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-153">Version of the device configuration.</span></span> <span data-ttu-id="b1a6f-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1a6f-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1a6f-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b1a6f-155">passwordRequired</span></span>|<span data-ttu-id="b1a6f-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1a6f-156">Boolean</span></span>|<span data-ttu-id="b1a6f-157">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="b1a6f-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b1a6f-158">passwordBlockSimple</span></span>|<span data-ttu-id="b1a6f-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1a6f-159">Boolean</span></span>|<span data-ttu-id="b1a6f-160">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="b1a6f-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b1a6f-161">passwordExpirationDays</span></span>|<span data-ttu-id="b1a6f-162">Int32</span><span class="sxs-lookup"><span data-stu-id="b1a6f-162">Int32</span></span>|<span data-ttu-id="b1a6f-163">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-163">Password expiration in days.</span></span>|
|<span data-ttu-id="b1a6f-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b1a6f-164">passwordMinimumLength</span></span>|<span data-ttu-id="b1a6f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b1a6f-165">Int32</span></span>|<span data-ttu-id="b1a6f-166">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-166">The minimum password length.</span></span>|
|<span data-ttu-id="b1a6f-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b1a6f-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b1a6f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="b1a6f-168">Int32</span></span>|<span data-ttu-id="b1a6f-169">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b1a6f-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b1a6f-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b1a6f-171">Int32</span><span class="sxs-lookup"><span data-stu-id="b1a6f-171">Int32</span></span>|<span data-ttu-id="b1a6f-172">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b1a6f-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b1a6f-173">passwordRequiredType</span></span>|[<span data-ttu-id="b1a6f-174">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b1a6f-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b1a6f-175">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-175">The required password type.</span></span> <span data-ttu-id="b1a6f-176">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b1a6f-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b1a6f-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b1a6f-178">Int32</span><span class="sxs-lookup"><span data-stu-id="b1a6f-178">Int32</span></span>|<span data-ttu-id="b1a6f-179">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-179">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="b1a6f-180">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="b1a6f-180">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b1a6f-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b1a6f-181">osMinimumVersion</span></span>|<span data-ttu-id="b1a6f-182">String</span><span class="sxs-lookup"><span data-stu-id="b1a6f-182">String</span></span>|<span data-ttu-id="b1a6f-183">最低 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-183">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="b1a6f-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b1a6f-184">osMaximumVersion</span></span>|<span data-ttu-id="b1a6f-185">String</span><span class="sxs-lookup"><span data-stu-id="b1a6f-185">String</span></span>|<span data-ttu-id="b1a6f-186">最高 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-186">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="b1a6f-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b1a6f-187">storageRequireEncryption</span></span>|<span data-ttu-id="b1a6f-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1a6f-188">Boolean</span></span>|<span data-ttu-id="b1a6f-189">指示是否要求对 Windows 8.1 设备加密。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-189">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="b1a6f-190">响应</span><span class="sxs-lookup"><span data-stu-id="b1a6f-190">Response</span></span>
<span data-ttu-id="b1a6f-191">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-191">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1a6f-192">示例</span><span class="sxs-lookup"><span data-stu-id="b1a6f-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1a6f-193">请求</span><span class="sxs-lookup"><span data-stu-id="b1a6f-193">Request</span></span>
<span data-ttu-id="b1a6f-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="b1a6f-195">响应</span><span class="sxs-lookup"><span data-stu-id="b1a6f-195">Response</span></span>
<span data-ttu-id="b1a6f-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1a6f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 774

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
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




