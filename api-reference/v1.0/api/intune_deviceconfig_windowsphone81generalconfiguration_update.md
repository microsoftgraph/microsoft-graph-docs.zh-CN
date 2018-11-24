# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="24701-101">更新 windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="24701-101">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="24701-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="24701-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24701-103">更新 [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="24701-103">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="24701-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="24701-104">Prerequisites</span></span>
<span data-ttu-id="24701-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="24701-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="24701-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="24701-107">Permission type</span></span>|<span data-ttu-id="24701-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="24701-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24701-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24701-109">Delegated (work or school account)</span></span>|<span data-ttu-id="24701-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24701-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24701-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24701-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24701-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="24701-112">Not supported.</span></span>|
|<span data-ttu-id="24701-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="24701-113">Application</span></span>|<span data-ttu-id="24701-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="24701-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24701-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24701-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="24701-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="24701-116">Request headers</span></span>
|<span data-ttu-id="24701-117">标头</span><span class="sxs-lookup"><span data-stu-id="24701-117">Header</span></span>|<span data-ttu-id="24701-118">值</span><span class="sxs-lookup"><span data-stu-id="24701-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24701-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="24701-119">Authorization</span></span>|<span data-ttu-id="24701-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="24701-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24701-121">Accept</span><span class="sxs-lookup"><span data-stu-id="24701-121">Accept</span></span>|<span data-ttu-id="24701-122">application/json</span><span class="sxs-lookup"><span data-stu-id="24701-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24701-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="24701-123">Request body</span></span>
<span data-ttu-id="24701-124">在请求正文中，提供 [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24701-124">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="24701-125">下表显示了创建 [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="24701-125">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="24701-126">属性</span><span class="sxs-lookup"><span data-stu-id="24701-126">Property</span></span>|<span data-ttu-id="24701-127">类型</span><span class="sxs-lookup"><span data-stu-id="24701-127">Type</span></span>|<span data-ttu-id="24701-128">说明</span><span class="sxs-lookup"><span data-stu-id="24701-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24701-129">id</span><span class="sxs-lookup"><span data-stu-id="24701-129">id</span></span>|<span data-ttu-id="24701-130">String</span><span class="sxs-lookup"><span data-stu-id="24701-130">String</span></span>|<span data-ttu-id="24701-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="24701-131">Key of the entity.</span></span> <span data-ttu-id="24701-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24701-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24701-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24701-133">lastModifiedDateTime</span></span>|<span data-ttu-id="24701-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24701-134">DateTimeOffset</span></span>|<span data-ttu-id="24701-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="24701-135">DateTime the object was last modified.</span></span> <span data-ttu-id="24701-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24701-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24701-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24701-137">createdDateTime</span></span>|<span data-ttu-id="24701-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24701-138">DateTimeOffset</span></span>|<span data-ttu-id="24701-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="24701-139">DateTime the object was created.</span></span> <span data-ttu-id="24701-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24701-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24701-141">description</span><span class="sxs-lookup"><span data-stu-id="24701-141">description</span></span>|<span data-ttu-id="24701-142">String</span><span class="sxs-lookup"><span data-stu-id="24701-142">String</span></span>|<span data-ttu-id="24701-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="24701-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="24701-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24701-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24701-145">displayName</span><span class="sxs-lookup"><span data-stu-id="24701-145">displayName</span></span>|<span data-ttu-id="24701-146">String</span><span class="sxs-lookup"><span data-stu-id="24701-146">String</span></span>|<span data-ttu-id="24701-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="24701-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="24701-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24701-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24701-149">version</span><span class="sxs-lookup"><span data-stu-id="24701-149">version</span></span>|<span data-ttu-id="24701-150">Int32</span><span class="sxs-lookup"><span data-stu-id="24701-150">Int32</span></span>|<span data-ttu-id="24701-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="24701-151">Version of the device configuration.</span></span> <span data-ttu-id="24701-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24701-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24701-153">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="24701-153">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="24701-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-154">Boolean</span></span>|<span data-ttu-id="24701-155">指示此策略是否仅适用于 Windows Phone 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="24701-155">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="24701-156">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="24701-156">This property is read-only.</span></span>|
|<span data-ttu-id="24701-157">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="24701-157">appsBlockCopyPaste</span></span>|<span data-ttu-id="24701-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-158">Boolean</span></span>|<span data-ttu-id="24701-159">指示是否阻止复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="24701-159">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="24701-160">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="24701-160">bluetoothBlocked</span></span>|<span data-ttu-id="24701-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-161">Boolean</span></span>|<span data-ttu-id="24701-162">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="24701-162">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="24701-163">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="24701-163">cameraBlocked</span></span>|<span data-ttu-id="24701-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-164">Boolean</span></span>|<span data-ttu-id="24701-165">指示是否阻止照相机。</span><span class="sxs-lookup"><span data-stu-id="24701-165">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="24701-166">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="24701-166">cellularBlockWifiTethering</span></span>|<span data-ttu-id="24701-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-167">Boolean</span></span>|<span data-ttu-id="24701-168">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="24701-168">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="24701-169">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="24701-169">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="24701-170">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="24701-170">compliantAppsList</span></span>|<span data-ttu-id="24701-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="24701-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="24701-172">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="24701-172">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="24701-173">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="24701-173">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="24701-174">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="24701-174">compliantAppListType</span></span>|[<span data-ttu-id="24701-175">appListType</span><span class="sxs-lookup"><span data-stu-id="24701-175">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="24701-176">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="24701-176">List that is in the AppComplianceList.</span></span> <span data-ttu-id="24701-177">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="24701-177">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="24701-178">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="24701-178">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="24701-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-179">Boolean</span></span>|<span data-ttu-id="24701-180">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="24701-180">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="24701-181">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="24701-181">emailBlockAddingAccounts</span></span>|<span data-ttu-id="24701-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-182">Boolean</span></span>|<span data-ttu-id="24701-183">指示是否阻止自定义电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="24701-183">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="24701-184">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="24701-184">locationServicesBlocked</span></span>|<span data-ttu-id="24701-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-185">Boolean</span></span>|<span data-ttu-id="24701-186">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="24701-186">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="24701-187">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="24701-187">microsoftAccountBlocked</span></span>|<span data-ttu-id="24701-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-188">Boolean</span></span>|<span data-ttu-id="24701-189">指示是否阻止使用 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="24701-189">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="24701-190">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="24701-190">nfcBlocked</span></span>|<span data-ttu-id="24701-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-191">Boolean</span></span>|<span data-ttu-id="24701-192">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="24701-192">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="24701-193">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="24701-193">passwordBlockSimple</span></span>|<span data-ttu-id="24701-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-194">Boolean</span></span>|<span data-ttu-id="24701-195">指示是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="24701-195">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="24701-196">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="24701-196">passwordExpirationDays</span></span>|<span data-ttu-id="24701-197">Int32</span><span class="sxs-lookup"><span data-stu-id="24701-197">Int32</span></span>|<span data-ttu-id="24701-198">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="24701-198">Number of days before the password expires.</span></span>|
|<span data-ttu-id="24701-199">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="24701-199">passwordMinimumLength</span></span>|<span data-ttu-id="24701-200">Int32</span><span class="sxs-lookup"><span data-stu-id="24701-200">Int32</span></span>|<span data-ttu-id="24701-201">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="24701-201">Minimum length of passwords.</span></span>|
|<span data-ttu-id="24701-202">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="24701-202">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="24701-203">Int32</span><span class="sxs-lookup"><span data-stu-id="24701-203">Int32</span></span>|<span data-ttu-id="24701-204">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="24701-204">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="24701-205">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="24701-205">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="24701-206">Int32</span><span class="sxs-lookup"><span data-stu-id="24701-206">Int32</span></span>|<span data-ttu-id="24701-207">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="24701-207">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="24701-208">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="24701-208">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="24701-209">Int32</span><span class="sxs-lookup"><span data-stu-id="24701-209">Int32</span></span>|<span data-ttu-id="24701-210">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="24701-210">Number of previous passwords to block.</span></span> <span data-ttu-id="24701-211">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="24701-211">Valid values 0 to 24</span></span>|
|<span data-ttu-id="24701-212">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="24701-212">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="24701-213">Int32</span><span class="sxs-lookup"><span data-stu-id="24701-213">Int32</span></span>|<span data-ttu-id="24701-214">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="24701-214">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="24701-215">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="24701-215">passwordRequiredType</span></span>|[<span data-ttu-id="24701-216">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="24701-216">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="24701-217">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="24701-217">Password type that is required.</span></span> <span data-ttu-id="24701-218">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="24701-218">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="24701-219">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="24701-219">passwordRequired</span></span>|<span data-ttu-id="24701-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-220">Boolean</span></span>|<span data-ttu-id="24701-221">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="24701-221">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="24701-222">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="24701-222">screenCaptureBlocked</span></span>|<span data-ttu-id="24701-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-223">Boolean</span></span>|<span data-ttu-id="24701-224">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="24701-224">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="24701-225">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="24701-225">storageBlockRemovableStorage</span></span>|<span data-ttu-id="24701-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-226">Boolean</span></span>|<span data-ttu-id="24701-227">指示是否阻止可移动存储。</span><span class="sxs-lookup"><span data-stu-id="24701-227">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="24701-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="24701-228">storageRequireEncryption</span></span>|<span data-ttu-id="24701-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-229">Boolean</span></span>|<span data-ttu-id="24701-230">指示是否需要加密。</span><span class="sxs-lookup"><span data-stu-id="24701-230">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="24701-231">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="24701-231">webBrowserBlocked</span></span>|<span data-ttu-id="24701-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-232">Boolean</span></span>|<span data-ttu-id="24701-233">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="24701-233">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="24701-234">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="24701-234">wifiBlocked</span></span>|<span data-ttu-id="24701-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-235">Boolean</span></span>|<span data-ttu-id="24701-236">指示是否阻止 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="24701-236">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="24701-237">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="24701-237">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="24701-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-238">Boolean</span></span>|<span data-ttu-id="24701-239">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="24701-239">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="24701-240">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="24701-240">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="24701-241">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="24701-241">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="24701-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-242">Boolean</span></span>|<span data-ttu-id="24701-243">指示是否阻止 Wi-Fi 热点报告。</span><span class="sxs-lookup"><span data-stu-id="24701-243">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="24701-244">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="24701-244">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="24701-245">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="24701-245">windowsStoreBlocked</span></span>|<span data-ttu-id="24701-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="24701-246">Boolean</span></span>|<span data-ttu-id="24701-247">指示是否阻止 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="24701-247">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="24701-248">响应</span><span class="sxs-lookup"><span data-stu-id="24701-248">Response</span></span>
<span data-ttu-id="24701-249">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="24701-249">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24701-250">示例</span><span class="sxs-lookup"><span data-stu-id="24701-250">Example</span></span>
### <a name="request"></a><span data-ttu-id="24701-251">请求</span><span class="sxs-lookup"><span data-stu-id="24701-251">Request</span></span>
<span data-ttu-id="24701-252">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24701-252">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="24701-253">响应</span><span class="sxs-lookup"><span data-stu-id="24701-253">Response</span></span>
<span data-ttu-id="24701-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24701-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```



