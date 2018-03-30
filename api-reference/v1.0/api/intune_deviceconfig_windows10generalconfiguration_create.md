# <a name="create-windows10generalconfiguration"></a><span data-ttu-id="18fc5-101">创建 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="18fc5-101">Create windows10GeneralConfiguration</span></span>

> <span data-ttu-id="18fc5-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="18fc5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18fc5-103">创建新的 [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18fc5-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windows10generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18fc5-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="18fc5-104">Prerequisites</span></span>
<span data-ttu-id="18fc5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="18fc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="18fc5-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="18fc5-107">Permission type</span></span>|<span data-ttu-id="18fc5-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="18fc5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18fc5-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18fc5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="18fc5-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18fc5-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18fc5-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18fc5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18fc5-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="18fc5-112">Not supported.</span></span>|
|<span data-ttu-id="18fc5-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="18fc5-113">Application</span></span>|<span data-ttu-id="18fc5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="18fc5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18fc5-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18fc5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="18fc5-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="18fc5-116">Request headers</span></span>
|<span data-ttu-id="18fc5-117">标头</span><span class="sxs-lookup"><span data-stu-id="18fc5-117">Header</span></span>|<span data-ttu-id="18fc5-118">值</span><span class="sxs-lookup"><span data-stu-id="18fc5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18fc5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="18fc5-119">Authorization</span></span>|<span data-ttu-id="18fc5-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="18fc5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="18fc5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="18fc5-121">Accept</span></span>|<span data-ttu-id="18fc5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="18fc5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18fc5-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="18fc5-123">Request body</span></span>
<span data-ttu-id="18fc5-124">在请求正文中，提供 windows10GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18fc5-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="18fc5-125">下表显示了创建 windows10GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="18fc5-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="18fc5-126">属性</span><span class="sxs-lookup"><span data-stu-id="18fc5-126">Property</span></span>|<span data-ttu-id="18fc5-127">类型</span><span class="sxs-lookup"><span data-stu-id="18fc5-127">Type</span></span>|<span data-ttu-id="18fc5-128">说明</span><span class="sxs-lookup"><span data-stu-id="18fc5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18fc5-129">id</span><span class="sxs-lookup"><span data-stu-id="18fc5-129">id</span></span>|<span data-ttu-id="18fc5-130">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-130">String</span></span>|<span data-ttu-id="18fc5-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="18fc5-131">Key of the setting.</span></span> <span data-ttu-id="18fc5-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18fc5-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18fc5-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18fc5-133">lastModifiedDateTime</span></span>|<span data-ttu-id="18fc5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18fc5-134">DateTimeOffset</span></span>|<span data-ttu-id="18fc5-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="18fc5-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="18fc5-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18fc5-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18fc5-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18fc5-137">createdDateTime</span></span>|<span data-ttu-id="18fc5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18fc5-138">DateTimeOffset</span></span>|<span data-ttu-id="18fc5-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="18fc5-139">DateTime the object was created.</span></span> <span data-ttu-id="18fc5-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18fc5-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18fc5-141">description</span><span class="sxs-lookup"><span data-stu-id="18fc5-141">description</span></span>|<span data-ttu-id="18fc5-142">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-142">String</span></span>|<span data-ttu-id="18fc5-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="18fc5-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="18fc5-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18fc5-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18fc5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="18fc5-145">displayName</span></span>|<span data-ttu-id="18fc5-146">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-146">String</span></span>|<span data-ttu-id="18fc5-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="18fc5-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="18fc5-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18fc5-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18fc5-149">version</span><span class="sxs-lookup"><span data-stu-id="18fc5-149">version</span></span>|<span data-ttu-id="18fc5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="18fc5-150">Int32</span></span>|<span data-ttu-id="18fc5-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="18fc5-151">Version of the device configuration.</span></span> <span data-ttu-id="18fc5-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18fc5-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18fc5-153">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="18fc5-153">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="18fc5-154">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-154">String</span></span>|<span data-ttu-id="18fc5-155">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="18fc5-155">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="18fc5-156">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="18fc5-156">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="18fc5-157">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-157">String</span></span>|<span data-ttu-id="18fc5-158">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="18fc5-158">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="18fc5-159">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="18fc5-159">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="18fc5-160">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-160">String</span></span>|<span data-ttu-id="18fc5-161">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="18fc5-161">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="18fc5-162">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="18fc5-162">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="18fc5-163">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-163">String</span></span>|<span data-ttu-id="18fc5-164">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="18fc5-164">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="18fc5-165">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="18fc5-165">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="18fc5-166">Int32</span><span class="sxs-lookup"><span data-stu-id="18fc5-166">Int32</span></span>|<span data-ttu-id="18fc5-167">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="18fc5-167">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="18fc5-168">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="18fc5-168">This is a mobile only setting.</span></span> <span data-ttu-id="18fc5-169">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="18fc5-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="18fc5-170">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="18fc5-170">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="18fc5-171">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-171">String</span></span>|<span data-ttu-id="18fc5-172">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="18fc5-172">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="18fc5-173">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="18fc5-173">searchBlockDiacritics</span></span>|<span data-ttu-id="18fc5-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-174">Boolean</span></span>|<span data-ttu-id="18fc5-175">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="18fc5-175">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="18fc5-176">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="18fc5-176">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="18fc5-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-177">Boolean</span></span>|<span data-ttu-id="18fc5-178">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="18fc5-178">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="18fc5-179">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="18fc5-179">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="18fc5-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-180">Boolean</span></span>|<span data-ttu-id="18fc5-181">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="18fc5-181">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="18fc5-182">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="18fc5-182">searchEnableRemoteQueries</span></span>|<span data-ttu-id="18fc5-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-183">Boolean</span></span>|<span data-ttu-id="18fc5-184">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="18fc5-184">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="18fc5-185">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="18fc5-185">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="18fc5-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-186">Boolean</span></span>|<span data-ttu-id="18fc5-187">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="18fc5-187">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="18fc5-188">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="18fc5-188">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="18fc5-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-189">Boolean</span></span>|<span data-ttu-id="18fc5-190">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="18fc5-190">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="18fc5-191">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="18fc5-191">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="18fc5-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-192">Boolean</span></span>|<span data-ttu-id="18fc5-193">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="18fc5-193">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="18fc5-194">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="18fc5-194">diagnosticsDataSubmissionMode</span></span>|<span data-ttu-id="18fc5-195">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-195">String</span></span>|<span data-ttu-id="18fc5-196">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="18fc5-196">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="18fc5-197">可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-197">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="18fc5-198">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="18fc5-198">oneDriveDisableFileSync</span></span>|<span data-ttu-id="18fc5-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-199">Boolean</span></span>|<span data-ttu-id="18fc5-200">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="18fc5-200">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="18fc5-201">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="18fc5-201">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="18fc5-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-202">Boolean</span></span>|<span data-ttu-id="18fc5-203">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="18fc5-203">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="18fc5-204">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="18fc5-204">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="18fc5-205">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-205">String</span></span>|<span data-ttu-id="18fc5-206">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="18fc5-206">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="18fc5-207">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="18fc5-207">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="18fc5-208">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-208">String</span></span>|<span data-ttu-id="18fc5-209">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="18fc5-209">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="18fc5-210">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="18fc5-210">bluetoothAllowedServices</span></span>|<span data-ttu-id="18fc5-211">String 集合</span><span class="sxs-lookup"><span data-stu-id="18fc5-211">String collection</span></span>|<span data-ttu-id="18fc5-212">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="18fc5-212">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="18fc5-213">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="18fc5-213">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="18fc5-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-214">Boolean</span></span>|<span data-ttu-id="18fc5-215">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="18fc5-215">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="18fc5-216">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="18fc5-216">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="18fc5-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-217">Boolean</span></span>|<span data-ttu-id="18fc5-218">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="18fc5-218">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="18fc5-219">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="18fc5-219">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="18fc5-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-220">Boolean</span></span>|<span data-ttu-id="18fc5-221">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="18fc5-221">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="18fc5-222">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="18fc5-222">edgeBlockAutofill</span></span>|<span data-ttu-id="18fc5-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-223">Boolean</span></span>|<span data-ttu-id="18fc5-224">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="18fc5-224">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="18fc5-225">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-225">edgeBlocked</span></span>|<span data-ttu-id="18fc5-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-226">Boolean</span></span>|<span data-ttu-id="18fc5-227">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="18fc5-227">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="18fc5-228">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="18fc5-228">edgeCookiePolicy</span></span>|<span data-ttu-id="18fc5-229">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-229">String</span></span>|<span data-ttu-id="18fc5-230">指示要在 Edge 浏览器中阻止的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="18fc5-230">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="18fc5-231">可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-231">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="18fc5-232">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="18fc5-232">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="18fc5-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-233">Boolean</span></span>|<span data-ttu-id="18fc5-234">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="18fc5-234">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="18fc5-235">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="18fc5-235">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="18fc5-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-236">Boolean</span></span>|<span data-ttu-id="18fc5-237">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="18fc5-237">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="18fc5-238">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="18fc5-238">edgeBlockExtensions</span></span>|<span data-ttu-id="18fc5-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-239">Boolean</span></span>|<span data-ttu-id="18fc5-240">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="18fc5-240">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="18fc5-241">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="18fc5-241">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="18fc5-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-242">Boolean</span></span>|<span data-ttu-id="18fc5-243">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="18fc5-243">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="18fc5-244">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="18fc5-244">edgeBlockJavaScript</span></span>|<span data-ttu-id="18fc5-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-245">Boolean</span></span>|<span data-ttu-id="18fc5-246">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="18fc5-246">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="18fc5-247">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="18fc5-247">edgeBlockPasswordManager</span></span>|<span data-ttu-id="18fc5-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-248">Boolean</span></span>|<span data-ttu-id="18fc5-249">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="18fc5-249">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="18fc5-250">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="18fc5-250">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="18fc5-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-251">Boolean</span></span>|<span data-ttu-id="18fc5-252">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="18fc5-252">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="18fc5-253">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="18fc5-253">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="18fc5-254">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="18fc5-254">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="18fc5-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-255">Boolean</span></span>|<span data-ttu-id="18fc5-256">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="18fc5-256">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="18fc5-257">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="18fc5-257">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="18fc5-258">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="18fc5-258">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="18fc5-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-259">Boolean</span></span>|<span data-ttu-id="18fc5-260">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="18fc5-260">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="18fc5-261">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="18fc5-261">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="18fc5-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-262">Boolean</span></span>|<span data-ttu-id="18fc5-263">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="18fc5-263">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="18fc5-264">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="18fc5-264">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="18fc5-265">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="18fc5-265">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="18fc5-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-266">Boolean</span></span>|<span data-ttu-id="18fc5-267">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="18fc5-267">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="18fc5-268">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="18fc5-268">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="18fc5-269">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="18fc5-269">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="18fc5-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-270">Boolean</span></span>|<span data-ttu-id="18fc5-271">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="18fc5-271">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="18fc5-272">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="18fc5-272">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="18fc5-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-273">Boolean</span></span>|<span data-ttu-id="18fc5-274">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="18fc5-274">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="18fc5-275">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="18fc5-275">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="18fc5-276">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="18fc5-276">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="18fc5-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-277">Boolean</span></span>|<span data-ttu-id="18fc5-278">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="18fc5-278">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="18fc5-279">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="18fc5-279">cellularBlockVpn</span></span>|<span data-ttu-id="18fc5-280">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-280">Boolean</span></span>|<span data-ttu-id="18fc5-281">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="18fc5-281">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="18fc5-282">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="18fc5-282">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="18fc5-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-283">Boolean</span></span>|<span data-ttu-id="18fc5-284">是否阻止用户在通过手机网络漫游时使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="18fc5-284">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="18fc5-285">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="18fc5-285">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="18fc5-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-286">Boolean</span></span>|<span data-ttu-id="18fc5-287">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="18fc5-287">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="18fc5-288">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="18fc5-288">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="18fc5-289">Int32</span><span class="sxs-lookup"><span data-stu-id="18fc5-289">Int32</span></span>|<span data-ttu-id="18fc5-290">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="18fc5-290">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="18fc5-291">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="18fc5-291">Valid values 0 to 90</span></span>|
|<span data-ttu-id="18fc5-292">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="18fc5-292">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="18fc5-293">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="18fc5-293">defenderDetectedMalwareActions</span></span>](../resources/intune_deviceconfig_defenderdetectedmalwareactions.md)|<span data-ttu-id="18fc5-294">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="18fc5-294">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="18fc5-295">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="18fc5-295">defenderSystemScanSchedule</span></span>|<span data-ttu-id="18fc5-296">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-296">String</span></span>|<span data-ttu-id="18fc5-297">Defender 进行系统扫描的星期几。</span><span class="sxs-lookup"><span data-stu-id="18fc5-297">Defender day of the week for the system scan.</span></span> <span data-ttu-id="18fc5-298">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-298">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`.</span></span>|
|<span data-ttu-id="18fc5-299">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="18fc5-299">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="18fc5-300">String 集合</span><span class="sxs-lookup"><span data-stu-id="18fc5-300">String collection</span></span>|<span data-ttu-id="18fc5-301">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="18fc5-301">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="18fc5-302">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="18fc5-302">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="18fc5-303">String 集合</span><span class="sxs-lookup"><span data-stu-id="18fc5-303">String collection</span></span>|<span data-ttu-id="18fc5-304">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="18fc5-304">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="18fc5-305">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="18fc5-305">defenderScanMaxCpu</span></span>|<span data-ttu-id="18fc5-306">Int32</span><span class="sxs-lookup"><span data-stu-id="18fc5-306">Int32</span></span>|<span data-ttu-id="18fc5-307">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="18fc5-307">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="18fc5-308">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="18fc5-308">Valid values 0 to 100</span></span>|
|<span data-ttu-id="18fc5-309">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="18fc5-309">defenderMonitorFileActivity</span></span>|<span data-ttu-id="18fc5-310">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-310">String</span></span>|<span data-ttu-id="18fc5-311">监视文件活动的值。</span><span class="sxs-lookup"><span data-stu-id="18fc5-311">Value for monitoring file activity.</span></span> <span data-ttu-id="18fc5-312">可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-312">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="18fc5-313">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="18fc5-313">defenderProcessesToExclude</span></span>|<span data-ttu-id="18fc5-314">String 集合</span><span class="sxs-lookup"><span data-stu-id="18fc5-314">String collection</span></span>|<span data-ttu-id="18fc5-315">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="18fc5-315">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="18fc5-316">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="18fc5-316">defenderPromptForSampleSubmission</span></span>|<span data-ttu-id="18fc5-317">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-317">String</span></span>|<span data-ttu-id="18fc5-318">如何提示用户提交样本的配置。</span><span class="sxs-lookup"><span data-stu-id="18fc5-318">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="18fc5-319">可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-319">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="18fc5-320">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="18fc5-320">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="18fc5-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-321">Boolean</span></span>|<span data-ttu-id="18fc5-322">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="18fc5-322">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="18fc5-323">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="18fc5-323">defenderRequireCloudProtection</span></span>|<span data-ttu-id="18fc5-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-324">Boolean</span></span>|<span data-ttu-id="18fc5-325">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="18fc5-325">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="18fc5-326">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="18fc5-326">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="18fc5-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-327">Boolean</span></span>|<span data-ttu-id="18fc5-328">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="18fc5-328">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="18fc5-329">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="18fc5-329">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="18fc5-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-330">Boolean</span></span>|<span data-ttu-id="18fc5-331">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="18fc5-331">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="18fc5-332">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="18fc5-332">defenderScanArchiveFiles</span></span>|<span data-ttu-id="18fc5-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-333">Boolean</span></span>|<span data-ttu-id="18fc5-334">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="18fc5-334">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="18fc5-335">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="18fc5-335">defenderScanDownloads</span></span>|<span data-ttu-id="18fc5-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-336">Boolean</span></span>|<span data-ttu-id="18fc5-337">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="18fc5-337">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="18fc5-338">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="18fc5-338">defenderScanNetworkFiles</span></span>|<span data-ttu-id="18fc5-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-339">Boolean</span></span>|<span data-ttu-id="18fc5-340">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="18fc5-340">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="18fc5-341">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="18fc5-341">defenderScanIncomingMail</span></span>|<span data-ttu-id="18fc5-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-342">Boolean</span></span>|<span data-ttu-id="18fc5-343">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="18fc5-343">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="18fc5-344">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="18fc5-344">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="18fc5-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-345">Boolean</span></span>|<span data-ttu-id="18fc5-346">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="18fc5-346">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="18fc5-347">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="18fc5-347">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="18fc5-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-348">Boolean</span></span>|<span data-ttu-id="18fc5-349">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="18fc5-349">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="18fc5-350">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="18fc5-350">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="18fc5-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-351">Boolean</span></span>|<span data-ttu-id="18fc5-352">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="18fc5-352">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="18fc5-353">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="18fc5-353">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="18fc5-354">Int32</span><span class="sxs-lookup"><span data-stu-id="18fc5-354">Int32</span></span>|<span data-ttu-id="18fc5-355">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="18fc5-355">The signature update interval in hours.</span></span> <span data-ttu-id="18fc5-356">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="18fc5-356">Specify 0 not to check.</span></span> <span data-ttu-id="18fc5-357">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="18fc5-357">Valid values 0 to 24</span></span>|
|<span data-ttu-id="18fc5-358">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="18fc5-358">defenderScanType</span></span>|<span data-ttu-id="18fc5-359">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-359">String</span></span>|<span data-ttu-id="18fc5-360">Defender 系统扫描类型。</span><span class="sxs-lookup"><span data-stu-id="18fc5-360">The defender system scan type.</span></span> <span data-ttu-id="18fc5-361">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-361">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="18fc5-362">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="18fc5-362">defenderScheduledScanTime</span></span>|<span data-ttu-id="18fc5-363">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="18fc5-363">TimeOfDay</span></span>|<span data-ttu-id="18fc5-364">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="18fc5-364">The defender time for the system scan.</span></span>|
|<span data-ttu-id="18fc5-365">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="18fc5-365">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="18fc5-366">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="18fc5-366">TimeOfDay</span></span>|<span data-ttu-id="18fc5-367">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="18fc5-367">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="18fc5-368">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="18fc5-368">defenderCloudBlockLevel</span></span>|<span data-ttu-id="18fc5-369">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-369">String</span></span>|<span data-ttu-id="18fc5-370">指定云提供的保护级别。</span><span class="sxs-lookup"><span data-stu-id="18fc5-370">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="18fc5-371">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-371">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="18fc5-372">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="18fc5-372">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="18fc5-373">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-373">Boolean</span></span>|<span data-ttu-id="18fc5-374">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="18fc5-374">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="18fc5-375">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="18fc5-375">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="18fc5-376">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="18fc5-376">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="18fc5-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-377">Boolean</span></span>|<span data-ttu-id="18fc5-378">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="18fc5-378">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="18fc5-379">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="18fc5-379">lockScreenBlockCortana</span></span>|<span data-ttu-id="18fc5-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-380">Boolean</span></span>|<span data-ttu-id="18fc5-381">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="18fc5-381">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="18fc5-382">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="18fc5-382">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="18fc5-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-383">Boolean</span></span>|<span data-ttu-id="18fc5-384">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="18fc5-384">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="18fc5-385">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="18fc5-385">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="18fc5-386">Int32</span><span class="sxs-lookup"><span data-stu-id="18fc5-386">Int32</span></span>|<span data-ttu-id="18fc5-387">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="18fc5-387">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="18fc5-388">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="18fc5-388">Supported values are 11-1800.</span></span> <span data-ttu-id="18fc5-389">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="18fc5-389">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="18fc5-390">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="18fc5-390">passwordBlockSimple</span></span>|<span data-ttu-id="18fc5-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-391">Boolean</span></span>|<span data-ttu-id="18fc5-392">指定是否允许 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="18fc5-392">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="18fc5-393">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="18fc5-393">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="18fc5-394">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="18fc5-394">passwordExpirationDays</span></span>|<span data-ttu-id="18fc5-395">Int32</span><span class="sxs-lookup"><span data-stu-id="18fc5-395">Int32</span></span>|<span data-ttu-id="18fc5-396">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="18fc5-396">The password expiration in days.</span></span> <span data-ttu-id="18fc5-397">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="18fc5-397">Valid values 0 to 730</span></span>|
|<span data-ttu-id="18fc5-398">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="18fc5-398">passwordMinimumLength</span></span>|<span data-ttu-id="18fc5-399">Int32</span><span class="sxs-lookup"><span data-stu-id="18fc5-399">Int32</span></span>|<span data-ttu-id="18fc5-400">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="18fc5-400">The minimum password length.</span></span> <span data-ttu-id="18fc5-401">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="18fc5-401">Valid values 4 to 16</span></span>|
|<span data-ttu-id="18fc5-402">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="18fc5-402">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="18fc5-403">Int32</span><span class="sxs-lookup"><span data-stu-id="18fc5-403">Int32</span></span>|<span data-ttu-id="18fc5-404">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="18fc5-404">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="18fc5-405">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="18fc5-405">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="18fc5-406">Int32</span><span class="sxs-lookup"><span data-stu-id="18fc5-406">Int32</span></span>|<span data-ttu-id="18fc5-407">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="18fc5-407">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="18fc5-408">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="18fc5-408">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="18fc5-409">Int32</span><span class="sxs-lookup"><span data-stu-id="18fc5-409">Int32</span></span>|<span data-ttu-id="18fc5-410">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="18fc5-410">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="18fc5-411">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="18fc5-411">Valid values 0 to 50</span></span>|
|<span data-ttu-id="18fc5-412">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="18fc5-412">passwordRequired</span></span>|<span data-ttu-id="18fc5-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-413">Boolean</span></span>|<span data-ttu-id="18fc5-414">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="18fc5-414">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="18fc5-415">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="18fc5-415">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="18fc5-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-416">Boolean</span></span>|<span data-ttu-id="18fc5-417">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="18fc5-417">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="18fc5-418">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="18fc5-418">passwordRequiredType</span></span>|<span data-ttu-id="18fc5-419">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-419">String</span></span>|<span data-ttu-id="18fc5-420">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="18fc5-420">The required password type.</span></span> <span data-ttu-id="18fc5-421">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-421">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="18fc5-422">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="18fc5-422">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="18fc5-423">Int32</span><span class="sxs-lookup"><span data-stu-id="18fc5-423">Int32</span></span>|<span data-ttu-id="18fc5-424">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="18fc5-424">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="18fc5-425">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="18fc5-425">Valid values 0 to 999</span></span>|
|<span data-ttu-id="18fc5-426">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="18fc5-426">privacyAdvertisingId</span></span>|<span data-ttu-id="18fc5-427">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-427">String</span></span>|<span data-ttu-id="18fc5-428">启用或禁用广告 ID 的使用。</span><span class="sxs-lookup"><span data-stu-id="18fc5-428">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="18fc5-429">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="18fc5-429">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="18fc5-430">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-430">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="18fc5-431">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="18fc5-431">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="18fc5-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-432">Boolean</span></span>|<span data-ttu-id="18fc5-433">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="18fc5-433">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="18fc5-434">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="18fc5-434">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="18fc5-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-435">Boolean</span></span>|<span data-ttu-id="18fc5-436">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="18fc5-436">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="18fc5-437">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="18fc5-437">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="18fc5-438">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-438">Boolean</span></span>|<span data-ttu-id="18fc5-439">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="18fc5-439">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="18fc5-440">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="18fc5-440">startMenuAppListVisibility</span></span>|<span data-ttu-id="18fc5-441">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-441">String</span></span>|<span data-ttu-id="18fc5-442">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。</span><span class="sxs-lookup"><span data-stu-id="18fc5-442">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="18fc5-443">可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-443">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="18fc5-444">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="18fc5-444">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="18fc5-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-445">Boolean</span></span>|<span data-ttu-id="18fc5-446">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="18fc5-446">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="18fc5-447">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="18fc5-447">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="18fc5-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-448">Boolean</span></span>|<span data-ttu-id="18fc5-449">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="18fc5-449">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="18fc5-450">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="18fc5-450">startMenuHideHibernate</span></span>|<span data-ttu-id="18fc5-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-451">Boolean</span></span>|<span data-ttu-id="18fc5-452">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="18fc5-452">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="18fc5-453">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="18fc5-453">startMenuHideLock</span></span>|<span data-ttu-id="18fc5-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-454">Boolean</span></span>|<span data-ttu-id="18fc5-455">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="18fc5-455">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="18fc5-456">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="18fc5-456">startMenuHidePowerButton</span></span>|<span data-ttu-id="18fc5-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-457">Boolean</span></span>|<span data-ttu-id="18fc5-458">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="18fc5-458">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="18fc5-459">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="18fc5-459">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="18fc5-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-460">Boolean</span></span>|<span data-ttu-id="18fc5-461">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="18fc5-461">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="18fc5-462">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="18fc5-462">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="18fc5-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-463">Boolean</span></span>|<span data-ttu-id="18fc5-464">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="18fc5-464">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="18fc5-465">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="18fc5-465">startMenuHideRestartOptions</span></span>|<span data-ttu-id="18fc5-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-466">Boolean</span></span>|<span data-ttu-id="18fc5-467">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="18fc5-467">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="18fc5-468">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="18fc5-468">startMenuHideShutDown</span></span>|<span data-ttu-id="18fc5-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-469">Boolean</span></span>|<span data-ttu-id="18fc5-470">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="18fc5-470">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="18fc5-471">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="18fc5-471">startMenuHideSignOut</span></span>|<span data-ttu-id="18fc5-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-472">Boolean</span></span>|<span data-ttu-id="18fc5-473">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="18fc5-473">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="18fc5-474">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="18fc5-474">startMenuHideSleep</span></span>|<span data-ttu-id="18fc5-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-475">Boolean</span></span>|<span data-ttu-id="18fc5-476">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="18fc5-476">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="18fc5-477">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="18fc5-477">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="18fc5-478">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-478">Boolean</span></span>|<span data-ttu-id="18fc5-479">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="18fc5-479">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="18fc5-480">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="18fc5-480">startMenuHideUserTile</span></span>|<span data-ttu-id="18fc5-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-481">Boolean</span></span>|<span data-ttu-id="18fc5-482">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="18fc5-482">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="18fc5-483">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="18fc5-483">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="18fc5-484">Binary</span><span class="sxs-lookup"><span data-stu-id="18fc5-484">Binary</span></span>|<span data-ttu-id="18fc5-485">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="18fc5-485">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="18fc5-486">开始布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="18fc5-486">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="18fc5-487">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="18fc5-487">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="18fc5-488">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="18fc5-488">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="18fc5-489">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="18fc5-489">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="18fc5-490">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="18fc5-490">startMenuLayoutXml</span></span>|<span data-ttu-id="18fc5-491">Binary</span><span class="sxs-lookup"><span data-stu-id="18fc5-491">Binary</span></span>|<span data-ttu-id="18fc5-492">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="18fc5-492">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="18fc5-493">通过基于布局修改模式指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="18fc5-493">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="18fc5-494">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="18fc5-494">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="18fc5-495">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="18fc5-495">startMenuMode</span></span>|<span data-ttu-id="18fc5-496">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-496">String</span></span>|<span data-ttu-id="18fc5-497">允许管理员决定显示“开始”菜单的方式。</span><span class="sxs-lookup"><span data-stu-id="18fc5-497">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="18fc5-498">可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-498">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="18fc5-499">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="18fc5-499">startMenuPinnedFolderDocuments</span></span>|<span data-ttu-id="18fc5-500">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-500">String</span></span>|<span data-ttu-id="18fc5-501">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="18fc5-501">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="18fc5-502">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-502">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="18fc5-503">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="18fc5-503">startMenuPinnedFolderDownloads</span></span>|<span data-ttu-id="18fc5-504">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-504">String</span></span>|<span data-ttu-id="18fc5-505">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="18fc5-505">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="18fc5-506">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-506">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="18fc5-507">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="18fc5-507">startMenuPinnedFolderFileExplorer</span></span>|<span data-ttu-id="18fc5-508">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-508">String</span></span>|<span data-ttu-id="18fc5-509">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="18fc5-509">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="18fc5-510">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-510">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="18fc5-511">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="18fc5-511">startMenuPinnedFolderHomeGroup</span></span>|<span data-ttu-id="18fc5-512">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-512">String</span></span>|<span data-ttu-id="18fc5-513">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="18fc5-513">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="18fc5-514">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-514">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="18fc5-515">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="18fc5-515">startMenuPinnedFolderMusic</span></span>|<span data-ttu-id="18fc5-516">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-516">String</span></span>|<span data-ttu-id="18fc5-517">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="18fc5-517">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="18fc5-518">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-518">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="18fc5-519">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="18fc5-519">startMenuPinnedFolderNetwork</span></span>|<span data-ttu-id="18fc5-520">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-520">String</span></span>|<span data-ttu-id="18fc5-521">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="18fc5-521">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="18fc5-522">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-522">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="18fc5-523">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="18fc5-523">startMenuPinnedFolderPersonalFolder</span></span>|<span data-ttu-id="18fc5-524">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-524">String</span></span>|<span data-ttu-id="18fc5-525">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="18fc5-525">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="18fc5-526">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-526">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="18fc5-527">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="18fc5-527">startMenuPinnedFolderPictures</span></span>|<span data-ttu-id="18fc5-528">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-528">String</span></span>|<span data-ttu-id="18fc5-529">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="18fc5-529">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="18fc5-530">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-530">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="18fc5-531">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="18fc5-531">startMenuPinnedFolderSettings</span></span>|<span data-ttu-id="18fc5-532">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-532">String</span></span>|<span data-ttu-id="18fc5-533">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="18fc5-533">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="18fc5-534">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-534">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="18fc5-535">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="18fc5-535">startMenuPinnedFolderVideos</span></span>|<span data-ttu-id="18fc5-536">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-536">String</span></span>|<span data-ttu-id="18fc5-537">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="18fc5-537">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="18fc5-538">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-538">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="18fc5-539">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="18fc5-539">settingsBlockSettingsApp</span></span>|<span data-ttu-id="18fc5-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-540">Boolean</span></span>|<span data-ttu-id="18fc5-541">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="18fc5-541">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="18fc5-542">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="18fc5-542">settingsBlockSystemPage</span></span>|<span data-ttu-id="18fc5-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-543">Boolean</span></span>|<span data-ttu-id="18fc5-544">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="18fc5-544">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="18fc5-545">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="18fc5-545">settingsBlockDevicesPage</span></span>|<span data-ttu-id="18fc5-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-546">Boolean</span></span>|<span data-ttu-id="18fc5-547">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="18fc5-547">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="18fc5-548">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="18fc5-548">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="18fc5-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-549">Boolean</span></span>|<span data-ttu-id="18fc5-550">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="18fc5-550">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="18fc5-551">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="18fc5-551">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="18fc5-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-552">Boolean</span></span>|<span data-ttu-id="18fc5-553">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="18fc5-553">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="18fc5-554">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="18fc5-554">settingsBlockAccountsPage</span></span>|<span data-ttu-id="18fc5-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-555">Boolean</span></span>|<span data-ttu-id="18fc5-556">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="18fc5-556">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="18fc5-557">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="18fc5-557">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="18fc5-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-558">Boolean</span></span>|<span data-ttu-id="18fc5-559">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="18fc5-559">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="18fc5-560">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="18fc5-560">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="18fc5-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-561">Boolean</span></span>|<span data-ttu-id="18fc5-562">指示是否阻止在“设置”应用中访问“辅助功能”。</span><span class="sxs-lookup"><span data-stu-id="18fc5-562">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="18fc5-563">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="18fc5-563">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="18fc5-564">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-564">Boolean</span></span>|<span data-ttu-id="18fc5-565">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="18fc5-565">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="18fc5-566">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="18fc5-566">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="18fc5-567">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-567">Boolean</span></span>|<span data-ttu-id="18fc5-568">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="18fc5-568">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="18fc5-569">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="18fc5-569">settingsBlockAppsPage</span></span>|<span data-ttu-id="18fc5-570">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-570">Boolean</span></span>|<span data-ttu-id="18fc5-571">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="18fc5-571">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="18fc5-572">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="18fc5-572">settingsBlockGamingPage</span></span>|<span data-ttu-id="18fc5-573">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-573">Boolean</span></span>|<span data-ttu-id="18fc5-574">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="18fc5-574">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="18fc5-575">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="18fc5-575">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="18fc5-576">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-576">Boolean</span></span>|<span data-ttu-id="18fc5-577">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="18fc5-577">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="18fc5-578">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-578">windowsSpotlightBlocked</span></span>|<span data-ttu-id="18fc5-579">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-579">Boolean</span></span>|<span data-ttu-id="18fc5-580">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="18fc5-580">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="18fc5-581">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="18fc5-581">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="18fc5-582">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-582">Boolean</span></span>|<span data-ttu-id="18fc5-583">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="18fc5-583">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="18fc5-584">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="18fc5-584">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="18fc5-585">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-585">Boolean</span></span>|<span data-ttu-id="18fc5-586">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="18fc5-586">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="18fc5-587">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="18fc5-587">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="18fc5-588">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-588">Boolean</span></span>|<span data-ttu-id="18fc5-589">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="18fc5-589">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="18fc5-590">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="18fc5-590">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="18fc5-591">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-591">Boolean</span></span>|<span data-ttu-id="18fc5-592">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="18fc5-592">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="18fc5-593">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="18fc5-593">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="18fc5-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-594">Boolean</span></span>|<span data-ttu-id="18fc5-595">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="18fc5-595">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="18fc5-596">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="18fc5-596">windowsSpotlightConfigureOnLockScreen</span></span>|<span data-ttu-id="18fc5-597">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-597">String</span></span>|<span data-ttu-id="18fc5-598">指定的聚焦的类型。可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-598">Specifies the type of Spotlight Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="18fc5-599">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="18fc5-599">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="18fc5-600">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-600">Boolean</span></span>|<span data-ttu-id="18fc5-601">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="18fc5-601">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="18fc5-602">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="18fc5-602">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="18fc5-603">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="18fc5-603">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="18fc5-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-604">Boolean</span></span>|<span data-ttu-id="18fc5-605">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="18fc5-605">Disable automatic detection of settings.</span></span> <span data-ttu-id="18fc5-606">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="18fc5-606">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="18fc5-607">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="18fc5-607">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="18fc5-608">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-608">String</span></span>|<span data-ttu-id="18fc5-609">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="18fc5-609">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="18fc5-610">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="18fc5-610">networkProxyServer</span></span>|[<span data-ttu-id="18fc5-611">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="18fc5-611">windows10NetworkProxyServer</span></span>](../resources/intune_deviceconfig_windows10networkproxyserver.md)|<span data-ttu-id="18fc5-612">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="18fc5-612">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="18fc5-613">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="18fc5-613">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="18fc5-614">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-614">Boolean</span></span>|<span data-ttu-id="18fc5-615">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="18fc5-615">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="18fc5-616">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-616">antiTheftModeBlocked</span></span>|<span data-ttu-id="18fc5-617">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-617">Boolean</span></span>|<span data-ttu-id="18fc5-618">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="18fc5-618">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="18fc5-619">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-619">bluetoothBlocked</span></span>|<span data-ttu-id="18fc5-620">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-620">Boolean</span></span>|<span data-ttu-id="18fc5-621">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="18fc5-621">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="18fc5-622">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-622">cameraBlocked</span></span>|<span data-ttu-id="18fc5-623">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-623">Boolean</span></span>|<span data-ttu-id="18fc5-624">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="18fc5-624">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="18fc5-625">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-625">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="18fc5-626">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-626">Boolean</span></span>|<span data-ttu-id="18fc5-627">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="18fc5-627">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="18fc5-628">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="18fc5-628">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="18fc5-629">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-629">Boolean</span></span>|<span data-ttu-id="18fc5-630">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="18fc5-630">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="18fc5-631">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-631">copyPasteBlocked</span></span>|<span data-ttu-id="18fc5-632">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-632">Boolean</span></span>|<span data-ttu-id="18fc5-633">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="18fc5-633">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="18fc5-634">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-634">cortanaBlocked</span></span>|<span data-ttu-id="18fc5-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-635">Boolean</span></span>|<span data-ttu-id="18fc5-636">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="18fc5-636">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="18fc5-637">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="18fc5-637">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="18fc5-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-638">Boolean</span></span>|<span data-ttu-id="18fc5-639">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="18fc5-639">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="18fc5-640">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="18fc5-640">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="18fc5-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-641">Boolean</span></span>|<span data-ttu-id="18fc5-642">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="18fc5-642">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="18fc5-643">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="18fc5-643">safeSearchFilter</span></span>|<span data-ttu-id="18fc5-644">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-644">String</span></span>|<span data-ttu-id="18fc5-645">指定需要的安全搜索筛选级别。</span><span class="sxs-lookup"><span data-stu-id="18fc5-645">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="18fc5-646">可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-646">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="18fc5-647">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="18fc5-647">edgeBlockPopups</span></span>|<span data-ttu-id="18fc5-648">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-648">Boolean</span></span>|<span data-ttu-id="18fc5-649">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="18fc5-649">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="18fc5-650">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="18fc5-650">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="18fc5-651">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-651">Boolean</span></span>|<span data-ttu-id="18fc5-652">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="18fc5-652">Indicates whether or not to Block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="18fc5-653">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="18fc5-653">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="18fc5-654">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-654">Boolean</span></span>|<span data-ttu-id="18fc5-655">指示是否阻止用户将 Intranet 流量从 Edge 发送到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="18fc5-655">Indicates whether or not to Block the user from sending Intranet traffic to Internet Explorer from Edge.</span></span>|
|<span data-ttu-id="18fc5-656">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="18fc5-656">edgeRequireSmartScreen</span></span>|<span data-ttu-id="18fc5-657">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-657">Boolean</span></span>|<span data-ttu-id="18fc5-658">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="18fc5-658">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="18fc5-659">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="18fc5-659">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="18fc5-660">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-660">String</span></span>|<span data-ttu-id="18fc5-661">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="18fc5-661">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="18fc5-662">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="18fc5-662">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="18fc5-663">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="18fc5-663">edgeFirstRunUrl</span></span>|<span data-ttu-id="18fc5-664">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-664">String</span></span>|<span data-ttu-id="18fc5-665">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="18fc5-665">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="18fc5-666">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="18fc5-666">edgeSearchEngine</span></span>|[<span data-ttu-id="18fc5-667">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="18fc5-667">edgeSearchEngineBase</span></span>](../resources/intune_deviceconfig_edgesearchenginebase.md)|<span data-ttu-id="18fc5-668">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="18fc5-668">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="18fc5-669">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="18fc5-669">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="18fc5-670">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="18fc5-670">edgeHomepageUrls</span></span>|<span data-ttu-id="18fc5-671">String 集合</span><span class="sxs-lookup"><span data-stu-id="18fc5-671">String collection</span></span>|<span data-ttu-id="18fc5-672">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="18fc5-672">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="18fc5-673">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="18fc5-673">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="18fc5-674">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-674">Boolean</span></span>|<span data-ttu-id="18fc5-675">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="18fc5-675">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="18fc5-676">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="18fc5-676">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="18fc5-677">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-677">Boolean</span></span>|<span data-ttu-id="18fc5-678">指示用户是否可以覆盖有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="18fc5-678">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="18fc5-679">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="18fc5-679">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="18fc5-680">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-680">Boolean</span></span>|<span data-ttu-id="18fc5-681">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="18fc5-681">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="18fc5-682">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="18fc5-682">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="18fc5-683">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-683">Boolean</span></span>|<span data-ttu-id="18fc5-684">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="18fc5-684">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="18fc5-685">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-685">internetSharingBlocked</span></span>|<span data-ttu-id="18fc5-686">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-686">Boolean</span></span>|<span data-ttu-id="18fc5-687">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="18fc5-687">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="18fc5-688">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="18fc5-688">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="18fc5-689">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-689">Boolean</span></span>|<span data-ttu-id="18fc5-690">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="18fc5-690">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="18fc5-691">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="18fc5-691">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="18fc5-692">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-692">Boolean</span></span>|<span data-ttu-id="18fc5-693">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="18fc5-693">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="18fc5-694">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="18fc5-694">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="18fc5-695">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-695">Boolean</span></span>|<span data-ttu-id="18fc5-696">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="18fc5-696">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="18fc5-697">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="18fc5-697">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="18fc5-698">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-698">Boolean</span></span>|<span data-ttu-id="18fc5-699">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="18fc5-699">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="18fc5-700">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="18fc5-700">settingsBlockChangeRegion</span></span>|<span data-ttu-id="18fc5-701">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-701">Boolean</span></span>|<span data-ttu-id="18fc5-702">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="18fc5-702">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="18fc5-703">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="18fc5-703">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="18fc5-704">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-704">Boolean</span></span>|<span data-ttu-id="18fc5-705">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="18fc5-705">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="18fc5-706">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="18fc5-706">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="18fc5-707">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-707">Boolean</span></span>|<span data-ttu-id="18fc5-708">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="18fc5-708">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="18fc5-709">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-709">locationServicesBlocked</span></span>|<span data-ttu-id="18fc5-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-710">Boolean</span></span>|<span data-ttu-id="18fc5-711">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="18fc5-711">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="18fc5-712">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-712">microsoftAccountBlocked</span></span>|<span data-ttu-id="18fc5-713">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-713">Boolean</span></span>|<span data-ttu-id="18fc5-714">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="18fc5-714">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="18fc5-715">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="18fc5-715">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="18fc5-716">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-716">Boolean</span></span>|<span data-ttu-id="18fc5-717">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="18fc5-717">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="18fc5-718">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-718">nfcBlocked</span></span>|<span data-ttu-id="18fc5-719">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-719">Boolean</span></span>|<span data-ttu-id="18fc5-720">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="18fc5-720">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="18fc5-721">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-721">resetProtectionModeBlocked</span></span>|<span data-ttu-id="18fc5-722">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-722">Boolean</span></span>|<span data-ttu-id="18fc5-723">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="18fc5-723">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="18fc5-724">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-724">screenCaptureBlocked</span></span>|<span data-ttu-id="18fc5-725">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-725">Boolean</span></span>|<span data-ttu-id="18fc5-726">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="18fc5-726">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="18fc5-727">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="18fc5-727">storageBlockRemovableStorage</span></span>|<span data-ttu-id="18fc5-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-728">Boolean</span></span>|<span data-ttu-id="18fc5-729">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="18fc5-729">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="18fc5-730">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="18fc5-730">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="18fc5-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-731">Boolean</span></span>|<span data-ttu-id="18fc5-732">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="18fc5-732">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="18fc5-733">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-733">usbBlocked</span></span>|<span data-ttu-id="18fc5-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-734">Boolean</span></span>|<span data-ttu-id="18fc5-735">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="18fc5-735">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="18fc5-736">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-736">voiceRecordingBlocked</span></span>|<span data-ttu-id="18fc5-737">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-737">Boolean</span></span>|<span data-ttu-id="18fc5-738">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="18fc5-738">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="18fc5-739">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="18fc5-739">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="18fc5-740">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-740">Boolean</span></span>|<span data-ttu-id="18fc5-741">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="18fc5-741">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="18fc5-742">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="18fc5-742">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="18fc5-743">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-743">wiFiBlocked</span></span>|<span data-ttu-id="18fc5-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-744">Boolean</span></span>|<span data-ttu-id="18fc5-745">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="18fc5-745">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="18fc5-746">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="18fc5-746">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="18fc5-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-747">Boolean</span></span>|<span data-ttu-id="18fc5-748">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="18fc5-748">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="18fc5-749">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="18fc5-749">wiFiScanInterval</span></span>|<span data-ttu-id="18fc5-750">Int32</span><span class="sxs-lookup"><span data-stu-id="18fc5-750">Int32</span></span>|<span data-ttu-id="18fc5-751">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="18fc5-751">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="18fc5-752">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="18fc5-752">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="18fc5-753">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="18fc5-753">Valid values 1 to 500</span></span>|
|<span data-ttu-id="18fc5-754">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="18fc5-754">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="18fc5-755">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-755">Boolean</span></span>|<span data-ttu-id="18fc5-756">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="18fc5-756">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="18fc5-757">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="18fc5-757">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="18fc5-758">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-758">Boolean</span></span>|<span data-ttu-id="18fc5-759">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="18fc5-759">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="18fc5-760">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="18fc5-760">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="18fc5-761">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-761">Boolean</span></span>|<span data-ttu-id="18fc5-762">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="18fc5-762">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="18fc5-763">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-763">windowsStoreBlocked</span></span>|<span data-ttu-id="18fc5-764">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-764">Boolean</span></span>|<span data-ttu-id="18fc5-765">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="18fc5-765">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="18fc5-766">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="18fc5-766">appsAllowTrustedAppsSideloading</span></span>|<span data-ttu-id="18fc5-767">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-767">String</span></span>|<span data-ttu-id="18fc5-768">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。</span><span class="sxs-lookup"><span data-stu-id="18fc5-768">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="18fc5-769">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-769">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="18fc5-770">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="18fc5-770">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="18fc5-771">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-771">Boolean</span></span>|<span data-ttu-id="18fc5-772">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="18fc5-772">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="18fc5-773">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="18fc5-773">developerUnlockSetting</span></span>|<span data-ttu-id="18fc5-774">String</span><span class="sxs-lookup"><span data-stu-id="18fc5-774">String</span></span>|<span data-ttu-id="18fc5-775">指示是否允许开发人员解锁。</span><span class="sxs-lookup"><span data-stu-id="18fc5-775">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="18fc5-776">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="18fc5-776">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="18fc5-777">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="18fc5-777">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="18fc5-778">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-778">Boolean</span></span>|<span data-ttu-id="18fc5-779">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="18fc5-779">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="18fc5-780">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="18fc5-780">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="18fc5-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-781">Boolean</span></span>|<span data-ttu-id="18fc5-782">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="18fc5-782">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="18fc5-783">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="18fc5-783">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="18fc5-784">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-784">Boolean</span></span>|<span data-ttu-id="18fc5-785">指示是否启用“仅限私人应用商店”。</span><span class="sxs-lookup"><span data-stu-id="18fc5-785">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="18fc5-786">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="18fc5-786">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="18fc5-787">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-787">Boolean</span></span>|<span data-ttu-id="18fc5-788">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="18fc5-788">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="18fc5-789">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="18fc5-789">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="18fc5-790">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-790">Boolean</span></span>|<span data-ttu-id="18fc5-791">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="18fc5-791">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="18fc5-792">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="18fc5-792">gameDvrBlocked</span></span>|<span data-ttu-id="18fc5-793">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-793">Boolean</span></span>|<span data-ttu-id="18fc5-794">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="18fc5-794">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="18fc5-795">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="18fc5-795">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="18fc5-796">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-796">Boolean</span></span>|<span data-ttu-id="18fc5-797">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="18fc5-797">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="18fc5-798">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="18fc5-798">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="18fc5-799">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-799">Boolean</span></span>|<span data-ttu-id="18fc5-800">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="18fc5-800">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="18fc5-801">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="18fc5-801">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="18fc5-802">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-802">Boolean</span></span>|<span data-ttu-id="18fc5-803">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="18fc5-803">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="18fc5-804">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="18fc5-804">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="18fc5-805">Boolean</span><span class="sxs-lookup"><span data-stu-id="18fc5-805">Boolean</span></span>|<span data-ttu-id="18fc5-806">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="18fc5-806">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|



## <a name="response"></a><span data-ttu-id="18fc5-807">响应</span><span class="sxs-lookup"><span data-stu-id="18fc5-807">Response</span></span>
<span data-ttu-id="18fc5-808">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18fc5-808">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_deviceconfig_windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18fc5-809">示例</span><span class="sxs-lookup"><span data-stu-id="18fc5-809">Example</span></span>
### <a name="request"></a><span data-ttu-id="18fc5-810">请求</span><span class="sxs-lookup"><span data-stu-id="18fc5-810">Request</span></span>
<span data-ttu-id="18fc5-811">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18fc5-811">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 9767

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true
}
```

### <a name="response"></a><span data-ttu-id="18fc5-812">响应</span><span class="sxs-lookup"><span data-stu-id="18fc5-812">Response</span></span>
<span data-ttu-id="18fc5-p156">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18fc5-p156">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9875

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true
}
```



