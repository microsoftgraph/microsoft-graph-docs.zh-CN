# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="ddce1-101">更新 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ddce1-101">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="ddce1-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ddce1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddce1-103">更新 [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ddce1-103">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ddce1-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="ddce1-104">Prerequisites</span></span>
<span data-ttu-id="ddce1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ddce1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ddce1-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddce1-107">Permission type</span></span>|<span data-ttu-id="ddce1-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ddce1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddce1-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddce1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ddce1-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddce1-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ddce1-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddce1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddce1-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddce1-112">Not supported.</span></span>|
|<span data-ttu-id="ddce1-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddce1-113">Application</span></span>|<span data-ttu-id="ddce1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddce1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddce1-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddce1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ddce1-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddce1-116">Request headers</span></span>
|<span data-ttu-id="ddce1-117">标头</span><span class="sxs-lookup"><span data-stu-id="ddce1-117">Header</span></span>|<span data-ttu-id="ddce1-118">值</span><span class="sxs-lookup"><span data-stu-id="ddce1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddce1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddce1-119">Authorization</span></span>|<span data-ttu-id="ddce1-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ddce1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddce1-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ddce1-121">Accept</span></span>|<span data-ttu-id="ddce1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ddce1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddce1-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddce1-123">Request body</span></span>
<span data-ttu-id="ddce1-124">在请求正文中，提供 [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddce1-124">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="ddce1-125">下表显示创建 [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ddce1-125">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="ddce1-126">属性</span><span class="sxs-lookup"><span data-stu-id="ddce1-126">Property</span></span>|<span data-ttu-id="ddce1-127">类型</span><span class="sxs-lookup"><span data-stu-id="ddce1-127">Type</span></span>|<span data-ttu-id="ddce1-128">说明</span><span class="sxs-lookup"><span data-stu-id="ddce1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddce1-129">id</span><span class="sxs-lookup"><span data-stu-id="ddce1-129">id</span></span>|<span data-ttu-id="ddce1-130">String</span><span class="sxs-lookup"><span data-stu-id="ddce1-130">String</span></span>|<span data-ttu-id="ddce1-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ddce1-131">Key of the entity.</span></span> <span data-ttu-id="ddce1-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddce1-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddce1-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddce1-133">lastModifiedDateTime</span></span>|<span data-ttu-id="ddce1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddce1-134">DateTimeOffset</span></span>|<span data-ttu-id="ddce1-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ddce1-135">DateTime the object was last modified.</span></span> <span data-ttu-id="ddce1-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddce1-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddce1-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddce1-137">createdDateTime</span></span>|<span data-ttu-id="ddce1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddce1-138">DateTimeOffset</span></span>|<span data-ttu-id="ddce1-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ddce1-139">DateTime the object was created.</span></span> <span data-ttu-id="ddce1-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddce1-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddce1-141">description</span><span class="sxs-lookup"><span data-stu-id="ddce1-141">description</span></span>|<span data-ttu-id="ddce1-142">String</span><span class="sxs-lookup"><span data-stu-id="ddce1-142">String</span></span>|<span data-ttu-id="ddce1-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ddce1-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ddce1-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddce1-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddce1-145">displayName</span><span class="sxs-lookup"><span data-stu-id="ddce1-145">displayName</span></span>|<span data-ttu-id="ddce1-146">String</span><span class="sxs-lookup"><span data-stu-id="ddce1-146">String</span></span>|<span data-ttu-id="ddce1-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ddce1-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ddce1-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddce1-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddce1-149">version</span><span class="sxs-lookup"><span data-stu-id="ddce1-149">version</span></span>|<span data-ttu-id="ddce1-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ddce1-150">Int32</span></span>|<span data-ttu-id="ddce1-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ddce1-151">Version of the device configuration.</span></span> <span data-ttu-id="ddce1-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddce1-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddce1-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="ddce1-153">accountBlockModification</span></span>|<span data-ttu-id="ddce1-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-154">Boolean</span></span>|<span data-ttu-id="ddce1-155">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="ddce1-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddce1-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="ddce1-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="ddce1-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-157">Boolean</span></span>|<span data-ttu-id="ddce1-158">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="ddce1-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="ddce1-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-159">airDropBlocked</span></span>|<span data-ttu-id="ddce1-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-160">Boolean</span></span>|<span data-ttu-id="ddce1-161">指示设备处于监督模式时是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="ddce1-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddce1-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="ddce1-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="ddce1-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-163">Boolean</span></span>|<span data-ttu-id="ddce1-164">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddce1-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="ddce1-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="ddce1-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-166">Boolean</span></span>|<span data-ttu-id="ddce1-167">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="ddce1-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="ddce1-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="ddce1-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="ddce1-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-169">Boolean</span></span>|<span data-ttu-id="ddce1-170">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddce1-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="ddce1-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="ddce1-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-172">Boolean</span></span>|<span data-ttu-id="ddce1-173">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="ddce1-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-174">appleNewsBlocked</span></span>|<span data-ttu-id="ddce1-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-175">Boolean</span></span>|<span data-ttu-id="ddce1-176">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddce1-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="ddce1-177">appsSingleAppModeList</span></span>|<span data-ttu-id="ddce1-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ddce1-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="ddce1-179">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="ddce1-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="ddce1-180">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="ddce1-180">Supervised only.</span></span> <span data-ttu-id="ddce1-181">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="ddce1-181">iOS 7.0 and later.</span></span> <span data-ttu-id="ddce1-182">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ddce1-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ddce1-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="ddce1-183">appsVisibilityList</span></span>|<span data-ttu-id="ddce1-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ddce1-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="ddce1-185">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="ddce1-186">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="ddce1-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ddce1-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="ddce1-187">appsVisibilityListType</span></span>|[<span data-ttu-id="ddce1-188">appListType</span><span class="sxs-lookup"><span data-stu-id="ddce1-188">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="ddce1-189">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="ddce1-189">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="ddce1-190">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="ddce1-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ddce1-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="ddce1-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="ddce1-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-192">Boolean</span></span>|<span data-ttu-id="ddce1-193">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddce1-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-194">appStoreBlocked</span></span>|<span data-ttu-id="ddce1-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-195">Boolean</span></span>|<span data-ttu-id="ddce1-196">指示是否阻止用户使用 App Store。</span><span class="sxs-lookup"><span data-stu-id="ddce1-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="ddce1-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="ddce1-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="ddce1-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-198">Boolean</span></span>|<span data-ttu-id="ddce1-199">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="ddce1-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="ddce1-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ddce1-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="ddce1-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-201">Boolean</span></span>|<span data-ttu-id="ddce1-202">指示是否阻止 App Store 应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="ddce1-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="ddce1-203">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddce1-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="ddce1-204">appStoreRequirePassword</span></span>|<span data-ttu-id="ddce1-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-205">Boolean</span></span>|<span data-ttu-id="ddce1-206">指示使用 App Store 时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="ddce1-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="ddce1-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="ddce1-207">bluetoothBlockModification</span></span>|<span data-ttu-id="ddce1-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-208">Boolean</span></span>|<span data-ttu-id="ddce1-209">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="ddce1-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-210">cameraBlocked</span></span>|<span data-ttu-id="ddce1-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-211">Boolean</span></span>|<span data-ttu-id="ddce1-212">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="ddce1-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="ddce1-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="ddce1-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="ddce1-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-214">Boolean</span></span>|<span data-ttu-id="ddce1-215">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="ddce1-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="ddce1-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="ddce1-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="ddce1-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-217">Boolean</span></span>|<span data-ttu-id="ddce1-218">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="ddce1-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="ddce1-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="ddce1-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="ddce1-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-220">Boolean</span></span>|<span data-ttu-id="ddce1-221">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="ddce1-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddce1-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="ddce1-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="ddce1-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-223">Boolean</span></span>|<span data-ttu-id="ddce1-224">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="ddce1-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="ddce1-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="ddce1-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="ddce1-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-226">Boolean</span></span>|<span data-ttu-id="ddce1-227">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="ddce1-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="ddce1-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="ddce1-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="ddce1-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-229">Boolean</span></span>|<span data-ttu-id="ddce1-230">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="ddce1-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="ddce1-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ddce1-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="ddce1-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-232">Boolean</span></span>|<span data-ttu-id="ddce1-233">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ddce1-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ddce1-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="ddce1-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-235">Boolean</span></span>|<span data-ttu-id="ddce1-236">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="ddce1-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddce1-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="ddce1-237">compliantAppsList</span></span>|<span data-ttu-id="ddce1-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ddce1-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="ddce1-239">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="ddce1-240">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="ddce1-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ddce1-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="ddce1-241">compliantAppListType</span></span>|[<span data-ttu-id="ddce1-242">appListType</span><span class="sxs-lookup"><span data-stu-id="ddce1-242">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="ddce1-243">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="ddce1-243">List that is in the AppComplianceList.</span></span> <span data-ttu-id="ddce1-244">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="ddce1-244">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ddce1-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="ddce1-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="ddce1-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-246">Boolean</span></span>|<span data-ttu-id="ddce1-247">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="ddce1-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddce1-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-248">definitionLookupBlocked</span></span>|<span data-ttu-id="ddce1-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-249">Boolean</span></span>|<span data-ttu-id="ddce1-250">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="ddce1-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="ddce1-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="ddce1-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-252">Boolean</span></span>|<span data-ttu-id="ddce1-253">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="ddce1-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddce1-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="ddce1-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="ddce1-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-255">Boolean</span></span>|<span data-ttu-id="ddce1-256">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="ddce1-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddce1-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="ddce1-257">deviceBlockNameModification</span></span>|<span data-ttu-id="ddce1-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-258">Boolean</span></span>|<span data-ttu-id="ddce1-259">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddce1-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="ddce1-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="ddce1-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-261">Boolean</span></span>|<span data-ttu-id="ddce1-262">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="ddce1-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="ddce1-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="ddce1-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="ddce1-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-264">Boolean</span></span>|<span data-ttu-id="ddce1-265">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="ddce1-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="ddce1-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="ddce1-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-267">Boolean</span></span>|<span data-ttu-id="ddce1-268">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="ddce1-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="ddce1-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="ddce1-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="ddce1-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-270">Boolean</span></span>|<span data-ttu-id="ddce1-271">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="ddce1-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="ddce1-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="ddce1-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="ddce1-273">String 集合</span><span class="sxs-lookup"><span data-stu-id="ddce1-273">String collection</span></span>|<span data-ttu-id="ddce1-274">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="ddce1-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="ddce1-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="ddce1-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="ddce1-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-276">Boolean</span></span>|<span data-ttu-id="ddce1-277">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="ddce1-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="ddce1-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="ddce1-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="ddce1-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-279">Boolean</span></span>|<span data-ttu-id="ddce1-280">指示是否阻止用户修改企业应用信任设置。</span><span class="sxs-lookup"><span data-stu-id="ddce1-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="ddce1-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-281">faceTimeBlocked</span></span>|<span data-ttu-id="ddce1-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-282">Boolean</span></span>|<span data-ttu-id="ddce1-283">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="ddce1-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="ddce1-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="ddce1-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-285">Boolean</span></span>|<span data-ttu-id="ddce1-286">指示设备处于监督模式时是否阻止查找我的好友。</span><span class="sxs-lookup"><span data-stu-id="ddce1-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddce1-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="ddce1-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="ddce1-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-288">Boolean</span></span>|<span data-ttu-id="ddce1-289">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="ddce1-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="ddce1-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="ddce1-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="ddce1-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-291">Boolean</span></span>|<span data-ttu-id="ddce1-292">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="ddce1-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="ddce1-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-293">gameCenterBlocked</span></span>|<span data-ttu-id="ddce1-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-294">Boolean</span></span>|<span data-ttu-id="ddce1-295">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="ddce1-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddce1-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-296">hostPairingBlocked</span></span>|<span data-ttu-id="ddce1-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-297">Boolean</span></span>|<span data-ttu-id="ddce1-298">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="ddce1-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="ddce1-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="ddce1-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-300">Boolean</span></span>|<span data-ttu-id="ddce1-301">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="ddce1-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddce1-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="ddce1-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="ddce1-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-303">Boolean</span></span>|<span data-ttu-id="ddce1-304">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="ddce1-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="ddce1-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="ddce1-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="ddce1-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-306">Boolean</span></span>|<span data-ttu-id="ddce1-307">指示是否阻止用户在另一个 iOS 或 MacOS 设备上继续从事在 iOS 设备上启动的工作。</span><span class="sxs-lookup"><span data-stu-id="ddce1-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="ddce1-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="ddce1-308">iCloudBlockBackup</span></span>|<span data-ttu-id="ddce1-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-309">Boolean</span></span>|<span data-ttu-id="ddce1-310">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="ddce1-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="ddce1-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="ddce1-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="ddce1-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-312">Boolean</span></span>|<span data-ttu-id="ddce1-313">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="ddce1-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="ddce1-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="ddce1-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="ddce1-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-315">Boolean</span></span>|<span data-ttu-id="ddce1-316">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="ddce1-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="ddce1-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="ddce1-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="ddce1-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-318">Boolean</span></span>|<span data-ttu-id="ddce1-319">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="ddce1-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="ddce1-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="ddce1-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="ddce1-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-321">Boolean</span></span>|<span data-ttu-id="ddce1-322">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="ddce1-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="ddce1-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="ddce1-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="ddce1-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-324">Boolean</span></span>|<span data-ttu-id="ddce1-325">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="ddce1-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="ddce1-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="ddce1-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="ddce1-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-327">Boolean</span></span>|<span data-ttu-id="ddce1-328">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="ddce1-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="ddce1-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="ddce1-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="ddce1-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-330">Boolean</span></span>|<span data-ttu-id="ddce1-331">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="ddce1-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="ddce1-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="ddce1-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="ddce1-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-333">Boolean</span></span>|<span data-ttu-id="ddce1-334">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="ddce1-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="ddce1-335">iTunesBlockRadio</span></span>|<span data-ttu-id="ddce1-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-336">Boolean</span></span>|<span data-ttu-id="ddce1-337">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ddce1-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="ddce1-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="ddce1-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-339">Boolean</span></span>|<span data-ttu-id="ddce1-340">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ddce1-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="ddce1-341">keyboardBlockDictation</span></span>|<span data-ttu-id="ddce1-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-342">Boolean</span></span>|<span data-ttu-id="ddce1-343">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="ddce1-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddce1-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="ddce1-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="ddce1-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-345">Boolean</span></span>|<span data-ttu-id="ddce1-346">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ddce1-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="ddce1-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="ddce1-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-348">Boolean</span></span>|<span data-ttu-id="ddce1-349">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddce1-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="ddce1-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="ddce1-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-351">Boolean</span></span>|<span data-ttu-id="ddce1-352">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ddce1-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="ddce1-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="ddce1-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-354">Boolean</span></span>|<span data-ttu-id="ddce1-355">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="ddce1-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="ddce1-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="ddce1-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-357">Boolean</span></span>|<span data-ttu-id="ddce1-358">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="ddce1-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="ddce1-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="ddce1-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-360">Boolean</span></span>|<span data-ttu-id="ddce1-361">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="ddce1-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="ddce1-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="ddce1-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-363">Boolean</span></span>|<span data-ttu-id="ddce1-364">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="ddce1-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="ddce1-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="ddce1-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-366">Boolean</span></span>|<span data-ttu-id="ddce1-367">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="ddce1-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="ddce1-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="ddce1-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-369">Boolean</span></span>|<span data-ttu-id="ddce1-370">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="ddce1-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="ddce1-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="ddce1-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-372">Boolean</span></span>|<span data-ttu-id="ddce1-373">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="ddce1-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="ddce1-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="ddce1-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-375">Boolean</span></span>|<span data-ttu-id="ddce1-376">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="ddce1-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="ddce1-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="ddce1-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-378">Boolean</span></span>|<span data-ttu-id="ddce1-379">指示在展台模式下是否允许访问语音插入设置。</span><span class="sxs-lookup"><span data-stu-id="ddce1-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="ddce1-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="ddce1-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-381">Boolean</span></span>|<span data-ttu-id="ddce1-382">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="ddce1-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="ddce1-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="ddce1-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-384">Boolean</span></span>|<span data-ttu-id="ddce1-385">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="ddce1-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ddce1-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="ddce1-387">String</span><span class="sxs-lookup"><span data-stu-id="ddce1-387">String</span></span>|<span data-ttu-id="ddce1-388">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="ddce1-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="ddce1-389">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="ddce1-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="ddce1-390">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="ddce1-390">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="ddce1-391">字符串</span><span class="sxs-lookup"><span data-stu-id="ddce1-391">String</span></span>|<span data-ttu-id="ddce1-392">用于展台模式内置应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="ddce1-392">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="ddce1-393">未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="ddce1-393">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="ddce1-394">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="ddce1-394">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="ddce1-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-395">Boolean</span></span>|<span data-ttu-id="ddce1-396">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="ddce1-396">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-397">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="ddce1-397">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="ddce1-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-398">Boolean</span></span>|<span data-ttu-id="ddce1-399">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="ddce1-399">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-400">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="ddce1-400">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="ddce1-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-401">Boolean</span></span>|<span data-ttu-id="ddce1-402">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="ddce1-402">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-403">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="ddce1-403">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="ddce1-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-404">Boolean</span></span>|<span data-ttu-id="ddce1-405">指示在展台模式下是否要求语音过滤。</span><span class="sxs-lookup"><span data-stu-id="ddce1-405">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-406">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="ddce1-406">kioskModeRequireZoom</span></span>|<span data-ttu-id="ddce1-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-407">Boolean</span></span>|<span data-ttu-id="ddce1-408">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="ddce1-408">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="ddce1-409">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="ddce1-409">kioskModeManagedAppId</span></span>|<span data-ttu-id="ddce1-410">String</span><span class="sxs-lookup"><span data-stu-id="ddce1-410">String</span></span>|<span data-ttu-id="ddce1-411">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="ddce1-411">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="ddce1-412">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="ddce1-412">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="ddce1-413">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="ddce1-413">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="ddce1-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-414">Boolean</span></span>|<span data-ttu-id="ddce1-415">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="ddce1-415">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="ddce1-416">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="ddce1-416">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="ddce1-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-417">Boolean</span></span>|<span data-ttu-id="ddce1-418">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="ddce1-418">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="ddce1-419">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="ddce1-419">lockScreenBlockPassbook</span></span>|<span data-ttu-id="ddce1-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-420">Boolean</span></span>|<span data-ttu-id="ddce1-421">指示设备处于锁定状态时是否阻止用户使用 passbook。</span><span class="sxs-lookup"><span data-stu-id="ddce1-421">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="ddce1-422">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="ddce1-422">lockScreenBlockTodayView</span></span>|<span data-ttu-id="ddce1-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-423">Boolean</span></span>|<span data-ttu-id="ddce1-424">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="ddce1-424">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="ddce1-425">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="ddce1-425">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="ddce1-426">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="ddce1-426">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="ddce1-427">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="ddce1-427">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="ddce1-428">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ddce1-428">mediaContentRatingCanada</span></span>|[<span data-ttu-id="ddce1-429">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ddce1-429">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="ddce1-430">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="ddce1-430">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="ddce1-431">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ddce1-431">mediaContentRatingFrance</span></span>|[<span data-ttu-id="ddce1-432">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ddce1-432">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="ddce1-433">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="ddce1-433">Media content rating settings for France</span></span>|
|<span data-ttu-id="ddce1-434">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ddce1-434">mediaContentRatingGermany</span></span>|[<span data-ttu-id="ddce1-435">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ddce1-435">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="ddce1-436">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="ddce1-436">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="ddce1-437">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ddce1-437">mediaContentRatingIreland</span></span>|[<span data-ttu-id="ddce1-438">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ddce1-438">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="ddce1-439">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="ddce1-439">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="ddce1-440">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ddce1-440">mediaContentRatingJapan</span></span>|[<span data-ttu-id="ddce1-441">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ddce1-441">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="ddce1-442">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="ddce1-442">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="ddce1-443">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ddce1-443">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="ddce1-444">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ddce1-444">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="ddce1-445">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="ddce1-445">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="ddce1-446">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ddce1-446">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="ddce1-447">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ddce1-447">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="ddce1-448">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="ddce1-448">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="ddce1-449">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ddce1-449">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="ddce1-450">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ddce1-450">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="ddce1-451">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="ddce1-451">Media content rating settings for United States</span></span>|
|<span data-ttu-id="ddce1-452">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="ddce1-452">networkUsageRules</span></span>|<span data-ttu-id="ddce1-453">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ddce1-453">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="ddce1-454">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="ddce1-454">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="ddce1-455">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="ddce1-455">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="ddce1-456">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="ddce1-456">mediaContentRatingApps</span></span>|[<span data-ttu-id="ddce1-457">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="ddce1-457">ratingAppsType</span></span>](../resources/intune_deviceconfig_ratingappstype.md)|<span data-ttu-id="ddce1-458">媒体内容应用程序的分级设置。</span><span class="sxs-lookup"><span data-stu-id="ddce1-458">Media content rating settings for Apps.</span></span> <span data-ttu-id="ddce1-459">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="ddce1-459">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="ddce1-460">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-460">messagesBlocked</span></span>|<span data-ttu-id="ddce1-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-461">Boolean</span></span>|<span data-ttu-id="ddce1-462">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="ddce1-462">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="ddce1-463">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="ddce1-463">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="ddce1-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-464">Boolean</span></span>|<span data-ttu-id="ddce1-465">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-465">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ddce1-466">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="ddce1-466">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="ddce1-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-467">Boolean</span></span>|<span data-ttu-id="ddce1-468">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="ddce1-468">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="ddce1-469">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="ddce1-469">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="ddce1-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-470">Boolean</span></span>|<span data-ttu-id="ddce1-471">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="ddce1-471">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="ddce1-472">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="ddce1-472">passcodeBlockModification</span></span>|<span data-ttu-id="ddce1-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-473">Boolean</span></span>|<span data-ttu-id="ddce1-474">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-474">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddce1-475">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ddce1-475">passcodeBlockSimple</span></span>|<span data-ttu-id="ddce1-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-476">Boolean</span></span>|<span data-ttu-id="ddce1-477">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="ddce1-477">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="ddce1-478">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ddce1-478">passcodeExpirationDays</span></span>|<span data-ttu-id="ddce1-479">Int32</span><span class="sxs-lookup"><span data-stu-id="ddce1-479">Int32</span></span>|<span data-ttu-id="ddce1-480">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="ddce1-480">Number of days before the passcode expires.</span></span> <span data-ttu-id="ddce1-481">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="ddce1-481">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="ddce1-482">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ddce1-482">passcodeMinimumLength</span></span>|<span data-ttu-id="ddce1-483">Int32</span><span class="sxs-lookup"><span data-stu-id="ddce1-483">Int32</span></span>|<span data-ttu-id="ddce1-484">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="ddce1-484">Minimum length of passcode.</span></span> <span data-ttu-id="ddce1-485">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="ddce1-485">Valid values 4 to 14</span></span>|
|<span data-ttu-id="ddce1-486">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ddce1-486">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ddce1-487">Int32</span><span class="sxs-lookup"><span data-stu-id="ddce1-487">Int32</span></span>|<span data-ttu-id="ddce1-488">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="ddce1-488">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="ddce1-489">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ddce1-489">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ddce1-490">Int32</span><span class="sxs-lookup"><span data-stu-id="ddce1-490">Int32</span></span>|<span data-ttu-id="ddce1-491">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="ddce1-491">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ddce1-492">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ddce1-492">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="ddce1-493">Int32</span><span class="sxs-lookup"><span data-stu-id="ddce1-493">Int32</span></span>|<span data-ttu-id="ddce1-494">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="ddce1-494">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="ddce1-495">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="ddce1-495">Valid values 0 to 4</span></span>|
|<span data-ttu-id="ddce1-496">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="ddce1-496">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="ddce1-497">Int32</span><span class="sxs-lookup"><span data-stu-id="ddce1-497">Int32</span></span>|<span data-ttu-id="ddce1-498">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="ddce1-498">Number of previous passcodes to block.</span></span> <span data-ttu-id="ddce1-499">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="ddce1-499">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ddce1-500">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="ddce1-500">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="ddce1-501">Int32</span><span class="sxs-lookup"><span data-stu-id="ddce1-501">Int32</span></span>|<span data-ttu-id="ddce1-502">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="ddce1-502">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="ddce1-503">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="ddce1-503">Valid values 4 to 11</span></span>|
|<span data-ttu-id="ddce1-504">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="ddce1-504">passcodeRequiredType</span></span>|[<span data-ttu-id="ddce1-505">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ddce1-505">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="ddce1-506">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="ddce1-506">Type of passcode that is required.</span></span> <span data-ttu-id="ddce1-507">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="ddce1-507">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ddce1-508">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="ddce1-508">passcodeRequired</span></span>|<span data-ttu-id="ddce1-509">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-509">Boolean</span></span>|<span data-ttu-id="ddce1-510">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="ddce1-510">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="ddce1-511">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-511">podcastsBlocked</span></span>|<span data-ttu-id="ddce1-512">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-512">Boolean</span></span>|<span data-ttu-id="ddce1-513">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-513">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="ddce1-514">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="ddce1-514">safariBlockAutofill</span></span>|<span data-ttu-id="ddce1-515">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-515">Boolean</span></span>|<span data-ttu-id="ddce1-516">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="ddce1-516">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="ddce1-517">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="ddce1-517">safariBlockJavaScript</span></span>|<span data-ttu-id="ddce1-518">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-518">Boolean</span></span>|<span data-ttu-id="ddce1-519">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="ddce1-519">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="ddce1-520">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="ddce1-520">safariBlockPopups</span></span>|<span data-ttu-id="ddce1-521">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-521">Boolean</span></span>|<span data-ttu-id="ddce1-522">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="ddce1-522">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="ddce1-523">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-523">safariBlocked</span></span>|<span data-ttu-id="ddce1-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-524">Boolean</span></span>|<span data-ttu-id="ddce1-525">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="ddce1-525">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="ddce1-526">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="ddce1-526">safariCookieSettings</span></span>|[<span data-ttu-id="ddce1-527">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="ddce1-527">webBrowserCookieSettings</span></span>](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|<span data-ttu-id="ddce1-528">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="ddce1-528">Cookie settings for Safari.</span></span> <span data-ttu-id="ddce1-529">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="ddce1-529">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="ddce1-530">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="ddce1-530">safariManagedDomains</span></span>|<span data-ttu-id="ddce1-531">String 集合</span><span class="sxs-lookup"><span data-stu-id="ddce1-531">String collection</span></span>|<span data-ttu-id="ddce1-532">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="ddce1-532">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="ddce1-533">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="ddce1-533">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="ddce1-534">String 集合</span><span class="sxs-lookup"><span data-stu-id="ddce1-534">String collection</span></span>|<span data-ttu-id="ddce1-535">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="ddce1-535">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="ddce1-536">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-536">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ddce1-537">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="ddce1-537">safariRequireFraudWarning</span></span>|<span data-ttu-id="ddce1-538">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-538">Boolean</span></span>|<span data-ttu-id="ddce1-539">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="ddce1-539">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="ddce1-540">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-540">screenCaptureBlocked</span></span>|<span data-ttu-id="ddce1-541">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-541">Boolean</span></span>|<span data-ttu-id="ddce1-542">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="ddce1-542">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="ddce1-543">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-543">siriBlocked</span></span>|<span data-ttu-id="ddce1-544">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-544">Boolean</span></span>|<span data-ttu-id="ddce1-545">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="ddce1-545">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="ddce1-546">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-546">siriBlockedWhenLocked</span></span>|<span data-ttu-id="ddce1-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-547">Boolean</span></span>|<span data-ttu-id="ddce1-548">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="ddce1-548">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="ddce1-549">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="ddce1-549">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="ddce1-550">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-550">Boolean</span></span>|<span data-ttu-id="ddce1-551">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="ddce1-551">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="ddce1-552">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="ddce1-552">siriRequireProfanityFilter</span></span>|<span data-ttu-id="ddce1-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-553">Boolean</span></span>|<span data-ttu-id="ddce1-554">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="ddce1-554">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="ddce1-555">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="ddce1-555">spotlightBlockInternetResults</span></span>|<span data-ttu-id="ddce1-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-556">Boolean</span></span>|<span data-ttu-id="ddce1-557">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="ddce1-557">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="ddce1-558">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="ddce1-558">voiceDialingBlocked</span></span>|<span data-ttu-id="ddce1-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-559">Boolean</span></span>|<span data-ttu-id="ddce1-560">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="ddce1-560">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="ddce1-561">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="ddce1-561">wallpaperBlockModification</span></span>|<span data-ttu-id="ddce1-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-562">Boolean</span></span>|<span data-ttu-id="ddce1-563">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ddce1-563">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="ddce1-564">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="ddce1-564">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="ddce1-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddce1-565">Boolean</span></span>|<span data-ttu-id="ddce1-566">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="ddce1-566">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="ddce1-567">响应</span><span class="sxs-lookup"><span data-stu-id="ddce1-567">Response</span></span>
<span data-ttu-id="ddce1-568">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ddce1-568">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddce1-569">示例</span><span class="sxs-lookup"><span data-stu-id="ddce1-569">Example</span></span>
### <a name="request"></a><span data-ttu-id="ddce1-570">请求</span><span class="sxs-lookup"><span data-stu-id="ddce1-570">Request</span></span>
<span data-ttu-id="ddce1-571">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ddce1-571">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 7841

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```

### <a name="response"></a><span data-ttu-id="ddce1-572">响应</span><span class="sxs-lookup"><span data-stu-id="ddce1-572">Response</span></span>
<span data-ttu-id="ddce1-p127">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ddce1-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8013

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```



