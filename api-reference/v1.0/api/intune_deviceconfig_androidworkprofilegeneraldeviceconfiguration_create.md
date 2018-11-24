# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="1e2d6-101">创建 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e2d6-101">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="1e2d6-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e2d6-103">创建新的[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-103">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e2d6-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="1e2d6-104">Prerequisites</span></span>
<span data-ttu-id="1e2d6-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。
</span><span class="sxs-lookup"><span data-stu-id="1e2d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1e2d6-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e2d6-107">Permission type</span></span>|<span data-ttu-id="1e2d6-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1e2d6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e2d6-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e2d6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1e2d6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e2d6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e2d6-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e2d6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e2d6-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-112">Not supported.</span></span>|
|<span data-ttu-id="1e2d6-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e2d6-113">Application</span></span>|<span data-ttu-id="1e2d6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e2d6-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e2d6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1e2d6-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e2d6-116">Request headers</span></span>
|<span data-ttu-id="1e2d6-117">标头</span><span class="sxs-lookup"><span data-stu-id="1e2d6-117">Header</span></span>|<span data-ttu-id="1e2d6-118">值</span><span class="sxs-lookup"><span data-stu-id="1e2d6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e2d6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e2d6-119">Authorization</span></span>|<span data-ttu-id="1e2d6-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e2d6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1e2d6-121">Accept</span></span>|<span data-ttu-id="1e2d6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1e2d6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e2d6-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e2d6-123">Request body</span></span>
<span data-ttu-id="1e2d6-124">在请求正文中，提供 androidWorkProfileGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-124">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="1e2d6-125">下表显示时创建 androidWorkProfileGeneralDeviceConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-125">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="1e2d6-126">属性</span><span class="sxs-lookup"><span data-stu-id="1e2d6-126">Property</span></span>|<span data-ttu-id="1e2d6-127">类型</span><span class="sxs-lookup"><span data-stu-id="1e2d6-127">Type</span></span>|<span data-ttu-id="1e2d6-128">说明</span><span class="sxs-lookup"><span data-stu-id="1e2d6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e2d6-129">id</span><span class="sxs-lookup"><span data-stu-id="1e2d6-129">id</span></span>|<span data-ttu-id="1e2d6-130">String</span><span class="sxs-lookup"><span data-stu-id="1e2d6-130">String</span></span>|<span data-ttu-id="1e2d6-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-131">Key of the entity.</span></span> <span data-ttu-id="1e2d6-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e2d6-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e2d6-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e2d6-133">lastModifiedDateTime</span></span>|<span data-ttu-id="1e2d6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e2d6-134">DateTimeOffset</span></span>|<span data-ttu-id="1e2d6-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-135">DateTime the object was last modified.</span></span> <span data-ttu-id="1e2d6-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e2d6-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e2d6-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e2d6-137">createdDateTime</span></span>|<span data-ttu-id="1e2d6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e2d6-138">DateTimeOffset</span></span>|<span data-ttu-id="1e2d6-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-139">DateTime the object was created.</span></span> <span data-ttu-id="1e2d6-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e2d6-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e2d6-141">description</span><span class="sxs-lookup"><span data-stu-id="1e2d6-141">description</span></span>|<span data-ttu-id="1e2d6-142">String</span><span class="sxs-lookup"><span data-stu-id="1e2d6-142">String</span></span>|<span data-ttu-id="1e2d6-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1e2d6-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e2d6-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e2d6-145">displayName</span><span class="sxs-lookup"><span data-stu-id="1e2d6-145">displayName</span></span>|<span data-ttu-id="1e2d6-146">String</span><span class="sxs-lookup"><span data-stu-id="1e2d6-146">String</span></span>|<span data-ttu-id="1e2d6-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1e2d6-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e2d6-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e2d6-149">version</span><span class="sxs-lookup"><span data-stu-id="1e2d6-149">version</span></span>|<span data-ttu-id="1e2d6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-150">Int32</span></span>|<span data-ttu-id="1e2d6-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-151">Version of the device configuration.</span></span> <span data-ttu-id="1e2d6-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e2d6-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e2d6-153">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="1e2d6-153">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="1e2d6-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e2d6-154">Boolean</span></span>|<span data-ttu-id="1e2d6-155">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-155">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="1e2d6-156">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="1e2d6-156">passwordBlockTrustAgents</span></span>|<span data-ttu-id="1e2d6-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e2d6-157">Boolean</span></span>|<span data-ttu-id="1e2d6-158">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-158">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="1e2d6-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1e2d6-159">passwordExpirationDays</span></span>|<span data-ttu-id="1e2d6-160">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-160">Int32</span></span>|<span data-ttu-id="1e2d6-161">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-161">Number of days before the password expires.</span></span> <span data-ttu-id="1e2d6-162">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-162">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1e2d6-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1e2d6-163">passwordMinimumLength</span></span>|<span data-ttu-id="1e2d6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-164">Int32</span></span>|<span data-ttu-id="1e2d6-165">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-165">Minimum length of passwords.</span></span> <span data-ttu-id="1e2d6-166">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="1e2d6-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1e2d6-167">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1e2d6-167">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1e2d6-168">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-168">Int32</span></span>|<span data-ttu-id="1e2d6-169">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-169">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="1e2d6-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1e2d6-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1e2d6-171">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-171">Int32</span></span>|<span data-ttu-id="1e2d6-172">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-172">Number of previous passwords to block.</span></span> <span data-ttu-id="1e2d6-173">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="1e2d6-173">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1e2d6-174">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1e2d6-174">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1e2d6-175">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-175">Int32</span></span>|<span data-ttu-id="1e2d6-176">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-176">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="1e2d6-177">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="1e2d6-177">Valid values 4 to 11</span></span>|
|<span data-ttu-id="1e2d6-178">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1e2d6-178">passwordRequiredType</span></span>|[<span data-ttu-id="1e2d6-179">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1e2d6-179">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="1e2d6-180">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-180">Type of password that is required.</span></span> <span data-ttu-id="1e2d6-181">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-181">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="1e2d6-182">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="1e2d6-182">workProfileDataSharingType</span></span>|[<span data-ttu-id="1e2d6-183">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="1e2d6-183">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune_deviceconfig_androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="1e2d6-184">允许共享的数据的类型。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-184">Type of data sharing that is allowed.</span></span> <span data-ttu-id="1e2d6-185">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-185">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="1e2d6-186">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="1e2d6-186">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="1e2d6-187">布尔</span><span class="sxs-lookup"><span data-stu-id="1e2d6-187">Boolean</span></span>|<span data-ttu-id="1e2d6-188">指示阻止通知时设备锁定。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-188">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="1e2d6-189">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="1e2d6-189">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="1e2d6-190">布尔</span><span class="sxs-lookup"><span data-stu-id="1e2d6-190">Boolean</span></span>|<span data-ttu-id="1e2d6-191">阻止用户添加/移除工作配置文件中的帐户。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-191">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="1e2d6-192">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="1e2d6-192">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="1e2d6-193">布尔</span><span class="sxs-lookup"><span data-stu-id="1e2d6-193">Boolean</span></span>|<span data-ttu-id="1e2d6-194">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-194">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="1e2d6-195">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="1e2d6-195">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="1e2d6-196">布尔</span><span class="sxs-lookup"><span data-stu-id="1e2d6-196">Boolean</span></span>|<span data-ttu-id="1e2d6-197">阻止工作配置文件中的屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-197">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="1e2d6-198">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="1e2d6-198">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="1e2d6-199">布尔</span><span class="sxs-lookup"><span data-stu-id="1e2d6-199">Boolean</span></span>|<span data-ttu-id="1e2d6-200">阻止显示工作 profile 呼叫者 ID 个人配置文件中。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-200">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="1e2d6-201">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="1e2d6-201">workProfileBlockCamera</span></span>|<span data-ttu-id="1e2d6-202">布尔</span><span class="sxs-lookup"><span data-stu-id="1e2d6-202">Boolean</span></span>|<span data-ttu-id="1e2d6-203">阻止工作 profile 摄像头。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-203">Block work profile camera.</span></span>|
|<span data-ttu-id="1e2d6-204">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="1e2d6-204">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="1e2d6-205">布尔</span><span class="sxs-lookup"><span data-stu-id="1e2d6-205">Boolean</span></span>|<span data-ttu-id="1e2d6-206">个人配置文件中，阻止工作 profile 联系人可用性。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-206">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="1e2d6-207">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="1e2d6-207">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="1e2d6-208">布尔</span><span class="sxs-lookup"><span data-stu-id="1e2d6-208">Boolean</span></span>|<span data-ttu-id="1e2d6-209">布尔值，指示设置不允许跨是否启用配置文件复制/粘贴。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-209">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="1e2d6-210">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="1e2d6-210">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="1e2d6-211">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="1e2d6-211">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune_deviceconfig_androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="1e2d6-212">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-212">Type of password that is required.</span></span> <span data-ttu-id="1e2d6-213">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-213">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="1e2d6-214">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="1e2d6-214">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="1e2d6-215">布尔</span><span class="sxs-lookup"><span data-stu-id="1e2d6-215">Boolean</span></span>|<span data-ttu-id="1e2d6-216">指示是否阻止指纹解锁工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-216">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="1e2d6-217">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="1e2d6-217">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="1e2d6-218">布尔</span><span class="sxs-lookup"><span data-stu-id="1e2d6-218">Boolean</span></span>|<span data-ttu-id="1e2d6-219">指示阻止智能锁定和其他信任代理工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-219">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="1e2d6-220">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1e2d6-220">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="1e2d6-221">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-221">Int32</span></span>|<span data-ttu-id="1e2d6-222">过期工作配置文件密码之前的天数。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-222">Number of days before the work profile password expires.</span></span> <span data-ttu-id="1e2d6-223">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-223">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1e2d6-224">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1e2d6-224">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="1e2d6-225">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-225">Int32</span></span>|<span data-ttu-id="1e2d6-226">工作配置文件密码最小长度。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-226">Minimum length of work profile password.</span></span> <span data-ttu-id="1e2d6-227">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="1e2d6-227">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1e2d6-228">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="1e2d6-228">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="1e2d6-229">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-229">Int32</span></span>|<span data-ttu-id="1e2d6-230">最小 ハ  工作配置文件密码中所需的数字字符。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-230">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="1e2d6-231">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="1e2d6-231">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1e2d6-232">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="1e2d6-232">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="1e2d6-233">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-233">Int32</span></span>|<span data-ttu-id="1e2d6-234">最小 ハ  中工作配置文件密码必须包含非字母字符。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-234">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="1e2d6-235">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="1e2d6-235">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1e2d6-236">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="1e2d6-236">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="1e2d6-237">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-237">Int32</span></span>|<span data-ttu-id="1e2d6-238">最小 ハ  中工作配置文件密码必须包含字母字符。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-238">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="1e2d6-239">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="1e2d6-239">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1e2d6-240">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="1e2d6-240">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="1e2d6-241">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-241">Int32</span></span>|<span data-ttu-id="1e2d6-242">最小 ハ  工作配置文件密码中需要的小写字符。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-242">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="1e2d6-243">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="1e2d6-243">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1e2d6-244">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="1e2d6-244">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="1e2d6-245">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-245">Int32</span></span>|<span data-ttu-id="1e2d6-246">最小 ハ  中工作配置文件密码必须大写字符。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-246">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="1e2d6-247">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="1e2d6-247">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1e2d6-248">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="1e2d6-248">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="1e2d6-249">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-249">Int32</span></span>|<span data-ttu-id="1e2d6-250">最小 ハ  工作配置文件密码中需要的符号。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-250">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="1e2d6-251">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="1e2d6-251">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1e2d6-252">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1e2d6-252">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1e2d6-253">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-253">Int32</span></span>|<span data-ttu-id="1e2d6-254">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-254">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="1e2d6-255">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1e2d6-255">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1e2d6-256">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-256">Int32</span></span>|<span data-ttu-id="1e2d6-257">以前的工作配置文件密码，以阻止数。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-257">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="1e2d6-258">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="1e2d6-258">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1e2d6-259">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1e2d6-259">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1e2d6-260">Int32</span><span class="sxs-lookup"><span data-stu-id="1e2d6-260">Int32</span></span>|<span data-ttu-id="1e2d6-261">登录失败之前删除工作配置文件允许和已删除的所有企业数据的数量。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-261">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="1e2d6-262">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="1e2d6-262">Valid values 4 to 11</span></span>|
|<span data-ttu-id="1e2d6-263">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1e2d6-263">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="1e2d6-264">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1e2d6-264">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="1e2d6-265">工作所需的配置文件密码的类型。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-265">Type of work profile password that is required.</span></span> <span data-ttu-id="1e2d6-266">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-266">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="1e2d6-267">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="1e2d6-267">workProfileRequirePassword</span></span>|<span data-ttu-id="1e2d6-268">布尔</span><span class="sxs-lookup"><span data-stu-id="1e2d6-268">Boolean</span></span>|<span data-ttu-id="1e2d6-269">密码，则需要或不工作配置文件</span><span class="sxs-lookup"><span data-stu-id="1e2d6-269">Password is required or not for work profile</span></span>|
|<span data-ttu-id="1e2d6-270">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="1e2d6-270">securityRequireVerifyApps</span></span>|<span data-ttu-id="1e2d6-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e2d6-271">Boolean</span></span>|<span data-ttu-id="1e2d6-272">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-272">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="1e2d6-273">响应</span><span class="sxs-lookup"><span data-stu-id="1e2d6-273">Response</span></span>
<span data-ttu-id="1e2d6-274">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-274">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e2d6-275">示例</span><span class="sxs-lookup"><span data-stu-id="1e2d6-275">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e2d6-276">请求</span><span class="sxs-lookup"><span data-stu-id="1e2d6-276">Request</span></span>
<span data-ttu-id="1e2d6-277">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-277">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1831

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="1e2d6-278">响应</span><span class="sxs-lookup"><span data-stu-id="1e2d6-278">Response</span></span>
<span data-ttu-id="1e2d6-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e2d6-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



