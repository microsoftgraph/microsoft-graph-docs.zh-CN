---
title: 创建 windows81CompliancePolicy
description: 创建新的 windows81CompliancePolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e494c419e6a81c48f2ea46d886a2af016ab9e95f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981397"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="6ac5c-103">创建 windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6ac5c-103">Create windows81CompliancePolicy</span></span>

> <span data-ttu-id="6ac5c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ac5c-105">创建新的 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-105">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ac5c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="6ac5c-106">Prerequisites</span></span>
<span data-ttu-id="6ac5c-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6ac5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ac5c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ac5c-109">Permission type</span></span>|<span data-ttu-id="6ac5c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6ac5c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ac5c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ac5c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6ac5c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ac5c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ac5c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ac5c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ac5c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-114">Not supported.</span></span>|
|<span data-ttu-id="6ac5c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ac5c-115">Application</span></span>|<span data-ttu-id="6ac5c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ac5c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ac5c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6ac5c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ac5c-118">Request headers</span></span>
|<span data-ttu-id="6ac5c-119">标头</span><span class="sxs-lookup"><span data-stu-id="6ac5c-119">Header</span></span>|<span data-ttu-id="6ac5c-120">值</span><span class="sxs-lookup"><span data-stu-id="6ac5c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ac5c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ac5c-121">Authorization</span></span>|<span data-ttu-id="6ac5c-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ac5c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6ac5c-123">Accept</span></span>|<span data-ttu-id="6ac5c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6ac5c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ac5c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ac5c-125">Request body</span></span>
<span data-ttu-id="6ac5c-126">在请求正文中，提供 windows81CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-126">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="6ac5c-127">下表显示创建 windows81CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-127">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="6ac5c-128">属性</span><span class="sxs-lookup"><span data-stu-id="6ac5c-128">Property</span></span>|<span data-ttu-id="6ac5c-129">类型</span><span class="sxs-lookup"><span data-stu-id="6ac5c-129">Type</span></span>|<span data-ttu-id="6ac5c-130">说明</span><span class="sxs-lookup"><span data-stu-id="6ac5c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ac5c-131">id</span><span class="sxs-lookup"><span data-stu-id="6ac5c-131">id</span></span>|<span data-ttu-id="6ac5c-132">String</span><span class="sxs-lookup"><span data-stu-id="6ac5c-132">String</span></span>|<span data-ttu-id="6ac5c-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-133">Key of the entity.</span></span> <span data-ttu-id="6ac5c-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6ac5c-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6ac5c-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ac5c-135">createdDateTime</span></span>|<span data-ttu-id="6ac5c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ac5c-136">DateTimeOffset</span></span>|<span data-ttu-id="6ac5c-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-137">DateTime the object was created.</span></span> <span data-ttu-id="6ac5c-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6ac5c-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6ac5c-139">description</span><span class="sxs-lookup"><span data-stu-id="6ac5c-139">description</span></span>|<span data-ttu-id="6ac5c-140">String</span><span class="sxs-lookup"><span data-stu-id="6ac5c-140">String</span></span>|<span data-ttu-id="6ac5c-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6ac5c-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6ac5c-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6ac5c-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ac5c-143">lastModifiedDateTime</span></span>|<span data-ttu-id="6ac5c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ac5c-144">DateTimeOffset</span></span>|<span data-ttu-id="6ac5c-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-145">DateTime the object was last modified.</span></span> <span data-ttu-id="6ac5c-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6ac5c-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6ac5c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6ac5c-147">displayName</span></span>|<span data-ttu-id="6ac5c-148">String</span><span class="sxs-lookup"><span data-stu-id="6ac5c-148">String</span></span>|<span data-ttu-id="6ac5c-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6ac5c-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6ac5c-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6ac5c-151">version</span><span class="sxs-lookup"><span data-stu-id="6ac5c-151">version</span></span>|<span data-ttu-id="6ac5c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6ac5c-152">Int32</span></span>|<span data-ttu-id="6ac5c-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-153">Version of the device configuration.</span></span> <span data-ttu-id="6ac5c-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6ac5c-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6ac5c-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6ac5c-155">passwordRequired</span></span>|<span data-ttu-id="6ac5c-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ac5c-156">Boolean</span></span>|<span data-ttu-id="6ac5c-157">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="6ac5c-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6ac5c-158">passwordBlockSimple</span></span>|<span data-ttu-id="6ac5c-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ac5c-159">Boolean</span></span>|<span data-ttu-id="6ac5c-160">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="6ac5c-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6ac5c-161">passwordExpirationDays</span></span>|<span data-ttu-id="6ac5c-162">Int32</span><span class="sxs-lookup"><span data-stu-id="6ac5c-162">Int32</span></span>|<span data-ttu-id="6ac5c-163">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-163">Password expiration in days.</span></span>|
|<span data-ttu-id="6ac5c-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6ac5c-164">passwordMinimumLength</span></span>|<span data-ttu-id="6ac5c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6ac5c-165">Int32</span></span>|<span data-ttu-id="6ac5c-166">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-166">The minimum password length.</span></span>|
|<span data-ttu-id="6ac5c-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6ac5c-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6ac5c-168">Int32</span><span class="sxs-lookup"><span data-stu-id="6ac5c-168">Int32</span></span>|<span data-ttu-id="6ac5c-169">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6ac5c-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6ac5c-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6ac5c-171">Int32</span><span class="sxs-lookup"><span data-stu-id="6ac5c-171">Int32</span></span>|<span data-ttu-id="6ac5c-172">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6ac5c-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6ac5c-173">passwordRequiredType</span></span>|[<span data-ttu-id="6ac5c-174">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6ac5c-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6ac5c-175">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-175">The required password type.</span></span> <span data-ttu-id="6ac5c-176">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6ac5c-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6ac5c-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6ac5c-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6ac5c-178">Int32</span></span>|<span data-ttu-id="6ac5c-179">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-179">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="6ac5c-180">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="6ac5c-180">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6ac5c-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6ac5c-181">osMinimumVersion</span></span>|<span data-ttu-id="6ac5c-182">String</span><span class="sxs-lookup"><span data-stu-id="6ac5c-182">String</span></span>|<span data-ttu-id="6ac5c-183">最低 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-183">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="6ac5c-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6ac5c-184">osMaximumVersion</span></span>|<span data-ttu-id="6ac5c-185">String</span><span class="sxs-lookup"><span data-stu-id="6ac5c-185">String</span></span>|<span data-ttu-id="6ac5c-186">最高 Windows 8.1 版本。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-186">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="6ac5c-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6ac5c-187">storageRequireEncryption</span></span>|<span data-ttu-id="6ac5c-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ac5c-188">Boolean</span></span>|<span data-ttu-id="6ac5c-189">指示是否要求对 Windows 8.1 设备加密。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-189">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="6ac5c-190">响应</span><span class="sxs-lookup"><span data-stu-id="6ac5c-190">Response</span></span>
<span data-ttu-id="6ac5c-191">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-191">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ac5c-192">示例</span><span class="sxs-lookup"><span data-stu-id="6ac5c-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ac5c-193">请求</span><span class="sxs-lookup"><span data-stu-id="6ac5c-193">Request</span></span>
<span data-ttu-id="6ac5c-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6ac5c-195">响应</span><span class="sxs-lookup"><span data-stu-id="6ac5c-195">Response</span></span>
<span data-ttu-id="6ac5c-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6ac5c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



