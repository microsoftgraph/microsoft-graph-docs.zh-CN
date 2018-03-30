# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="56dc9-101">创建 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="56dc9-101">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="56dc9-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="56dc9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56dc9-103">创建新的 [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56dc9-103">Create a new [plannerBucket](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56dc9-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="56dc9-104">Prerequisites</span></span>
<span data-ttu-id="56dc9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="56dc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="56dc9-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="56dc9-107">Permission type</span></span>|<span data-ttu-id="56dc9-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="56dc9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56dc9-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56dc9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="56dc9-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56dc9-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56dc9-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56dc9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56dc9-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="56dc9-112">Not supported.</span></span>|
|<span data-ttu-id="56dc9-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="56dc9-113">Application</span></span>|<span data-ttu-id="56dc9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="56dc9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56dc9-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56dc9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="56dc9-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="56dc9-116">Request headers</span></span>
|<span data-ttu-id="56dc9-117">标头</span><span class="sxs-lookup"><span data-stu-id="56dc9-117">Header</span></span>|<span data-ttu-id="56dc9-118">值</span><span class="sxs-lookup"><span data-stu-id="56dc9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56dc9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="56dc9-119">Authorization</span></span>|<span data-ttu-id="56dc9-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="56dc9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="56dc9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="56dc9-121">Accept</span></span>|<span data-ttu-id="56dc9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="56dc9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56dc9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="56dc9-123">Request body</span></span>
<span data-ttu-id="56dc9-124">在请求正文中，提供 androidGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56dc9-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="56dc9-125">下表显示创建 androidGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="56dc9-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="56dc9-126">属性</span><span class="sxs-lookup"><span data-stu-id="56dc9-126">Property</span></span>|<span data-ttu-id="56dc9-127">类型</span><span class="sxs-lookup"><span data-stu-id="56dc9-127">Type</span></span>|<span data-ttu-id="56dc9-128">说明</span><span class="sxs-lookup"><span data-stu-id="56dc9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56dc9-129">id</span><span class="sxs-lookup"><span data-stu-id="56dc9-129">id</span></span>|<span data-ttu-id="56dc9-130">String</span><span class="sxs-lookup"><span data-stu-id="56dc9-130">String</span></span>|<span data-ttu-id="56dc9-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="56dc9-131">Key of the setting.</span></span> <span data-ttu-id="56dc9-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56dc9-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56dc9-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56dc9-133">lastModifiedDateTime</span></span>|<span data-ttu-id="56dc9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56dc9-134">DateTimeOffset</span></span>|<span data-ttu-id="56dc9-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="56dc9-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="56dc9-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56dc9-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56dc9-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56dc9-137">createdDateTime</span></span>|<span data-ttu-id="56dc9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56dc9-138">DateTimeOffset</span></span>|<span data-ttu-id="56dc9-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="56dc9-139">DateTime the object was created.</span></span> <span data-ttu-id="56dc9-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56dc9-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56dc9-141">description</span><span class="sxs-lookup"><span data-stu-id="56dc9-141">description</span></span>|<span data-ttu-id="56dc9-142">String</span><span class="sxs-lookup"><span data-stu-id="56dc9-142">String</span></span>|<span data-ttu-id="56dc9-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="56dc9-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="56dc9-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56dc9-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56dc9-145">displayName</span><span class="sxs-lookup"><span data-stu-id="56dc9-145">displayName</span></span>|<span data-ttu-id="56dc9-146">String</span><span class="sxs-lookup"><span data-stu-id="56dc9-146">String</span></span>|<span data-ttu-id="56dc9-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="56dc9-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="56dc9-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56dc9-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56dc9-149">version</span><span class="sxs-lookup"><span data-stu-id="56dc9-149">version</span></span>|<span data-ttu-id="56dc9-150">Int32</span><span class="sxs-lookup"><span data-stu-id="56dc9-150">Int32</span></span>|<span data-ttu-id="56dc9-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="56dc9-151">Version of the device configuration.</span></span> <span data-ttu-id="56dc9-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56dc9-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56dc9-153">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="56dc9-153">appsBlockClipboardSharing</span></span>|<span data-ttu-id="56dc9-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-154">Boolean</span></span>|<span data-ttu-id="56dc9-155">指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="56dc9-155">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="56dc9-156">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="56dc9-156">appsBlockCopyPaste</span></span>|<span data-ttu-id="56dc9-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-157">Boolean</span></span>|<span data-ttu-id="56dc9-158">指示是否阻止在应用程序内复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="56dc9-158">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="56dc9-159">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="56dc9-159">appsBlockYouTube</span></span>|<span data-ttu-id="56dc9-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-160">Boolean</span></span>|<span data-ttu-id="56dc9-161">指示是否阻止 YouTube 应用。</span><span class="sxs-lookup"><span data-stu-id="56dc9-161">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="56dc9-162">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="56dc9-162">bluetoothBlocked</span></span>|<span data-ttu-id="56dc9-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-163">Boolean</span></span>|<span data-ttu-id="56dc9-164">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="56dc9-164">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="56dc9-165">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="56dc9-165">cameraBlocked</span></span>|<span data-ttu-id="56dc9-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-166">Boolean</span></span>|<span data-ttu-id="56dc9-167">指示是否阻止照相机的使用。</span><span class="sxs-lookup"><span data-stu-id="56dc9-167">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="56dc9-168">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="56dc9-168">cellularBlockDataRoaming</span></span>|<span data-ttu-id="56dc9-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-169">Boolean</span></span>|<span data-ttu-id="56dc9-170">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="56dc9-170">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="56dc9-171">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="56dc9-171">cellularBlockMessaging</span></span>|<span data-ttu-id="56dc9-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-172">Boolean</span></span>|<span data-ttu-id="56dc9-173">指示是否阻止 SMS/MMS 消息。</span><span class="sxs-lookup"><span data-stu-id="56dc9-173">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="56dc9-174">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="56dc9-174">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="56dc9-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-175">Boolean</span></span>|<span data-ttu-id="56dc9-176">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="56dc9-176">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="56dc9-177">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="56dc9-177">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="56dc9-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-178">Boolean</span></span>|<span data-ttu-id="56dc9-179">指示是否阻止同步 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="56dc9-179">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="56dc9-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="56dc9-180">compliantAppsList</span></span>|<span data-ttu-id="56dc9-181">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56dc9-181">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="56dc9-182">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="56dc9-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="56dc9-183">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="56dc9-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="56dc9-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="56dc9-184">compliantAppListType</span></span>|<span data-ttu-id="56dc9-185">String</span><span class="sxs-lookup"><span data-stu-id="56dc9-185">String</span></span>|<span data-ttu-id="56dc9-186">位于 CompliantAppsList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="56dc9-186">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="56dc9-187">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="56dc9-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="56dc9-188">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="56dc9-188">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="56dc9-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-189">Boolean</span></span>|<span data-ttu-id="56dc9-190">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="56dc9-190">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="56dc9-191">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="56dc9-191">locationServicesBlocked</span></span>|<span data-ttu-id="56dc9-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-192">Boolean</span></span>|<span data-ttu-id="56dc9-193">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="56dc9-193">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="56dc9-194">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="56dc9-194">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="56dc9-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-195">Boolean</span></span>|<span data-ttu-id="56dc9-196">指示是否阻止 Google 帐户自动同步。</span><span class="sxs-lookup"><span data-stu-id="56dc9-196">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="56dc9-197">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="56dc9-197">googlePlayStoreBlocked</span></span>|<span data-ttu-id="56dc9-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-198">Boolean</span></span>|<span data-ttu-id="56dc9-199">指示是否阻止 Google Play 商店。</span><span class="sxs-lookup"><span data-stu-id="56dc9-199">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="56dc9-200">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="56dc9-200">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="56dc9-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-201">Boolean</span></span>|<span data-ttu-id="56dc9-202">指示在展台模式下是否阻止屏幕睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="56dc9-202">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="56dc9-203">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="56dc9-203">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="56dc9-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-204">Boolean</span></span>|<span data-ttu-id="56dc9-205">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="56dc9-205">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="56dc9-206">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="56dc9-206">kioskModeApps</span></span>|<span data-ttu-id="56dc9-207">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56dc9-207">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="56dc9-208">设备处于展台模式时将允许运行的应用列表。</span><span class="sxs-lookup"><span data-stu-id="56dc9-208">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="56dc9-209">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="56dc9-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="56dc9-210">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="56dc9-210">nfcBlocked</span></span>|<span data-ttu-id="56dc9-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-211">Boolean</span></span>|<span data-ttu-id="56dc9-212">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="56dc9-212">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="56dc9-213">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="56dc9-213">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="56dc9-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-214">Boolean</span></span>|<span data-ttu-id="56dc9-215">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="56dc9-215">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="56dc9-216">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="56dc9-216">passwordBlockTrustAgents</span></span>|<span data-ttu-id="56dc9-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-217">Boolean</span></span>|<span data-ttu-id="56dc9-218">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="56dc9-218">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="56dc9-219">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="56dc9-219">passwordExpirationDays</span></span>|<span data-ttu-id="56dc9-220">Int32</span><span class="sxs-lookup"><span data-stu-id="56dc9-220">Int32</span></span>|<span data-ttu-id="56dc9-221">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="56dc9-221">Number of days before the password expires.</span></span> <span data-ttu-id="56dc9-222">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="56dc9-222">Valid values 1 to 365</span></span>|
|<span data-ttu-id="56dc9-223">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="56dc9-223">passwordMinimumLength</span></span>|<span data-ttu-id="56dc9-224">Int32</span><span class="sxs-lookup"><span data-stu-id="56dc9-224">Int32</span></span>|<span data-ttu-id="56dc9-225">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="56dc9-225">Minimum length of passwords.</span></span> <span data-ttu-id="56dc9-226">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="56dc9-226">Valid values 4 to 16</span></span>|
|<span data-ttu-id="56dc9-227">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="56dc9-227">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="56dc9-228">Int32</span><span class="sxs-lookup"><span data-stu-id="56dc9-228">Int32</span></span>|<span data-ttu-id="56dc9-229">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="56dc9-229">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="56dc9-230">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="56dc9-230">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="56dc9-231">Int32</span><span class="sxs-lookup"><span data-stu-id="56dc9-231">Int32</span></span>|<span data-ttu-id="56dc9-232">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="56dc9-232">Number of previous passwords to block.</span></span> <span data-ttu-id="56dc9-233">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="56dc9-233">Valid values 0 to 24</span></span>|
|<span data-ttu-id="56dc9-234">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="56dc9-234">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="56dc9-235">Int32</span><span class="sxs-lookup"><span data-stu-id="56dc9-235">Int32</span></span>|<span data-ttu-id="56dc9-236">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="56dc9-236">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="56dc9-237">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="56dc9-237">Valid values 4 to 11</span></span>|
|<span data-ttu-id="56dc9-238">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="56dc9-238">passwordRequiredType</span></span>|<span data-ttu-id="56dc9-239">String</span><span class="sxs-lookup"><span data-stu-id="56dc9-239">String</span></span>|<span data-ttu-id="56dc9-240">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="56dc9-240">Type of password that is required.</span></span> <span data-ttu-id="56dc9-241">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="56dc9-241">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`.</span></span>|
|<span data-ttu-id="56dc9-242">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="56dc9-242">passwordRequired</span></span>|<span data-ttu-id="56dc9-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-243">Boolean</span></span>|<span data-ttu-id="56dc9-244">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="56dc9-244">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="56dc9-245">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="56dc9-245">powerOffBlocked</span></span>|<span data-ttu-id="56dc9-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-246">Boolean</span></span>|<span data-ttu-id="56dc9-247">指示是否阻止关闭设备。</span><span class="sxs-lookup"><span data-stu-id="56dc9-247">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="56dc9-248">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="56dc9-248">factoryResetBlocked</span></span>|<span data-ttu-id="56dc9-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-249">Boolean</span></span>|<span data-ttu-id="56dc9-250">指示是否阻止用户执行恢复出厂设置。</span><span class="sxs-lookup"><span data-stu-id="56dc9-250">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="56dc9-251">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="56dc9-251">screenCaptureBlocked</span></span>|<span data-ttu-id="56dc9-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-252">Boolean</span></span>|<span data-ttu-id="56dc9-253">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="56dc9-253">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="56dc9-254">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="56dc9-254">deviceSharingAllowed</span></span>|<span data-ttu-id="56dc9-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-255">Boolean</span></span>|<span data-ttu-id="56dc9-256">指示是否允许设备共享模式。</span><span class="sxs-lookup"><span data-stu-id="56dc9-256">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="56dc9-257">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="56dc9-257">storageBlockGoogleBackup</span></span>|<span data-ttu-id="56dc9-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-258">Boolean</span></span>|<span data-ttu-id="56dc9-259">指示是否阻止 Google 备份。</span><span class="sxs-lookup"><span data-stu-id="56dc9-259">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="56dc9-260">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="56dc9-260">storageBlockRemovableStorage</span></span>|<span data-ttu-id="56dc9-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-261">Boolean</span></span>|<span data-ttu-id="56dc9-262">指示是否阻止可移动存储使用。</span><span class="sxs-lookup"><span data-stu-id="56dc9-262">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="56dc9-263">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="56dc9-263">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="56dc9-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-264">Boolean</span></span>|<span data-ttu-id="56dc9-265">指示是否需要设备加密。</span><span class="sxs-lookup"><span data-stu-id="56dc9-265">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="56dc9-266">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="56dc9-266">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="56dc9-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-267">Boolean</span></span>|<span data-ttu-id="56dc9-268">指示是否需要可移动存储加密。</span><span class="sxs-lookup"><span data-stu-id="56dc9-268">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="56dc9-269">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="56dc9-269">voiceAssistantBlocked</span></span>|<span data-ttu-id="56dc9-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-270">Boolean</span></span>|<span data-ttu-id="56dc9-271">指示是否阻止使用语音助手。</span><span class="sxs-lookup"><span data-stu-id="56dc9-271">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="56dc9-272">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="56dc9-272">voiceDialingBlocked</span></span>|<span data-ttu-id="56dc9-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-273">Boolean</span></span>|<span data-ttu-id="56dc9-274">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="56dc9-274">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="56dc9-275">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="56dc9-275">webBrowserBlockPopups</span></span>|<span data-ttu-id="56dc9-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-276">Boolean</span></span>|<span data-ttu-id="56dc9-277">指示是否阻止 Web 浏览器内的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="56dc9-277">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="56dc9-278">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="56dc9-278">webBrowserBlockAutofill</span></span>|<span data-ttu-id="56dc9-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-279">Boolean</span></span>|<span data-ttu-id="56dc9-280">指示是否阻止 Web 浏览器的自动填充功能。</span><span class="sxs-lookup"><span data-stu-id="56dc9-280">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="56dc9-281">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="56dc9-281">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="56dc9-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-282">Boolean</span></span>|<span data-ttu-id="56dc9-283">指示是否阻止 Web 浏览器内的 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="56dc9-283">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="56dc9-284">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="56dc9-284">webBrowserBlocked</span></span>|<span data-ttu-id="56dc9-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-285">Boolean</span></span>|<span data-ttu-id="56dc9-286">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="56dc9-286">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="56dc9-287">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="56dc9-287">webBrowserCookieSettings</span></span>|<span data-ttu-id="56dc9-288">String</span><span class="sxs-lookup"><span data-stu-id="56dc9-288">String</span></span>|<span data-ttu-id="56dc9-289">Web 浏览器内的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="56dc9-289">Cookie settings within the web browser.</span></span> <span data-ttu-id="56dc9-290">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="56dc9-290">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="56dc9-291">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="56dc9-291">wiFiBlocked</span></span>|<span data-ttu-id="56dc9-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-292">Boolean</span></span>|<span data-ttu-id="56dc9-293">指示是否阻止同步 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="56dc9-293">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="56dc9-294">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="56dc9-294">appsInstallAllowList</span></span>|<span data-ttu-id="56dc9-295">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56dc9-295">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="56dc9-296">可以在 KNOX 设备上安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="56dc9-296">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="56dc9-297">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="56dc9-297">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="56dc9-298">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="56dc9-298">appsLaunchBlockList</span></span>|<span data-ttu-id="56dc9-299">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56dc9-299">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="56dc9-300">阻止在 KNOX 设备上启动的应用列表。</span><span class="sxs-lookup"><span data-stu-id="56dc9-300">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="56dc9-301">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="56dc9-301">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="56dc9-302">appsHideList</span><span class="sxs-lookup"><span data-stu-id="56dc9-302">appsHideList</span></span>|<span data-ttu-id="56dc9-303">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56dc9-303">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="56dc9-304">要在 KNOX 设备上隐藏的应用列表。</span><span class="sxs-lookup"><span data-stu-id="56dc9-304">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="56dc9-305">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="56dc9-305">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="56dc9-306">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="56dc9-306">securityRequireVerifyApps</span></span>|<span data-ttu-id="56dc9-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="56dc9-307">Boolean</span></span>|<span data-ttu-id="56dc9-308">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="56dc9-308">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="56dc9-309">响应</span><span class="sxs-lookup"><span data-stu-id="56dc9-309">Response</span></span>
<span data-ttu-id="56dc9-310">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56dc9-310">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56dc9-311">示例</span><span class="sxs-lookup"><span data-stu-id="56dc9-311">Example</span></span>
### <a name="request"></a><span data-ttu-id="56dc9-312">请求</span><span class="sxs-lookup"><span data-stu-id="56dc9-312">Request</span></span>
<span data-ttu-id="56dc9-313">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="56dc9-313">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3097

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
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
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="56dc9-314">响应</span><span class="sxs-lookup"><span data-stu-id="56dc9-314">Response</span></span>
<span data-ttu-id="56dc9-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="56dc9-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3205

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
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
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```



