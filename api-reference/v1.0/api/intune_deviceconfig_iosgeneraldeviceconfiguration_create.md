# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="4267e-101">创建 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4267e-101">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="4267e-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4267e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4267e-103">创建新的 [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4267e-103">Create a new [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4267e-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="4267e-104">Prerequisites</span></span>
<span data-ttu-id="4267e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4267e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4267e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="4267e-107">Permission type</span></span>|<span data-ttu-id="4267e-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4267e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4267e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4267e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4267e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4267e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4267e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4267e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4267e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="4267e-112">Not supported.</span></span>|
|<span data-ttu-id="4267e-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="4267e-113">Application</span></span>|<span data-ttu-id="4267e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4267e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4267e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4267e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4267e-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="4267e-116">Request headers</span></span>
|<span data-ttu-id="4267e-117">标头</span><span class="sxs-lookup"><span data-stu-id="4267e-117">Header</span></span>|<span data-ttu-id="4267e-118">值</span><span class="sxs-lookup"><span data-stu-id="4267e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4267e-119">授权</span><span class="sxs-lookup"><span data-stu-id="4267e-119">Authorization</span></span>|<span data-ttu-id="4267e-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4267e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4267e-121">接受</span><span class="sxs-lookup"><span data-stu-id="4267e-121">Accept</span></span>|<span data-ttu-id="4267e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4267e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4267e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4267e-123">Request body</span></span>
<span data-ttu-id="4267e-124">在请求正文中，提供 iosGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4267e-124">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="4267e-125">下表显示创建 iosGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4267e-125">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="4267e-126">属性</span><span class="sxs-lookup"><span data-stu-id="4267e-126">Property</span></span>|<span data-ttu-id="4267e-127">类型</span><span class="sxs-lookup"><span data-stu-id="4267e-127">Type</span></span>|<span data-ttu-id="4267e-128">说明</span><span class="sxs-lookup"><span data-stu-id="4267e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4267e-129">ID</span><span class="sxs-lookup"><span data-stu-id="4267e-129">id</span></span>|<span data-ttu-id="4267e-130">字符串</span><span class="sxs-lookup"><span data-stu-id="4267e-130">String</span></span>|<span data-ttu-id="4267e-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4267e-131">Key of the entity.</span></span> <span data-ttu-id="4267e-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4267e-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4267e-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4267e-133">lastModifiedDateTime</span></span>|<span data-ttu-id="4267e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4267e-134">DateTimeOffset</span></span>|<span data-ttu-id="4267e-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4267e-135">DateTime the object was last modified.</span></span> <span data-ttu-id="4267e-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4267e-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4267e-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4267e-137">createdDateTime</span></span>|<span data-ttu-id="4267e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4267e-138">DateTimeOffset</span></span>|<span data-ttu-id="4267e-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4267e-139">DateTime the object was created.</span></span> <span data-ttu-id="4267e-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4267e-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4267e-141">描述</span><span class="sxs-lookup"><span data-stu-id="4267e-141">description</span></span>|<span data-ttu-id="4267e-142">字符串</span><span class="sxs-lookup"><span data-stu-id="4267e-142">String</span></span>|<span data-ttu-id="4267e-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4267e-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4267e-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4267e-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4267e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="4267e-145">displayName</span></span>|<span data-ttu-id="4267e-146">字符串</span><span class="sxs-lookup"><span data-stu-id="4267e-146">String</span></span>|<span data-ttu-id="4267e-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4267e-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4267e-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4267e-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4267e-149">版本</span><span class="sxs-lookup"><span data-stu-id="4267e-149">version</span></span>|<span data-ttu-id="4267e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4267e-150">Int32</span></span>|<span data-ttu-id="4267e-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4267e-151">Version of the device configuration.</span></span> <span data-ttu-id="4267e-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4267e-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4267e-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="4267e-153">accountBlockModification</span></span>|<span data-ttu-id="4267e-154">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-154">Boolean</span></span>|<span data-ttu-id="4267e-155">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="4267e-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="4267e-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="4267e-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="4267e-157">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-157">Boolean</span></span>|<span data-ttu-id="4267e-158">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="4267e-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="4267e-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-159">airDropBlocked</span></span>|<span data-ttu-id="4267e-160">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-160">Boolean</span></span>|<span data-ttu-id="4267e-161">指示设备处于监督模式时是否允许使用 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="4267e-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="4267e-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="4267e-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="4267e-163">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-163">Boolean</span></span>|<span data-ttu-id="4267e-164">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="4267e-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="4267e-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="4267e-166">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-166">Boolean</span></span>|<span data-ttu-id="4267e-167">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="4267e-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="4267e-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="4267e-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="4267e-169">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-169">Boolean</span></span>|<span data-ttu-id="4267e-170">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="4267e-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="4267e-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="4267e-172">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-172">Boolean</span></span>|<span data-ttu-id="4267e-173">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="4267e-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-174">appleNewsBlocked</span></span>|<span data-ttu-id="4267e-175">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-175">Boolean</span></span>|<span data-ttu-id="4267e-176">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="4267e-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="4267e-177">appsSingleAppModeList</span></span>|<span data-ttu-id="4267e-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4267e-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="4267e-179">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="4267e-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="4267e-180">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="4267e-180">Supervised only.</span></span> <span data-ttu-id="4267e-181">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="4267e-181">iOS 7.0 and later.</span></span> <span data-ttu-id="4267e-182">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4267e-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4267e-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="4267e-183">appsVisibilityList</span></span>|<span data-ttu-id="4267e-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4267e-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="4267e-185">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="4267e-186">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="4267e-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4267e-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="4267e-187">appsVisibilityListType</span></span>|[<span data-ttu-id="4267e-188">appListType</span><span class="sxs-lookup"><span data-stu-id="4267e-188">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="4267e-p110">位于 AppsVisibilityList 中的列表类型。 可能的值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="4267e-p110">Type of list that is in the AppsVisibilityList. The possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="4267e-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="4267e-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="4267e-192">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-192">Boolean</span></span>|<span data-ttu-id="4267e-193">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="4267e-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-194">appStoreBlocked</span></span>|<span data-ttu-id="4267e-195">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-195">Boolean</span></span>|<span data-ttu-id="4267e-196">指示是否阻止用户使用应用商店。</span><span class="sxs-lookup"><span data-stu-id="4267e-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="4267e-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="4267e-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="4267e-198">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-198">Boolean</span></span>|<span data-ttu-id="4267e-199">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="4267e-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="4267e-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="4267e-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="4267e-201">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-201">Boolean</span></span>|<span data-ttu-id="4267e-202">指示是否阻止应用商店应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="4267e-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="4267e-203">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="4267e-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="4267e-204">appStoreRequirePassword</span></span>|<span data-ttu-id="4267e-205">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-205">Boolean</span></span>|<span data-ttu-id="4267e-206">指示使用应用商店时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="4267e-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="4267e-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="4267e-207">bluetoothBlockModification</span></span>|<span data-ttu-id="4267e-208">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-208">Boolean</span></span>|<span data-ttu-id="4267e-209">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="4267e-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-210">cameraBlocked</span></span>|<span data-ttu-id="4267e-211">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-211">Boolean</span></span>|<span data-ttu-id="4267e-212">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="4267e-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="4267e-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="4267e-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="4267e-214">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-214">Boolean</span></span>|<span data-ttu-id="4267e-215">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="4267e-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="4267e-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="4267e-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="4267e-217">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-217">Boolean</span></span>|<span data-ttu-id="4267e-218">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="4267e-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="4267e-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="4267e-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="4267e-220">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-220">Boolean</span></span>|<span data-ttu-id="4267e-221">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="4267e-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="4267e-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="4267e-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="4267e-223">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-223">Boolean</span></span>|<span data-ttu-id="4267e-224">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="4267e-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="4267e-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="4267e-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="4267e-226">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-226">Boolean</span></span>|<span data-ttu-id="4267e-227">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="4267e-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="4267e-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="4267e-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="4267e-229">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-229">Boolean</span></span>|<span data-ttu-id="4267e-230">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="4267e-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="4267e-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="4267e-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="4267e-232">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-232">Boolean</span></span>|<span data-ttu-id="4267e-233">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="4267e-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="4267e-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="4267e-235">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-235">Boolean</span></span>|<span data-ttu-id="4267e-236">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="4267e-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="4267e-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="4267e-237">compliantAppsList</span></span>|<span data-ttu-id="4267e-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4267e-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="4267e-239">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="4267e-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="4267e-240">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="4267e-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4267e-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="4267e-241">compliantAppListType</span></span>|[<span data-ttu-id="4267e-242">appListType</span><span class="sxs-lookup"><span data-stu-id="4267e-242">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="4267e-p113">位于 AppComplianceList 中的列表。可能的值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="4267e-p113">List that is in the AppComplianceList. The possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="4267e-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="4267e-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="4267e-246">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-246">Boolean</span></span>|<span data-ttu-id="4267e-247">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="4267e-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="4267e-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-248">definitionLookupBlocked</span></span>|<span data-ttu-id="4267e-249">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-249">Boolean</span></span>|<span data-ttu-id="4267e-250">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="4267e-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="4267e-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="4267e-252">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-252">Boolean</span></span>|<span data-ttu-id="4267e-253">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="4267e-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="4267e-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="4267e-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="4267e-255">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-255">Boolean</span></span>|<span data-ttu-id="4267e-256">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="4267e-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="4267e-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="4267e-257">deviceBlockNameModification</span></span>|<span data-ttu-id="4267e-258">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-258">Boolean</span></span>|<span data-ttu-id="4267e-259">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="4267e-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="4267e-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="4267e-261">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-261">Boolean</span></span>|<span data-ttu-id="4267e-262">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="4267e-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="4267e-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="4267e-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="4267e-264">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-264">Boolean</span></span>|<span data-ttu-id="4267e-265">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="4267e-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="4267e-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="4267e-267">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-267">Boolean</span></span>|<span data-ttu-id="4267e-268">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="4267e-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="4267e-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="4267e-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="4267e-270">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-270">Boolean</span></span>|<span data-ttu-id="4267e-271">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="4267e-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="4267e-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="4267e-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="4267e-273">String 集合</span><span class="sxs-lookup"><span data-stu-id="4267e-273">String collection</span></span>|<span data-ttu-id="4267e-274">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="4267e-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="4267e-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="4267e-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="4267e-276">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-276">Boolean</span></span>|<span data-ttu-id="4267e-277">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="4267e-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="4267e-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="4267e-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="4267e-279">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-279">Boolean</span></span>|<span data-ttu-id="4267e-280">指示是否阻止用户修改企业应用信任设置。</span><span class="sxs-lookup"><span data-stu-id="4267e-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="4267e-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-281">faceTimeBlocked</span></span>|<span data-ttu-id="4267e-282">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-282">Boolean</span></span>|<span data-ttu-id="4267e-283">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="4267e-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="4267e-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="4267e-285">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-285">Boolean</span></span>|<span data-ttu-id="4267e-286">指示设备处于监督模式时是否阻止查找我的好友。</span><span class="sxs-lookup"><span data-stu-id="4267e-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="4267e-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="4267e-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="4267e-288">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-288">Boolean</span></span>|<span data-ttu-id="4267e-289">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="4267e-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="4267e-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="4267e-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="4267e-291">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-291">Boolean</span></span>|<span data-ttu-id="4267e-292">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="4267e-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="4267e-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-293">gameCenterBlocked</span></span>|<span data-ttu-id="4267e-294">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-294">Boolean</span></span>|<span data-ttu-id="4267e-295">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="4267e-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="4267e-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-296">hostPairingBlocked</span></span>|<span data-ttu-id="4267e-297">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-297">Boolean</span></span>|<span data-ttu-id="4267e-298">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="4267e-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="4267e-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="4267e-300">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-300">Boolean</span></span>|<span data-ttu-id="4267e-301">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="4267e-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="4267e-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="4267e-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="4267e-303">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-303">Boolean</span></span>|<span data-ttu-id="4267e-304">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="4267e-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="4267e-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="4267e-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="4267e-306">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-306">Boolean</span></span>|<span data-ttu-id="4267e-307">指示是否阻止用户在另一个 iOS 或 MacOS 设备上继续从事在 iOS 设备上启动的工作。</span><span class="sxs-lookup"><span data-stu-id="4267e-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="4267e-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="4267e-308">iCloudBlockBackup</span></span>|<span data-ttu-id="4267e-309">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-309">Boolean</span></span>|<span data-ttu-id="4267e-310">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="4267e-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="4267e-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="4267e-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="4267e-312">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-312">Boolean</span></span>|<span data-ttu-id="4267e-313">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="4267e-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="4267e-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="4267e-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="4267e-315">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-315">Boolean</span></span>|<span data-ttu-id="4267e-316">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="4267e-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="4267e-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="4267e-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="4267e-318">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-318">Boolean</span></span>|<span data-ttu-id="4267e-319">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="4267e-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="4267e-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="4267e-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="4267e-321">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-321">Boolean</span></span>|<span data-ttu-id="4267e-322">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="4267e-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="4267e-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="4267e-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="4267e-324">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-324">Boolean</span></span>|<span data-ttu-id="4267e-325">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="4267e-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="4267e-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="4267e-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="4267e-327">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-327">Boolean</span></span>|<span data-ttu-id="4267e-328">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="4267e-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="4267e-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="4267e-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="4267e-330">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-330">Boolean</span></span>|<span data-ttu-id="4267e-331">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="4267e-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="4267e-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="4267e-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="4267e-333">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-333">Boolean</span></span>|<span data-ttu-id="4267e-334">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="4267e-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="4267e-335">iTunesBlockRadio</span></span>|<span data-ttu-id="4267e-336">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-336">Boolean</span></span>|<span data-ttu-id="4267e-337">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="4267e-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="4267e-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="4267e-339">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-339">Boolean</span></span>|<span data-ttu-id="4267e-340">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="4267e-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="4267e-341">keyboardBlockDictation</span></span>|<span data-ttu-id="4267e-342">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-342">Boolean</span></span>|<span data-ttu-id="4267e-343">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="4267e-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="4267e-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="4267e-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="4267e-345">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-345">Boolean</span></span>|<span data-ttu-id="4267e-346">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="4267e-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="4267e-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="4267e-348">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-348">Boolean</span></span>|<span data-ttu-id="4267e-349">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="4267e-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="4267e-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="4267e-351">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-351">Boolean</span></span>|<span data-ttu-id="4267e-352">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="4267e-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="4267e-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="4267e-354">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-354">Boolean</span></span>|<span data-ttu-id="4267e-355">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="4267e-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="4267e-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="4267e-357">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-357">Boolean</span></span>|<span data-ttu-id="4267e-358">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="4267e-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="4267e-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="4267e-360">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-360">Boolean</span></span>|<span data-ttu-id="4267e-361">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="4267e-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="4267e-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="4267e-363">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-363">Boolean</span></span>|<span data-ttu-id="4267e-364">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="4267e-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="4267e-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="4267e-366">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-366">Boolean</span></span>|<span data-ttu-id="4267e-367">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="4267e-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="4267e-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="4267e-369">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-369">Boolean</span></span>|<span data-ttu-id="4267e-370">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="4267e-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="4267e-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="4267e-372">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-372">Boolean</span></span>|<span data-ttu-id="4267e-373">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="4267e-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="4267e-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="4267e-375">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-375">Boolean</span></span>|<span data-ttu-id="4267e-376">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="4267e-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="4267e-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="4267e-378">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-378">Boolean</span></span>|<span data-ttu-id="4267e-379">指示在展台模式下是否允许访问语音过滤设置。</span><span class="sxs-lookup"><span data-stu-id="4267e-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="4267e-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="4267e-381">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-381">Boolean</span></span>|<span data-ttu-id="4267e-382">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="4267e-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="4267e-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="4267e-384">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-384">Boolean</span></span>|<span data-ttu-id="4267e-385">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="4267e-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4267e-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="4267e-387">字符串</span><span class="sxs-lookup"><span data-stu-id="4267e-387">String</span></span>|<span data-ttu-id="4267e-388">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="4267e-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="4267e-389">如果 KioskModeManagedAppId 未知，请使用。</span><span class="sxs-lookup"><span data-stu-id="4267e-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="4267e-390">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="4267e-390">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="4267e-391">字符串</span><span class="sxs-lookup"><span data-stu-id="4267e-391">String</span></span>|<span data-ttu-id="4267e-392">用于展台模式内置应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="4267e-392">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="4267e-393">未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="4267e-393">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="4267e-394">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="4267e-394">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="4267e-395">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-395">Boolean</span></span>|<span data-ttu-id="4267e-396">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="4267e-396">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-397">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="4267e-397">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="4267e-398">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-398">Boolean</span></span>|<span data-ttu-id="4267e-399">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="4267e-399">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-400">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="4267e-400">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="4267e-401">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-401">Boolean</span></span>|<span data-ttu-id="4267e-402">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="4267e-402">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-403">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="4267e-403">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="4267e-404">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-404">Boolean</span></span>|<span data-ttu-id="4267e-405">指示在展台模式下是否要求语音过滤。</span><span class="sxs-lookup"><span data-stu-id="4267e-405">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-406">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="4267e-406">kioskModeRequireZoom</span></span>|<span data-ttu-id="4267e-407">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-407">Boolean</span></span>|<span data-ttu-id="4267e-408">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="4267e-408">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="4267e-409">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="4267e-409">kioskModeManagedAppId</span></span>|<span data-ttu-id="4267e-410">字符串</span><span class="sxs-lookup"><span data-stu-id="4267e-410">String</span></span>|<span data-ttu-id="4267e-411">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="4267e-411">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="4267e-412">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="4267e-412">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="4267e-413">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="4267e-413">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="4267e-414">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-414">Boolean</span></span>|<span data-ttu-id="4267e-415">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="4267e-415">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="4267e-416">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="4267e-416">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="4267e-417">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-417">Boolean</span></span>|<span data-ttu-id="4267e-418">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="4267e-418">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="4267e-419">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="4267e-419">lockScreenBlockPassbook</span></span>|<span data-ttu-id="4267e-420">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-420">Boolean</span></span>|<span data-ttu-id="4267e-421">指示设备处于锁定状态时是否阻止用户使用 passbook。</span><span class="sxs-lookup"><span data-stu-id="4267e-421">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="4267e-422">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="4267e-422">lockScreenBlockTodayView</span></span>|<span data-ttu-id="4267e-423">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-423">Boolean</span></span>|<span data-ttu-id="4267e-424">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="4267e-424">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="4267e-425">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="4267e-425">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="4267e-426">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="4267e-426">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="4267e-427">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="4267e-427">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="4267e-428">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="4267e-428">mediaContentRatingCanada</span></span>|[<span data-ttu-id="4267e-429">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="4267e-429">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="4267e-430">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="4267e-430">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="4267e-431">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="4267e-431">mediaContentRatingFrance</span></span>|[<span data-ttu-id="4267e-432">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="4267e-432">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="4267e-433">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="4267e-433">Media content rating settings for France</span></span>|
|<span data-ttu-id="4267e-434">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="4267e-434">mediaContentRatingGermany</span></span>|[<span data-ttu-id="4267e-435">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="4267e-435">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="4267e-436">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="4267e-436">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="4267e-437">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="4267e-437">mediaContentRatingIreland</span></span>|[<span data-ttu-id="4267e-438">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="4267e-438">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="4267e-439">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="4267e-439">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="4267e-440">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="4267e-440">mediaContentRatingJapan</span></span>|[<span data-ttu-id="4267e-441">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="4267e-441">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="4267e-442">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="4267e-442">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="4267e-443">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="4267e-443">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="4267e-444">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="4267e-444">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="4267e-445">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="4267e-445">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="4267e-446">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="4267e-446">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="4267e-447">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="4267e-447">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="4267e-448">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="4267e-448">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="4267e-449">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="4267e-449">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="4267e-450">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="4267e-450">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="4267e-451">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="4267e-451">Media content rating settings for United States</span></span>|
|<span data-ttu-id="4267e-452">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="4267e-452">networkUsageRules</span></span>|<span data-ttu-id="4267e-453">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4267e-453">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="4267e-454">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="4267e-454">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="4267e-455">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="4267e-455">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="4267e-456">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="4267e-456">mediaContentRatingApps</span></span>|[<span data-ttu-id="4267e-457">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="4267e-457">ratingAppsType</span></span>](../resources/intune_deviceconfig_ratingappstype.md)|<span data-ttu-id="4267e-458">应用程序的媒体内容分级设置。</span><span class="sxs-lookup"><span data-stu-id="4267e-458">Media content rating settings for Canada</span></span> <span data-ttu-id="4267e-459">可能的值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="4267e-459">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="4267e-460">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-460">messagesBlocked</span></span>|<span data-ttu-id="4267e-461">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-461">Boolean</span></span>|<span data-ttu-id="4267e-462">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="4267e-462">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="4267e-463">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="4267e-463">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="4267e-464">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-464">Boolean</span></span>|<span data-ttu-id="4267e-465">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-465">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="4267e-466">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="4267e-466">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="4267e-467">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-467">Boolean</span></span>|<span data-ttu-id="4267e-468">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="4267e-468">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="4267e-469">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="4267e-469">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="4267e-470">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-470">Boolean</span></span>|<span data-ttu-id="4267e-471">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="4267e-471">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="4267e-472">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="4267e-472">passcodeBlockModification</span></span>|<span data-ttu-id="4267e-473">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-473">Boolean</span></span>|<span data-ttu-id="4267e-474">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-474">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="4267e-475">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4267e-475">passcodeBlockSimple</span></span>|<span data-ttu-id="4267e-476">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-476">Boolean</span></span>|<span data-ttu-id="4267e-477">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="4267e-477">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="4267e-478">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4267e-478">passcodeExpirationDays</span></span>|<span data-ttu-id="4267e-479">Int32</span><span class="sxs-lookup"><span data-stu-id="4267e-479">Int32</span></span>|<span data-ttu-id="4267e-480">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="4267e-480">Number of days before the passcode expires.</span></span> <span data-ttu-id="4267e-481">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="4267e-481">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="4267e-482">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4267e-482">passcodeMinimumLength</span></span>|<span data-ttu-id="4267e-483">Int32</span><span class="sxs-lookup"><span data-stu-id="4267e-483">Int32</span></span>|<span data-ttu-id="4267e-484">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="4267e-484">Minimum length of passcode.</span></span> <span data-ttu-id="4267e-485">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="4267e-485">Valid values 4 to 14</span></span>|
|<span data-ttu-id="4267e-486">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4267e-486">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4267e-487">Int32</span><span class="sxs-lookup"><span data-stu-id="4267e-487">Int32</span></span>|<span data-ttu-id="4267e-488">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="4267e-488">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="4267e-489">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4267e-489">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4267e-490">Int32</span><span class="sxs-lookup"><span data-stu-id="4267e-490">Int32</span></span>|<span data-ttu-id="4267e-491">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="4267e-491">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4267e-492">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4267e-492">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="4267e-493">Int32</span><span class="sxs-lookup"><span data-stu-id="4267e-493">Int32</span></span>|<span data-ttu-id="4267e-494">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="4267e-494">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="4267e-495">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="4267e-495">Valid values 0 to 4</span></span>|
|<span data-ttu-id="4267e-496">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="4267e-496">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="4267e-497">Int32</span><span class="sxs-lookup"><span data-stu-id="4267e-497">Int32</span></span>|<span data-ttu-id="4267e-498">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="4267e-498">Number of previous passcodes to block.</span></span> <span data-ttu-id="4267e-499">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="4267e-499">Valid values 1 to 24</span></span>|
|<span data-ttu-id="4267e-500">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="4267e-500">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="4267e-501">Int32</span><span class="sxs-lookup"><span data-stu-id="4267e-501">Int32</span></span>|<span data-ttu-id="4267e-502">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="4267e-502">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="4267e-503">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="4267e-503">Valid values 4 to 11</span></span>|
|<span data-ttu-id="4267e-504">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="4267e-504">passcodeRequiredType</span></span>|[<span data-ttu-id="4267e-505">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4267e-505">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="4267e-506">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="4267e-506">Type of passcode that is required.</span></span> <span data-ttu-id="4267e-507">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="4267e-507">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4267e-508">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="4267e-508">passcodeRequired</span></span>|<span data-ttu-id="4267e-509">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-509">Boolean</span></span>|<span data-ttu-id="4267e-510">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="4267e-510">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="4267e-511">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-511">podcastsBlocked</span></span>|<span data-ttu-id="4267e-512">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-512">Boolean</span></span>|<span data-ttu-id="4267e-513">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-513">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="4267e-514">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="4267e-514">safariBlockAutofill</span></span>|<span data-ttu-id="4267e-515">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-515">Boolean</span></span>|<span data-ttu-id="4267e-516">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="4267e-516">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="4267e-517">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="4267e-517">safariBlockJavaScript</span></span>|<span data-ttu-id="4267e-518">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-518">Boolean</span></span>|<span data-ttu-id="4267e-519">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="4267e-519">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="4267e-520">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="4267e-520">safariBlockPopups</span></span>|<span data-ttu-id="4267e-521">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-521">Boolean</span></span>|<span data-ttu-id="4267e-522">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="4267e-522">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="4267e-523">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-523">safariBlocked</span></span>|<span data-ttu-id="4267e-524">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-524">Boolean</span></span>|<span data-ttu-id="4267e-525">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="4267e-525">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="4267e-526">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="4267e-526">safariCookieSettings</span></span>|[<span data-ttu-id="4267e-527">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="4267e-527">webBrowserCookieSettings</span></span>](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|<span data-ttu-id="4267e-528">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="4267e-528">Cookie settings for Safari.</span></span> <span data-ttu-id="4267e-529">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="4267e-529">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="4267e-530">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="4267e-530">safariManagedDomains</span></span>|<span data-ttu-id="4267e-531">String 集合</span><span class="sxs-lookup"><span data-stu-id="4267e-531">String collection</span></span>|<span data-ttu-id="4267e-532">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="4267e-532">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="4267e-533">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="4267e-533">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="4267e-534">String 集合</span><span class="sxs-lookup"><span data-stu-id="4267e-534">String collection</span></span>|<span data-ttu-id="4267e-535">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="4267e-535">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="4267e-536">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-536">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="4267e-537">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="4267e-537">safariRequireFraudWarning</span></span>|<span data-ttu-id="4267e-538">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-538">Boolean</span></span>|<span data-ttu-id="4267e-539">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="4267e-539">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="4267e-540">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-540">screenCaptureBlocked</span></span>|<span data-ttu-id="4267e-541">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-541">Boolean</span></span>|<span data-ttu-id="4267e-542">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="4267e-542">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="4267e-543">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-543">siriBlocked</span></span>|<span data-ttu-id="4267e-544">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-544">Boolean</span></span>|<span data-ttu-id="4267e-545">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="4267e-545">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="4267e-546">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="4267e-546">siriBlockedWhenLocked</span></span>|<span data-ttu-id="4267e-547">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-547">Boolean</span></span>|<span data-ttu-id="4267e-548">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="4267e-548">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="4267e-549">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="4267e-549">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="4267e-550">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-550">Boolean</span></span>|<span data-ttu-id="4267e-551">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="4267e-551">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="4267e-552">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="4267e-552">siriRequireProfanityFilter</span></span>|<span data-ttu-id="4267e-553">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-553">Boolean</span></span>|<span data-ttu-id="4267e-554">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="4267e-554">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="4267e-555">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="4267e-555">spotlightBlockInternetResults</span></span>|<span data-ttu-id="4267e-556">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-556">Boolean</span></span>|<span data-ttu-id="4267e-557">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="4267e-557">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="4267e-558">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="4267e-558">voiceDialingBlocked</span></span>|<span data-ttu-id="4267e-559">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-559">Boolean</span></span>|<span data-ttu-id="4267e-560">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="4267e-560">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="4267e-561">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="4267e-561">wallpaperBlockModification</span></span>|<span data-ttu-id="4267e-562">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-562">Boolean</span></span>|<span data-ttu-id="4267e-563">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="4267e-563">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="4267e-564">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="4267e-564">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="4267e-565">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267e-565">Boolean</span></span>|<span data-ttu-id="4267e-566">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="4267e-566">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="4267e-567">响应</span><span class="sxs-lookup"><span data-stu-id="4267e-567">Response</span></span>
<span data-ttu-id="4267e-568">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4267e-568">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4267e-569">示例</span><span class="sxs-lookup"><span data-stu-id="4267e-569">Example</span></span>
### <a name="request"></a><span data-ttu-id="4267e-570">请求</span><span class="sxs-lookup"><span data-stu-id="4267e-570">Request</span></span>
<span data-ttu-id="4267e-571">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4267e-571">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 7905

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="4267e-572">响应</span><span class="sxs-lookup"><span data-stu-id="4267e-572">Response</span></span>
<span data-ttu-id="4267e-p127">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4267e-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








