---
title: 创建 windowsPhone81CompliancePolicy
description: 创建新的 windowsPhone81CompliancePolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed87c8639fff2a1399cd88b1ad6dd30c800e70b5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462024"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="df29d-103">创建 windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="df29d-103">Create windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="df29d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df29d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df29d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df29d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df29d-106">创建新的 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df29d-106">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df29d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="df29d-107">Prerequisites</span></span>
<span data-ttu-id="df29d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df29d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df29d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="df29d-110">Permission type</span></span>|<span data-ttu-id="df29d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df29d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df29d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df29d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df29d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df29d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df29d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df29d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df29d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="df29d-115">Not supported.</span></span>|
|<span data-ttu-id="df29d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="df29d-116">Application</span></span>|<span data-ttu-id="df29d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="df29d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df29d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df29d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="df29d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="df29d-119">Request headers</span></span>
|<span data-ttu-id="df29d-120">标头</span><span class="sxs-lookup"><span data-stu-id="df29d-120">Header</span></span>|<span data-ttu-id="df29d-121">值</span><span class="sxs-lookup"><span data-stu-id="df29d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df29d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="df29d-122">Authorization</span></span>|<span data-ttu-id="df29d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df29d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df29d-124">接受</span><span class="sxs-lookup"><span data-stu-id="df29d-124">Accept</span></span>|<span data-ttu-id="df29d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df29d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df29d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="df29d-126">Request body</span></span>
<span data-ttu-id="df29d-127">在请求正文中，提供 windowsPhone81CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df29d-127">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="df29d-128">下表显示创建 windowsPhone81CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="df29d-128">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="df29d-129">属性</span><span class="sxs-lookup"><span data-stu-id="df29d-129">Property</span></span>|<span data-ttu-id="df29d-130">类型</span><span class="sxs-lookup"><span data-stu-id="df29d-130">Type</span></span>|<span data-ttu-id="df29d-131">说明</span><span class="sxs-lookup"><span data-stu-id="df29d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df29d-132">id</span><span class="sxs-lookup"><span data-stu-id="df29d-132">id</span></span>|<span data-ttu-id="df29d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="df29d-133">String</span></span>|<span data-ttu-id="df29d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="df29d-134">Key of the entity.</span></span> <span data-ttu-id="df29d-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df29d-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="df29d-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df29d-136">createdDateTime</span></span>|<span data-ttu-id="df29d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df29d-137">DateTimeOffset</span></span>|<span data-ttu-id="df29d-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="df29d-138">DateTime the object was created.</span></span> <span data-ttu-id="df29d-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df29d-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="df29d-140">description</span><span class="sxs-lookup"><span data-stu-id="df29d-140">description</span></span>|<span data-ttu-id="df29d-141">String</span><span class="sxs-lookup"><span data-stu-id="df29d-141">String</span></span>|<span data-ttu-id="df29d-142">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="df29d-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="df29d-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df29d-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="df29d-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df29d-144">lastModifiedDateTime</span></span>|<span data-ttu-id="df29d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df29d-145">DateTimeOffset</span></span>|<span data-ttu-id="df29d-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="df29d-146">DateTime the object was last modified.</span></span> <span data-ttu-id="df29d-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df29d-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="df29d-148">displayName</span><span class="sxs-lookup"><span data-stu-id="df29d-148">displayName</span></span>|<span data-ttu-id="df29d-149">字符串</span><span class="sxs-lookup"><span data-stu-id="df29d-149">String</span></span>|<span data-ttu-id="df29d-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="df29d-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="df29d-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df29d-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="df29d-152">version</span><span class="sxs-lookup"><span data-stu-id="df29d-152">version</span></span>|<span data-ttu-id="df29d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="df29d-153">Int32</span></span>|<span data-ttu-id="df29d-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="df29d-154">Version of the device configuration.</span></span> <span data-ttu-id="df29d-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df29d-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="df29d-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="df29d-156">passwordBlockSimple</span></span>|<span data-ttu-id="df29d-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="df29d-157">Boolean</span></span>|<span data-ttu-id="df29d-158">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="df29d-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="df29d-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="df29d-159">passwordExpirationDays</span></span>|<span data-ttu-id="df29d-160">Int32</span><span class="sxs-lookup"><span data-stu-id="df29d-160">Int32</span></span>|<span data-ttu-id="df29d-161">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="df29d-161">Number of days before the password expires.</span></span>|
|<span data-ttu-id="df29d-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="df29d-162">passwordMinimumLength</span></span>|<span data-ttu-id="df29d-163">Int32</span><span class="sxs-lookup"><span data-stu-id="df29d-163">Int32</span></span>|<span data-ttu-id="df29d-164">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="df29d-164">Minimum length of passwords.</span></span>|
|<span data-ttu-id="df29d-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="df29d-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="df29d-166">Int32</span><span class="sxs-lookup"><span data-stu-id="df29d-166">Int32</span></span>|<span data-ttu-id="df29d-167">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="df29d-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="df29d-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="df29d-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="df29d-169">Int32</span><span class="sxs-lookup"><span data-stu-id="df29d-169">Int32</span></span>|<span data-ttu-id="df29d-170">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="df29d-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="df29d-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="df29d-171">passwordRequiredType</span></span>|[<span data-ttu-id="df29d-172">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="df29d-172">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="df29d-173">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="df29d-173">The required password type.</span></span> <span data-ttu-id="df29d-174">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="df29d-174">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="df29d-175">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="df29d-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="df29d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="df29d-176">Int32</span></span>|<span data-ttu-id="df29d-177">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="df29d-177">Number of previous passwords to block.</span></span> <span data-ttu-id="df29d-178">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="df29d-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="df29d-179">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="df29d-179">passwordRequired</span></span>|<span data-ttu-id="df29d-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="df29d-180">Boolean</span></span>|<span data-ttu-id="df29d-181">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="df29d-181">Whether or not to require a password.</span></span>|
|<span data-ttu-id="df29d-182">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="df29d-182">osMinimumVersion</span></span>|<span data-ttu-id="df29d-183">String</span><span class="sxs-lookup"><span data-stu-id="df29d-183">String</span></span>|<span data-ttu-id="df29d-184">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="df29d-184">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="df29d-185">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="df29d-185">osMaximumVersion</span></span>|<span data-ttu-id="df29d-186">String</span><span class="sxs-lookup"><span data-stu-id="df29d-186">String</span></span>|<span data-ttu-id="df29d-187">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="df29d-187">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="df29d-188">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="df29d-188">storageRequireEncryption</span></span>|<span data-ttu-id="df29d-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="df29d-189">Boolean</span></span>|<span data-ttu-id="df29d-190">要求对 Windows Phone 设备加密。</span><span class="sxs-lookup"><span data-stu-id="df29d-190">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="df29d-191">响应</span><span class="sxs-lookup"><span data-stu-id="df29d-191">Response</span></span>
<span data-ttu-id="df29d-192">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df29d-192">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df29d-193">示例</span><span class="sxs-lookup"><span data-stu-id="df29d-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="df29d-194">请求</span><span class="sxs-lookup"><span data-stu-id="df29d-194">Request</span></span>
<span data-ttu-id="df29d-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df29d-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 607

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="df29d-196">响应</span><span class="sxs-lookup"><span data-stu-id="df29d-196">Response</span></span>
<span data-ttu-id="df29d-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df29d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 779

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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






