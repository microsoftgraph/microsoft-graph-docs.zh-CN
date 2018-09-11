# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="86f18-101">创建 windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="86f18-101">Create windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="86f18-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="86f18-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86f18-103">创建新的 [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86f18-103">Create a new [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86f18-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="86f18-104">Prerequisites</span></span>
<span data-ttu-id="86f18-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="86f18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="86f18-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="86f18-107">Permission type</span></span>|<span data-ttu-id="86f18-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="86f18-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86f18-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86f18-109">Delegated (work or school account)</span></span>|<span data-ttu-id="86f18-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86f18-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86f18-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86f18-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86f18-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="86f18-112">Not supported.</span></span>|
|<span data-ttu-id="86f18-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="86f18-113">Application</span></span>|<span data-ttu-id="86f18-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="86f18-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86f18-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86f18-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="86f18-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="86f18-116">Request headers</span></span>
|<span data-ttu-id="86f18-117">标头</span><span class="sxs-lookup"><span data-stu-id="86f18-117">Header</span></span>|<span data-ttu-id="86f18-118">值</span><span class="sxs-lookup"><span data-stu-id="86f18-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86f18-119">授权</span><span class="sxs-lookup"><span data-stu-id="86f18-119">Authorization</span></span>|<span data-ttu-id="86f18-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="86f18-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86f18-121">接受</span><span class="sxs-lookup"><span data-stu-id="86f18-121">Accept</span></span>|<span data-ttu-id="86f18-122">application/json</span><span class="sxs-lookup"><span data-stu-id="86f18-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86f18-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="86f18-123">Request body</span></span>
<span data-ttu-id="86f18-124">在请求正文中，提供 windowsPhone81GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86f18-124">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="86f18-125">下表显示了创建 windowsPhone81GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="86f18-125">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="86f18-126">属性</span><span class="sxs-lookup"><span data-stu-id="86f18-126">Property</span></span>|<span data-ttu-id="86f18-127">类型</span><span class="sxs-lookup"><span data-stu-id="86f18-127">Type</span></span>|<span data-ttu-id="86f18-128">说明</span><span class="sxs-lookup"><span data-stu-id="86f18-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86f18-129">ID</span><span class="sxs-lookup"><span data-stu-id="86f18-129">id</span></span>|<span data-ttu-id="86f18-130">字符串</span><span class="sxs-lookup"><span data-stu-id="86f18-130">String</span></span>|<span data-ttu-id="86f18-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="86f18-131">Key of the entity.</span></span> <span data-ttu-id="86f18-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86f18-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86f18-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86f18-133">lastModifiedDateTime</span></span>|<span data-ttu-id="86f18-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86f18-134">DateTimeOffset</span></span>|<span data-ttu-id="86f18-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86f18-135">DateTime the object was last modified.</span></span> <span data-ttu-id="86f18-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86f18-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86f18-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86f18-137">createdDateTime</span></span>|<span data-ttu-id="86f18-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86f18-138">DateTimeOffset</span></span>|<span data-ttu-id="86f18-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86f18-139">DateTime the object was created.</span></span> <span data-ttu-id="86f18-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86f18-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86f18-141">说明</span><span class="sxs-lookup"><span data-stu-id="86f18-141">description</span></span>|<span data-ttu-id="86f18-142">字符串</span><span class="sxs-lookup"><span data-stu-id="86f18-142">String</span></span>|<span data-ttu-id="86f18-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="86f18-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86f18-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86f18-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86f18-145">displayName</span><span class="sxs-lookup"><span data-stu-id="86f18-145">displayName</span></span>|<span data-ttu-id="86f18-146">字符串</span><span class="sxs-lookup"><span data-stu-id="86f18-146">String</span></span>|<span data-ttu-id="86f18-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="86f18-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86f18-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86f18-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86f18-149">version</span><span class="sxs-lookup"><span data-stu-id="86f18-149">version</span></span>|<span data-ttu-id="86f18-150">Int32</span><span class="sxs-lookup"><span data-stu-id="86f18-150">Int32</span></span>|<span data-ttu-id="86f18-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="86f18-151">Version of the device configuration.</span></span> <span data-ttu-id="86f18-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86f18-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86f18-153">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="86f18-153">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="86f18-154">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-154">Boolean</span></span>|<span data-ttu-id="86f18-155">指示此策略是否仅适用于 Windows Phone 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="86f18-155">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="86f18-156">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="86f18-156">This property is read-only.</span></span>|
|<span data-ttu-id="86f18-157">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="86f18-157">appsBlockCopyPaste</span></span>|<span data-ttu-id="86f18-158">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-158">Boolean</span></span>|<span data-ttu-id="86f18-159">指示是否阻止复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="86f18-159">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="86f18-160">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="86f18-160">bluetoothBlocked</span></span>|<span data-ttu-id="86f18-161">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-161">Boolean</span></span>|<span data-ttu-id="86f18-162">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="86f18-162">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="86f18-163">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="86f18-163">cameraBlocked</span></span>|<span data-ttu-id="86f18-164">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-164">Boolean</span></span>|<span data-ttu-id="86f18-165">指示是否阻止照相机。</span><span class="sxs-lookup"><span data-stu-id="86f18-165">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="86f18-166">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="86f18-166">cellularBlockWifiTethering</span></span>|<span data-ttu-id="86f18-167">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-167">Boolean</span></span>|<span data-ttu-id="86f18-168">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="86f18-168">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="86f18-169">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="86f18-169">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="86f18-170">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="86f18-170">compliantAppsList</span></span>|<span data-ttu-id="86f18-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="86f18-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="86f18-172">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="86f18-172">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="86f18-173">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="86f18-173">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="86f18-174">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="86f18-174">compliantAppListType</span></span>|[<span data-ttu-id="86f18-175">appListType</span><span class="sxs-lookup"><span data-stu-id="86f18-175">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="86f18-176">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="86f18-176">List that is in the AppComplianceList.</span></span> <span data-ttu-id="86f18-177">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="86f18-177">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="86f18-178">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="86f18-178">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="86f18-179">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-179">Boolean</span></span>|<span data-ttu-id="86f18-180">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="86f18-180">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="86f18-181">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="86f18-181">emailBlockAddingAccounts</span></span>|<span data-ttu-id="86f18-182">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-182">Boolean</span></span>|<span data-ttu-id="86f18-183">指示是否阻止自定义电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="86f18-183">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="86f18-184">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="86f18-184">locationServicesBlocked</span></span>|<span data-ttu-id="86f18-185">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-185">Boolean</span></span>|<span data-ttu-id="86f18-186">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="86f18-186">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="86f18-187">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="86f18-187">microsoftAccountBlocked</span></span>|<span data-ttu-id="86f18-188">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-188">Boolean</span></span>|<span data-ttu-id="86f18-189">指示是否阻止使用 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="86f18-189">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="86f18-190">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="86f18-190">nfcBlocked</span></span>|<span data-ttu-id="86f18-191">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-191">Boolean</span></span>|<span data-ttu-id="86f18-192">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="86f18-192">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="86f18-193">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="86f18-193">passwordBlockSimple</span></span>|<span data-ttu-id="86f18-194">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-194">Boolean</span></span>|<span data-ttu-id="86f18-195">指示是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="86f18-195">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="86f18-196">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="86f18-196">passwordExpirationDays</span></span>|<span data-ttu-id="86f18-197">Int32</span><span class="sxs-lookup"><span data-stu-id="86f18-197">Int32</span></span>|<span data-ttu-id="86f18-198">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="86f18-198">Number of days before the password expires.</span></span>|
|<span data-ttu-id="86f18-199">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="86f18-199">passwordMinimumLength</span></span>|<span data-ttu-id="86f18-200">Int32</span><span class="sxs-lookup"><span data-stu-id="86f18-200">Int32</span></span>|<span data-ttu-id="86f18-201">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="86f18-201">Minimum length of passwords.</span></span>|
|<span data-ttu-id="86f18-202">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="86f18-202">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="86f18-203">Int32</span><span class="sxs-lookup"><span data-stu-id="86f18-203">Int32</span></span>|<span data-ttu-id="86f18-204">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="86f18-204">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="86f18-205">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="86f18-205">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="86f18-206">Int32</span><span class="sxs-lookup"><span data-stu-id="86f18-206">Int32</span></span>|<span data-ttu-id="86f18-207">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="86f18-207">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="86f18-208">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="86f18-208">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="86f18-209">Int32</span><span class="sxs-lookup"><span data-stu-id="86f18-209">Int32</span></span>|<span data-ttu-id="86f18-210">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="86f18-210">Number of previous passwords to block.</span></span> <span data-ttu-id="86f18-211">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="86f18-211">Valid values 0 to 24</span></span>|
|<span data-ttu-id="86f18-212">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="86f18-212">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="86f18-213">Int32</span><span class="sxs-lookup"><span data-stu-id="86f18-213">Int32</span></span>|<span data-ttu-id="86f18-214">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="86f18-214">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="86f18-215">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="86f18-215">passwordRequiredType</span></span>|[<span data-ttu-id="86f18-216">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="86f18-216">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="86f18-217">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="86f18-217">Password type that is required.</span></span> <span data-ttu-id="86f18-218">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="86f18-218">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="86f18-219">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="86f18-219">passwordRequired</span></span>|<span data-ttu-id="86f18-220">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-220">Boolean</span></span>|<span data-ttu-id="86f18-221">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="86f18-221">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="86f18-222">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="86f18-222">screenCaptureBlocked</span></span>|<span data-ttu-id="86f18-223">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-223">Boolean</span></span>|<span data-ttu-id="86f18-224">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="86f18-224">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="86f18-225">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="86f18-225">storageBlockRemovableStorage</span></span>|<span data-ttu-id="86f18-226">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-226">Boolean</span></span>|<span data-ttu-id="86f18-227">指示是否阻止可移动存储。</span><span class="sxs-lookup"><span data-stu-id="86f18-227">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="86f18-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="86f18-228">storageRequireEncryption</span></span>|<span data-ttu-id="86f18-229">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-229">Boolean</span></span>|<span data-ttu-id="86f18-230">指示是否需要加密。</span><span class="sxs-lookup"><span data-stu-id="86f18-230">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="86f18-231">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="86f18-231">webBrowserBlocked</span></span>|<span data-ttu-id="86f18-232">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-232">Boolean</span></span>|<span data-ttu-id="86f18-233">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="86f18-233">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="86f18-234">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="86f18-234">wifiBlocked</span></span>|<span data-ttu-id="86f18-235">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-235">Boolean</span></span>|<span data-ttu-id="86f18-236">指示是否阻止 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="86f18-236">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="86f18-237">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="86f18-237">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="86f18-238">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-238">Boolean</span></span>|<span data-ttu-id="86f18-239">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="86f18-239">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="86f18-240">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="86f18-240">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="86f18-241">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="86f18-241">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="86f18-242">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-242">Boolean</span></span>|<span data-ttu-id="86f18-243">指示是否阻止 Wi-Fi 热点报告。</span><span class="sxs-lookup"><span data-stu-id="86f18-243">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="86f18-244">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="86f18-244">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="86f18-245">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="86f18-245">windowsStoreBlocked</span></span>|<span data-ttu-id="86f18-246">布尔值</span><span class="sxs-lookup"><span data-stu-id="86f18-246">Boolean</span></span>|<span data-ttu-id="86f18-247">指示是否阻止 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="86f18-247">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="86f18-248">响应</span><span class="sxs-lookup"><span data-stu-id="86f18-248">Response</span></span>
<span data-ttu-id="86f18-249">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86f18-249">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86f18-250">示例</span><span class="sxs-lookup"><span data-stu-id="86f18-250">Example</span></span>
### <a name="request"></a><span data-ttu-id="86f18-251">请求</span><span class="sxs-lookup"><span data-stu-id="86f18-251">Request</span></span>
<span data-ttu-id="86f18-252">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86f18-252">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1525

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="86f18-253">响应</span><span class="sxs-lookup"><span data-stu-id="86f18-253">Response</span></span>
<span data-ttu-id="86f18-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86f18-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








