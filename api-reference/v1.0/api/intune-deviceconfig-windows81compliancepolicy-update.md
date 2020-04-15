---
title: 更新 windows81CompliancePolicy
description: 更新 windows81CompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 094e7146382993ba700b8b85ee63a659b741bcde
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441936"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="dbd3a-103">更新 windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="dbd3a-103">Update windows81CompliancePolicy</span></span>

<span data-ttu-id="dbd3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbd3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbd3a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbd3a-106">更新 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-106">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbd3a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dbd3a-107">Prerequisites</span></span>
<span data-ttu-id="dbd3a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbd3a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbd3a-110">Permission type</span></span>|<span data-ttu-id="dbd3a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dbd3a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbd3a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbd3a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dbd3a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbd3a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dbd3a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbd3a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbd3a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-115">Not supported.</span></span>|
|<span data-ttu-id="dbd3a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbd3a-116">Application</span></span>|<span data-ttu-id="dbd3a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbd3a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbd3a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="dbd3a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dbd3a-119">Request headers</span></span>
|<span data-ttu-id="dbd3a-120">标头</span><span class="sxs-lookup"><span data-stu-id="dbd3a-120">Header</span></span>|<span data-ttu-id="dbd3a-121">值</span><span class="sxs-lookup"><span data-stu-id="dbd3a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbd3a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbd3a-122">Authorization</span></span>|<span data-ttu-id="dbd3a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbd3a-124">接受</span><span class="sxs-lookup"><span data-stu-id="dbd3a-124">Accept</span></span>|<span data-ttu-id="dbd3a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dbd3a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbd3a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dbd3a-126">Request body</span></span>
<span data-ttu-id="dbd3a-127">在请求正文中，提供 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-127">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="dbd3a-128">下表显示创建 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-128">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="dbd3a-129">属性</span><span class="sxs-lookup"><span data-stu-id="dbd3a-129">Property</span></span>|<span data-ttu-id="dbd3a-130">类型</span><span class="sxs-lookup"><span data-stu-id="dbd3a-130">Type</span></span>|<span data-ttu-id="dbd3a-131">说明</span><span class="sxs-lookup"><span data-stu-id="dbd3a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbd3a-132">id</span><span class="sxs-lookup"><span data-stu-id="dbd3a-132">id</span></span>|<span data-ttu-id="dbd3a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="dbd3a-133">String</span></span>|<span data-ttu-id="dbd3a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-134">Key of the entity.</span></span> <span data-ttu-id="dbd3a-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dbd3a-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dbd3a-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dbd3a-136">createdDateTime</span></span>|<span data-ttu-id="dbd3a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbd3a-137">DateTimeOffset</span></span>|<span data-ttu-id="dbd3a-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-138">DateTime the object was created.</span></span> <span data-ttu-id="dbd3a-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dbd3a-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dbd3a-140">description</span><span class="sxs-lookup"><span data-stu-id="dbd3a-140">description</span></span>|<span data-ttu-id="dbd3a-141">String</span><span class="sxs-lookup"><span data-stu-id="dbd3a-141">String</span></span>|<span data-ttu-id="dbd3a-142">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dbd3a-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dbd3a-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dbd3a-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbd3a-144">lastModifiedDateTime</span></span>|<span data-ttu-id="dbd3a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbd3a-145">DateTimeOffset</span></span>|<span data-ttu-id="dbd3a-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-146">DateTime the object was last modified.</span></span> <span data-ttu-id="dbd3a-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dbd3a-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dbd3a-148">displayName</span><span class="sxs-lookup"><span data-stu-id="dbd3a-148">displayName</span></span>|<span data-ttu-id="dbd3a-149">字符串</span><span class="sxs-lookup"><span data-stu-id="dbd3a-149">String</span></span>|<span data-ttu-id="dbd3a-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dbd3a-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dbd3a-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dbd3a-152">version</span><span class="sxs-lookup"><span data-stu-id="dbd3a-152">version</span></span>|<span data-ttu-id="dbd3a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="dbd3a-153">Int32</span></span>|<span data-ttu-id="dbd3a-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-154">Version of the device configuration.</span></span> <span data-ttu-id="dbd3a-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dbd3a-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dbd3a-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="dbd3a-156">passwordRequired</span></span>|<span data-ttu-id="dbd3a-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbd3a-157">Boolean</span></span>|<span data-ttu-id="dbd3a-158">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-158">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="dbd3a-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="dbd3a-159">passwordBlockSimple</span></span>|<span data-ttu-id="dbd3a-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbd3a-160">Boolean</span></span>|<span data-ttu-id="dbd3a-161">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-161">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="dbd3a-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="dbd3a-162">passwordExpirationDays</span></span>|<span data-ttu-id="dbd3a-163">Int32</span><span class="sxs-lookup"><span data-stu-id="dbd3a-163">Int32</span></span>|<span data-ttu-id="dbd3a-164">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-164">Password expiration in days.</span></span>|
|<span data-ttu-id="dbd3a-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="dbd3a-165">passwordMinimumLength</span></span>|<span data-ttu-id="dbd3a-166">Int32</span><span class="sxs-lookup"><span data-stu-id="dbd3a-166">Int32</span></span>|<span data-ttu-id="dbd3a-167">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-167">The minimum password length.</span></span>|
|<span data-ttu-id="dbd3a-168">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="dbd3a-168">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="dbd3a-169">Int32</span><span class="sxs-lookup"><span data-stu-id="dbd3a-169">Int32</span></span>|<span data-ttu-id="dbd3a-170">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-170">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="dbd3a-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="dbd3a-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="dbd3a-172">Int32</span><span class="sxs-lookup"><span data-stu-id="dbd3a-172">Int32</span></span>|<span data-ttu-id="dbd3a-173">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="dbd3a-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="dbd3a-174">passwordRequiredType</span></span>|[<span data-ttu-id="dbd3a-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="dbd3a-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="dbd3a-176">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-176">The required password type.</span></span> <span data-ttu-id="dbd3a-177">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="dbd3a-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="dbd3a-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="dbd3a-179">Int32</span><span class="sxs-lookup"><span data-stu-id="dbd3a-179">Int32</span></span>|<span data-ttu-id="dbd3a-180">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-180">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="dbd3a-181">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="dbd3a-181">Valid values 0 to 24</span></span>|
|<span data-ttu-id="dbd3a-182">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="dbd3a-182">osMinimumVersion</span></span>|<span data-ttu-id="dbd3a-183">String</span><span class="sxs-lookup"><span data-stu-id="dbd3a-183">String</span></span>|<span data-ttu-id="dbd3a-184">最低 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-184">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="dbd3a-185">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="dbd3a-185">osMaximumVersion</span></span>|<span data-ttu-id="dbd3a-186">String</span><span class="sxs-lookup"><span data-stu-id="dbd3a-186">String</span></span>|<span data-ttu-id="dbd3a-187">最高 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-187">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="dbd3a-188">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="dbd3a-188">storageRequireEncryption</span></span>|<span data-ttu-id="dbd3a-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbd3a-189">Boolean</span></span>|<span data-ttu-id="dbd3a-190">指示是否要求对 Windows 8.1 设备加密。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-190">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="dbd3a-191">响应</span><span class="sxs-lookup"><span data-stu-id="dbd3a-191">Response</span></span>
<span data-ttu-id="dbd3a-192">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-192">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbd3a-193">示例</span><span class="sxs-lookup"><span data-stu-id="dbd3a-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbd3a-194">请求</span><span class="sxs-lookup"><span data-stu-id="dbd3a-194">Request</span></span>
<span data-ttu-id="dbd3a-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dbd3a-196">响应</span><span class="sxs-lookup"><span data-stu-id="dbd3a-196">Response</span></span>
<span data-ttu-id="dbd3a-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dbd3a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






