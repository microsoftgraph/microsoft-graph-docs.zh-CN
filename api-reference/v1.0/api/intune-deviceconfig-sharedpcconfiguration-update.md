---
title: 更新 sharedPCConfiguration
description: 更新 sharedPCConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2163ae07a30d1a5c3dca616956fedce76ea6e96c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558228"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="cb920-103">更新 sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb920-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="cb920-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cb920-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb920-105">更新 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cb920-105">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb920-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="cb920-106">Prerequisites</span></span>
<span data-ttu-id="cb920-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb920-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb920-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb920-109">Permission type</span></span>|<span data-ttu-id="cb920-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cb920-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb920-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb920-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cb920-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb920-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cb920-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb920-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb920-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb920-114">Not supported.</span></span>|
|<span data-ttu-id="cb920-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb920-115">Application</span></span>|<span data-ttu-id="cb920-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb920-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb920-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb920-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cb920-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb920-118">Request headers</span></span>
|<span data-ttu-id="cb920-119">标头</span><span class="sxs-lookup"><span data-stu-id="cb920-119">Header</span></span>|<span data-ttu-id="cb920-120">值</span><span class="sxs-lookup"><span data-stu-id="cb920-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb920-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb920-121">Authorization</span></span>|<span data-ttu-id="cb920-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cb920-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb920-123">接受</span><span class="sxs-lookup"><span data-stu-id="cb920-123">Accept</span></span>|<span data-ttu-id="cb920-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cb920-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb920-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb920-125">Request body</span></span>
<span data-ttu-id="cb920-126">在请求正文中，提供 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb920-126">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="cb920-127">下表显示创建 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cb920-127">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="cb920-128">属性</span><span class="sxs-lookup"><span data-stu-id="cb920-128">Property</span></span>|<span data-ttu-id="cb920-129">类型</span><span class="sxs-lookup"><span data-stu-id="cb920-129">Type</span></span>|<span data-ttu-id="cb920-130">说明</span><span class="sxs-lookup"><span data-stu-id="cb920-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb920-131">id</span><span class="sxs-lookup"><span data-stu-id="cb920-131">id</span></span>|<span data-ttu-id="cb920-132">字符串</span><span class="sxs-lookup"><span data-stu-id="cb920-132">String</span></span>|<span data-ttu-id="cb920-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cb920-133">Key of the entity.</span></span> <span data-ttu-id="cb920-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb920-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb920-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb920-135">lastModifiedDateTime</span></span>|<span data-ttu-id="cb920-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb920-136">DateTimeOffset</span></span>|<span data-ttu-id="cb920-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cb920-137">DateTime the object was last modified.</span></span> <span data-ttu-id="cb920-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb920-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb920-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb920-139">createdDateTime</span></span>|<span data-ttu-id="cb920-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb920-140">DateTimeOffset</span></span>|<span data-ttu-id="cb920-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cb920-141">DateTime the object was created.</span></span> <span data-ttu-id="cb920-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb920-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb920-143">description</span><span class="sxs-lookup"><span data-stu-id="cb920-143">description</span></span>|<span data-ttu-id="cb920-144">String</span><span class="sxs-lookup"><span data-stu-id="cb920-144">String</span></span>|<span data-ttu-id="cb920-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="cb920-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cb920-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb920-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb920-147">displayName</span><span class="sxs-lookup"><span data-stu-id="cb920-147">displayName</span></span>|<span data-ttu-id="cb920-148">字符串</span><span class="sxs-lookup"><span data-stu-id="cb920-148">String</span></span>|<span data-ttu-id="cb920-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="cb920-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cb920-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb920-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb920-151">version</span><span class="sxs-lookup"><span data-stu-id="cb920-151">version</span></span>|<span data-ttu-id="cb920-152">Int32</span><span class="sxs-lookup"><span data-stu-id="cb920-152">Int32</span></span>|<span data-ttu-id="cb920-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="cb920-153">Version of the device configuration.</span></span> <span data-ttu-id="cb920-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb920-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb920-155">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="cb920-155">accountManagerPolicy</span></span>|[<span data-ttu-id="cb920-156">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="cb920-156">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="cb920-157">指定在共享电脑上管理帐户的方式。</span><span class="sxs-lookup"><span data-stu-id="cb920-157">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="cb920-158">仅当 disableAccountManager 为 false 时适用。</span><span class="sxs-lookup"><span data-stu-id="cb920-158">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="cb920-159">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="cb920-159">allowedAccounts</span></span>|[<span data-ttu-id="cb920-160">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="cb920-160">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="cb920-161">指示允许在共享电脑上使用哪种类型的帐户。</span><span class="sxs-lookup"><span data-stu-id="cb920-161">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="cb920-162">可取值为：`guest`、`domain`。</span><span class="sxs-lookup"><span data-stu-id="cb920-162">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="cb920-163">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="cb920-163">allowLocalStorage</span></span>|<span data-ttu-id="cb920-164">布尔值</span><span class="sxs-lookup"><span data-stu-id="cb920-164">Boolean</span></span>|<span data-ttu-id="cb920-165">指定在共享电脑上是否允许本地存储。</span><span class="sxs-lookup"><span data-stu-id="cb920-165">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="cb920-166">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="cb920-166">disableAccountManager</span></span>|<span data-ttu-id="cb920-167">布尔值</span><span class="sxs-lookup"><span data-stu-id="cb920-167">Boolean</span></span>|<span data-ttu-id="cb920-168">禁用共享电脑模式的帐户管理器。</span><span class="sxs-lookup"><span data-stu-id="cb920-168">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="cb920-169">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="cb920-169">disableEduPolicies</span></span>|<span data-ttu-id="cb920-170">布尔值</span><span class="sxs-lookup"><span data-stu-id="cb920-170">Boolean</span></span>|<span data-ttu-id="cb920-171">指定是否应禁用默认的共享电脑教育环境策略。</span><span class="sxs-lookup"><span data-stu-id="cb920-171">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="cb920-172">对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="cb920-172">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="cb920-173">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="cb920-173">disablePowerPolicies</span></span>|<span data-ttu-id="cb920-174">布尔值</span><span class="sxs-lookup"><span data-stu-id="cb920-174">Boolean</span></span>|<span data-ttu-id="cb920-175">指定是否应禁用默认的共享电脑电源策略。</span><span class="sxs-lookup"><span data-stu-id="cb920-175">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="cb920-176">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="cb920-176">disableSignInOnResume</span></span>|<span data-ttu-id="cb920-177">布尔值</span><span class="sxs-lookup"><span data-stu-id="cb920-177">Boolean</span></span>|<span data-ttu-id="cb920-178">禁用每当设备从睡眠模式唤醒时需要登录的要求。</span><span class="sxs-lookup"><span data-stu-id="cb920-178">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="cb920-179">enabled</span><span class="sxs-lookup"><span data-stu-id="cb920-179">enabled</span></span>|<span data-ttu-id="cb920-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb920-180">Boolean</span></span>|<span data-ttu-id="cb920-181">启用共享的电脑模式并应用共享的电脑策略。</span><span class="sxs-lookup"><span data-stu-id="cb920-181">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="cb920-182">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="cb920-182">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="cb920-183">Int32</span><span class="sxs-lookup"><span data-stu-id="cb920-183">Int32</span></span>|<span data-ttu-id="cb920-184">指定电脑进入睡眠状态之前设备必须保持空闲状态的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="cb920-184">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="cb920-185">将此值设置为 0 可防止发生睡眠超时。</span><span class="sxs-lookup"><span data-stu-id="cb920-185">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="cb920-186">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="cb920-186">kioskAppDisplayName</span></span>|<span data-ttu-id="cb920-187">String</span><span class="sxs-lookup"><span data-stu-id="cb920-187">String</span></span>|<span data-ttu-id="cb920-188">指定启动由 SetKioskAppUserModelId 指定的应用的登录屏幕上显示的帐户的显示文本。</span><span class="sxs-lookup"><span data-stu-id="cb920-188">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="cb920-189">仅在设置 KioskAppUserModelId 后适用。</span><span class="sxs-lookup"><span data-stu-id="cb920-189">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="cb920-190">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="cb920-190">kioskAppUserModelId</span></span>|<span data-ttu-id="cb920-191">String</span><span class="sxs-lookup"><span data-stu-id="cb920-191">String</span></span>|<span data-ttu-id="cb920-192">指定要与分配的访问权限结合使用的应用的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="cb920-192">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="cb920-193">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="cb920-193">maintenanceStartTime</span></span>|<span data-ttu-id="cb920-194">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="cb920-194">TimeOfDay</span></span>|<span data-ttu-id="cb920-195">指定维护小时的每日开始时间。</span><span class="sxs-lookup"><span data-stu-id="cb920-195">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="cb920-196">响应</span><span class="sxs-lookup"><span data-stu-id="cb920-196">Response</span></span>
<span data-ttu-id="cb920-197">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb920-197">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb920-198">示例</span><span class="sxs-lookup"><span data-stu-id="cb920-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb920-199">请求</span><span class="sxs-lookup"><span data-stu-id="cb920-199">Request</span></span>
<span data-ttu-id="cb920-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cb920-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="cb920-201">响应</span><span class="sxs-lookup"><span data-stu-id="cb920-201">Response</span></span>
<span data-ttu-id="cb920-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cb920-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



