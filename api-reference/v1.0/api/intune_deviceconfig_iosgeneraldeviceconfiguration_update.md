# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="b0a64-101">更新 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0a64-101">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="b0a64-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b0a64-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0a64-103">更新 [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b0a64-103">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0a64-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="b0a64-104">Prerequisites</span></span>
<span data-ttu-id="b0a64-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b0a64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b0a64-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0a64-107">Permission type</span></span>|<span data-ttu-id="b0a64-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b0a64-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0a64-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0a64-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b0a64-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0a64-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0a64-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0a64-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0a64-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0a64-112">Not supported.</span></span>|
|<span data-ttu-id="b0a64-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0a64-113">Application</span></span>|<span data-ttu-id="b0a64-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0a64-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0a64-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0a64-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b0a64-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0a64-116">Request headers</span></span>
|<span data-ttu-id="b0a64-117">标头</span><span class="sxs-lookup"><span data-stu-id="b0a64-117">Header</span></span>|<span data-ttu-id="b0a64-118">值</span><span class="sxs-lookup"><span data-stu-id="b0a64-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0a64-119">授权</span><span class="sxs-lookup"><span data-stu-id="b0a64-119">Authorization</span></span>|<span data-ttu-id="b0a64-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b0a64-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0a64-121">接受</span><span class="sxs-lookup"><span data-stu-id="b0a64-121">Accept</span></span>|<span data-ttu-id="b0a64-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b0a64-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0a64-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0a64-123">Request body</span></span>
<span data-ttu-id="b0a64-124">在请求正文中，提供 [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0a64-124">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="b0a64-125">下表显示创建 [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b0a64-125">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="b0a64-126">属性</span><span class="sxs-lookup"><span data-stu-id="b0a64-126">Property</span></span>|<span data-ttu-id="b0a64-127">类型</span><span class="sxs-lookup"><span data-stu-id="b0a64-127">Type</span></span>|<span data-ttu-id="b0a64-128">说明</span><span class="sxs-lookup"><span data-stu-id="b0a64-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0a64-129">id</span><span class="sxs-lookup"><span data-stu-id="b0a64-129">id</span></span>|<span data-ttu-id="b0a64-130">字符串</span><span class="sxs-lookup"><span data-stu-id="b0a64-130">String</span></span>|<span data-ttu-id="b0a64-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b0a64-131">Key of the entity.</span></span> <span data-ttu-id="b0a64-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0a64-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0a64-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0a64-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b0a64-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0a64-134">DateTimeOffset</span></span>|<span data-ttu-id="b0a64-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b0a64-135">DateTime the object was last modified.</span></span> <span data-ttu-id="b0a64-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0a64-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0a64-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0a64-137">createdDateTime</span></span>|<span data-ttu-id="b0a64-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0a64-138">DateTimeOffset</span></span>|<span data-ttu-id="b0a64-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b0a64-139">DateTime the object was created.</span></span> <span data-ttu-id="b0a64-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0a64-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0a64-141">description</span><span class="sxs-lookup"><span data-stu-id="b0a64-141">description</span></span>|<span data-ttu-id="b0a64-142">String</span><span class="sxs-lookup"><span data-stu-id="b0a64-142">String</span></span>|<span data-ttu-id="b0a64-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b0a64-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b0a64-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0a64-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0a64-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b0a64-145">displayName</span></span>|<span data-ttu-id="b0a64-146">String</span><span class="sxs-lookup"><span data-stu-id="b0a64-146">String</span></span>|<span data-ttu-id="b0a64-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b0a64-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b0a64-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0a64-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0a64-149">version</span><span class="sxs-lookup"><span data-stu-id="b0a64-149">version</span></span>|<span data-ttu-id="b0a64-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a64-150">Int32</span></span>|<span data-ttu-id="b0a64-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b0a64-151">Version of the device configuration.</span></span> <span data-ttu-id="b0a64-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0a64-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0a64-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="b0a64-153">accountBlockModification</span></span>|<span data-ttu-id="b0a64-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-154">Boolean</span></span>|<span data-ttu-id="b0a64-155">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="b0a64-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0a64-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="b0a64-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="b0a64-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-157">Boolean</span></span>|<span data-ttu-id="b0a64-158">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="b0a64-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="b0a64-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-159">airDropBlocked</span></span>|<span data-ttu-id="b0a64-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-160">Boolean</span></span>|<span data-ttu-id="b0a64-161">指示设备处于监督模式时是否允许使用 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="b0a64-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0a64-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="b0a64-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="b0a64-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-163">Boolean</span></span>|<span data-ttu-id="b0a64-164">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0a64-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="b0a64-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="b0a64-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-166">Boolean</span></span>|<span data-ttu-id="b0a64-167">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="b0a64-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="b0a64-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="b0a64-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="b0a64-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-169">Boolean</span></span>|<span data-ttu-id="b0a64-170">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0a64-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="b0a64-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="b0a64-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-172">Boolean</span></span>|<span data-ttu-id="b0a64-173">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="b0a64-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-174">appleNewsBlocked</span></span>|<span data-ttu-id="b0a64-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-175">Boolean</span></span>|<span data-ttu-id="b0a64-176">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0a64-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="b0a64-177">appsSingleAppModeList</span></span>|<span data-ttu-id="b0a64-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b0a64-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="b0a64-179">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="b0a64-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="b0a64-180">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="b0a64-180">Supervised only.</span></span> <span data-ttu-id="b0a64-181">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="b0a64-181">iOS 7.0 and later.</span></span> <span data-ttu-id="b0a64-182">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="b0a64-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b0a64-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="b0a64-183">appsVisibilityList</span></span>|<span data-ttu-id="b0a64-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b0a64-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="b0a64-185">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="b0a64-186">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b0a64-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b0a64-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="b0a64-187">appsVisibilityListType</span></span>|[<span data-ttu-id="b0a64-188">appListType</span><span class="sxs-lookup"><span data-stu-id="b0a64-188">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="b0a64-189">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="b0a64-189">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="b0a64-190">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="b0a64-190">The possible values are `none`, `appsInListCompliant`, `appsNotInListCompliant`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="b0a64-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="b0a64-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="b0a64-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-192">Boolean</span></span>|<span data-ttu-id="b0a64-193">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0a64-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-194">appStoreBlocked</span></span>|<span data-ttu-id="b0a64-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-195">Boolean</span></span>|<span data-ttu-id="b0a64-196">指示是否阻止用户使用应用商店。</span><span class="sxs-lookup"><span data-stu-id="b0a64-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="b0a64-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="b0a64-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="b0a64-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-198">Boolean</span></span>|<span data-ttu-id="b0a64-199">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="b0a64-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="b0a64-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b0a64-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="b0a64-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-201">Boolean</span></span>|<span data-ttu-id="b0a64-202">指示是否阻止应用商店应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="b0a64-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="b0a64-203">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0a64-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="b0a64-204">appStoreRequirePassword</span></span>|<span data-ttu-id="b0a64-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-205">Boolean</span></span>|<span data-ttu-id="b0a64-206">指示使用应用商店时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="b0a64-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="b0a64-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="b0a64-207">bluetoothBlockModification</span></span>|<span data-ttu-id="b0a64-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-208">Boolean</span></span>|<span data-ttu-id="b0a64-209">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="b0a64-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-210">cameraBlocked</span></span>|<span data-ttu-id="b0a64-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-211">Boolean</span></span>|<span data-ttu-id="b0a64-212">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="b0a64-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="b0a64-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="b0a64-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="b0a64-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-214">Boolean</span></span>|<span data-ttu-id="b0a64-215">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="b0a64-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="b0a64-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="b0a64-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="b0a64-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-217">Boolean</span></span>|<span data-ttu-id="b0a64-218">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="b0a64-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="b0a64-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="b0a64-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="b0a64-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-220">Boolean</span></span>|<span data-ttu-id="b0a64-221">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="b0a64-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0a64-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="b0a64-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="b0a64-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-223">Boolean</span></span>|<span data-ttu-id="b0a64-224">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="b0a64-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="b0a64-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="b0a64-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="b0a64-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-226">Boolean</span></span>|<span data-ttu-id="b0a64-227">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="b0a64-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="b0a64-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="b0a64-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="b0a64-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-229">Boolean</span></span>|<span data-ttu-id="b0a64-230">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="b0a64-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="b0a64-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="b0a64-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="b0a64-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-232">Boolean</span></span>|<span data-ttu-id="b0a64-233">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b0a64-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="b0a64-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="b0a64-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-235">Boolean</span></span>|<span data-ttu-id="b0a64-236">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="b0a64-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0a64-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="b0a64-237">compliantAppsList</span></span>|<span data-ttu-id="b0a64-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b0a64-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="b0a64-239">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="b0a64-240">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b0a64-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b0a64-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="b0a64-241">compliantAppListType</span></span>|[<span data-ttu-id="b0a64-242">appListType</span><span class="sxs-lookup"><span data-stu-id="b0a64-242">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="b0a64-243">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="b0a64-243">List that is in the AppComplianceList.</span></span> <span data-ttu-id="b0a64-244">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="b0a64-244">The possible values are `none`, `appsInListCompliant`, `appsNotInListCompliant`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="b0a64-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="b0a64-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="b0a64-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-246">Boolean</span></span>|<span data-ttu-id="b0a64-247">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="b0a64-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0a64-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-248">definitionLookupBlocked</span></span>|<span data-ttu-id="b0a64-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-249">Boolean</span></span>|<span data-ttu-id="b0a64-250">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="b0a64-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="b0a64-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="b0a64-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-252">Boolean</span></span>|<span data-ttu-id="b0a64-253">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="b0a64-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0a64-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="b0a64-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="b0a64-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-255">Boolean</span></span>|<span data-ttu-id="b0a64-256">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="b0a64-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0a64-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="b0a64-257">deviceBlockNameModification</span></span>|<span data-ttu-id="b0a64-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-258">Boolean</span></span>|<span data-ttu-id="b0a64-259">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0a64-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="b0a64-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="b0a64-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-261">Boolean</span></span>|<span data-ttu-id="b0a64-262">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="b0a64-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="b0a64-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="b0a64-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="b0a64-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-264">Boolean</span></span>|<span data-ttu-id="b0a64-265">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="b0a64-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="b0a64-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="b0a64-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-267">Boolean</span></span>|<span data-ttu-id="b0a64-268">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="b0a64-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="b0a64-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="b0a64-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="b0a64-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-270">Boolean</span></span>|<span data-ttu-id="b0a64-271">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="b0a64-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="b0a64-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="b0a64-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="b0a64-273">String 集合</span><span class="sxs-lookup"><span data-stu-id="b0a64-273">String collection</span></span>|<span data-ttu-id="b0a64-274">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="b0a64-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="b0a64-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="b0a64-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="b0a64-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-276">Boolean</span></span>|<span data-ttu-id="b0a64-277">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="b0a64-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="b0a64-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="b0a64-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="b0a64-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-279">Boolean</span></span>|<span data-ttu-id="b0a64-280">指示是否阻止用户修改企业应用信任设置。</span><span class="sxs-lookup"><span data-stu-id="b0a64-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="b0a64-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-281">faceTimeBlocked</span></span>|<span data-ttu-id="b0a64-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-282">Boolean</span></span>|<span data-ttu-id="b0a64-283">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="b0a64-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="b0a64-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="b0a64-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-285">Boolean</span></span>|<span data-ttu-id="b0a64-286">指示设备处于监督模式时是否阻止查找我的好友。</span><span class="sxs-lookup"><span data-stu-id="b0a64-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0a64-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="b0a64-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="b0a64-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-288">Boolean</span></span>|<span data-ttu-id="b0a64-289">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="b0a64-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="b0a64-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="b0a64-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="b0a64-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-291">Boolean</span></span>|<span data-ttu-id="b0a64-292">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="b0a64-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="b0a64-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-293">gameCenterBlocked</span></span>|<span data-ttu-id="b0a64-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-294">Boolean</span></span>|<span data-ttu-id="b0a64-295">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="b0a64-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0a64-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-296">hostPairingBlocked</span></span>|<span data-ttu-id="b0a64-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-297">Boolean</span></span>|<span data-ttu-id="b0a64-298">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="b0a64-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="b0a64-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="b0a64-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-300">Boolean</span></span>|<span data-ttu-id="b0a64-301">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="b0a64-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0a64-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="b0a64-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="b0a64-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-303">Boolean</span></span>|<span data-ttu-id="b0a64-304">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="b0a64-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="b0a64-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="b0a64-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="b0a64-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-306">Boolean</span></span>|<span data-ttu-id="b0a64-307">指示是否阻止用户在另一个 iOS 或 MacOS 设备上继续从事在 iOS 设备上启动的工作。</span><span class="sxs-lookup"><span data-stu-id="b0a64-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="b0a64-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="b0a64-308">iCloudBlockBackup</span></span>|<span data-ttu-id="b0a64-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-309">Boolean</span></span>|<span data-ttu-id="b0a64-310">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="b0a64-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="b0a64-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="b0a64-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="b0a64-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-312">Boolean</span></span>|<span data-ttu-id="b0a64-313">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="b0a64-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="b0a64-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="b0a64-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="b0a64-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-315">Boolean</span></span>|<span data-ttu-id="b0a64-316">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="b0a64-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="b0a64-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="b0a64-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="b0a64-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-318">Boolean</span></span>|<span data-ttu-id="b0a64-319">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="b0a64-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="b0a64-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="b0a64-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="b0a64-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-321">Boolean</span></span>|<span data-ttu-id="b0a64-322">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="b0a64-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="b0a64-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="b0a64-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="b0a64-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-324">Boolean</span></span>|<span data-ttu-id="b0a64-325">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="b0a64-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="b0a64-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="b0a64-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="b0a64-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-327">Boolean</span></span>|<span data-ttu-id="b0a64-328">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="b0a64-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="b0a64-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="b0a64-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="b0a64-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-330">Boolean</span></span>|<span data-ttu-id="b0a64-331">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="b0a64-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="b0a64-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="b0a64-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="b0a64-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-333">Boolean</span></span>|<span data-ttu-id="b0a64-334">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="b0a64-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="b0a64-335">iTunesBlockRadio</span></span>|<span data-ttu-id="b0a64-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-336">Boolean</span></span>|<span data-ttu-id="b0a64-337">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b0a64-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="b0a64-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="b0a64-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-339">Boolean</span></span>|<span data-ttu-id="b0a64-340">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b0a64-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="b0a64-341">keyboardBlockDictation</span></span>|<span data-ttu-id="b0a64-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-342">Boolean</span></span>|<span data-ttu-id="b0a64-343">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="b0a64-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0a64-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="b0a64-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="b0a64-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-345">Boolean</span></span>|<span data-ttu-id="b0a64-346">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b0a64-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="b0a64-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="b0a64-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-348">Boolean</span></span>|<span data-ttu-id="b0a64-349">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0a64-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="b0a64-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="b0a64-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-351">Boolean</span></span>|<span data-ttu-id="b0a64-352">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b0a64-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="b0a64-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="b0a64-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-354">Boolean</span></span>|<span data-ttu-id="b0a64-355">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="b0a64-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="b0a64-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="b0a64-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-357">Boolean</span></span>|<span data-ttu-id="b0a64-358">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="b0a64-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="b0a64-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="b0a64-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-360">Boolean</span></span>|<span data-ttu-id="b0a64-361">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="b0a64-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="b0a64-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="b0a64-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-363">Boolean</span></span>|<span data-ttu-id="b0a64-364">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="b0a64-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="b0a64-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="b0a64-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-366">Boolean</span></span>|<span data-ttu-id="b0a64-367">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="b0a64-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="b0a64-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="b0a64-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-369">Boolean</span></span>|<span data-ttu-id="b0a64-370">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="b0a64-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="b0a64-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="b0a64-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-372">Boolean</span></span>|<span data-ttu-id="b0a64-373">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="b0a64-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="b0a64-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="b0a64-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-375">Boolean</span></span>|<span data-ttu-id="b0a64-376">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="b0a64-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="b0a64-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="b0a64-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-378">Boolean</span></span>|<span data-ttu-id="b0a64-379">指示在展台模式下是否允许访问语音过滤设置。</span><span class="sxs-lookup"><span data-stu-id="b0a64-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="b0a64-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="b0a64-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-381">Boolean</span></span>|<span data-ttu-id="b0a64-382">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="b0a64-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="b0a64-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="b0a64-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-384">Boolean</span></span>|<span data-ttu-id="b0a64-385">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="b0a64-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b0a64-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="b0a64-387">String</span><span class="sxs-lookup"><span data-stu-id="b0a64-387">String</span></span>|<span data-ttu-id="b0a64-388">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="b0a64-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="b0a64-389">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="b0a64-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="b0a64-390">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="b0a64-390">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="b0a64-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-391">Boolean</span></span>|<span data-ttu-id="b0a64-392">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="b0a64-392">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-393">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="b0a64-393">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="b0a64-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-394">Boolean</span></span>|<span data-ttu-id="b0a64-395">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="b0a64-395">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-396">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="b0a64-396">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="b0a64-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-397">Boolean</span></span>|<span data-ttu-id="b0a64-398">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="b0a64-398">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-399">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="b0a64-399">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="b0a64-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-400">Boolean</span></span>|<span data-ttu-id="b0a64-401">指示在展台模式下是否要求语音过滤。</span><span class="sxs-lookup"><span data-stu-id="b0a64-401">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-402">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="b0a64-402">kioskModeRequireZoom</span></span>|<span data-ttu-id="b0a64-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-403">Boolean</span></span>|<span data-ttu-id="b0a64-404">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="b0a64-404">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="b0a64-405">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="b0a64-405">kioskModeManagedAppId</span></span>|<span data-ttu-id="b0a64-406">String</span><span class="sxs-lookup"><span data-stu-id="b0a64-406">String</span></span>|<span data-ttu-id="b0a64-407">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="b0a64-407">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="b0a64-408">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="b0a64-408">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="b0a64-409">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="b0a64-409">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="b0a64-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-410">Boolean</span></span>|<span data-ttu-id="b0a64-411">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="b0a64-411">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="b0a64-412">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="b0a64-412">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="b0a64-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-413">Boolean</span></span>|<span data-ttu-id="b0a64-414">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="b0a64-414">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="b0a64-415">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="b0a64-415">lockScreenBlockPassbook</span></span>|<span data-ttu-id="b0a64-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-416">Boolean</span></span>|<span data-ttu-id="b0a64-417">指示设备处于锁定状态时是否阻止用户使用 passbook。</span><span class="sxs-lookup"><span data-stu-id="b0a64-417">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="b0a64-418">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="b0a64-418">lockScreenBlockTodayView</span></span>|<span data-ttu-id="b0a64-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-419">Boolean</span></span>|<span data-ttu-id="b0a64-420">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="b0a64-420">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="b0a64-421">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b0a64-421">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="b0a64-422">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b0a64-422">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="b0a64-423">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b0a64-423">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="b0a64-424">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b0a64-424">mediaContentRatingCanada</span></span>|[<span data-ttu-id="b0a64-425">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b0a64-425">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="b0a64-426">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b0a64-426">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="b0a64-427">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="b0a64-427">mediaContentRatingFrance</span></span>|[<span data-ttu-id="b0a64-428">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="b0a64-428">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="b0a64-429">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b0a64-429">Media content rating settings for France</span></span>|
|<span data-ttu-id="b0a64-430">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="b0a64-430">mediaContentRatingGermany</span></span>|[<span data-ttu-id="b0a64-431">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="b0a64-431">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="b0a64-432">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b0a64-432">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="b0a64-433">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b0a64-433">mediaContentRatingIreland</span></span>|[<span data-ttu-id="b0a64-434">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b0a64-434">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="b0a64-435">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b0a64-435">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="b0a64-436">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="b0a64-436">mediaContentRatingJapan</span></span>|[<span data-ttu-id="b0a64-437">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="b0a64-437">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="b0a64-438">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b0a64-438">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="b0a64-439">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="b0a64-439">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="b0a64-440">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="b0a64-440">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="b0a64-441">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b0a64-441">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="b0a64-442">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="b0a64-442">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="b0a64-443">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="b0a64-443">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="b0a64-444">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b0a64-444">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="b0a64-445">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="b0a64-445">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="b0a64-446">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="b0a64-446">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="b0a64-447">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b0a64-447">Media content rating settings for United States</span></span>|
|<span data-ttu-id="b0a64-448">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="b0a64-448">networkUsageRules</span></span>|<span data-ttu-id="b0a64-449">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b0a64-449">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="b0a64-450">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="b0a64-450">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="b0a64-451">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b0a64-451">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="b0a64-452">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="b0a64-452">mediaContentRatingApps</span></span>|[<span data-ttu-id="b0a64-453">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="b0a64-453">ratingAppsType</span></span>](../resources/intune_deviceconfig_ratingappstype.md)|<span data-ttu-id="b0a64-454">媒体内容应用程序的分级设置。</span><span class="sxs-lookup"><span data-stu-id="b0a64-454">Media content rating settings for Germany</span></span> <span data-ttu-id="b0a64-455">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="b0a64-455">The possible values are `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`, , , , , , or .</span></span>|
|<span data-ttu-id="b0a64-456">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-456">messagesBlocked</span></span>|<span data-ttu-id="b0a64-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-457">Boolean</span></span>|<span data-ttu-id="b0a64-458">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="b0a64-458">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="b0a64-459">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="b0a64-459">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="b0a64-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-460">Boolean</span></span>|<span data-ttu-id="b0a64-461">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-461">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b0a64-462">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="b0a64-462">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="b0a64-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-463">Boolean</span></span>|<span data-ttu-id="b0a64-464">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="b0a64-464">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="b0a64-465">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="b0a64-465">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="b0a64-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-466">Boolean</span></span>|<span data-ttu-id="b0a64-467">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="b0a64-467">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="b0a64-468">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="b0a64-468">passcodeBlockModification</span></span>|<span data-ttu-id="b0a64-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-469">Boolean</span></span>|<span data-ttu-id="b0a64-470">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-470">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0a64-471">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b0a64-471">passcodeBlockSimple</span></span>|<span data-ttu-id="b0a64-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-472">Boolean</span></span>|<span data-ttu-id="b0a64-473">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="b0a64-473">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="b0a64-474">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b0a64-474">passcodeExpirationDays</span></span>|<span data-ttu-id="b0a64-475">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a64-475">Int32</span></span>|<span data-ttu-id="b0a64-476">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="b0a64-476">Number of days before the passcode expires.</span></span> <span data-ttu-id="b0a64-477">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="b0a64-477">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b0a64-478">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b0a64-478">passcodeMinimumLength</span></span>|<span data-ttu-id="b0a64-479">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a64-479">Int32</span></span>|<span data-ttu-id="b0a64-480">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="b0a64-480">Minimum length of passcode.</span></span> <span data-ttu-id="b0a64-481">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="b0a64-481">Valid values 4 to 14</span></span>|
|<span data-ttu-id="b0a64-482">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b0a64-482">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b0a64-483">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a64-483">Int32</span></span>|<span data-ttu-id="b0a64-484">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="b0a64-484">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="b0a64-485">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b0a64-485">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b0a64-486">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a64-486">Int32</span></span>|<span data-ttu-id="b0a64-487">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="b0a64-487">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b0a64-488">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b0a64-488">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="b0a64-489">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a64-489">Int32</span></span>|<span data-ttu-id="b0a64-490">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="b0a64-490">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="b0a64-491">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="b0a64-491">Valid values 0 to 4</span></span>|
|<span data-ttu-id="b0a64-492">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="b0a64-492">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="b0a64-493">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a64-493">Int32</span></span>|<span data-ttu-id="b0a64-494">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="b0a64-494">Number of previous passcodes to block.</span></span> <span data-ttu-id="b0a64-495">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="b0a64-495">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b0a64-496">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="b0a64-496">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="b0a64-497">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a64-497">Int32</span></span>|<span data-ttu-id="b0a64-498">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="b0a64-498">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="b0a64-499">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="b0a64-499">Valid values 4 to 11</span></span>|
|<span data-ttu-id="b0a64-500">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="b0a64-500">passcodeRequiredType</span></span>|[<span data-ttu-id="b0a64-501">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b0a64-501">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="b0a64-502">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="b0a64-502">Type of passcode that is required.</span></span> <span data-ttu-id="b0a64-503">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="b0a64-503">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="b0a64-504">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="b0a64-504">passcodeRequired</span></span>|<span data-ttu-id="b0a64-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-505">Boolean</span></span>|<span data-ttu-id="b0a64-506">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="b0a64-506">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="b0a64-507">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-507">podcastsBlocked</span></span>|<span data-ttu-id="b0a64-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-508">Boolean</span></span>|<span data-ttu-id="b0a64-509">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-509">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="b0a64-510">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b0a64-510">safariBlockAutofill</span></span>|<span data-ttu-id="b0a64-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-511">Boolean</span></span>|<span data-ttu-id="b0a64-512">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="b0a64-512">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="b0a64-513">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="b0a64-513">safariBlockJavaScript</span></span>|<span data-ttu-id="b0a64-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-514">Boolean</span></span>|<span data-ttu-id="b0a64-515">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="b0a64-515">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="b0a64-516">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="b0a64-516">safariBlockPopups</span></span>|<span data-ttu-id="b0a64-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-517">Boolean</span></span>|<span data-ttu-id="b0a64-518">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="b0a64-518">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="b0a64-519">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-519">safariBlocked</span></span>|<span data-ttu-id="b0a64-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-520">Boolean</span></span>|<span data-ttu-id="b0a64-521">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="b0a64-521">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="b0a64-522">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="b0a64-522">safariCookieSettings</span></span>|[<span data-ttu-id="b0a64-523">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="b0a64-523">webBrowserCookieSettings</span></span>](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|<span data-ttu-id="b0a64-524">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="b0a64-524">Cookie settings for Safari.</span></span> <span data-ttu-id="b0a64-525">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="b0a64-525">The possible values are `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`, , , , , , , or .</span></span>|
|<span data-ttu-id="b0a64-526">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="b0a64-526">safariManagedDomains</span></span>|<span data-ttu-id="b0a64-527">String 集合</span><span class="sxs-lookup"><span data-stu-id="b0a64-527">String collection</span></span>|<span data-ttu-id="b0a64-528">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="b0a64-528">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="b0a64-529">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="b0a64-529">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="b0a64-530">String 集合</span><span class="sxs-lookup"><span data-stu-id="b0a64-530">String collection</span></span>|<span data-ttu-id="b0a64-531">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="b0a64-531">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="b0a64-532">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-532">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b0a64-533">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="b0a64-533">safariRequireFraudWarning</span></span>|<span data-ttu-id="b0a64-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-534">Boolean</span></span>|<span data-ttu-id="b0a64-535">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="b0a64-535">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="b0a64-536">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-536">screenCaptureBlocked</span></span>|<span data-ttu-id="b0a64-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-537">Boolean</span></span>|<span data-ttu-id="b0a64-538">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="b0a64-538">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="b0a64-539">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-539">siriBlocked</span></span>|<span data-ttu-id="b0a64-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-540">Boolean</span></span>|<span data-ttu-id="b0a64-541">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="b0a64-541">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="b0a64-542">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-542">siriBlockedWhenLocked</span></span>|<span data-ttu-id="b0a64-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-543">Boolean</span></span>|<span data-ttu-id="b0a64-544">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="b0a64-544">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="b0a64-545">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="b0a64-545">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="b0a64-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-546">Boolean</span></span>|<span data-ttu-id="b0a64-547">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="b0a64-547">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="b0a64-548">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="b0a64-548">siriRequireProfanityFilter</span></span>|<span data-ttu-id="b0a64-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-549">Boolean</span></span>|<span data-ttu-id="b0a64-550">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="b0a64-550">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="b0a64-551">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="b0a64-551">spotlightBlockInternetResults</span></span>|<span data-ttu-id="b0a64-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-552">Boolean</span></span>|<span data-ttu-id="b0a64-553">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="b0a64-553">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="b0a64-554">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="b0a64-554">voiceDialingBlocked</span></span>|<span data-ttu-id="b0a64-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-555">Boolean</span></span>|<span data-ttu-id="b0a64-556">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="b0a64-556">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="b0a64-557">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="b0a64-557">wallpaperBlockModification</span></span>|<span data-ttu-id="b0a64-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-558">Boolean</span></span>|<span data-ttu-id="b0a64-559">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b0a64-559">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="b0a64-560">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="b0a64-560">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="b0a64-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a64-561">Boolean</span></span>|<span data-ttu-id="b0a64-562">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="b0a64-562">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="b0a64-563">响应</span><span class="sxs-lookup"><span data-stu-id="b0a64-563">Response</span></span>
<span data-ttu-id="b0a64-564">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b0a64-564">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0a64-565">示例</span><span class="sxs-lookup"><span data-stu-id="b0a64-565">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0a64-566">请求</span><span class="sxs-lookup"><span data-stu-id="b0a64-566">Request</span></span>
<span data-ttu-id="b0a64-567">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0a64-567">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 7773

{
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

### <a name="response"></a><span data-ttu-id="b0a64-568">响应</span><span class="sxs-lookup"><span data-stu-id="b0a64-568">Response</span></span>
<span data-ttu-id="b0a64-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b0a64-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7949

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



