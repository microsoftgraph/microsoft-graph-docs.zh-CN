# <a name="update-defaultmanagedappprotection"></a><span data-ttu-id="d394f-101">更新 defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="d394f-101">Update defaultManagedAppProtection</span></span>

> <span data-ttu-id="d394f-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d394f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d394f-103">更新 [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d394f-103">Update the properties of a [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d394f-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="d394f-104">Prerequisites</span></span>
<span data-ttu-id="d394f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d394f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d394f-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="d394f-107">Permission type</span></span>|<span data-ttu-id="d394f-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d394f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d394f-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d394f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d394f-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d394f-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d394f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d394f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d394f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="d394f-112">Not supported.</span></span>|
|<span data-ttu-id="d394f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="d394f-113">Application</span></span>|<span data-ttu-id="d394f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d394f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d394f-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d394f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="d394f-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="d394f-116">Request headers</span></span>
|<span data-ttu-id="d394f-117">标头</span><span class="sxs-lookup"><span data-stu-id="d394f-117">Header</span></span>|<span data-ttu-id="d394f-118">值</span><span class="sxs-lookup"><span data-stu-id="d394f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d394f-119">授权</span><span class="sxs-lookup"><span data-stu-id="d394f-119">Authorization</span></span>|<span data-ttu-id="d394f-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d394f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d394f-121">接受</span><span class="sxs-lookup"><span data-stu-id="d394f-121">Accept</span></span>|<span data-ttu-id="d394f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d394f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d394f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d394f-123">Request body</span></span>
<span data-ttu-id="d394f-124">在请求正文中，提供 [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d394f-124">In the request body, supply a JSON representation for the [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) object.</span></span>

<span data-ttu-id="d394f-125">下表显示创建 [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d394f-125">The following table shows the properties that are required when you create the [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md).</span></span>

|<span data-ttu-id="d394f-126">属性</span><span class="sxs-lookup"><span data-stu-id="d394f-126">Property</span></span>|<span data-ttu-id="d394f-127">类型</span><span class="sxs-lookup"><span data-stu-id="d394f-127">Type</span></span>|<span data-ttu-id="d394f-128">说明</span><span class="sxs-lookup"><span data-stu-id="d394f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d394f-129">displayName</span><span class="sxs-lookup"><span data-stu-id="d394f-129">displayName</span></span>|<span data-ttu-id="d394f-130">字符串</span><span class="sxs-lookup"><span data-stu-id="d394f-130">String</span></span>|<span data-ttu-id="d394f-131">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="d394f-131">Policy display name.</span></span> <span data-ttu-id="d394f-132">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d394f-133">说明</span><span class="sxs-lookup"><span data-stu-id="d394f-133">description</span></span>|<span data-ttu-id="d394f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d394f-134">String</span></span>|<span data-ttu-id="d394f-135">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="d394f-135">The policy's description.</span></span> <span data-ttu-id="d394f-136">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d394f-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d394f-137">createdDateTime</span></span>|<span data-ttu-id="d394f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d394f-138">DateTimeOffset</span></span>|<span data-ttu-id="d394f-139">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d394f-139">The date and time the policy was created.</span></span> <span data-ttu-id="d394f-140">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d394f-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d394f-141">lastModifiedDateTime</span></span>|<span data-ttu-id="d394f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d394f-142">DateTimeOffset</span></span>|<span data-ttu-id="d394f-143">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="d394f-143">Last time the policy was modified.</span></span> <span data-ttu-id="d394f-144">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d394f-145">ID</span><span class="sxs-lookup"><span data-stu-id="d394f-145">id</span></span>|<span data-ttu-id="d394f-146">字符串</span><span class="sxs-lookup"><span data-stu-id="d394f-146">String</span></span>|<span data-ttu-id="d394f-147">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d394f-147">Key of the entity.</span></span> <span data-ttu-id="d394f-148">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d394f-149">版本</span><span class="sxs-lookup"><span data-stu-id="d394f-149">version</span></span>|<span data-ttu-id="d394f-150">字符串</span><span class="sxs-lookup"><span data-stu-id="d394f-150">String</span></span>|<span data-ttu-id="d394f-151">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="d394f-151">Version of the entity.</span></span> <span data-ttu-id="d394f-152">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="d394f-153">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="d394f-153">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="d394f-154">持续时间</span><span class="sxs-lookup"><span data-stu-id="d394f-154">Duration</span></span>|<span data-ttu-id="d394f-155">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="d394f-155">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="d394f-156">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-156">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-157">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="d394f-157">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="d394f-158">持续时间</span><span class="sxs-lookup"><span data-stu-id="d394f-158">Duration</span></span>|<span data-ttu-id="d394f-159">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="d394f-159">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="d394f-160">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-160">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-161">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="d394f-161">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="d394f-162">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="d394f-162">managedAppDataTransferLevel</span></span>](../resources/intune_mam_managedappdatatransferlevel.md)|<span data-ttu-id="d394f-p110">允许传输数据的来源。继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="d394f-p110">Sources from which data is allowed to be transferred. Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md). The possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="d394f-166">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="d394f-166">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="d394f-167">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="d394f-167">managedAppDataTransferLevel</span></span>](../resources/intune_mam_managedappdatatransferlevel.md)|<span data-ttu-id="d394f-p111">允许传输数据的目标。继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="d394f-p111">Destinations to which data is allowed to be transferred. Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md). The possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="d394f-171">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="d394f-171">organizationalCredentialsRequired</span></span>|<span data-ttu-id="d394f-172">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-172">Boolean</span></span>|<span data-ttu-id="d394f-173">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="d394f-173">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="d394f-174">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-174">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-175">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="d394f-175">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="d394f-176">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="d394f-176">managedAppClipboardSharingLevel</span></span>](../resources/intune_mam_managedappclipboardsharinglevel.md)|<span data-ttu-id="d394f-p113">托管设备上的应用程序之间可以共享剪贴板的级别。继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="d394f-p113">The level to which the clipboard may be shared between apps on the managed device. Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md). The possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="d394f-180">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="d394f-180">dataBackupBlocked</span></span>|<span data-ttu-id="d394f-181">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-181">Boolean</span></span>|<span data-ttu-id="d394f-182">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="d394f-182">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="d394f-183">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-183">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-184">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="d394f-184">deviceComplianceRequired</span></span>|<span data-ttu-id="d394f-185">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-185">Boolean</span></span>|<span data-ttu-id="d394f-186">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="d394f-186">Indicates whether device compliance is required.</span></span> <span data-ttu-id="d394f-187">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-187">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-188">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="d394f-188">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="d394f-189">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-189">Boolean</span></span>|<span data-ttu-id="d394f-190">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="d394f-190">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="d394f-191">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-191">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-192">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="d394f-192">saveAsBlocked</span></span>|<span data-ttu-id="d394f-193">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-193">Boolean</span></span>|<span data-ttu-id="d394f-194">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="d394f-194">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="d394f-195">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-195">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-196">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="d394f-196">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="d394f-197">持续时间</span><span class="sxs-lookup"><span data-stu-id="d394f-197">Duration</span></span>|<span data-ttu-id="d394f-198">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="d394f-198">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="d394f-199">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-199">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-200">pinRequired</span><span class="sxs-lookup"><span data-stu-id="d394f-200">pinRequired</span></span>|<span data-ttu-id="d394f-201">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-201">Boolean</span></span>|<span data-ttu-id="d394f-202">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="d394f-202">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="d394f-203">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-203">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-204">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="d394f-204">maximumPinRetries</span></span>|<span data-ttu-id="d394f-205">Int32</span><span class="sxs-lookup"><span data-stu-id="d394f-205">Int32</span></span>|<span data-ttu-id="d394f-206">在阻止或擦除托管应用程序之前，不正确 PIN 重试的最大尝试次数。</span><span class="sxs-lookup"><span data-stu-id="d394f-206">Maximum number of incorrect pin retry attempts before the managed app is wiped.</span></span> <span data-ttu-id="d394f-207">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-207">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-208">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="d394f-208">simplePinBlocked</span></span>|<span data-ttu-id="d394f-209">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-209">Boolean</span></span>|<span data-ttu-id="d394f-210">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="d394f-210">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="d394f-211">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-211">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-212">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="d394f-212">minimumPinLength</span></span>|<span data-ttu-id="d394f-213">Int32</span><span class="sxs-lookup"><span data-stu-id="d394f-213">Int32</span></span>|<span data-ttu-id="d394f-214">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-214">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-215">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="d394f-215">pinCharacterSet</span></span>|[<span data-ttu-id="d394f-216">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="d394f-216">managedAppPinCharacterSet</span></span>](../resources/intune_mam_managedapppincharacterset.md)|<span data-ttu-id="d394f-p122">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="d394f-p122">Character set which may be used for an app-level pin if PinRequired is set to True. Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md). The possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="d394f-220">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="d394f-220">periodBeforePinReset</span></span>|<span data-ttu-id="d394f-221">持续时间</span><span class="sxs-lookup"><span data-stu-id="d394f-221">Duration</span></span>|<span data-ttu-id="d394f-222">PinRequired 设置为 True 时，在此时间段之后必须重置所有级别的 PIN。</span><span class="sxs-lookup"><span data-stu-id="d394f-222">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="d394f-223">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-223">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-224">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="d394f-224">allowedDataStorageLocations</span></span>|<span data-ttu-id="d394f-225">[managedAppDataStorageLocation](../resources/intune_mam_managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="d394f-225">[managedAppDataStorageLocation enum](../resources/intune_mam_managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="d394f-p124">用户可能存储托管数据的数据存储位置。继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="d394f-p124">Data storage locations where a user may store managed data. Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md). The possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="d394f-229">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="d394f-229">contactSyncBlocked</span></span>|<span data-ttu-id="d394f-230">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-230">Boolean</span></span>|<span data-ttu-id="d394f-231">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="d394f-231">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="d394f-232">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-232">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-233">printBlocked</span><span class="sxs-lookup"><span data-stu-id="d394f-233">printBlocked</span></span>|<span data-ttu-id="d394f-234">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-234">Boolean</span></span>|<span data-ttu-id="d394f-235">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="d394f-235">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="d394f-236">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-236">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-237">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="d394f-237">fingerprintBlocked</span></span>|<span data-ttu-id="d394f-238">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-238">Boolean</span></span>|<span data-ttu-id="d394f-239">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="d394f-239">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="d394f-240">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-240">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-241">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="d394f-241">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="d394f-242">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-242">Boolean</span></span>|<span data-ttu-id="d394f-243">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="d394f-243">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="d394f-244">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-244">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-245">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="d394f-245">minimumRequiredOsVersion</span></span>|<span data-ttu-id="d394f-246">字符串</span><span class="sxs-lookup"><span data-stu-id="d394f-246">String</span></span>|<span data-ttu-id="d394f-247">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="d394f-247">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="d394f-248">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-248">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-249">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="d394f-249">minimumWarningOsVersion</span></span>|<span data-ttu-id="d394f-250">字符串</span><span class="sxs-lookup"><span data-stu-id="d394f-250">String</span></span>|<span data-ttu-id="d394f-251">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="d394f-251">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="d394f-252">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-252">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-253">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="d394f-253">minimumRequiredAppVersion</span></span>|<span data-ttu-id="d394f-254">字符串</span><span class="sxs-lookup"><span data-stu-id="d394f-254">String</span></span>|<span data-ttu-id="d394f-255">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="d394f-255">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="d394f-256">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-256">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-257">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="d394f-257">minimumWarningAppVersion</span></span>|<span data-ttu-id="d394f-258">字符串</span><span class="sxs-lookup"><span data-stu-id="d394f-258">String</span></span>|<span data-ttu-id="d394f-259">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="d394f-259">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="d394f-260">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d394f-260">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="d394f-261">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="d394f-261">appDataEncryptionType</span></span>|[<span data-ttu-id="d394f-262">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="d394f-262">managedAppDataEncryptionType</span></span>](../resources/intune_mam_managedappdataencryptiontype.md)|<span data-ttu-id="d394f-p133">托管应用程序 （仅适用于 iOS）中的数据应使用的加密类型。可取值为： `useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="d394f-p133">Type of encryption which should be used for data in a managed app. (iOS Only). The possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="d394f-266">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="d394f-266">screenCaptureBlocked</span></span>|<span data-ttu-id="d394f-267">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-267">Boolean</span></span>|<span data-ttu-id="d394f-268">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="d394f-268">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="d394f-269">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="d394f-269">(Android only)</span></span>|
|<span data-ttu-id="d394f-270">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="d394f-270">encryptAppData</span></span>|<span data-ttu-id="d394f-271">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-271">Boolean</span></span>|<span data-ttu-id="d394f-272">指示是否应加密托管应用数据。</span><span class="sxs-lookup"><span data-stu-id="d394f-272">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="d394f-273">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="d394f-273">(Android only)</span></span>|
|<span data-ttu-id="d394f-274">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="d394f-274">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="d394f-275">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-275">Boolean</span></span>|<span data-ttu-id="d394f-276">启用此设置后，如果启用设备级加密，则应用程序级加密将被禁用。</span><span class="sxs-lookup"><span data-stu-id="d394f-276">When this setting is enabled, app level encryption is disabled if device level encryption is enabled</span></span> <span data-ttu-id="d394f-277">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="d394f-277">(Android only)</span></span>|
|<span data-ttu-id="d394f-278">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="d394f-278">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="d394f-279">字符串</span><span class="sxs-lookup"><span data-stu-id="d394f-279">String</span></span>|<span data-ttu-id="d394f-280">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="d394f-280">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="d394f-281">（仅适用于iOS）</span><span class="sxs-lookup"><span data-stu-id="d394f-281">(iOS Only).</span></span>|
|<span data-ttu-id="d394f-282">customSettings</span><span class="sxs-lookup"><span data-stu-id="d394f-282">customSettings</span></span>|<span data-ttu-id="d394f-283">[keyValuePair](../resources/intune_mam_keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d394f-283">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="d394f-284">要发送给受影响用户的一组字符串键和字符串值对，不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="d394f-284">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="d394f-285">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="d394f-285">deployedAppCount</span></span>|<span data-ttu-id="d394f-286">Int32</span><span class="sxs-lookup"><span data-stu-id="d394f-286">Int32</span></span>|<span data-ttu-id="d394f-287">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="d394f-287">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="d394f-288">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="d394f-288">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="d394f-289">字符串</span><span class="sxs-lookup"><span data-stu-id="d394f-289">String</span></span>|<span data-ttu-id="d394f-290">定义用户可以拥有的最早的必需 Android 安全修补程序级别，用户可借此获得对应用的安全访问权限。</span><span class="sxs-lookup"><span data-stu-id="d394f-290">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="d394f-291">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="d394f-291">(Android only)</span></span>|
|<span data-ttu-id="d394f-292">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="d394f-292">minimumWarningPatchVersion</span></span>|<span data-ttu-id="d394f-293">字符串</span><span class="sxs-lookup"><span data-stu-id="d394f-293">String</span></span>|<span data-ttu-id="d394f-294">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="d394f-294">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="d394f-295">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="d394f-295">(Android only)</span></span>|
|<span data-ttu-id="d394f-296">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="d394f-296">faceIdBlocked</span></span>|<span data-ttu-id="d394f-297">布尔</span><span class="sxs-lookup"><span data-stu-id="d394f-297">Boolean</span></span>|<span data-ttu-id="d394f-298">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="d394f-298">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="d394f-299">（仅适用于iOS）</span><span class="sxs-lookup"><span data-stu-id="d394f-299">(iOS Only).</span></span>|



## <a name="response"></a><span data-ttu-id="d394f-300">响应</span><span class="sxs-lookup"><span data-stu-id="d394f-300">Response</span></span>
<span data-ttu-id="d394f-301">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d394f-301">If successful, this method returns a `200 OK` response code and an updated [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d394f-302">示例</span><span class="sxs-lookup"><span data-stu-id="d394f-302">Example</span></span>
### <a name="request"></a><span data-ttu-id="d394f-303">请求</span><span class="sxs-lookup"><span data-stu-id="d394f-303">Request</span></span>
<span data-ttu-id="d394f-304">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d394f-304">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
Content-type: application/json
Content-length: 1969

{
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "appDataEncryptionType": "afterDeviceRestart",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "faceIdBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="d394f-305">响应</span><span class="sxs-lookup"><span data-stu-id="d394f-305">Response</span></span>
<span data-ttu-id="d394f-p141">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d394f-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2143

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "77064c51-4c51-7706-514c-0677514c0677",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "appDataEncryptionType": "afterDeviceRestart",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "faceIdBlocked": true
}
```








