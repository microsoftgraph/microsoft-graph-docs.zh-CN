# <a name="create-windows10generalconfiguration"></a><span data-ttu-id="a061b-101">创建 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="a061b-101">Create windows10GeneralConfiguration</span></span>

> <span data-ttu-id="a061b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a061b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a061b-103">创建新的 [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a061b-103">Create a new [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a061b-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="a061b-104">Prerequisites</span></span>
<span data-ttu-id="a061b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a061b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a061b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a061b-107">Permission type</span></span>|<span data-ttu-id="a061b-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a061b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a061b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a061b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a061b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a061b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a061b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a061b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a061b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a061b-112">Not supported.</span></span>|
|<span data-ttu-id="a061b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a061b-113">Application</span></span>|<span data-ttu-id="a061b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a061b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a061b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a061b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a061b-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="a061b-116">Request headers</span></span>
|<span data-ttu-id="a061b-117">标头</span><span class="sxs-lookup"><span data-stu-id="a061b-117">Header</span></span>|<span data-ttu-id="a061b-118">值</span><span class="sxs-lookup"><span data-stu-id="a061b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a061b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a061b-119">Authorization</span></span>|<span data-ttu-id="a061b-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a061b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a061b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a061b-121">Accept</span></span>|<span data-ttu-id="a061b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a061b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a061b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a061b-123">Request body</span></span>
<span data-ttu-id="a061b-124">在请求正文中，提供 windows10GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a061b-124">In the request body, supply a JSON representation for the windows10GeneralConfiguration object.</span></span>

<span data-ttu-id="a061b-125">下表显示了创建 windows10GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a061b-125">The following table shows the properties that are required when you create the windows10GeneralConfiguration.</span></span>

|<span data-ttu-id="a061b-126">属性</span><span class="sxs-lookup"><span data-stu-id="a061b-126">Property</span></span>|<span data-ttu-id="a061b-127">类型</span><span class="sxs-lookup"><span data-stu-id="a061b-127">Type</span></span>|<span data-ttu-id="a061b-128">说明</span><span class="sxs-lookup"><span data-stu-id="a061b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a061b-129">id</span><span class="sxs-lookup"><span data-stu-id="a061b-129">id</span></span>|<span data-ttu-id="a061b-130">String</span><span class="sxs-lookup"><span data-stu-id="a061b-130">String</span></span>|<span data-ttu-id="a061b-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a061b-131">Key of the entity.</span></span> <span data-ttu-id="a061b-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a061b-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a061b-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a061b-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a061b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a061b-134">DateTimeOffset</span></span>|<span data-ttu-id="a061b-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a061b-135">DateTime the object was last modified.</span></span> <span data-ttu-id="a061b-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a061b-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a061b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a061b-137">createdDateTime</span></span>|<span data-ttu-id="a061b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a061b-138">DateTimeOffset</span></span>|<span data-ttu-id="a061b-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a061b-139">DateTime the object was created.</span></span> <span data-ttu-id="a061b-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a061b-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a061b-141">description</span><span class="sxs-lookup"><span data-stu-id="a061b-141">description</span></span>|<span data-ttu-id="a061b-142">String</span><span class="sxs-lookup"><span data-stu-id="a061b-142">String</span></span>|<span data-ttu-id="a061b-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a061b-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a061b-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a061b-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a061b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a061b-145">displayName</span></span>|<span data-ttu-id="a061b-146">String</span><span class="sxs-lookup"><span data-stu-id="a061b-146">String</span></span>|<span data-ttu-id="a061b-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a061b-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a061b-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a061b-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a061b-149">version</span><span class="sxs-lookup"><span data-stu-id="a061b-149">version</span></span>|<span data-ttu-id="a061b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a061b-150">Int32</span></span>|<span data-ttu-id="a061b-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a061b-151">Version of the device configuration.</span></span> <span data-ttu-id="a061b-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a061b-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a061b-153">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="a061b-153">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="a061b-154">String</span><span class="sxs-lookup"><span data-stu-id="a061b-154">String</span></span>|<span data-ttu-id="a061b-155">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="a061b-155">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="a061b-156">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="a061b-156">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="a061b-157">String</span><span class="sxs-lookup"><span data-stu-id="a061b-157">String</span></span>|<span data-ttu-id="a061b-158">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="a061b-158">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="a061b-159">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="a061b-159">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="a061b-160">String</span><span class="sxs-lookup"><span data-stu-id="a061b-160">String</span></span>|<span data-ttu-id="a061b-161">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="a061b-161">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="a061b-162">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a061b-162">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="a061b-163">String</span><span class="sxs-lookup"><span data-stu-id="a061b-163">String</span></span>|<span data-ttu-id="a061b-164">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="a061b-164">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="a061b-165">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="a061b-165">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="a061b-166">Int32</span><span class="sxs-lookup"><span data-stu-id="a061b-166">Int32</span></span>|<span data-ttu-id="a061b-167">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="a061b-167">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="a061b-168">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="a061b-168">This is a mobile only setting.</span></span> <span data-ttu-id="a061b-169">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="a061b-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="a061b-170">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a061b-170">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="a061b-171">String</span><span class="sxs-lookup"><span data-stu-id="a061b-171">String</span></span>|<span data-ttu-id="a061b-172">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="a061b-172">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="a061b-173">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="a061b-173">searchBlockDiacritics</span></span>|<span data-ttu-id="a061b-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-174">Boolean</span></span>|<span data-ttu-id="a061b-175">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="a061b-175">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="a061b-176">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="a061b-176">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="a061b-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-177">Boolean</span></span>|<span data-ttu-id="a061b-178">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="a061b-178">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="a061b-179">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="a061b-179">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="a061b-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-180">Boolean</span></span>|<span data-ttu-id="a061b-181">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="a061b-181">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="a061b-182">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="a061b-182">searchEnableRemoteQueries</span></span>|<span data-ttu-id="a061b-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-183">Boolean</span></span>|<span data-ttu-id="a061b-184">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="a061b-184">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="a061b-185">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="a061b-185">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="a061b-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-186">Boolean</span></span>|<span data-ttu-id="a061b-187">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="a061b-187">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="a061b-188">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="a061b-188">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="a061b-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-189">Boolean</span></span>|<span data-ttu-id="a061b-190">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="a061b-190">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="a061b-191">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="a061b-191">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="a061b-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-192">Boolean</span></span>|<span data-ttu-id="a061b-193">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="a061b-193">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="a061b-194">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="a061b-194">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="a061b-195">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="a061b-195">diagnosticDataSubmissionMode</span></span>](../resources/intune_deviceconfig_diagnosticdatasubmissionmode.md)|<span data-ttu-id="a061b-196">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="a061b-196">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="a061b-197">可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="a061b-197">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="a061b-198">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="a061b-198">oneDriveDisableFileSync</span></span>|<span data-ttu-id="a061b-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-199">Boolean</span></span>|<span data-ttu-id="a061b-200">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="a061b-200">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="a061b-201">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="a061b-201">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="a061b-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-202">Boolean</span></span>|<span data-ttu-id="a061b-203">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="a061b-203">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="a061b-204">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="a061b-204">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="a061b-205">String</span><span class="sxs-lookup"><span data-stu-id="a061b-205">String</span></span>|<span data-ttu-id="a061b-206">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="a061b-206">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="a061b-207">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="a061b-207">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="a061b-208">String</span><span class="sxs-lookup"><span data-stu-id="a061b-208">String</span></span>|<span data-ttu-id="a061b-209">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="a061b-209">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="a061b-210">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="a061b-210">bluetoothAllowedServices</span></span>|<span data-ttu-id="a061b-211">String 集合</span><span class="sxs-lookup"><span data-stu-id="a061b-211">String collection</span></span>|<span data-ttu-id="a061b-212">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="a061b-212">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="a061b-213">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="a061b-213">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="a061b-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-214">Boolean</span></span>|<span data-ttu-id="a061b-215">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="a061b-215">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="a061b-216">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="a061b-216">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="a061b-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-217">Boolean</span></span>|<span data-ttu-id="a061b-218">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="a061b-218">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="a061b-219">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="a061b-219">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="a061b-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-220">Boolean</span></span>|<span data-ttu-id="a061b-221">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="a061b-221">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="a061b-222">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="a061b-222">edgeBlockAutofill</span></span>|<span data-ttu-id="a061b-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-223">Boolean</span></span>|<span data-ttu-id="a061b-224">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="a061b-224">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="a061b-225">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-225">edgeBlocked</span></span>|<span data-ttu-id="a061b-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-226">Boolean</span></span>|<span data-ttu-id="a061b-227">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="a061b-227">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="a061b-228">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="a061b-228">edgeCookiePolicy</span></span>|[<span data-ttu-id="a061b-229">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="a061b-229">edgeCookiePolicy</span></span>](../resources/intune_deviceconfig_edgecookiepolicy.md)|<span data-ttu-id="a061b-230">指示要在 Edge 浏览器中阻止的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="a061b-230">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="a061b-231">可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="a061b-231">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="a061b-232">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="a061b-232">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="a061b-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-233">Boolean</span></span>|<span data-ttu-id="a061b-234">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="a061b-234">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="a061b-235">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="a061b-235">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="a061b-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-236">Boolean</span></span>|<span data-ttu-id="a061b-237">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="a061b-237">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="a061b-238">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="a061b-238">edgeBlockExtensions</span></span>|<span data-ttu-id="a061b-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-239">Boolean</span></span>|<span data-ttu-id="a061b-240">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="a061b-240">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="a061b-241">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="a061b-241">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="a061b-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-242">Boolean</span></span>|<span data-ttu-id="a061b-243">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="a061b-243">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="a061b-244">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="a061b-244">edgeBlockJavaScript</span></span>|<span data-ttu-id="a061b-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-245">Boolean</span></span>|<span data-ttu-id="a061b-246">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="a061b-246">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="a061b-247">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="a061b-247">edgeBlockPasswordManager</span></span>|<span data-ttu-id="a061b-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-248">Boolean</span></span>|<span data-ttu-id="a061b-249">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="a061b-249">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="a061b-250">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="a061b-250">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="a061b-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-251">Boolean</span></span>|<span data-ttu-id="a061b-252">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="a061b-252">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="a061b-253">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="a061b-253">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="a061b-254">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="a061b-254">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="a061b-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-255">Boolean</span></span>|<span data-ttu-id="a061b-256">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="a061b-256">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="a061b-257">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="a061b-257">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="a061b-258">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="a061b-258">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="a061b-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-259">Boolean</span></span>|<span data-ttu-id="a061b-260">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="a061b-260">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="a061b-261">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="a061b-261">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="a061b-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-262">Boolean</span></span>|<span data-ttu-id="a061b-263">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="a061b-263">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="a061b-264">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="a061b-264">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="a061b-265">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="a061b-265">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="a061b-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-266">Boolean</span></span>|<span data-ttu-id="a061b-267">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="a061b-267">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="a061b-268">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="a061b-268">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="a061b-269">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="a061b-269">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="a061b-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-270">Boolean</span></span>|<span data-ttu-id="a061b-271">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="a061b-271">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="a061b-272">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="a061b-272">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="a061b-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-273">Boolean</span></span>|<span data-ttu-id="a061b-274">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="a061b-274">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="a061b-275">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="a061b-275">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="a061b-276">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="a061b-276">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="a061b-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-277">Boolean</span></span>|<span data-ttu-id="a061b-278">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="a061b-278">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="a061b-279">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="a061b-279">cellularBlockVpn</span></span>|<span data-ttu-id="a061b-280">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-280">Boolean</span></span>|<span data-ttu-id="a061b-281">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="a061b-281">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="a061b-282">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="a061b-282">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="a061b-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-283">Boolean</span></span>|<span data-ttu-id="a061b-284">是否阻止用户在通过手机网络漫游时使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="a061b-284">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="a061b-285">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="a061b-285">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="a061b-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-286">Boolean</span></span>|<span data-ttu-id="a061b-287">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="a061b-287">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="a061b-288">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="a061b-288">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="a061b-289">Int32</span><span class="sxs-lookup"><span data-stu-id="a061b-289">Int32</span></span>|<span data-ttu-id="a061b-290">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="a061b-290">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="a061b-291">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="a061b-291">Valid values 0 to 90</span></span>|
|<span data-ttu-id="a061b-292">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="a061b-292">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="a061b-293">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="a061b-293">defenderDetectedMalwareActions</span></span>](../resources/intune_deviceconfig_defenderdetectedmalwareactions.md)|<span data-ttu-id="a061b-294">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="a061b-294">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="a061b-295">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="a061b-295">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="a061b-296">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="a061b-296">weeklySchedule</span></span>](../resources/intune_deviceconfig_weeklyschedule.md)|<span data-ttu-id="a061b-297">Defender 进行系统扫描的星期几。</span><span class="sxs-lookup"><span data-stu-id="a061b-297">Defender day of the week for the system scan.</span></span> <span data-ttu-id="a061b-298">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="a061b-298">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="a061b-299">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="a061b-299">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="a061b-300">String 集合</span><span class="sxs-lookup"><span data-stu-id="a061b-300">String collection</span></span>|<span data-ttu-id="a061b-301">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="a061b-301">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="a061b-302">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="a061b-302">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="a061b-303">String 集合</span><span class="sxs-lookup"><span data-stu-id="a061b-303">String collection</span></span>|<span data-ttu-id="a061b-304">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="a061b-304">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="a061b-305">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="a061b-305">defenderScanMaxCpu</span></span>|<span data-ttu-id="a061b-306">Int32</span><span class="sxs-lookup"><span data-stu-id="a061b-306">Int32</span></span>|<span data-ttu-id="a061b-307">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="a061b-307">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="a061b-308">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="a061b-308">Valid values 0 to 100</span></span>|
|<span data-ttu-id="a061b-309">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="a061b-309">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="a061b-310">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="a061b-310">defenderMonitorFileActivity</span></span>](../resources/intune_deviceconfig_defendermonitorfileactivity.md)|<span data-ttu-id="a061b-311">监视文件活动的值。</span><span class="sxs-lookup"><span data-stu-id="a061b-311">Value for monitoring file activity.</span></span> <span data-ttu-id="a061b-312">可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="a061b-312">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="a061b-313">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="a061b-313">defenderProcessesToExclude</span></span>|<span data-ttu-id="a061b-314">String 集合</span><span class="sxs-lookup"><span data-stu-id="a061b-314">String collection</span></span>|<span data-ttu-id="a061b-315">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="a061b-315">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="a061b-316">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="a061b-316">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="a061b-317">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="a061b-317">defenderPromptForSampleSubmission</span></span>](../resources/intune_deviceconfig_defenderpromptforsamplesubmission.md)|<span data-ttu-id="a061b-318">如何提示用户提交样本的配置。</span><span class="sxs-lookup"><span data-stu-id="a061b-318">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="a061b-319">可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="a061b-319">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="a061b-320">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="a061b-320">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="a061b-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-321">Boolean</span></span>|<span data-ttu-id="a061b-322">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="a061b-322">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="a061b-323">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="a061b-323">defenderRequireCloudProtection</span></span>|<span data-ttu-id="a061b-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-324">Boolean</span></span>|<span data-ttu-id="a061b-325">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="a061b-325">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="a061b-326">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="a061b-326">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="a061b-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-327">Boolean</span></span>|<span data-ttu-id="a061b-328">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="a061b-328">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="a061b-329">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="a061b-329">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="a061b-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-330">Boolean</span></span>|<span data-ttu-id="a061b-331">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="a061b-331">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="a061b-332">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="a061b-332">defenderScanArchiveFiles</span></span>|<span data-ttu-id="a061b-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-333">Boolean</span></span>|<span data-ttu-id="a061b-334">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="a061b-334">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="a061b-335">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="a061b-335">defenderScanDownloads</span></span>|<span data-ttu-id="a061b-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-336">Boolean</span></span>|<span data-ttu-id="a061b-337">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="a061b-337">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="a061b-338">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="a061b-338">defenderScanNetworkFiles</span></span>|<span data-ttu-id="a061b-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-339">Boolean</span></span>|<span data-ttu-id="a061b-340">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="a061b-340">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="a061b-341">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="a061b-341">defenderScanIncomingMail</span></span>|<span data-ttu-id="a061b-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-342">Boolean</span></span>|<span data-ttu-id="a061b-343">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="a061b-343">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="a061b-344">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="a061b-344">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="a061b-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-345">Boolean</span></span>|<span data-ttu-id="a061b-346">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="a061b-346">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="a061b-347">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="a061b-347">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="a061b-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-348">Boolean</span></span>|<span data-ttu-id="a061b-349">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="a061b-349">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="a061b-350">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="a061b-350">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="a061b-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-351">Boolean</span></span>|<span data-ttu-id="a061b-352">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="a061b-352">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="a061b-353">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="a061b-353">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="a061b-354">Int32</span><span class="sxs-lookup"><span data-stu-id="a061b-354">Int32</span></span>|<span data-ttu-id="a061b-355">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="a061b-355">The signature update interval in hours.</span></span> <span data-ttu-id="a061b-356">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="a061b-356">Specify 0 not to check.</span></span> <span data-ttu-id="a061b-357">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="a061b-357">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a061b-358">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="a061b-358">defenderScanType</span></span>|[<span data-ttu-id="a061b-359">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="a061b-359">defenderScanType</span></span>](../resources/intune_deviceconfig_defenderscantype.md)|<span data-ttu-id="a061b-360">Defender 系统扫描类型。</span><span class="sxs-lookup"><span data-stu-id="a061b-360">The defender system scan type.</span></span> <span data-ttu-id="a061b-361">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="a061b-361">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="a061b-362">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="a061b-362">defenderScheduledScanTime</span></span>|<span data-ttu-id="a061b-363">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a061b-363">TimeOfDay</span></span>|<span data-ttu-id="a061b-364">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="a061b-364">The defender time for the system scan.</span></span>|
|<span data-ttu-id="a061b-365">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="a061b-365">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="a061b-366">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a061b-366">TimeOfDay</span></span>|<span data-ttu-id="a061b-367">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="a061b-367">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="a061b-368">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="a061b-368">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="a061b-369">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="a061b-369">defenderCloudBlockLevelType</span></span>](../resources/intune_deviceconfig_defendercloudblockleveltype.md)|<span data-ttu-id="a061b-370">指定云提供的保护级别。</span><span class="sxs-lookup"><span data-stu-id="a061b-370">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="a061b-371">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="a061b-371">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="a061b-372">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="a061b-372">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="a061b-373">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-373">Boolean</span></span>|<span data-ttu-id="a061b-374">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="a061b-374">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="a061b-375">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="a061b-375">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="a061b-376">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="a061b-376">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="a061b-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-377">Boolean</span></span>|<span data-ttu-id="a061b-378">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="a061b-378">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="a061b-379">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="a061b-379">lockScreenBlockCortana</span></span>|<span data-ttu-id="a061b-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-380">Boolean</span></span>|<span data-ttu-id="a061b-381">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="a061b-381">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="a061b-382">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="a061b-382">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="a061b-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-383">Boolean</span></span>|<span data-ttu-id="a061b-384">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="a061b-384">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="a061b-385">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="a061b-385">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="a061b-386">Int32</span><span class="sxs-lookup"><span data-stu-id="a061b-386">Int32</span></span>|<span data-ttu-id="a061b-387">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="a061b-387">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="a061b-388">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="a061b-388">Supported values are 11-1800.</span></span> <span data-ttu-id="a061b-389">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="a061b-389">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="a061b-390">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="a061b-390">passwordBlockSimple</span></span>|<span data-ttu-id="a061b-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-391">Boolean</span></span>|<span data-ttu-id="a061b-392">指定是否允许 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="a061b-392">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="a061b-393">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="a061b-393">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="a061b-394">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a061b-394">passwordExpirationDays</span></span>|<span data-ttu-id="a061b-395">Int32</span><span class="sxs-lookup"><span data-stu-id="a061b-395">Int32</span></span>|<span data-ttu-id="a061b-396">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="a061b-396">The password expiration in days.</span></span> <span data-ttu-id="a061b-397">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="a061b-397">Valid values 0 to 730</span></span>|
|<span data-ttu-id="a061b-398">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a061b-398">passwordMinimumLength</span></span>|<span data-ttu-id="a061b-399">Int32</span><span class="sxs-lookup"><span data-stu-id="a061b-399">Int32</span></span>|<span data-ttu-id="a061b-400">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="a061b-400">The minimum password length.</span></span> <span data-ttu-id="a061b-401">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="a061b-401">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a061b-402">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a061b-402">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a061b-403">Int32</span><span class="sxs-lookup"><span data-stu-id="a061b-403">Int32</span></span>|<span data-ttu-id="a061b-404">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="a061b-404">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a061b-405">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="a061b-405">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="a061b-406">Int32</span><span class="sxs-lookup"><span data-stu-id="a061b-406">Int32</span></span>|<span data-ttu-id="a061b-407">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="a061b-407">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="a061b-408">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a061b-408">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a061b-409">Int32</span><span class="sxs-lookup"><span data-stu-id="a061b-409">Int32</span></span>|<span data-ttu-id="a061b-410">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="a061b-410">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="a061b-411">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="a061b-411">Valid values 0 to 50</span></span>|
|<span data-ttu-id="a061b-412">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="a061b-412">passwordRequired</span></span>|<span data-ttu-id="a061b-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-413">Boolean</span></span>|<span data-ttu-id="a061b-414">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="a061b-414">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="a061b-415">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="a061b-415">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="a061b-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-416">Boolean</span></span>|<span data-ttu-id="a061b-417">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="a061b-417">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="a061b-418">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a061b-418">passwordRequiredType</span></span>|[<span data-ttu-id="a061b-419">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a061b-419">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="a061b-420">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="a061b-420">The required password type.</span></span> <span data-ttu-id="a061b-421">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="a061b-421">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="a061b-422">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a061b-422">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a061b-423">Int32</span><span class="sxs-lookup"><span data-stu-id="a061b-423">Int32</span></span>|<span data-ttu-id="a061b-424">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="a061b-424">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="a061b-425">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="a061b-425">Valid values 0 to 999</span></span>|
|<span data-ttu-id="a061b-426">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="a061b-426">privacyAdvertisingId</span></span>|[<span data-ttu-id="a061b-427">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="a061b-427">stateManagementSetting</span></span>](../resources/intune_deviceconfig_statemanagementsetting.md)|<span data-ttu-id="a061b-428">启用或禁用广告 ID 的使用。</span><span class="sxs-lookup"><span data-stu-id="a061b-428">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="a061b-429">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="a061b-429">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="a061b-430">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="a061b-430">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="a061b-431">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="a061b-431">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="a061b-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-432">Boolean</span></span>|<span data-ttu-id="a061b-433">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="a061b-433">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="a061b-434">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="a061b-434">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="a061b-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-435">Boolean</span></span>|<span data-ttu-id="a061b-436">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="a061b-436">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="a061b-437">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="a061b-437">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="a061b-438">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-438">Boolean</span></span>|<span data-ttu-id="a061b-439">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="a061b-439">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="a061b-440">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="a061b-440">startMenuAppListVisibility</span></span>|[<span data-ttu-id="a061b-441">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="a061b-441">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune_deviceconfig_windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="a061b-442">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。</span><span class="sxs-lookup"><span data-stu-id="a061b-442">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="a061b-443">可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="a061b-443">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="a061b-444">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="a061b-444">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="a061b-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-445">Boolean</span></span>|<span data-ttu-id="a061b-446">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="a061b-446">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="a061b-447">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="a061b-447">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="a061b-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-448">Boolean</span></span>|<span data-ttu-id="a061b-449">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="a061b-449">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="a061b-450">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="a061b-450">startMenuHideHibernate</span></span>|<span data-ttu-id="a061b-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-451">Boolean</span></span>|<span data-ttu-id="a061b-452">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="a061b-452">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="a061b-453">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="a061b-453">startMenuHideLock</span></span>|<span data-ttu-id="a061b-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-454">Boolean</span></span>|<span data-ttu-id="a061b-455">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="a061b-455">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="a061b-456">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="a061b-456">startMenuHidePowerButton</span></span>|<span data-ttu-id="a061b-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-457">Boolean</span></span>|<span data-ttu-id="a061b-458">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="a061b-458">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="a061b-459">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="a061b-459">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="a061b-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-460">Boolean</span></span>|<span data-ttu-id="a061b-461">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="a061b-461">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="a061b-462">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="a061b-462">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="a061b-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-463">Boolean</span></span>|<span data-ttu-id="a061b-464">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="a061b-464">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="a061b-465">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="a061b-465">startMenuHideRestartOptions</span></span>|<span data-ttu-id="a061b-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-466">Boolean</span></span>|<span data-ttu-id="a061b-467">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="a061b-467">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="a061b-468">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="a061b-468">startMenuHideShutDown</span></span>|<span data-ttu-id="a061b-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-469">Boolean</span></span>|<span data-ttu-id="a061b-470">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="a061b-470">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="a061b-471">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="a061b-471">startMenuHideSignOut</span></span>|<span data-ttu-id="a061b-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-472">Boolean</span></span>|<span data-ttu-id="a061b-473">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="a061b-473">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="a061b-474">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="a061b-474">startMenuHideSleep</span></span>|<span data-ttu-id="a061b-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-475">Boolean</span></span>|<span data-ttu-id="a061b-476">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="a061b-476">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="a061b-477">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="a061b-477">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="a061b-478">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-478">Boolean</span></span>|<span data-ttu-id="a061b-479">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="a061b-479">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="a061b-480">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="a061b-480">startMenuHideUserTile</span></span>|<span data-ttu-id="a061b-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-481">Boolean</span></span>|<span data-ttu-id="a061b-482">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="a061b-482">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="a061b-483">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="a061b-483">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="a061b-484">Binary</span><span class="sxs-lookup"><span data-stu-id="a061b-484">Binary</span></span>|<span data-ttu-id="a061b-485">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="a061b-485">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="a061b-486">开始布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="a061b-486">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="a061b-487">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="a061b-487">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="a061b-488">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="a061b-488">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="a061b-489">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="a061b-489">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="a061b-490">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="a061b-490">startMenuLayoutXml</span></span>|<span data-ttu-id="a061b-491">Binary</span><span class="sxs-lookup"><span data-stu-id="a061b-491">Binary</span></span>|<span data-ttu-id="a061b-492">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="a061b-492">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="a061b-493">通过基于布局修改模式指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="a061b-493">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="a061b-494">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="a061b-494">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="a061b-495">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="a061b-495">startMenuMode</span></span>|[<span data-ttu-id="a061b-496">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="a061b-496">windowsStartMenuModeType</span></span>](../resources/intune_deviceconfig_windowsstartmenumodetype.md)|<span data-ttu-id="a061b-497">允许管理员决定显示“开始”菜单的方式。</span><span class="sxs-lookup"><span data-stu-id="a061b-497">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="a061b-498">可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="a061b-498">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="a061b-499">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="a061b-499">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="a061b-500">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="a061b-500">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="a061b-501">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="a061b-501">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="a061b-502">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="a061b-502">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="a061b-503">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="a061b-503">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="a061b-504">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="a061b-504">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="a061b-505">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="a061b-505">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="a061b-506">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="a061b-506">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="a061b-507">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="a061b-507">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="a061b-508">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="a061b-508">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="a061b-509">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="a061b-509">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="a061b-510">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="a061b-510">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="a061b-511">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="a061b-511">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="a061b-512">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="a061b-512">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="a061b-513">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="a061b-513">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="a061b-514">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="a061b-514">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="a061b-515">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="a061b-515">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="a061b-516">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="a061b-516">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="a061b-517">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="a061b-517">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="a061b-518">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="a061b-518">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="a061b-519">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="a061b-519">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="a061b-520">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="a061b-520">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="a061b-521">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="a061b-521">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="a061b-522">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="a061b-522">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="a061b-523">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="a061b-523">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="a061b-524">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="a061b-524">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="a061b-525">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="a061b-525">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="a061b-526">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="a061b-526">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="a061b-527">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="a061b-527">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="a061b-528">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="a061b-528">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="a061b-529">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="a061b-529">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="a061b-530">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="a061b-530">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="a061b-531">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="a061b-531">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="a061b-532">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="a061b-532">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="a061b-533">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="a061b-533">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="a061b-534">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="a061b-534">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="a061b-535">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="a061b-535">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="a061b-536">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="a061b-536">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="a061b-537">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="a061b-537">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="a061b-538">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="a061b-538">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="a061b-539">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="a061b-539">settingsBlockSettingsApp</span></span>|<span data-ttu-id="a061b-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-540">Boolean</span></span>|<span data-ttu-id="a061b-541">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="a061b-541">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="a061b-542">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="a061b-542">settingsBlockSystemPage</span></span>|<span data-ttu-id="a061b-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-543">Boolean</span></span>|<span data-ttu-id="a061b-544">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="a061b-544">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="a061b-545">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="a061b-545">settingsBlockDevicesPage</span></span>|<span data-ttu-id="a061b-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-546">Boolean</span></span>|<span data-ttu-id="a061b-547">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="a061b-547">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="a061b-548">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="a061b-548">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="a061b-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-549">Boolean</span></span>|<span data-ttu-id="a061b-550">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="a061b-550">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="a061b-551">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="a061b-551">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="a061b-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-552">Boolean</span></span>|<span data-ttu-id="a061b-553">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="a061b-553">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="a061b-554">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="a061b-554">settingsBlockAccountsPage</span></span>|<span data-ttu-id="a061b-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-555">Boolean</span></span>|<span data-ttu-id="a061b-556">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="a061b-556">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="a061b-557">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="a061b-557">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="a061b-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-558">Boolean</span></span>|<span data-ttu-id="a061b-559">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="a061b-559">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="a061b-560">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="a061b-560">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="a061b-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-561">Boolean</span></span>|<span data-ttu-id="a061b-562">指示是否阻止在“设置”应用中访问“辅助功能”。</span><span class="sxs-lookup"><span data-stu-id="a061b-562">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="a061b-563">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="a061b-563">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="a061b-564">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-564">Boolean</span></span>|<span data-ttu-id="a061b-565">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="a061b-565">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="a061b-566">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="a061b-566">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="a061b-567">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-567">Boolean</span></span>|<span data-ttu-id="a061b-568">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="a061b-568">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="a061b-569">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="a061b-569">settingsBlockAppsPage</span></span>|<span data-ttu-id="a061b-570">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-570">Boolean</span></span>|<span data-ttu-id="a061b-571">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="a061b-571">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="a061b-572">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="a061b-572">settingsBlockGamingPage</span></span>|<span data-ttu-id="a061b-573">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-573">Boolean</span></span>|<span data-ttu-id="a061b-574">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="a061b-574">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="a061b-575">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="a061b-575">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="a061b-576">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-576">Boolean</span></span>|<span data-ttu-id="a061b-577">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="a061b-577">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="a061b-578">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-578">windowsSpotlightBlocked</span></span>|<span data-ttu-id="a061b-579">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-579">Boolean</span></span>|<span data-ttu-id="a061b-580">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="a061b-580">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="a061b-581">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="a061b-581">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="a061b-582">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-582">Boolean</span></span>|<span data-ttu-id="a061b-583">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="a061b-583">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="a061b-584">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="a061b-584">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="a061b-585">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-585">Boolean</span></span>|<span data-ttu-id="a061b-586">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="a061b-586">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="a061b-587">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="a061b-587">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="a061b-588">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-588">Boolean</span></span>|<span data-ttu-id="a061b-589">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="a061b-589">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="a061b-590">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="a061b-590">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="a061b-591">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-591">Boolean</span></span>|<span data-ttu-id="a061b-592">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="a061b-592">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="a061b-593">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="a061b-593">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="a061b-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-594">Boolean</span></span>|<span data-ttu-id="a061b-595">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="a061b-595">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="a061b-596">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="a061b-596">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="a061b-597">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="a061b-597">windowsSpotlightEnablementSettings</span></span>](../resources/intune_deviceconfig_windowsspotlightenablementsettings.md)|<span data-ttu-id="a061b-598">指定聚焦的类型。</span><span class="sxs-lookup"><span data-stu-id="a061b-598">Specifies the type of Spotlight.</span></span> <span data-ttu-id="a061b-599">可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="a061b-599">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="a061b-600">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="a061b-600">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="a061b-601">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-601">Boolean</span></span>|<span data-ttu-id="a061b-602">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="a061b-602">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="a061b-603">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="a061b-603">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="a061b-604">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="a061b-604">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="a061b-605">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-605">Boolean</span></span>|<span data-ttu-id="a061b-606">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="a061b-606">Disable automatic detection of settings.</span></span> <span data-ttu-id="a061b-607">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="a061b-607">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="a061b-608">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="a061b-608">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="a061b-609">String</span><span class="sxs-lookup"><span data-stu-id="a061b-609">String</span></span>|<span data-ttu-id="a061b-610">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="a061b-610">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="a061b-611">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="a061b-611">networkProxyServer</span></span>|[<span data-ttu-id="a061b-612">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="a061b-612">windows10NetworkProxyServer</span></span>](../resources/intune_deviceconfig_windows10networkproxyserver.md)|<span data-ttu-id="a061b-613">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="a061b-613">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="a061b-614">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="a061b-614">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="a061b-615">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-615">Boolean</span></span>|<span data-ttu-id="a061b-616">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="a061b-616">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="a061b-617">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-617">antiTheftModeBlocked</span></span>|<span data-ttu-id="a061b-618">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-618">Boolean</span></span>|<span data-ttu-id="a061b-619">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="a061b-619">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="a061b-620">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-620">bluetoothBlocked</span></span>|<span data-ttu-id="a061b-621">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-621">Boolean</span></span>|<span data-ttu-id="a061b-622">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="a061b-622">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="a061b-623">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-623">cameraBlocked</span></span>|<span data-ttu-id="a061b-624">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-624">Boolean</span></span>|<span data-ttu-id="a061b-625">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="a061b-625">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="a061b-626">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-626">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="a061b-627">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-627">Boolean</span></span>|<span data-ttu-id="a061b-628">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="a061b-628">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="a061b-629">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="a061b-629">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="a061b-630">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-630">Boolean</span></span>|<span data-ttu-id="a061b-631">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="a061b-631">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="a061b-632">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-632">copyPasteBlocked</span></span>|<span data-ttu-id="a061b-633">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-633">Boolean</span></span>|<span data-ttu-id="a061b-634">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="a061b-634">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="a061b-635">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-635">cortanaBlocked</span></span>|<span data-ttu-id="a061b-636">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-636">Boolean</span></span>|<span data-ttu-id="a061b-637">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="a061b-637">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="a061b-638">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="a061b-638">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="a061b-639">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-639">Boolean</span></span>|<span data-ttu-id="a061b-640">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="a061b-640">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="a061b-641">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="a061b-641">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="a061b-642">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-642">Boolean</span></span>|<span data-ttu-id="a061b-643">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="a061b-643">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="a061b-644">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="a061b-644">safeSearchFilter</span></span>|[<span data-ttu-id="a061b-645">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="a061b-645">safeSearchFilterType</span></span>](../resources/intune_deviceconfig_safesearchfiltertype.md)|<span data-ttu-id="a061b-646">指定需要的安全搜索筛选级别。</span><span class="sxs-lookup"><span data-stu-id="a061b-646">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="a061b-647">可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="a061b-647">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="a061b-648">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="a061b-648">edgeBlockPopups</span></span>|<span data-ttu-id="a061b-649">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-649">Boolean</span></span>|<span data-ttu-id="a061b-650">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="a061b-650">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="a061b-651">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="a061b-651">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="a061b-652">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-652">Boolean</span></span>|<span data-ttu-id="a061b-653">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="a061b-653">Indicates whether or not to Block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="a061b-654">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="a061b-654">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="a061b-655">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-655">Boolean</span></span>|<span data-ttu-id="a061b-656">指示是否阻止用户将 Intranet 流量从 Edge 发送到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="a061b-656">Indicates whether or not to Block the user from sending Intranet traffic to Internet Explorer from Edge.</span></span>|
|<span data-ttu-id="a061b-657">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="a061b-657">edgeRequireSmartScreen</span></span>|<span data-ttu-id="a061b-658">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-658">Boolean</span></span>|<span data-ttu-id="a061b-659">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="a061b-659">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="a061b-660">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="a061b-660">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="a061b-661">String</span><span class="sxs-lookup"><span data-stu-id="a061b-661">String</span></span>|<span data-ttu-id="a061b-662">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="a061b-662">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="a061b-663">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="a061b-663">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="a061b-664">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="a061b-664">edgeFirstRunUrl</span></span>|<span data-ttu-id="a061b-665">String</span><span class="sxs-lookup"><span data-stu-id="a061b-665">String</span></span>|<span data-ttu-id="a061b-666">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="a061b-666">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="a061b-667">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="a061b-667">edgeSearchEngine</span></span>|[<span data-ttu-id="a061b-668">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="a061b-668">edgeSearchEngineBase</span></span>](../resources/intune_deviceconfig_edgesearchenginebase.md)|<span data-ttu-id="a061b-669">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="a061b-669">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="a061b-670">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="a061b-670">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="a061b-671">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="a061b-671">edgeHomepageUrls</span></span>|<span data-ttu-id="a061b-672">String 集合</span><span class="sxs-lookup"><span data-stu-id="a061b-672">String collection</span></span>|<span data-ttu-id="a061b-673">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="a061b-673">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="a061b-674">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="a061b-674">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="a061b-675">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-675">Boolean</span></span>|<span data-ttu-id="a061b-676">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="a061b-676">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="a061b-677">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="a061b-677">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="a061b-678">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-678">Boolean</span></span>|<span data-ttu-id="a061b-679">指示用户是否可以覆盖有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="a061b-679">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="a061b-680">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="a061b-680">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="a061b-681">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-681">Boolean</span></span>|<span data-ttu-id="a061b-682">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="a061b-682">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="a061b-683">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="a061b-683">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="a061b-684">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-684">Boolean</span></span>|<span data-ttu-id="a061b-685">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="a061b-685">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="a061b-686">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-686">internetSharingBlocked</span></span>|<span data-ttu-id="a061b-687">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-687">Boolean</span></span>|<span data-ttu-id="a061b-688">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="a061b-688">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="a061b-689">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="a061b-689">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="a061b-690">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-690">Boolean</span></span>|<span data-ttu-id="a061b-691">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="a061b-691">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="a061b-692">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="a061b-692">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="a061b-693">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-693">Boolean</span></span>|<span data-ttu-id="a061b-694">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="a061b-694">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="a061b-695">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="a061b-695">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="a061b-696">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-696">Boolean</span></span>|<span data-ttu-id="a061b-697">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="a061b-697">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="a061b-698">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="a061b-698">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="a061b-699">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-699">Boolean</span></span>|<span data-ttu-id="a061b-700">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="a061b-700">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="a061b-701">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="a061b-701">settingsBlockChangeRegion</span></span>|<span data-ttu-id="a061b-702">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-702">Boolean</span></span>|<span data-ttu-id="a061b-703">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="a061b-703">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="a061b-704">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="a061b-704">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="a061b-705">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-705">Boolean</span></span>|<span data-ttu-id="a061b-706">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="a061b-706">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="a061b-707">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="a061b-707">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="a061b-708">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-708">Boolean</span></span>|<span data-ttu-id="a061b-709">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="a061b-709">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="a061b-710">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-710">locationServicesBlocked</span></span>|<span data-ttu-id="a061b-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-711">Boolean</span></span>|<span data-ttu-id="a061b-712">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="a061b-712">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="a061b-713">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-713">microsoftAccountBlocked</span></span>|<span data-ttu-id="a061b-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-714">Boolean</span></span>|<span data-ttu-id="a061b-715">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="a061b-715">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="a061b-716">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="a061b-716">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="a061b-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-717">Boolean</span></span>|<span data-ttu-id="a061b-718">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="a061b-718">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="a061b-719">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-719">nfcBlocked</span></span>|<span data-ttu-id="a061b-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-720">Boolean</span></span>|<span data-ttu-id="a061b-721">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="a061b-721">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="a061b-722">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-722">resetProtectionModeBlocked</span></span>|<span data-ttu-id="a061b-723">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-723">Boolean</span></span>|<span data-ttu-id="a061b-724">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="a061b-724">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="a061b-725">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-725">screenCaptureBlocked</span></span>|<span data-ttu-id="a061b-726">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-726">Boolean</span></span>|<span data-ttu-id="a061b-727">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="a061b-727">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="a061b-728">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="a061b-728">storageBlockRemovableStorage</span></span>|<span data-ttu-id="a061b-729">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-729">Boolean</span></span>|<span data-ttu-id="a061b-730">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="a061b-730">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="a061b-731">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="a061b-731">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="a061b-732">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-732">Boolean</span></span>|<span data-ttu-id="a061b-733">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="a061b-733">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="a061b-734">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-734">usbBlocked</span></span>|<span data-ttu-id="a061b-735">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-735">Boolean</span></span>|<span data-ttu-id="a061b-736">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="a061b-736">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="a061b-737">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-737">voiceRecordingBlocked</span></span>|<span data-ttu-id="a061b-738">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-738">Boolean</span></span>|<span data-ttu-id="a061b-739">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="a061b-739">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="a061b-740">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="a061b-740">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="a061b-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-741">Boolean</span></span>|<span data-ttu-id="a061b-742">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="a061b-742">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="a061b-743">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="a061b-743">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="a061b-744">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-744">wiFiBlocked</span></span>|<span data-ttu-id="a061b-745">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-745">Boolean</span></span>|<span data-ttu-id="a061b-746">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="a061b-746">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="a061b-747">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="a061b-747">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="a061b-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-748">Boolean</span></span>|<span data-ttu-id="a061b-749">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="a061b-749">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="a061b-750">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="a061b-750">wiFiScanInterval</span></span>|<span data-ttu-id="a061b-751">Int32</span><span class="sxs-lookup"><span data-stu-id="a061b-751">Int32</span></span>|<span data-ttu-id="a061b-752">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="a061b-752">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="a061b-753">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="a061b-753">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="a061b-754">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="a061b-754">Valid values 1 to 500</span></span>|
|<span data-ttu-id="a061b-755">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="a061b-755">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="a061b-756">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-756">Boolean</span></span>|<span data-ttu-id="a061b-757">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="a061b-757">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="a061b-758">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="a061b-758">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="a061b-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-759">Boolean</span></span>|<span data-ttu-id="a061b-760">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="a061b-760">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="a061b-761">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="a061b-761">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="a061b-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-762">Boolean</span></span>|<span data-ttu-id="a061b-763">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="a061b-763">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="a061b-764">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-764">windowsStoreBlocked</span></span>|<span data-ttu-id="a061b-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-765">Boolean</span></span>|<span data-ttu-id="a061b-766">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="a061b-766">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="a061b-767">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="a061b-767">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="a061b-768">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="a061b-768">stateManagementSetting</span></span>](../resources/intune_deviceconfig_statemanagementsetting.md)|<span data-ttu-id="a061b-769">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。</span><span class="sxs-lookup"><span data-stu-id="a061b-769">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="a061b-770">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="a061b-770">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="a061b-771">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="a061b-771">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="a061b-772">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-772">Boolean</span></span>|<span data-ttu-id="a061b-773">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="a061b-773">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="a061b-774">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="a061b-774">developerUnlockSetting</span></span>|[<span data-ttu-id="a061b-775">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="a061b-775">stateManagementSetting</span></span>](../resources/intune_deviceconfig_statemanagementsetting.md)|<span data-ttu-id="a061b-776">指示是否允许开发人员解锁。</span><span class="sxs-lookup"><span data-stu-id="a061b-776">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="a061b-777">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="a061b-777">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="a061b-778">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="a061b-778">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="a061b-779">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-779">Boolean</span></span>|<span data-ttu-id="a061b-780">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="a061b-780">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="a061b-781">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="a061b-781">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="a061b-782">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-782">Boolean</span></span>|<span data-ttu-id="a061b-783">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="a061b-783">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="a061b-784">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="a061b-784">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="a061b-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-785">Boolean</span></span>|<span data-ttu-id="a061b-786">指示是否启用“仅限私人应用商店”。</span><span class="sxs-lookup"><span data-stu-id="a061b-786">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="a061b-787">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="a061b-787">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="a061b-788">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-788">Boolean</span></span>|<span data-ttu-id="a061b-789">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="a061b-789">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="a061b-790">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="a061b-790">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="a061b-791">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-791">Boolean</span></span>|<span data-ttu-id="a061b-792">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="a061b-792">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="a061b-793">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="a061b-793">gameDvrBlocked</span></span>|<span data-ttu-id="a061b-794">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-794">Boolean</span></span>|<span data-ttu-id="a061b-795">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="a061b-795">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="a061b-796">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="a061b-796">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="a061b-797">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-797">Boolean</span></span>|<span data-ttu-id="a061b-798">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="a061b-798">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="a061b-799">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="a061b-799">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="a061b-800">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-800">Boolean</span></span>|<span data-ttu-id="a061b-801">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="a061b-801">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="a061b-802">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="a061b-802">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="a061b-803">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-803">Boolean</span></span>|<span data-ttu-id="a061b-804">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="a061b-804">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="a061b-805">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="a061b-805">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="a061b-806">Boolean</span><span class="sxs-lookup"><span data-stu-id="a061b-806">Boolean</span></span>|<span data-ttu-id="a061b-807">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="a061b-807">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="a061b-808">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="a061b-808">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="a061b-809">布尔</span><span class="sxs-lookup"><span data-stu-id="a061b-809">Boolean</span></span>|<span data-ttu-id="a061b-810">设备是否需要连接到网络。</span><span class="sxs-lookup"><span data-stu-id="a061b-810">Whether the device is required to connect to the network.</span></span>|



## <a name="response"></a><span data-ttu-id="a061b-811">响应</span><span class="sxs-lookup"><span data-stu-id="a061b-811">Response</span></span>
<span data-ttu-id="a061b-812">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a061b-812">If successful, this method returns a `201 Created` response code and a [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a061b-813">示例</span><span class="sxs-lookup"><span data-stu-id="a061b-813">Example</span></span>
### <a name="request"></a><span data-ttu-id="a061b-814">请求</span><span class="sxs-lookup"><span data-stu-id="a061b-814">Request</span></span>
<span data-ttu-id="a061b-815">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a061b-815">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 9768

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
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
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true
}
```

### <a name="response"></a><span data-ttu-id="a061b-816">响应</span><span class="sxs-lookup"><span data-stu-id="a061b-816">Response</span></span>
<span data-ttu-id="a061b-p157">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a061b-p157">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9940

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
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true
}
```



