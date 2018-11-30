---
title: 创建 sharedPCConfiguration
description: 创建新的 sharedPCConfiguration 对象。
ms.openlocfilehash: 3033bc44c683db6f574e794eb9a7d409b6de5ea7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011201"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="7f560-103">创建 sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f560-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="7f560-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7f560-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f560-105">创建新的 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f560-105">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f560-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="7f560-106">Prerequisites</span></span>
<span data-ttu-id="7f560-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7f560-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f560-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f560-109">Permission type</span></span>|<span data-ttu-id="7f560-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7f560-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f560-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f560-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7f560-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f560-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f560-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f560-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f560-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f560-114">Not supported.</span></span>|
|<span data-ttu-id="7f560-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f560-115">Application</span></span>|<span data-ttu-id="7f560-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f560-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f560-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f560-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7f560-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f560-118">Request headers</span></span>
|<span data-ttu-id="7f560-119">标头</span><span class="sxs-lookup"><span data-stu-id="7f560-119">Header</span></span>|<span data-ttu-id="7f560-120">值</span><span class="sxs-lookup"><span data-stu-id="7f560-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f560-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f560-121">Authorization</span></span>|<span data-ttu-id="7f560-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7f560-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f560-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7f560-123">Accept</span></span>|<span data-ttu-id="7f560-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7f560-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f560-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f560-125">Request body</span></span>
<span data-ttu-id="7f560-126">在请求正文中，提供 sharedPCConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f560-126">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="7f560-127">下表显示创建 sharedPCConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7f560-127">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="7f560-128">属性</span><span class="sxs-lookup"><span data-stu-id="7f560-128">Property</span></span>|<span data-ttu-id="7f560-129">类型</span><span class="sxs-lookup"><span data-stu-id="7f560-129">Type</span></span>|<span data-ttu-id="7f560-130">说明</span><span class="sxs-lookup"><span data-stu-id="7f560-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f560-131">id</span><span class="sxs-lookup"><span data-stu-id="7f560-131">id</span></span>|<span data-ttu-id="7f560-132">String</span><span class="sxs-lookup"><span data-stu-id="7f560-132">String</span></span>|<span data-ttu-id="7f560-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7f560-133">Key of the entity.</span></span> <span data-ttu-id="7f560-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f560-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f560-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f560-135">lastModifiedDateTime</span></span>|<span data-ttu-id="7f560-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f560-136">DateTimeOffset</span></span>|<span data-ttu-id="7f560-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7f560-137">DateTime the object was last modified.</span></span> <span data-ttu-id="7f560-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f560-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f560-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f560-139">createdDateTime</span></span>|<span data-ttu-id="7f560-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f560-140">DateTimeOffset</span></span>|<span data-ttu-id="7f560-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7f560-141">DateTime the object was created.</span></span> <span data-ttu-id="7f560-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f560-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f560-143">description</span><span class="sxs-lookup"><span data-stu-id="7f560-143">description</span></span>|<span data-ttu-id="7f560-144">String</span><span class="sxs-lookup"><span data-stu-id="7f560-144">String</span></span>|<span data-ttu-id="7f560-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7f560-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7f560-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f560-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f560-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7f560-147">displayName</span></span>|<span data-ttu-id="7f560-148">String</span><span class="sxs-lookup"><span data-stu-id="7f560-148">String</span></span>|<span data-ttu-id="7f560-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7f560-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7f560-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f560-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f560-151">version</span><span class="sxs-lookup"><span data-stu-id="7f560-151">version</span></span>|<span data-ttu-id="7f560-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7f560-152">Int32</span></span>|<span data-ttu-id="7f560-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7f560-153">Version of the device configuration.</span></span> <span data-ttu-id="7f560-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f560-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f560-155">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="7f560-155">accountManagerPolicy</span></span>|[<span data-ttu-id="7f560-156">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="7f560-156">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="7f560-157">指定在共享电脑上管理帐户的方式。</span><span class="sxs-lookup"><span data-stu-id="7f560-157">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="7f560-158">仅当 disableAccountManager 为 false 时适用。</span><span class="sxs-lookup"><span data-stu-id="7f560-158">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="7f560-159">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="7f560-159">allowedAccounts</span></span>|[<span data-ttu-id="7f560-160">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="7f560-160">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="7f560-161">指示允许在共享电脑上使用哪种类型的帐户。</span><span class="sxs-lookup"><span data-stu-id="7f560-161">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="7f560-162">可取值为：`guest`、`domain`。</span><span class="sxs-lookup"><span data-stu-id="7f560-162">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="7f560-163">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="7f560-163">allowLocalStorage</span></span>|<span data-ttu-id="7f560-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f560-164">Boolean</span></span>|<span data-ttu-id="7f560-165">指定在共享电脑上是否允许本地存储。</span><span class="sxs-lookup"><span data-stu-id="7f560-165">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="7f560-166">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="7f560-166">disableAccountManager</span></span>|<span data-ttu-id="7f560-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f560-167">Boolean</span></span>|<span data-ttu-id="7f560-168">禁用共享电脑模式的帐户管理器。</span><span class="sxs-lookup"><span data-stu-id="7f560-168">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="7f560-169">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="7f560-169">disableEduPolicies</span></span>|<span data-ttu-id="7f560-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f560-170">Boolean</span></span>|<span data-ttu-id="7f560-171">指定是否应禁用默认的共享电脑教育环境策略。</span><span class="sxs-lookup"><span data-stu-id="7f560-171">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="7f560-172">对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="7f560-172">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="7f560-173">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="7f560-173">disablePowerPolicies</span></span>|<span data-ttu-id="7f560-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f560-174">Boolean</span></span>|<span data-ttu-id="7f560-175">指定是否应禁用默认的共享电脑电源策略。</span><span class="sxs-lookup"><span data-stu-id="7f560-175">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="7f560-176">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="7f560-176">disableSignInOnResume</span></span>|<span data-ttu-id="7f560-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f560-177">Boolean</span></span>|<span data-ttu-id="7f560-178">禁用每当设备从睡眠模式唤醒时需要登录的要求。</span><span class="sxs-lookup"><span data-stu-id="7f560-178">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="7f560-179">enabled</span><span class="sxs-lookup"><span data-stu-id="7f560-179">enabled</span></span>|<span data-ttu-id="7f560-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f560-180">Boolean</span></span>|<span data-ttu-id="7f560-181">启用共享的电脑模式并应用共享的电脑策略。</span><span class="sxs-lookup"><span data-stu-id="7f560-181">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="7f560-182">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="7f560-182">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="7f560-183">Int32</span><span class="sxs-lookup"><span data-stu-id="7f560-183">Int32</span></span>|<span data-ttu-id="7f560-184">指定电脑进入睡眠状态之前设备必须保持空闲状态的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="7f560-184">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="7f560-185">将此值设置为 0 可防止发生睡眠超时。</span><span class="sxs-lookup"><span data-stu-id="7f560-185">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="7f560-186">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="7f560-186">kioskAppDisplayName</span></span>|<span data-ttu-id="7f560-187">String</span><span class="sxs-lookup"><span data-stu-id="7f560-187">String</span></span>|<span data-ttu-id="7f560-188">指定启动由 SetKioskAppUserModelId 指定的应用的登录屏幕上显示的帐户的显示文本。</span><span class="sxs-lookup"><span data-stu-id="7f560-188">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="7f560-189">仅在设置 KioskAppUserModelId 后适用。</span><span class="sxs-lookup"><span data-stu-id="7f560-189">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="7f560-190">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="7f560-190">kioskAppUserModelId</span></span>|<span data-ttu-id="7f560-191">String</span><span class="sxs-lookup"><span data-stu-id="7f560-191">String</span></span>|<span data-ttu-id="7f560-192">指定要与分配的访问权限结合使用的应用的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="7f560-192">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="7f560-193">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="7f560-193">maintenanceStartTime</span></span>|<span data-ttu-id="7f560-194">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7f560-194">TimeOfDay</span></span>|<span data-ttu-id="7f560-195">指定维护小时的每日开始时间。</span><span class="sxs-lookup"><span data-stu-id="7f560-195">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="7f560-196">响应</span><span class="sxs-lookup"><span data-stu-id="7f560-196">Response</span></span>
<span data-ttu-id="7f560-197">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f560-197">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f560-198">示例</span><span class="sxs-lookup"><span data-stu-id="7f560-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f560-199">请求</span><span class="sxs-lookup"><span data-stu-id="7f560-199">Request</span></span>
<span data-ttu-id="7f560-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f560-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 860

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="7f560-201">响应</span><span class="sxs-lookup"><span data-stu-id="7f560-201">Response</span></span>
<span data-ttu-id="7f560-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f560-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1032

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```



