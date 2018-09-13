# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="6672a-101">更新 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6672a-101">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="6672a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6672a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6672a-103">更新 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6672a-103">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6672a-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="6672a-104">Prerequisites</span></span>
<span data-ttu-id="6672a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6672a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6672a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6672a-107">Permission type</span></span>|<span data-ttu-id="6672a-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6672a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6672a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6672a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6672a-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6672a-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6672a-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6672a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6672a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6672a-112">Not supported.</span></span>|
|<span data-ttu-id="6672a-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="6672a-113">Application</span></span>|<span data-ttu-id="6672a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6672a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6672a-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6672a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6672a-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="6672a-116">Request headers</span></span>
|<span data-ttu-id="6672a-117">标头</span><span class="sxs-lookup"><span data-stu-id="6672a-117">Header</span></span>|<span data-ttu-id="6672a-118">值</span><span class="sxs-lookup"><span data-stu-id="6672a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6672a-119">授权</span><span class="sxs-lookup"><span data-stu-id="6672a-119">Authorization</span></span>|<span data-ttu-id="6672a-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6672a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6672a-121">接受</span><span class="sxs-lookup"><span data-stu-id="6672a-121">Accept</span></span>|<span data-ttu-id="6672a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6672a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6672a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6672a-123">Request body</span></span>
<span data-ttu-id="6672a-124">在请求正文中，提供 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6672a-124">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="6672a-125">下表显示创建 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6672a-125">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="6672a-126">属性</span><span class="sxs-lookup"><span data-stu-id="6672a-126">Property</span></span>|<span data-ttu-id="6672a-127">类型</span><span class="sxs-lookup"><span data-stu-id="6672a-127">Type</span></span>|<span data-ttu-id="6672a-128">说明</span><span class="sxs-lookup"><span data-stu-id="6672a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6672a-129">ID</span><span class="sxs-lookup"><span data-stu-id="6672a-129">id</span></span>|<span data-ttu-id="6672a-130">字符串</span><span class="sxs-lookup"><span data-stu-id="6672a-130">String</span></span>|<span data-ttu-id="6672a-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6672a-131">Key of the entity.</span></span> <span data-ttu-id="6672a-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6672a-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6672a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6672a-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6672a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6672a-134">DateTimeOffset</span></span>|<span data-ttu-id="6672a-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6672a-135">DateTime the object was last modified.</span></span> <span data-ttu-id="6672a-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6672a-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6672a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6672a-137">createdDateTime</span></span>|<span data-ttu-id="6672a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6672a-138">DateTimeOffset</span></span>|<span data-ttu-id="6672a-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6672a-139">DateTime the object was created.</span></span> <span data-ttu-id="6672a-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6672a-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6672a-141">说明</span><span class="sxs-lookup"><span data-stu-id="6672a-141">description</span></span>|<span data-ttu-id="6672a-142">字符串</span><span class="sxs-lookup"><span data-stu-id="6672a-142">String</span></span>|<span data-ttu-id="6672a-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6672a-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6672a-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6672a-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6672a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6672a-145">displayName</span></span>|<span data-ttu-id="6672a-146">字符串</span><span class="sxs-lookup"><span data-stu-id="6672a-146">String</span></span>|<span data-ttu-id="6672a-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6672a-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6672a-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6672a-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6672a-149">version</span><span class="sxs-lookup"><span data-stu-id="6672a-149">version</span></span>|<span data-ttu-id="6672a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-150">Int32</span></span>|<span data-ttu-id="6672a-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6672a-151">Version of the device configuration.</span></span> <span data-ttu-id="6672a-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6672a-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6672a-153">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6672a-153">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="6672a-154">布尔</span><span class="sxs-lookup"><span data-stu-id="6672a-154">Boolean</span></span>|<span data-ttu-id="6672a-155">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="6672a-155">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="6672a-156">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="6672a-156">passwordBlockTrustAgents</span></span>|<span data-ttu-id="6672a-157">布尔</span><span class="sxs-lookup"><span data-stu-id="6672a-157">Boolean</span></span>|<span data-ttu-id="6672a-158">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="6672a-158">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="6672a-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6672a-159">passwordExpirationDays</span></span>|<span data-ttu-id="6672a-160">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-160">Int32</span></span>|<span data-ttu-id="6672a-161">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="6672a-161">Number of days before the password expires.</span></span> <span data-ttu-id="6672a-162">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="6672a-162">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6672a-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6672a-163">passwordMinimumLength</span></span>|<span data-ttu-id="6672a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-164">Int32</span></span>|<span data-ttu-id="6672a-165">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="6672a-165">Minimum length of passwords.</span></span> <span data-ttu-id="6672a-166">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="6672a-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6672a-167">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6672a-167">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6672a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-168">Int32</span></span>|<span data-ttu-id="6672a-169">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="6672a-169">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6672a-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6672a-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6672a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-171">Int32</span></span>|<span data-ttu-id="6672a-172">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="6672a-172">Number of previous passwords to block.</span></span> <span data-ttu-id="6672a-173">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="6672a-173">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6672a-174">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="6672a-174">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="6672a-175">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-175">Int32</span></span>|<span data-ttu-id="6672a-176">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="6672a-176">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="6672a-177">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="6672a-177">Valid values 4 to 11</span></span>|
|<span data-ttu-id="6672a-178">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6672a-178">passwordRequiredType</span></span>|[<span data-ttu-id="6672a-179">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6672a-179">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="6672a-180">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="6672a-180">Type of password that is required.</span></span> <span data-ttu-id="6672a-181">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="6672a-181">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="6672a-182">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="6672a-182">workProfileDataSharingType</span></span>|[<span data-ttu-id="6672a-183">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="6672a-183">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune_deviceconfig_androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="6672a-184">允许共享的数据的类型。</span><span class="sxs-lookup"><span data-stu-id="6672a-184">Type of data sharing that is allowed.</span></span> <span data-ttu-id="6672a-185">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="6672a-185">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="6672a-186">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="6672a-186">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="6672a-187">布尔值</span><span class="sxs-lookup"><span data-stu-id="6672a-187">Boolean</span></span>|<span data-ttu-id="6672a-188">指示在设备锁定时是否阻止通知。</span><span class="sxs-lookup"><span data-stu-id="6672a-188">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="6672a-189">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="6672a-189">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="6672a-190">布尔值</span><span class="sxs-lookup"><span data-stu-id="6672a-190">Boolean</span></span>|<span data-ttu-id="6672a-191">阻止用户在工作配置文件中添加/删除帐户。</span><span class="sxs-lookup"><span data-stu-id="6672a-191">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="6672a-192">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="6672a-192">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="6672a-193">布尔值</span><span class="sxs-lookup"><span data-stu-id="6672a-193">Boolean</span></span>|<span data-ttu-id="6672a-194">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="6672a-194">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="6672a-195">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="6672a-195">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="6672a-196">布尔值</span><span class="sxs-lookup"><span data-stu-id="6672a-196">Boolean</span></span>|<span data-ttu-id="6672a-197">阻止工作配置文件中的屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="6672a-197">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="6672a-198">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="6672a-198">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="6672a-199">布尔值</span><span class="sxs-lookup"><span data-stu-id="6672a-199">Boolean</span></span>|<span data-ttu-id="6672a-200">阻止在个人资料中显示工作配置文件来电显示。</span><span class="sxs-lookup"><span data-stu-id="6672a-200">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="6672a-201">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="6672a-201">workProfileBlockCamera</span></span>|<span data-ttu-id="6672a-202">布尔值</span><span class="sxs-lookup"><span data-stu-id="6672a-202">Boolean</span></span>|<span data-ttu-id="6672a-203">阻止工作配置文件摄像头。</span><span class="sxs-lookup"><span data-stu-id="6672a-203">Block work profile camera.</span></span>|
|<span data-ttu-id="6672a-204">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="6672a-204">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="6672a-205">布尔值</span><span class="sxs-lookup"><span data-stu-id="6672a-205">Boolean</span></span>|<span data-ttu-id="6672a-206">阻止工作配置文件联系人在个人资料中的可用性。</span><span class="sxs-lookup"><span data-stu-id="6672a-206">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="6672a-207">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="6672a-207">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="6672a-208">布尔值</span><span class="sxs-lookup"><span data-stu-id="6672a-208">Boolean</span></span>|<span data-ttu-id="6672a-209">布尔值，指示是否启用了禁止交叉配置文件复制/粘贴的设置。</span><span class="sxs-lookup"><span data-stu-id="6672a-209">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="6672a-210">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="6672a-210">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="6672a-211">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="6672a-211">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune_deviceconfig_androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="6672a-212">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="6672a-212">Type of password that is required.</span></span> <span data-ttu-id="6672a-213">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="6672a-213">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="6672a-214">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6672a-214">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="6672a-215">布尔值</span><span class="sxs-lookup"><span data-stu-id="6672a-215">Boolean</span></span>|<span data-ttu-id="6672a-216">指示是否阻止工作配置文件的指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="6672a-216">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="6672a-217">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="6672a-217">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="6672a-218">布尔值</span><span class="sxs-lookup"><span data-stu-id="6672a-218">Boolean</span></span>|<span data-ttu-id="6672a-219">指示是否阻止工作配置文件的 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="6672a-219">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="6672a-220">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6672a-220">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="6672a-221">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-221">Int32</span></span>|<span data-ttu-id="6672a-222">工作配置文件密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="6672a-222">Number of days before the password expires.</span></span> <span data-ttu-id="6672a-223">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="6672a-223">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6672a-224">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6672a-224">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="6672a-225">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-225">Int32</span></span>|<span data-ttu-id="6672a-226">工作配置文件密码最小长度。</span><span class="sxs-lookup"><span data-stu-id="6672a-226">Minimum length of work profile password.</span></span> <span data-ttu-id="6672a-227">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="6672a-227">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6672a-228">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="6672a-228">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="6672a-229">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-229">Int32</span></span>|<span data-ttu-id="6672a-230">工作配置文件密码中所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="6672a-230">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="6672a-231">有效值为 1 至 10</span><span class="sxs-lookup"><span data-stu-id="6672a-231">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6672a-232">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6672a-232">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="6672a-233">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-233">Int32</span></span>|<span data-ttu-id="6672a-234">工作配置文件密码必须包含的最小非字母数。</span><span class="sxs-lookup"><span data-stu-id="6672a-234">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="6672a-235">有效值为 1 至 10</span><span class="sxs-lookup"><span data-stu-id="6672a-235">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6672a-236">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6672a-236">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="6672a-237">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-237">Int32</span></span>|<span data-ttu-id="6672a-238">工作配置文件密码必须包含的最小字母数。</span><span class="sxs-lookup"><span data-stu-id="6672a-238">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="6672a-239">有效值为 1 至 10</span><span class="sxs-lookup"><span data-stu-id="6672a-239">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6672a-240">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6672a-240">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="6672a-241">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-241">Int32</span></span>|<span data-ttu-id="6672a-242">工作配置文件密码中必须包含的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="6672a-242">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="6672a-243">有效值为 1 至 10</span><span class="sxs-lookup"><span data-stu-id="6672a-243">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6672a-244">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6672a-244">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="6672a-245">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-245">Int32</span></span>|<span data-ttu-id="6672a-246">工作配置文件密码中必须包含的最小大写字符数。</span><span class="sxs-lookup"><span data-stu-id="6672a-246">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="6672a-247">有效值为 1 至 10</span><span class="sxs-lookup"><span data-stu-id="6672a-247">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6672a-248">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="6672a-248">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="6672a-249">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-249">Int32</span></span>|<span data-ttu-id="6672a-250">工作配置文件密码中必须包含的最小符号数。</span><span class="sxs-lookup"><span data-stu-id="6672a-250">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="6672a-251">有效值为 1 至 10</span><span class="sxs-lookup"><span data-stu-id="6672a-251">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6672a-252">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6672a-252">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6672a-253">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-253">Int32</span></span>|<span data-ttu-id="6672a-254">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="6672a-254">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6672a-255">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6672a-255">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6672a-256">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-256">Int32</span></span>|<span data-ttu-id="6672a-257">要阻止的以前工作配置文件密码的数量。</span><span class="sxs-lookup"><span data-stu-id="6672a-257">Number of previous passwords to block.</span></span> <span data-ttu-id="6672a-258">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="6672a-258">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6672a-259">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="6672a-259">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="6672a-260">Int32</span><span class="sxs-lookup"><span data-stu-id="6672a-260">Int32</span></span>|<span data-ttu-id="6672a-261">删除工作配置文件并删除所有公司数据之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="6672a-261">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="6672a-262">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="6672a-262">Valid values 4 to 11</span></span>|
|<span data-ttu-id="6672a-263">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6672a-263">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="6672a-264">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6672a-264">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="6672a-265">所需的工作配置文件密码的类型。</span><span class="sxs-lookup"><span data-stu-id="6672a-265">Type of password that is required.</span></span> <span data-ttu-id="6672a-266">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="6672a-266">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="6672a-267">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="6672a-267">workProfileRequirePassword</span></span>|<span data-ttu-id="6672a-268">布尔值</span><span class="sxs-lookup"><span data-stu-id="6672a-268">Boolean</span></span>|<span data-ttu-id="6672a-269">工作配置文件是否需要密码</span><span class="sxs-lookup"><span data-stu-id="6672a-269">Password is required or not for work profile</span></span>|
|<span data-ttu-id="6672a-270">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="6672a-270">securityRequireVerifyApps</span></span>|<span data-ttu-id="6672a-271">布尔</span><span class="sxs-lookup"><span data-stu-id="6672a-271">Boolean</span></span>|<span data-ttu-id="6672a-272">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="6672a-272">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="6672a-273">响应</span><span class="sxs-lookup"><span data-stu-id="6672a-273">Response</span></span>
<span data-ttu-id="6672a-274">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6672a-274">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6672a-275">示例</span><span class="sxs-lookup"><span data-stu-id="6672a-275">Example</span></span>
### <a name="request"></a><span data-ttu-id="6672a-276">请求</span><span class="sxs-lookup"><span data-stu-id="6672a-276">Request</span></span>
<span data-ttu-id="6672a-277">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6672a-277">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1812

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="6672a-278">响应</span><span class="sxs-lookup"><span data-stu-id="6672a-278">Response</span></span>
<span data-ttu-id="6672a-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6672a-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```








