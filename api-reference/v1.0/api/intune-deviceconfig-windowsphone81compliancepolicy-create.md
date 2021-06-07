---
title: 创建 windowsPhone81CompliancePolicy
description: 创建新的 windowsPhone81CompliancePolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 00bc01765c5b6f6fac30c45e93ce65ea3b6da974
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52747212"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="79799-103">创建 windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="79799-103">Create windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="79799-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79799-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79799-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79799-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79799-106">创建新的 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79799-106">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79799-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="79799-107">Prerequisites</span></span>
<span data-ttu-id="79799-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79799-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79799-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="79799-110">Permission type</span></span>|<span data-ttu-id="79799-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79799-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79799-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79799-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79799-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79799-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79799-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79799-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79799-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="79799-115">Not supported.</span></span>|
|<span data-ttu-id="79799-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="79799-116">Application</span></span>|<span data-ttu-id="79799-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79799-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79799-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79799-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="79799-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="79799-119">Request headers</span></span>
|<span data-ttu-id="79799-120">标头</span><span class="sxs-lookup"><span data-stu-id="79799-120">Header</span></span>|<span data-ttu-id="79799-121">值</span><span class="sxs-lookup"><span data-stu-id="79799-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79799-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79799-122">Authorization</span></span>|<span data-ttu-id="79799-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="79799-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79799-124">接受</span><span class="sxs-lookup"><span data-stu-id="79799-124">Accept</span></span>|<span data-ttu-id="79799-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79799-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79799-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="79799-126">Request body</span></span>
<span data-ttu-id="79799-127">在请求正文中，提供 windowsPhone81CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79799-127">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="79799-128">下表显示创建 windowsPhone81CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="79799-128">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="79799-129">属性</span><span class="sxs-lookup"><span data-stu-id="79799-129">Property</span></span>|<span data-ttu-id="79799-130">类型</span><span class="sxs-lookup"><span data-stu-id="79799-130">Type</span></span>|<span data-ttu-id="79799-131">说明</span><span class="sxs-lookup"><span data-stu-id="79799-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79799-132">id</span><span class="sxs-lookup"><span data-stu-id="79799-132">id</span></span>|<span data-ttu-id="79799-133">String</span><span class="sxs-lookup"><span data-stu-id="79799-133">String</span></span>|<span data-ttu-id="79799-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="79799-134">Key of the entity.</span></span> <span data-ttu-id="79799-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79799-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="79799-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79799-136">createdDateTime</span></span>|<span data-ttu-id="79799-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79799-137">DateTimeOffset</span></span>|<span data-ttu-id="79799-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="79799-138">DateTime the object was created.</span></span> <span data-ttu-id="79799-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79799-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="79799-140">说明</span><span class="sxs-lookup"><span data-stu-id="79799-140">description</span></span>|<span data-ttu-id="79799-141">String</span><span class="sxs-lookup"><span data-stu-id="79799-141">String</span></span>|<span data-ttu-id="79799-142">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="79799-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="79799-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79799-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="79799-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79799-144">lastModifiedDateTime</span></span>|<span data-ttu-id="79799-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79799-145">DateTimeOffset</span></span>|<span data-ttu-id="79799-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="79799-146">DateTime the object was last modified.</span></span> <span data-ttu-id="79799-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79799-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="79799-148">displayName</span><span class="sxs-lookup"><span data-stu-id="79799-148">displayName</span></span>|<span data-ttu-id="79799-149">String</span><span class="sxs-lookup"><span data-stu-id="79799-149">String</span></span>|<span data-ttu-id="79799-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="79799-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="79799-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79799-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="79799-152">version</span><span class="sxs-lookup"><span data-stu-id="79799-152">version</span></span>|<span data-ttu-id="79799-153">Int32</span><span class="sxs-lookup"><span data-stu-id="79799-153">Int32</span></span>|<span data-ttu-id="79799-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="79799-154">Version of the device configuration.</span></span> <span data-ttu-id="79799-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79799-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="79799-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="79799-156">passwordBlockSimple</span></span>|<span data-ttu-id="79799-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="79799-157">Boolean</span></span>|<span data-ttu-id="79799-158">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="79799-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="79799-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="79799-159">passwordExpirationDays</span></span>|<span data-ttu-id="79799-160">Int32</span><span class="sxs-lookup"><span data-stu-id="79799-160">Int32</span></span>|<span data-ttu-id="79799-161">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="79799-161">Number of days before the password expires.</span></span>|
|<span data-ttu-id="79799-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="79799-162">passwordMinimumLength</span></span>|<span data-ttu-id="79799-163">Int32</span><span class="sxs-lookup"><span data-stu-id="79799-163">Int32</span></span>|<span data-ttu-id="79799-164">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="79799-164">Minimum length of passwords.</span></span>|
|<span data-ttu-id="79799-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="79799-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="79799-166">Int32</span><span class="sxs-lookup"><span data-stu-id="79799-166">Int32</span></span>|<span data-ttu-id="79799-167">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="79799-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="79799-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="79799-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="79799-169">Int32</span><span class="sxs-lookup"><span data-stu-id="79799-169">Int32</span></span>|<span data-ttu-id="79799-170">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="79799-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="79799-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="79799-171">passwordRequiredType</span></span>|[<span data-ttu-id="79799-172">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="79799-172">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="79799-173">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="79799-173">The required password type.</span></span> <span data-ttu-id="79799-174">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="79799-174">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="79799-175">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="79799-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="79799-176">Int32</span><span class="sxs-lookup"><span data-stu-id="79799-176">Int32</span></span>|<span data-ttu-id="79799-177">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="79799-177">Number of previous passwords to block.</span></span> <span data-ttu-id="79799-178">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="79799-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="79799-179">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="79799-179">passwordRequired</span></span>|<span data-ttu-id="79799-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="79799-180">Boolean</span></span>|<span data-ttu-id="79799-181">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="79799-181">Whether or not to require a password.</span></span>|
|<span data-ttu-id="79799-182">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="79799-182">osMinimumVersion</span></span>|<span data-ttu-id="79799-183">String</span><span class="sxs-lookup"><span data-stu-id="79799-183">String</span></span>|<span data-ttu-id="79799-184">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="79799-184">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="79799-185">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="79799-185">osMaximumVersion</span></span>|<span data-ttu-id="79799-186">String</span><span class="sxs-lookup"><span data-stu-id="79799-186">String</span></span>|<span data-ttu-id="79799-187">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="79799-187">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="79799-188">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="79799-188">storageRequireEncryption</span></span>|<span data-ttu-id="79799-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="79799-189">Boolean</span></span>|<span data-ttu-id="79799-190">要求对 Windows Phone 设备加密。</span><span class="sxs-lookup"><span data-stu-id="79799-190">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="79799-191">响应</span><span class="sxs-lookup"><span data-stu-id="79799-191">Response</span></span>
<span data-ttu-id="79799-192">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79799-192">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79799-193">示例</span><span class="sxs-lookup"><span data-stu-id="79799-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="79799-194">请求</span><span class="sxs-lookup"><span data-stu-id="79799-194">Request</span></span>
<span data-ttu-id="79799-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79799-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="79799-196">响应</span><span class="sxs-lookup"><span data-stu-id="79799-196">Response</span></span>
<span data-ttu-id="79799-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="79799-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




