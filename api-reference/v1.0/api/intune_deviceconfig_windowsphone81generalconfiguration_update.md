# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="a7952-101">更新 windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7952-101">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="a7952-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a7952-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7952-103">更新 [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a7952-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a7952-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="a7952-104">Prerequisites</span></span>
<span data-ttu-id="a7952-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a7952-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a7952-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7952-107">Permission type</span></span>|<span data-ttu-id="a7952-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a7952-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7952-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7952-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a7952-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7952-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7952-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7952-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7952-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7952-112">Not supported.</span></span>|
|<span data-ttu-id="a7952-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7952-113">Application</span></span>|<span data-ttu-id="a7952-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7952-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7952-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7952-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a7952-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7952-116">Request headers</span></span>
|<span data-ttu-id="a7952-117">标头</span><span class="sxs-lookup"><span data-stu-id="a7952-117">Header</span></span>|<span data-ttu-id="a7952-118">值</span><span class="sxs-lookup"><span data-stu-id="a7952-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7952-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7952-119">Authorization</span></span>|<span data-ttu-id="a7952-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a7952-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a7952-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a7952-121">Accept</span></span>|<span data-ttu-id="a7952-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a7952-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7952-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7952-123">Request body</span></span>
<span data-ttu-id="a7952-124">在请求正文中，提供 [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7952-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="a7952-125">下表显示了创建 [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a7952-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="a7952-126">属性</span><span class="sxs-lookup"><span data-stu-id="a7952-126">Property</span></span>|<span data-ttu-id="a7952-127">类型</span><span class="sxs-lookup"><span data-stu-id="a7952-127">Type</span></span>|<span data-ttu-id="a7952-128">说明</span><span class="sxs-lookup"><span data-stu-id="a7952-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7952-129">id</span><span class="sxs-lookup"><span data-stu-id="a7952-129">id</span></span>|<span data-ttu-id="a7952-130">String</span><span class="sxs-lookup"><span data-stu-id="a7952-130">String</span></span>|<span data-ttu-id="a7952-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a7952-131">Key of the setting.</span></span> <span data-ttu-id="a7952-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7952-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7952-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7952-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a7952-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7952-134">DateTimeOffset</span></span>|<span data-ttu-id="a7952-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a7952-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="a7952-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7952-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7952-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7952-137">createdDateTime</span></span>|<span data-ttu-id="a7952-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7952-138">DateTimeOffset</span></span>|<span data-ttu-id="a7952-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a7952-139">DateTime the object was created.</span></span> <span data-ttu-id="a7952-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7952-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7952-141">description</span><span class="sxs-lookup"><span data-stu-id="a7952-141">description</span></span>|<span data-ttu-id="a7952-142">String</span><span class="sxs-lookup"><span data-stu-id="a7952-142">String</span></span>|<span data-ttu-id="a7952-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a7952-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a7952-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7952-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7952-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a7952-145">displayName</span></span>|<span data-ttu-id="a7952-146">String</span><span class="sxs-lookup"><span data-stu-id="a7952-146">String</span></span>|<span data-ttu-id="a7952-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a7952-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a7952-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7952-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7952-149">version</span><span class="sxs-lookup"><span data-stu-id="a7952-149">version</span></span>|<span data-ttu-id="a7952-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a7952-150">Int32</span></span>|<span data-ttu-id="a7952-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a7952-151">Version of the device configuration.</span></span> <span data-ttu-id="a7952-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7952-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7952-153">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="a7952-153">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="a7952-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-154">Boolean</span></span>|<span data-ttu-id="a7952-155">指示此策略是否仅适用于 Windows Phone 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="a7952-155">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="a7952-156">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a7952-156">This property is read-only.</span></span>|
|<span data-ttu-id="a7952-157">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="a7952-157">appsBlockCopyPaste</span></span>|<span data-ttu-id="a7952-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-158">Boolean</span></span>|<span data-ttu-id="a7952-159">指示是否阻止复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="a7952-159">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="a7952-160">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="a7952-160">bluetoothBlocked</span></span>|<span data-ttu-id="a7952-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-161">Boolean</span></span>|<span data-ttu-id="a7952-162">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="a7952-162">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="a7952-163">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="a7952-163">cameraBlocked</span></span>|<span data-ttu-id="a7952-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-164">Boolean</span></span>|<span data-ttu-id="a7952-165">指示是否阻止照相机。</span><span class="sxs-lookup"><span data-stu-id="a7952-165">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="a7952-166">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="a7952-166">cellularBlockWifiTethering</span></span>|<span data-ttu-id="a7952-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-167">Boolean</span></span>|<span data-ttu-id="a7952-168">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="a7952-168">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="a7952-169">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="a7952-169">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="a7952-170">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="a7952-170">compliantAppsList</span></span>|<span data-ttu-id="a7952-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7952-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="a7952-172">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="a7952-172">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="a7952-173">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="a7952-173">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="a7952-174">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="a7952-174">compliantAppListType</span></span>|<span data-ttu-id="a7952-175">String</span><span class="sxs-lookup"><span data-stu-id="a7952-175">String</span></span>|<span data-ttu-id="a7952-176">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="a7952-176">List that is in the AppComplianceList.</span></span> <span data-ttu-id="a7952-177">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="a7952-177">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="a7952-178">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="a7952-178">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="a7952-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-179">Boolean</span></span>|<span data-ttu-id="a7952-180">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="a7952-180">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="a7952-181">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="a7952-181">emailBlockAddingAccounts</span></span>|<span data-ttu-id="a7952-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-182">Boolean</span></span>|<span data-ttu-id="a7952-183">指示是否阻止自定义电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="a7952-183">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="a7952-184">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="a7952-184">locationServicesBlocked</span></span>|<span data-ttu-id="a7952-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-185">Boolean</span></span>|<span data-ttu-id="a7952-186">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="a7952-186">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="a7952-187">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="a7952-187">microsoftAccountBlocked</span></span>|<span data-ttu-id="a7952-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-188">Boolean</span></span>|<span data-ttu-id="a7952-189">指示是否阻止使用 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="a7952-189">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="a7952-190">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="a7952-190">nfcBlocked</span></span>|<span data-ttu-id="a7952-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-191">Boolean</span></span>|<span data-ttu-id="a7952-192">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="a7952-192">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="a7952-193">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="a7952-193">passwordBlockSimple</span></span>|<span data-ttu-id="a7952-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-194">Boolean</span></span>|<span data-ttu-id="a7952-195">指示是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="a7952-195">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="a7952-196">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a7952-196">passwordExpirationDays</span></span>|<span data-ttu-id="a7952-197">Int32</span><span class="sxs-lookup"><span data-stu-id="a7952-197">Int32</span></span>|<span data-ttu-id="a7952-198">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="a7952-198">Number of days before the password expires.</span></span>|
|<span data-ttu-id="a7952-199">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a7952-199">passwordMinimumLength</span></span>|<span data-ttu-id="a7952-200">Int32</span><span class="sxs-lookup"><span data-stu-id="a7952-200">Int32</span></span>|<span data-ttu-id="a7952-201">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="a7952-201">Minimum length of passwords.</span></span>|
|<span data-ttu-id="a7952-202">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a7952-202">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a7952-203">Int32</span><span class="sxs-lookup"><span data-stu-id="a7952-203">Int32</span></span>|<span data-ttu-id="a7952-204">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="a7952-204">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="a7952-205">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="a7952-205">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="a7952-206">Int32</span><span class="sxs-lookup"><span data-stu-id="a7952-206">Int32</span></span>|<span data-ttu-id="a7952-207">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="a7952-207">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="a7952-208">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a7952-208">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a7952-209">Int32</span><span class="sxs-lookup"><span data-stu-id="a7952-209">Int32</span></span>|<span data-ttu-id="a7952-210">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="a7952-210">Number of previous passwords to block.</span></span> <span data-ttu-id="a7952-211">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="a7952-211">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a7952-212">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a7952-212">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a7952-213">Int32</span><span class="sxs-lookup"><span data-stu-id="a7952-213">Int32</span></span>|<span data-ttu-id="a7952-214">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="a7952-214">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="a7952-215">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a7952-215">passwordRequiredType</span></span>|<span data-ttu-id="a7952-216">String</span><span class="sxs-lookup"><span data-stu-id="a7952-216">String</span></span>|<span data-ttu-id="a7952-217">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="a7952-217">Password type that is required.</span></span> <span data-ttu-id="a7952-218">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="a7952-218">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="a7952-219">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="a7952-219">passwordRequired</span></span>|<span data-ttu-id="a7952-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-220">Boolean</span></span>|<span data-ttu-id="a7952-221">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="a7952-221">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="a7952-222">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="a7952-222">screenCaptureBlocked</span></span>|<span data-ttu-id="a7952-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-223">Boolean</span></span>|<span data-ttu-id="a7952-224">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="a7952-224">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="a7952-225">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="a7952-225">storageBlockRemovableStorage</span></span>|<span data-ttu-id="a7952-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-226">Boolean</span></span>|<span data-ttu-id="a7952-227">指示是否阻止可移动存储。</span><span class="sxs-lookup"><span data-stu-id="a7952-227">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="a7952-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="a7952-228">storageRequireEncryption</span></span>|<span data-ttu-id="a7952-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-229">Boolean</span></span>|<span data-ttu-id="a7952-230">指示是否需要加密。</span><span class="sxs-lookup"><span data-stu-id="a7952-230">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="a7952-231">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="a7952-231">webBrowserBlocked</span></span>|<span data-ttu-id="a7952-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-232">Boolean</span></span>|<span data-ttu-id="a7952-233">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="a7952-233">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="a7952-234">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="a7952-234">wifiBlocked</span></span>|<span data-ttu-id="a7952-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-235">Boolean</span></span>|<span data-ttu-id="a7952-236">指示是否阻止 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="a7952-236">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="a7952-237">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="a7952-237">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="a7952-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-238">Boolean</span></span>|<span data-ttu-id="a7952-239">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="a7952-239">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="a7952-240">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="a7952-240">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="a7952-241">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="a7952-241">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="a7952-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-242">Boolean</span></span>|<span data-ttu-id="a7952-243">指示是否阻止 Wi-Fi 热点报告。</span><span class="sxs-lookup"><span data-stu-id="a7952-243">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="a7952-244">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="a7952-244">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="a7952-245">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="a7952-245">windowsStoreBlocked</span></span>|<span data-ttu-id="a7952-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7952-246">Boolean</span></span>|<span data-ttu-id="a7952-247">指示是否阻止 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="a7952-247">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="a7952-248">响应</span><span class="sxs-lookup"><span data-stu-id="a7952-248">Response</span></span>
<span data-ttu-id="a7952-249">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a7952-249">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7952-250">示例</span><span class="sxs-lookup"><span data-stu-id="a7952-250">Example</span></span>
### <a name="request"></a><span data-ttu-id="a7952-251">请求</span><span class="sxs-lookup"><span data-stu-id="a7952-251">Request</span></span>
<span data-ttu-id="a7952-252">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7952-252">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1452

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="a7952-253">响应</span><span class="sxs-lookup"><span data-stu-id="a7952-253">Response</span></span>
<span data-ttu-id="a7952-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a7952-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



