---
title: 创建 windowsPhone81CompliancePolicy
description: 创建新的 windowsPhone81CompliancePolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f544441787f8c5003a0831402d157436febdb1a8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567072"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="e725d-103">创建 windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e725d-103">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="e725d-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e725d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e725d-105">创建新的 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e725d-105">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e725d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="e725d-106">Prerequisites</span></span>
<span data-ttu-id="e725d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e725d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e725d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e725d-109">Permission type</span></span>|<span data-ttu-id="e725d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e725d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e725d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e725d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e725d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e725d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e725d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e725d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e725d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e725d-114">Not supported.</span></span>|
|<span data-ttu-id="e725d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e725d-115">Application</span></span>|<span data-ttu-id="e725d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e725d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e725d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e725d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e725d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e725d-118">Request headers</span></span>
|<span data-ttu-id="e725d-119">标头</span><span class="sxs-lookup"><span data-stu-id="e725d-119">Header</span></span>|<span data-ttu-id="e725d-120">值</span><span class="sxs-lookup"><span data-stu-id="e725d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e725d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e725d-121">Authorization</span></span>|<span data-ttu-id="e725d-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e725d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e725d-123">接受</span><span class="sxs-lookup"><span data-stu-id="e725d-123">Accept</span></span>|<span data-ttu-id="e725d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e725d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e725d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e725d-125">Request body</span></span>
<span data-ttu-id="e725d-126">在请求正文中，提供 windowsPhone81CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e725d-126">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="e725d-127">下表显示创建 windowsPhone81CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e725d-127">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="e725d-128">属性</span><span class="sxs-lookup"><span data-stu-id="e725d-128">Property</span></span>|<span data-ttu-id="e725d-129">类型</span><span class="sxs-lookup"><span data-stu-id="e725d-129">Type</span></span>|<span data-ttu-id="e725d-130">说明</span><span class="sxs-lookup"><span data-stu-id="e725d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e725d-131">id</span><span class="sxs-lookup"><span data-stu-id="e725d-131">id</span></span>|<span data-ttu-id="e725d-132">字符串</span><span class="sxs-lookup"><span data-stu-id="e725d-132">String</span></span>|<span data-ttu-id="e725d-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e725d-133">Key of the entity.</span></span> <span data-ttu-id="e725d-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e725d-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e725d-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e725d-135">createdDateTime</span></span>|<span data-ttu-id="e725d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e725d-136">DateTimeOffset</span></span>|<span data-ttu-id="e725d-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e725d-137">DateTime the object was created.</span></span> <span data-ttu-id="e725d-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e725d-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e725d-139">说明</span><span class="sxs-lookup"><span data-stu-id="e725d-139">description</span></span>|<span data-ttu-id="e725d-140">String</span><span class="sxs-lookup"><span data-stu-id="e725d-140">String</span></span>|<span data-ttu-id="e725d-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e725d-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e725d-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e725d-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e725d-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e725d-143">lastModifiedDateTime</span></span>|<span data-ttu-id="e725d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e725d-144">DateTimeOffset</span></span>|<span data-ttu-id="e725d-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e725d-145">DateTime the object was last modified.</span></span> <span data-ttu-id="e725d-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e725d-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e725d-147">displayName</span><span class="sxs-lookup"><span data-stu-id="e725d-147">displayName</span></span>|<span data-ttu-id="e725d-148">字符串</span><span class="sxs-lookup"><span data-stu-id="e725d-148">String</span></span>|<span data-ttu-id="e725d-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e725d-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e725d-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e725d-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e725d-151">version</span><span class="sxs-lookup"><span data-stu-id="e725d-151">version</span></span>|<span data-ttu-id="e725d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e725d-152">Int32</span></span>|<span data-ttu-id="e725d-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e725d-153">Version of the device configuration.</span></span> <span data-ttu-id="e725d-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e725d-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e725d-155">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e725d-155">passwordBlockSimple</span></span>|<span data-ttu-id="e725d-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="e725d-156">Boolean</span></span>|<span data-ttu-id="e725d-157">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="e725d-157">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="e725d-158">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e725d-158">passwordExpirationDays</span></span>|<span data-ttu-id="e725d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="e725d-159">Int32</span></span>|<span data-ttu-id="e725d-160">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="e725d-160">Number of days before the password expires.</span></span>|
|<span data-ttu-id="e725d-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e725d-161">passwordMinimumLength</span></span>|<span data-ttu-id="e725d-162">Int32</span><span class="sxs-lookup"><span data-stu-id="e725d-162">Int32</span></span>|<span data-ttu-id="e725d-163">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="e725d-163">Minimum length of passwords.</span></span>|
|<span data-ttu-id="e725d-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e725d-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e725d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e725d-165">Int32</span></span>|<span data-ttu-id="e725d-166">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="e725d-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e725d-167">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e725d-167">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e725d-168">Int32</span><span class="sxs-lookup"><span data-stu-id="e725d-168">Int32</span></span>|<span data-ttu-id="e725d-169">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="e725d-169">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e725d-170">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e725d-170">passwordRequiredType</span></span>|[<span data-ttu-id="e725d-171">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e725d-171">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e725d-172">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="e725d-172">The required password type.</span></span> <span data-ttu-id="e725d-173">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="e725d-173">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e725d-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e725d-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e725d-175">Int32</span><span class="sxs-lookup"><span data-stu-id="e725d-175">Int32</span></span>|<span data-ttu-id="e725d-176">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="e725d-176">Number of previous passwords to block.</span></span> <span data-ttu-id="e725d-177">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="e725d-177">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e725d-178">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e725d-178">passwordRequired</span></span>|<span data-ttu-id="e725d-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="e725d-179">Boolean</span></span>|<span data-ttu-id="e725d-180">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="e725d-180">Whether or not to require a password.</span></span>|
|<span data-ttu-id="e725d-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e725d-181">osMinimumVersion</span></span>|<span data-ttu-id="e725d-182">String</span><span class="sxs-lookup"><span data-stu-id="e725d-182">String</span></span>|<span data-ttu-id="e725d-183">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="e725d-183">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="e725d-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e725d-184">osMaximumVersion</span></span>|<span data-ttu-id="e725d-185">String</span><span class="sxs-lookup"><span data-stu-id="e725d-185">String</span></span>|<span data-ttu-id="e725d-186">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="e725d-186">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="e725d-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e725d-187">storageRequireEncryption</span></span>|<span data-ttu-id="e725d-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="e725d-188">Boolean</span></span>|<span data-ttu-id="e725d-189">要求对 Windows Phone 设备加密。</span><span class="sxs-lookup"><span data-stu-id="e725d-189">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="e725d-190">响应</span><span class="sxs-lookup"><span data-stu-id="e725d-190">Response</span></span>
<span data-ttu-id="e725d-191">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e725d-191">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e725d-192">示例</span><span class="sxs-lookup"><span data-stu-id="e725d-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="e725d-193">请求</span><span class="sxs-lookup"><span data-stu-id="e725d-193">Request</span></span>
<span data-ttu-id="e725d-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e725d-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e725d-195">响应</span><span class="sxs-lookup"><span data-stu-id="e725d-195">Response</span></span>
<span data-ttu-id="e725d-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e725d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



