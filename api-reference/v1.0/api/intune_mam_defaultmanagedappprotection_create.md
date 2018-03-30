# <a name="create-defaultmanagedappprotection"></a><span data-ttu-id="fecc2-101">创建 defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="fecc2-101">Create defaultManagedAppProtection</span></span>

> <span data-ttu-id="fecc2-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fecc2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fecc2-103">创建新的 [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fecc2-103">Create a new [plannerBucket](../resources/intune_mam_defaultmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fecc2-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="fecc2-104">Prerequisites</span></span>
<span data-ttu-id="fecc2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fecc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fecc2-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="fecc2-107">Permission type</span></span>|<span data-ttu-id="fecc2-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fecc2-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fecc2-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fecc2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fecc2-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fecc2-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fecc2-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fecc2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fecc2-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="fecc2-112">Not supported.</span></span>|
|<span data-ttu-id="fecc2-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="fecc2-113">Application</span></span>|<span data-ttu-id="fecc2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fecc2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fecc2-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fecc2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="fecc2-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="fecc2-116">Request headers</span></span>
|<span data-ttu-id="fecc2-117">标头</span><span class="sxs-lookup"><span data-stu-id="fecc2-117">Header</span></span>|<span data-ttu-id="fecc2-118">值</span><span class="sxs-lookup"><span data-stu-id="fecc2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fecc2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fecc2-119">Authorization</span></span>|<span data-ttu-id="fecc2-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fecc2-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fecc2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fecc2-121">Accept</span></span>|<span data-ttu-id="fecc2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fecc2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fecc2-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="fecc2-123">Request body</span></span>
<span data-ttu-id="fecc2-124">在请求正文中，提供 defaultManagedAppProtection 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fecc2-124">In the request body, supply a JSON representation of user object.</span></span>

<span data-ttu-id="fecc2-125">下表显示创建 defaultManagedAppProtection 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fecc2-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="fecc2-126">属性</span><span class="sxs-lookup"><span data-stu-id="fecc2-126">Property</span></span>|<span data-ttu-id="fecc2-127">类型</span><span class="sxs-lookup"><span data-stu-id="fecc2-127">Type</span></span>|<span data-ttu-id="fecc2-128">说明</span><span class="sxs-lookup"><span data-stu-id="fecc2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fecc2-129">displayName</span><span class="sxs-lookup"><span data-stu-id="fecc2-129">displayName</span></span>|<span data-ttu-id="fecc2-130">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-130">String</span></span>|<span data-ttu-id="fecc2-131">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="fecc2-131">Policy display name.</span></span> <span data-ttu-id="fecc2-132">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="fecc2-133">description</span><span class="sxs-lookup"><span data-stu-id="fecc2-133">description</span></span>|<span data-ttu-id="fecc2-134">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-134">String</span></span>|<span data-ttu-id="fecc2-135">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="fecc2-135">The policy's description.</span></span> <span data-ttu-id="fecc2-136">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="fecc2-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fecc2-137">createdDateTime</span></span>|<span data-ttu-id="fecc2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fecc2-138">DateTimeOffset</span></span>|<span data-ttu-id="fecc2-139">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fecc2-139">The date and time when the page was created.</span></span> <span data-ttu-id="fecc2-140">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="fecc2-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fecc2-141">lastModifiedDateTime</span></span>|<span data-ttu-id="fecc2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fecc2-142">DateTimeOffset</span></span>|<span data-ttu-id="fecc2-143">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="fecc2-143">Last time the policy was modified.</span></span> <span data-ttu-id="fecc2-144">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="fecc2-145">id</span><span class="sxs-lookup"><span data-stu-id="fecc2-145">id</span></span>|<span data-ttu-id="fecc2-146">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-146">String</span></span>|<span data-ttu-id="fecc2-147">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fecc2-147">Key of the setting.</span></span> <span data-ttu-id="fecc2-148">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="fecc2-149">version</span><span class="sxs-lookup"><span data-stu-id="fecc2-149">version</span></span>|<span data-ttu-id="fecc2-150">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-150">String</span></span>|<span data-ttu-id="fecc2-151">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="fecc2-151">Version of the entity.</span></span> <span data-ttu-id="fecc2-152">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="fecc2-153">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="fecc2-153">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="fecc2-154">Duration</span><span class="sxs-lookup"><span data-stu-id="fecc2-154">Duration</span></span>|<span data-ttu-id="fecc2-155">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="fecc2-155">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="fecc2-156">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-156">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-157">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="fecc2-157">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="fecc2-158">Duration</span><span class="sxs-lookup"><span data-stu-id="fecc2-158">Duration</span></span>|<span data-ttu-id="fecc2-159">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="fecc2-159">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="fecc2-160">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-160">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-161">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="fecc2-161">allowedInboundDataTransferSources</span></span>|<span data-ttu-id="fecc2-162">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-162">String</span></span>|<span data-ttu-id="fecc2-163">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="fecc2-163">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="fecc2-164">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="fecc2-164">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="fecc2-165">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="fecc2-165">allowedOutboundDataTransferDestinations</span></span>|<span data-ttu-id="fecc2-166">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-166">String</span></span>|<span data-ttu-id="fecc2-167">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="fecc2-167">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="fecc2-168">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="fecc2-168">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="fecc2-169">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="fecc2-169">organizationalCredentialsRequired</span></span>|<span data-ttu-id="fecc2-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-170">Boolean</span></span>|<span data-ttu-id="fecc2-171">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="fecc2-171">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="fecc2-172">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-172">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-173">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="fecc2-173">allowedOutboundClipboardSharingLevel</span></span>|<span data-ttu-id="fecc2-174">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-174">String</span></span>|<span data-ttu-id="fecc2-175">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="fecc2-175">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="fecc2-176">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="fecc2-176">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="fecc2-177">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="fecc2-177">dataBackupBlocked</span></span>|<span data-ttu-id="fecc2-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-178">Boolean</span></span>|<span data-ttu-id="fecc2-179">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="fecc2-179">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="fecc2-180">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-180">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-181">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="fecc2-181">deviceComplianceRequired</span></span>|<span data-ttu-id="fecc2-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-182">Boolean</span></span>|<span data-ttu-id="fecc2-183">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="fecc2-183">Indicates whether device compliance is required.</span></span> <span data-ttu-id="fecc2-184">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-184">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-185">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="fecc2-185">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="fecc2-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-186">Boolean</span></span>|<span data-ttu-id="fecc2-187">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="fecc2-187">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="fecc2-188">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-188">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-189">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="fecc2-189">saveAsBlocked</span></span>|<span data-ttu-id="fecc2-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-190">Boolean</span></span>|<span data-ttu-id="fecc2-191">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="fecc2-191">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="fecc2-192">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-192">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-193">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="fecc2-193">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="fecc2-194">Duration</span><span class="sxs-lookup"><span data-stu-id="fecc2-194">Duration</span></span>|<span data-ttu-id="fecc2-195">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="fecc2-195">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="fecc2-196">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-196">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-197">pinRequired</span><span class="sxs-lookup"><span data-stu-id="fecc2-197">pinRequired</span></span>|<span data-ttu-id="fecc2-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-198">Boolean</span></span>|<span data-ttu-id="fecc2-199">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="fecc2-199">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="fecc2-200">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-200">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-201">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="fecc2-201">maximumPinRetries</span></span>|<span data-ttu-id="fecc2-202">Int32</span><span class="sxs-lookup"><span data-stu-id="fecc2-202">Int32</span></span>|<span data-ttu-id="fecc2-203">在擦除托管应用之前，不正确 PIN 重新尝试的最大尝试次数。</span><span class="sxs-lookup"><span data-stu-id="fecc2-203">Maximum number of incorrect pin retry attempts before the managed app is wiped.</span></span> <span data-ttu-id="fecc2-204">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-204">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-205">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="fecc2-205">simplePinBlocked</span></span>|<span data-ttu-id="fecc2-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-206">Boolean</span></span>|<span data-ttu-id="fecc2-207">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="fecc2-207">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="fecc2-208">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-208">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-209">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="fecc2-209">minimumPinLength</span></span>|<span data-ttu-id="fecc2-210">Int32</span><span class="sxs-lookup"><span data-stu-id="fecc2-210">Int32</span></span>|<span data-ttu-id="fecc2-211">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-211">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-212">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="fecc2-212">pinCharacterSet</span></span>|<span data-ttu-id="fecc2-213">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-213">String</span></span>|<span data-ttu-id="fecc2-214">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="fecc2-214">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="fecc2-215">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="fecc2-215">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="fecc2-216">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="fecc2-216">periodBeforePinReset</span></span>|<span data-ttu-id="fecc2-217">Duration</span><span class="sxs-lookup"><span data-stu-id="fecc2-217">Duration</span></span>|<span data-ttu-id="fecc2-218">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。</span><span class="sxs-lookup"><span data-stu-id="fecc2-218">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="fecc2-219">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-219">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-220">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="fecc2-220">allowedDataStorageLocations</span></span>|<span data-ttu-id="fecc2-221">String 集合</span><span class="sxs-lookup"><span data-stu-id="fecc2-221">String collection</span></span>|<span data-ttu-id="fecc2-222">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="fecc2-222">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="fecc2-223">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="fecc2-223">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="fecc2-224">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="fecc2-224">contactSyncBlocked</span></span>|<span data-ttu-id="fecc2-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-225">Boolean</span></span>|<span data-ttu-id="fecc2-226">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="fecc2-226">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="fecc2-227">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-227">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-228">printBlocked</span><span class="sxs-lookup"><span data-stu-id="fecc2-228">printBlocked</span></span>|<span data-ttu-id="fecc2-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-229">Boolean</span></span>|<span data-ttu-id="fecc2-230">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="fecc2-230">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="fecc2-231">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-231">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-232">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="fecc2-232">fingerprintBlocked</span></span>|<span data-ttu-id="fecc2-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-233">Boolean</span></span>|<span data-ttu-id="fecc2-234">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="fecc2-234">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="fecc2-235">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-235">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-236">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="fecc2-236">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="fecc2-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-237">Boolean</span></span>|<span data-ttu-id="fecc2-238">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="fecc2-238">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="fecc2-239">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-239">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-240">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="fecc2-240">minimumRequiredOsVersion</span></span>|<span data-ttu-id="fecc2-241">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-241">String</span></span>|<span data-ttu-id="fecc2-242">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="fecc2-242">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="fecc2-243">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-243">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-244">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="fecc2-244">minimumWarningOsVersion</span></span>|<span data-ttu-id="fecc2-245">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-245">String</span></span>|<span data-ttu-id="fecc2-246">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="fecc2-246">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="fecc2-247">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-247">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-248">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="fecc2-248">minimumRequiredAppVersion</span></span>|<span data-ttu-id="fecc2-249">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-249">String</span></span>|<span data-ttu-id="fecc2-250">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="fecc2-250">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="fecc2-251">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-251">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-252">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="fecc2-252">minimumWarningAppVersion</span></span>|<span data-ttu-id="fecc2-253">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-253">String</span></span>|<span data-ttu-id="fecc2-254">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="fecc2-254">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="fecc2-255">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fecc2-255">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="fecc2-256">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="fecc2-256">appDataEncryptionType</span></span>|<span data-ttu-id="fecc2-257">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-257">String</span></span>|<span data-ttu-id="fecc2-258">应该用于托管应用中的数据的加密类型。</span><span class="sxs-lookup"><span data-stu-id="fecc2-258">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="fecc2-259">（仅限 iOS）。可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="fecc2-259">(iOS Only) Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="fecc2-260">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="fecc2-260">screenCaptureBlocked</span></span>|<span data-ttu-id="fecc2-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-261">Boolean</span></span>|<span data-ttu-id="fecc2-262">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="fecc2-262">Indicates whether screen capture is blocked.</span></span>|
|<span data-ttu-id="fecc2-263">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="fecc2-263">encryptAppData</span></span>|<span data-ttu-id="fecc2-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-264">Boolean</span></span>|<span data-ttu-id="fecc2-265">指示是否应加密托管应用数据。</span><span class="sxs-lookup"><span data-stu-id="fecc2-265">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="fecc2-266">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="fecc2-266">(Android only)</span></span>|
|<span data-ttu-id="fecc2-267">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="fecc2-267">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="fecc2-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-268">Boolean</span></span>|<span data-ttu-id="fecc2-269">启用此设置后，如果启用设备级加密，应用级加密将被禁用</span><span class="sxs-lookup"><span data-stu-id="fecc2-269">When this setting is enabled, app level encryption is disabled if device level encryption is enabled</span></span>|
|<span data-ttu-id="fecc2-270">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="fecc2-270">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="fecc2-271">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-271">String</span></span>|<span data-ttu-id="fecc2-272">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="fecc2-272">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="fecc2-273">customSettings</span><span class="sxs-lookup"><span data-stu-id="fecc2-273">customSettings</span></span>|<span data-ttu-id="fecc2-274">[keyValuePair](../resources/intune_mam_keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fecc2-274">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="fecc2-275">要发送给受影响用户的一组字符串键和字符串值对，不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="fecc2-275">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="fecc2-276">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="fecc2-276">deployedAppCount</span></span>|<span data-ttu-id="fecc2-277">Int32</span><span class="sxs-lookup"><span data-stu-id="fecc2-277">Int32</span></span>|<span data-ttu-id="fecc2-278">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="fecc2-278">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="fecc2-279">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="fecc2-279">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="fecc2-280">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-280">String</span></span>|<span data-ttu-id="fecc2-281">定义用户可以获得对应用的安全访问权限所需的最早的必需 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="fecc2-281">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span>|
|<span data-ttu-id="fecc2-282">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="fecc2-282">minimumWarningPatchVersion</span></span>|<span data-ttu-id="fecc2-283">String</span><span class="sxs-lookup"><span data-stu-id="fecc2-283">String</span></span>|<span data-ttu-id="fecc2-284">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="fecc2-284">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span>|
|<span data-ttu-id="fecc2-285">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="fecc2-285">faceIdBlocked</span></span>|<span data-ttu-id="fecc2-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="fecc2-286">Boolean</span></span>|<span data-ttu-id="fecc2-287">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="fecc2-287">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span>|



## <a name="response"></a><span data-ttu-id="fecc2-288">响应</span><span class="sxs-lookup"><span data-stu-id="fecc2-288">Response</span></span>
<span data-ttu-id="fecc2-289">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fecc2-289">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_mam_defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fecc2-290">示例</span><span class="sxs-lookup"><span data-stu-id="fecc2-290">Example</span></span>
### <a name="request"></a><span data-ttu-id="fecc2-291">请求</span><span class="sxs-lookup"><span data-stu-id="fecc2-291">Request</span></span>
<span data-ttu-id="fecc2-292">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fecc2-292">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections
Content-type: application/json
Content-length: 2035

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
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

### <a name="response"></a><span data-ttu-id="fecc2-293">响应</span><span class="sxs-lookup"><span data-stu-id="fecc2-293">Response</span></span>
<span data-ttu-id="fecc2-p135">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fecc2-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



