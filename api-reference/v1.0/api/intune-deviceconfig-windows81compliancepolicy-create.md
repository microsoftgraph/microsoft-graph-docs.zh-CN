---
title: 创建 windows81CompliancePolicy
description: 创建新的 windows81CompliancePolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b5cc71fa9e35021afae933079a76ea257328b37a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752656"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="c0b24-103">创建 windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c0b24-103">Create windows81CompliancePolicy</span></span>

<span data-ttu-id="c0b24-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0b24-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0b24-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0b24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0b24-106">创建新的 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0b24-106">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0b24-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c0b24-107">Prerequisites</span></span>
<span data-ttu-id="c0b24-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0b24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0b24-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0b24-110">Permission type</span></span>|<span data-ttu-id="c0b24-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0b24-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0b24-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0b24-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0b24-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0b24-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0b24-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0b24-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0b24-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0b24-115">Not supported.</span></span>|
|<span data-ttu-id="c0b24-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0b24-116">Application</span></span>|<span data-ttu-id="c0b24-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0b24-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0b24-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0b24-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c0b24-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0b24-119">Request headers</span></span>
|<span data-ttu-id="c0b24-120">标头</span><span class="sxs-lookup"><span data-stu-id="c0b24-120">Header</span></span>|<span data-ttu-id="c0b24-121">值</span><span class="sxs-lookup"><span data-stu-id="c0b24-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0b24-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0b24-122">Authorization</span></span>|<span data-ttu-id="c0b24-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c0b24-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0b24-124">接受</span><span class="sxs-lookup"><span data-stu-id="c0b24-124">Accept</span></span>|<span data-ttu-id="c0b24-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0b24-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0b24-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0b24-126">Request body</span></span>
<span data-ttu-id="c0b24-127">在请求正文中，提供 windows81CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0b24-127">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="c0b24-128">下表显示创建 windows81CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c0b24-128">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="c0b24-129">属性</span><span class="sxs-lookup"><span data-stu-id="c0b24-129">Property</span></span>|<span data-ttu-id="c0b24-130">类型</span><span class="sxs-lookup"><span data-stu-id="c0b24-130">Type</span></span>|<span data-ttu-id="c0b24-131">说明</span><span class="sxs-lookup"><span data-stu-id="c0b24-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0b24-132">id</span><span class="sxs-lookup"><span data-stu-id="c0b24-132">id</span></span>|<span data-ttu-id="c0b24-133">String</span><span class="sxs-lookup"><span data-stu-id="c0b24-133">String</span></span>|<span data-ttu-id="c0b24-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c0b24-134">Key of the entity.</span></span> <span data-ttu-id="c0b24-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c0b24-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c0b24-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0b24-136">createdDateTime</span></span>|<span data-ttu-id="c0b24-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0b24-137">DateTimeOffset</span></span>|<span data-ttu-id="c0b24-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c0b24-138">DateTime the object was created.</span></span> <span data-ttu-id="c0b24-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c0b24-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c0b24-140">说明</span><span class="sxs-lookup"><span data-stu-id="c0b24-140">description</span></span>|<span data-ttu-id="c0b24-141">String</span><span class="sxs-lookup"><span data-stu-id="c0b24-141">String</span></span>|<span data-ttu-id="c0b24-142">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c0b24-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c0b24-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c0b24-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c0b24-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0b24-144">lastModifiedDateTime</span></span>|<span data-ttu-id="c0b24-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0b24-145">DateTimeOffset</span></span>|<span data-ttu-id="c0b24-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c0b24-146">DateTime the object was last modified.</span></span> <span data-ttu-id="c0b24-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c0b24-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c0b24-148">displayName</span><span class="sxs-lookup"><span data-stu-id="c0b24-148">displayName</span></span>|<span data-ttu-id="c0b24-149">String</span><span class="sxs-lookup"><span data-stu-id="c0b24-149">String</span></span>|<span data-ttu-id="c0b24-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c0b24-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c0b24-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c0b24-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c0b24-152">version</span><span class="sxs-lookup"><span data-stu-id="c0b24-152">version</span></span>|<span data-ttu-id="c0b24-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c0b24-153">Int32</span></span>|<span data-ttu-id="c0b24-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c0b24-154">Version of the device configuration.</span></span> <span data-ttu-id="c0b24-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c0b24-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c0b24-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c0b24-156">passwordRequired</span></span>|<span data-ttu-id="c0b24-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0b24-157">Boolean</span></span>|<span data-ttu-id="c0b24-158">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="c0b24-158">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="c0b24-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c0b24-159">passwordBlockSimple</span></span>|<span data-ttu-id="c0b24-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0b24-160">Boolean</span></span>|<span data-ttu-id="c0b24-161">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="c0b24-161">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="c0b24-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c0b24-162">passwordExpirationDays</span></span>|<span data-ttu-id="c0b24-163">Int32</span><span class="sxs-lookup"><span data-stu-id="c0b24-163">Int32</span></span>|<span data-ttu-id="c0b24-164">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="c0b24-164">Password expiration in days.</span></span>|
|<span data-ttu-id="c0b24-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c0b24-165">passwordMinimumLength</span></span>|<span data-ttu-id="c0b24-166">Int32</span><span class="sxs-lookup"><span data-stu-id="c0b24-166">Int32</span></span>|<span data-ttu-id="c0b24-167">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="c0b24-167">The minimum password length.</span></span>|
|<span data-ttu-id="c0b24-168">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c0b24-168">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c0b24-169">Int32</span><span class="sxs-lookup"><span data-stu-id="c0b24-169">Int32</span></span>|<span data-ttu-id="c0b24-170">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c0b24-170">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c0b24-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c0b24-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c0b24-172">Int32</span><span class="sxs-lookup"><span data-stu-id="c0b24-172">Int32</span></span>|<span data-ttu-id="c0b24-173">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="c0b24-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c0b24-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c0b24-174">passwordRequiredType</span></span>|[<span data-ttu-id="c0b24-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c0b24-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c0b24-176">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="c0b24-176">The required password type.</span></span> <span data-ttu-id="c0b24-177">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="c0b24-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c0b24-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c0b24-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c0b24-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c0b24-179">Int32</span></span>|<span data-ttu-id="c0b24-180">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="c0b24-180">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="c0b24-181">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="c0b24-181">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c0b24-182">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c0b24-182">osMinimumVersion</span></span>|<span data-ttu-id="c0b24-183">String</span><span class="sxs-lookup"><span data-stu-id="c0b24-183">String</span></span>|<span data-ttu-id="c0b24-184">最低 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="c0b24-184">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="c0b24-185">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c0b24-185">osMaximumVersion</span></span>|<span data-ttu-id="c0b24-186">String</span><span class="sxs-lookup"><span data-stu-id="c0b24-186">String</span></span>|<span data-ttu-id="c0b24-187">最高 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="c0b24-187">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="c0b24-188">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c0b24-188">storageRequireEncryption</span></span>|<span data-ttu-id="c0b24-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0b24-189">Boolean</span></span>|<span data-ttu-id="c0b24-190">指示是否要求对 Windows 8.1 设备加密。</span><span class="sxs-lookup"><span data-stu-id="c0b24-190">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="c0b24-191">响应</span><span class="sxs-lookup"><span data-stu-id="c0b24-191">Response</span></span>
<span data-ttu-id="c0b24-192">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0b24-192">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0b24-193">示例</span><span class="sxs-lookup"><span data-stu-id="c0b24-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0b24-194">请求</span><span class="sxs-lookup"><span data-stu-id="c0b24-194">Request</span></span>
<span data-ttu-id="c0b24-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0b24-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="c0b24-196">响应</span><span class="sxs-lookup"><span data-stu-id="c0b24-196">Response</span></span>
<span data-ttu-id="c0b24-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c0b24-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




