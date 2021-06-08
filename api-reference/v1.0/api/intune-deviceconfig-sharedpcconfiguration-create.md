---
title: 创建 sharedPCConfiguration
description: 创建新的 sharedPCConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0946f2a8d38044e6dc02bb4ae06dd83c7fa67dad
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760571"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="ce651-103">创建 sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="ce651-103">Create sharedPCConfiguration</span></span>

<span data-ttu-id="ce651-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce651-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce651-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce651-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce651-106">创建新的 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ce651-106">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce651-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ce651-107">Prerequisites</span></span>
<span data-ttu-id="ce651-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce651-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce651-110">Permission type</span></span>|<span data-ttu-id="ce651-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce651-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce651-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce651-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce651-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce651-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce651-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce651-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce651-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce651-115">Not supported.</span></span>|
|<span data-ttu-id="ce651-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce651-116">Application</span></span>|<span data-ttu-id="ce651-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce651-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce651-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce651-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ce651-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce651-119">Request headers</span></span>
|<span data-ttu-id="ce651-120">标头</span><span class="sxs-lookup"><span data-stu-id="ce651-120">Header</span></span>|<span data-ttu-id="ce651-121">值</span><span class="sxs-lookup"><span data-stu-id="ce651-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce651-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce651-122">Authorization</span></span>|<span data-ttu-id="ce651-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ce651-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce651-124">接受</span><span class="sxs-lookup"><span data-stu-id="ce651-124">Accept</span></span>|<span data-ttu-id="ce651-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce651-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce651-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce651-126">Request body</span></span>
<span data-ttu-id="ce651-127">在请求正文中，提供 sharedPCConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce651-127">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="ce651-128">下表显示创建 sharedPCConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ce651-128">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="ce651-129">属性</span><span class="sxs-lookup"><span data-stu-id="ce651-129">Property</span></span>|<span data-ttu-id="ce651-130">类型</span><span class="sxs-lookup"><span data-stu-id="ce651-130">Type</span></span>|<span data-ttu-id="ce651-131">说明</span><span class="sxs-lookup"><span data-stu-id="ce651-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce651-132">id</span><span class="sxs-lookup"><span data-stu-id="ce651-132">id</span></span>|<span data-ttu-id="ce651-133">String</span><span class="sxs-lookup"><span data-stu-id="ce651-133">String</span></span>|<span data-ttu-id="ce651-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ce651-134">Key of the entity.</span></span> <span data-ttu-id="ce651-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce651-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce651-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce651-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ce651-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce651-137">DateTimeOffset</span></span>|<span data-ttu-id="ce651-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ce651-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ce651-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce651-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce651-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce651-140">createdDateTime</span></span>|<span data-ttu-id="ce651-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce651-141">DateTimeOffset</span></span>|<span data-ttu-id="ce651-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ce651-142">DateTime the object was created.</span></span> <span data-ttu-id="ce651-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce651-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce651-144">description</span><span class="sxs-lookup"><span data-stu-id="ce651-144">description</span></span>|<span data-ttu-id="ce651-145">String</span><span class="sxs-lookup"><span data-stu-id="ce651-145">String</span></span>|<span data-ttu-id="ce651-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ce651-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ce651-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce651-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce651-148">displayName</span><span class="sxs-lookup"><span data-stu-id="ce651-148">displayName</span></span>|<span data-ttu-id="ce651-149">String</span><span class="sxs-lookup"><span data-stu-id="ce651-149">String</span></span>|<span data-ttu-id="ce651-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ce651-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ce651-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce651-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce651-152">version</span><span class="sxs-lookup"><span data-stu-id="ce651-152">version</span></span>|<span data-ttu-id="ce651-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ce651-153">Int32</span></span>|<span data-ttu-id="ce651-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ce651-154">Version of the device configuration.</span></span> <span data-ttu-id="ce651-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce651-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce651-156">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="ce651-156">accountManagerPolicy</span></span>|[<span data-ttu-id="ce651-157">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="ce651-157">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="ce651-158">指定在共享电脑上管理帐户的方式。</span><span class="sxs-lookup"><span data-stu-id="ce651-158">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="ce651-159">仅当 disableAccountManager 为 false 时适用。</span><span class="sxs-lookup"><span data-stu-id="ce651-159">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="ce651-160">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="ce651-160">allowedAccounts</span></span>|[<span data-ttu-id="ce651-161">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="ce651-161">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="ce651-162">指示允许在共享电脑上使用哪种类型的帐户。</span><span class="sxs-lookup"><span data-stu-id="ce651-162">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="ce651-163">可取值为：`guest`、`domain`。</span><span class="sxs-lookup"><span data-stu-id="ce651-163">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="ce651-164">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="ce651-164">allowLocalStorage</span></span>|<span data-ttu-id="ce651-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce651-165">Boolean</span></span>|<span data-ttu-id="ce651-166">指定在共享电脑上是否允许本地存储。</span><span class="sxs-lookup"><span data-stu-id="ce651-166">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="ce651-167">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="ce651-167">disableAccountManager</span></span>|<span data-ttu-id="ce651-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce651-168">Boolean</span></span>|<span data-ttu-id="ce651-169">禁用共享电脑模式的帐户管理器。</span><span class="sxs-lookup"><span data-stu-id="ce651-169">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="ce651-170">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="ce651-170">disableEduPolicies</span></span>|<span data-ttu-id="ce651-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce651-171">Boolean</span></span>|<span data-ttu-id="ce651-172">指定是否应禁用默认的共享电脑教育环境策略。</span><span class="sxs-lookup"><span data-stu-id="ce651-172">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="ce651-173">对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="ce651-173">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="ce651-174">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="ce651-174">disablePowerPolicies</span></span>|<span data-ttu-id="ce651-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce651-175">Boolean</span></span>|<span data-ttu-id="ce651-176">指定是否应禁用默认的共享电脑电源策略。</span><span class="sxs-lookup"><span data-stu-id="ce651-176">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="ce651-177">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="ce651-177">disableSignInOnResume</span></span>|<span data-ttu-id="ce651-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce651-178">Boolean</span></span>|<span data-ttu-id="ce651-179">禁用每当设备从睡眠模式唤醒时需要登录的要求。</span><span class="sxs-lookup"><span data-stu-id="ce651-179">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="ce651-180">enabled</span><span class="sxs-lookup"><span data-stu-id="ce651-180">enabled</span></span>|<span data-ttu-id="ce651-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce651-181">Boolean</span></span>|<span data-ttu-id="ce651-182">启用共享的电脑模式并应用共享的电脑策略。</span><span class="sxs-lookup"><span data-stu-id="ce651-182">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="ce651-183">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="ce651-183">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="ce651-184">Int32</span><span class="sxs-lookup"><span data-stu-id="ce651-184">Int32</span></span>|<span data-ttu-id="ce651-185">指定电脑进入睡眠状态之前设备必须保持空闲状态的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="ce651-185">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="ce651-186">将此值设置为 0 可防止发生睡眠超时。</span><span class="sxs-lookup"><span data-stu-id="ce651-186">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="ce651-187">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="ce651-187">kioskAppDisplayName</span></span>|<span data-ttu-id="ce651-188">String</span><span class="sxs-lookup"><span data-stu-id="ce651-188">String</span></span>|<span data-ttu-id="ce651-189">指定启动由 SetKioskAppUserModelId 指定的应用的登录屏幕上显示的帐户的显示文本。</span><span class="sxs-lookup"><span data-stu-id="ce651-189">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="ce651-190">仅在设置 KioskAppUserModelId 后适用。</span><span class="sxs-lookup"><span data-stu-id="ce651-190">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="ce651-191">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="ce651-191">kioskAppUserModelId</span></span>|<span data-ttu-id="ce651-192">String</span><span class="sxs-lookup"><span data-stu-id="ce651-192">String</span></span>|<span data-ttu-id="ce651-193">指定要与分配的访问权限结合使用的应用的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="ce651-193">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="ce651-194">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="ce651-194">maintenanceStartTime</span></span>|<span data-ttu-id="ce651-195">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ce651-195">TimeOfDay</span></span>|<span data-ttu-id="ce651-196">指定维护小时的每日开始时间。</span><span class="sxs-lookup"><span data-stu-id="ce651-196">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="ce651-197">响应</span><span class="sxs-lookup"><span data-stu-id="ce651-197">Response</span></span>
<span data-ttu-id="ce651-198">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ce651-198">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce651-199">示例</span><span class="sxs-lookup"><span data-stu-id="ce651-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce651-200">请求</span><span class="sxs-lookup"><span data-stu-id="ce651-200">Request</span></span>
<span data-ttu-id="ce651-201">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce651-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ce651-202">响应</span><span class="sxs-lookup"><span data-stu-id="ce651-202">Response</span></span>
<span data-ttu-id="ce651-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ce651-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




