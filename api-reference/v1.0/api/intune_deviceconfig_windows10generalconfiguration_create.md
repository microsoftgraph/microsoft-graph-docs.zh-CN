# <a name="create-windows10generalconfiguration"></a><span data-ttu-id="8a839-101">创建 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a839-101">Create windows10GeneralConfiguration</span></span>

> <span data-ttu-id="8a839-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8a839-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a839-103">创建新的 [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a839-103">Create a new [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8a839-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="8a839-104">Prerequisites</span></span>
<span data-ttu-id="8a839-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8a839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8a839-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a839-107">Permission type</span></span>|<span data-ttu-id="8a839-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8a839-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a839-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a839-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8a839-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a839-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8a839-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a839-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a839-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a839-112">Not supported.</span></span>|
|<span data-ttu-id="8a839-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a839-113">Application</span></span>|<span data-ttu-id="8a839-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a839-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a839-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a839-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8a839-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a839-116">Request headers</span></span>
|<span data-ttu-id="8a839-117">标头</span><span class="sxs-lookup"><span data-stu-id="8a839-117">Header</span></span>|<span data-ttu-id="8a839-118">值</span><span class="sxs-lookup"><span data-stu-id="8a839-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a839-119">授权</span><span class="sxs-lookup"><span data-stu-id="8a839-119">Authorization</span></span>|<span data-ttu-id="8a839-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8a839-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a839-121">接受</span><span class="sxs-lookup"><span data-stu-id="8a839-121">Accept</span></span>|<span data-ttu-id="8a839-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8a839-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a839-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a839-123">Request body</span></span>
<span data-ttu-id="8a839-124">在请求正文中，提供 windows10GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a839-124">In the request body, supply a JSON representation for the windows10GeneralConfiguration object.</span></span>

<span data-ttu-id="8a839-125">下表显示了创建 windows10GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8a839-125">The following table shows the properties that are required when you create the windows10GeneralConfiguration.</span></span>

|<span data-ttu-id="8a839-126">属性</span><span class="sxs-lookup"><span data-stu-id="8a839-126">Property</span></span>|<span data-ttu-id="8a839-127">类型</span><span class="sxs-lookup"><span data-stu-id="8a839-127">Type</span></span>|<span data-ttu-id="8a839-128">说明</span><span class="sxs-lookup"><span data-stu-id="8a839-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a839-129">ID</span><span class="sxs-lookup"><span data-stu-id="8a839-129">id</span></span>|<span data-ttu-id="8a839-130">字符串</span><span class="sxs-lookup"><span data-stu-id="8a839-130">String</span></span>|<span data-ttu-id="8a839-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8a839-131">Key of the entity.</span></span> <span data-ttu-id="8a839-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a839-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a839-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a839-133">lastModifiedDateTime</span></span>|<span data-ttu-id="8a839-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a839-134">DateTimeOffset</span></span>|<span data-ttu-id="8a839-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8a839-135">DateTime the object was last modified.</span></span> <span data-ttu-id="8a839-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a839-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a839-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a839-137">createdDateTime</span></span>|<span data-ttu-id="8a839-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a839-138">DateTimeOffset</span></span>|<span data-ttu-id="8a839-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8a839-139">DateTime the object was created.</span></span> <span data-ttu-id="8a839-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a839-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a839-141">description</span><span class="sxs-lookup"><span data-stu-id="8a839-141">description</span></span>|<span data-ttu-id="8a839-142">字符串</span><span class="sxs-lookup"><span data-stu-id="8a839-142">String</span></span>|<span data-ttu-id="8a839-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8a839-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8a839-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a839-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a839-145">displayName</span><span class="sxs-lookup"><span data-stu-id="8a839-145">displayName</span></span>|<span data-ttu-id="8a839-146">字符串</span><span class="sxs-lookup"><span data-stu-id="8a839-146">String</span></span>|<span data-ttu-id="8a839-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8a839-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8a839-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a839-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a839-149">version</span><span class="sxs-lookup"><span data-stu-id="8a839-149">version</span></span>|<span data-ttu-id="8a839-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8a839-150">Int32</span></span>|<span data-ttu-id="8a839-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8a839-151">Version of the device configuration.</span></span> <span data-ttu-id="8a839-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a839-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a839-153">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="8a839-153">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="8a839-154">字符串</span><span class="sxs-lookup"><span data-stu-id="8a839-154">String</span></span>|<span data-ttu-id="8a839-155">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="8a839-155">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="8a839-156">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="8a839-156">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="8a839-157">字符串</span><span class="sxs-lookup"><span data-stu-id="8a839-157">String</span></span>|<span data-ttu-id="8a839-158">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="8a839-158">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="8a839-159">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="8a839-159">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="8a839-160">字符串</span><span class="sxs-lookup"><span data-stu-id="8a839-160">String</span></span>|<span data-ttu-id="8a839-161">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="8a839-161">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="8a839-162">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="8a839-162">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="8a839-163">字符串</span><span class="sxs-lookup"><span data-stu-id="8a839-163">String</span></span>|<span data-ttu-id="8a839-164">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="8a839-164">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="8a839-165">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="8a839-165">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="8a839-166">Int32</span><span class="sxs-lookup"><span data-stu-id="8a839-166">Int32</span></span>|<span data-ttu-id="8a839-167">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="8a839-167">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="8a839-168">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="8a839-168">This is a mobile only setting.</span></span> <span data-ttu-id="8a839-169">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="8a839-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="8a839-170">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="8a839-170">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="8a839-171">字符串</span><span class="sxs-lookup"><span data-stu-id="8a839-171">String</span></span>|<span data-ttu-id="8a839-172">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="8a839-172">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="8a839-173">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="8a839-173">searchBlockDiacritics</span></span>|<span data-ttu-id="8a839-174">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-174">Boolean</span></span>|<span data-ttu-id="8a839-175">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="8a839-175">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="8a839-176">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="8a839-176">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="8a839-177">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-177">Boolean</span></span>|<span data-ttu-id="8a839-178">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="8a839-178">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="8a839-179">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="8a839-179">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="8a839-180">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-180">Boolean</span></span>|<span data-ttu-id="8a839-181">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="8a839-181">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="8a839-182">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="8a839-182">searchEnableRemoteQueries</span></span>|<span data-ttu-id="8a839-183">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-183">Boolean</span></span>|<span data-ttu-id="8a839-184">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="8a839-184">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="8a839-185">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="8a839-185">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="8a839-186">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-186">Boolean</span></span>|<span data-ttu-id="8a839-187">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="8a839-187">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="8a839-188">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="8a839-188">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="8a839-189">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-189">Boolean</span></span>|<span data-ttu-id="8a839-190">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="8a839-190">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="8a839-191">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="8a839-191">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="8a839-192">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-192">Boolean</span></span>|<span data-ttu-id="8a839-193">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="8a839-193">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="8a839-194">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="8a839-194">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="8a839-195">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="8a839-195">diagnosticDataSubmissionMode</span></span>](../resources/intune_deviceconfig_diagnosticdatasubmissionmode.md)|<span data-ttu-id="8a839-p109">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p109">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson. The possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="8a839-198">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="8a839-198">oneDriveDisableFileSync</span></span>|<span data-ttu-id="8a839-199">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-199">Boolean</span></span>|<span data-ttu-id="8a839-200">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="8a839-200">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="8a839-201">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="8a839-201">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="8a839-202">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-202">Boolean</span></span>|<span data-ttu-id="8a839-203">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="8a839-203">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="8a839-204">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="8a839-204">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="8a839-205">字符串</span><span class="sxs-lookup"><span data-stu-id="8a839-205">String</span></span>|<span data-ttu-id="8a839-206">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="8a839-206">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="8a839-207">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="8a839-207">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="8a839-208">字符串</span><span class="sxs-lookup"><span data-stu-id="8a839-208">String</span></span>|<span data-ttu-id="8a839-209">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="8a839-209">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="8a839-210">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="8a839-210">bluetoothAllowedServices</span></span>|<span data-ttu-id="8a839-211">String 集合</span><span class="sxs-lookup"><span data-stu-id="8a839-211">String collection</span></span>|<span data-ttu-id="8a839-212">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="8a839-212">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="8a839-213">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="8a839-213">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="8a839-214">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-214">Boolean</span></span>|<span data-ttu-id="8a839-215">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="8a839-215">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="8a839-216">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="8a839-216">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="8a839-217">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-217">Boolean</span></span>|<span data-ttu-id="8a839-218">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="8a839-218">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="8a839-219">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="8a839-219">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="8a839-220">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-220">Boolean</span></span>|<span data-ttu-id="8a839-221">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="8a839-221">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="8a839-222">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="8a839-222">edgeBlockAutofill</span></span>|<span data-ttu-id="8a839-223">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-223">Boolean</span></span>|<span data-ttu-id="8a839-224">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="8a839-224">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="8a839-225">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-225">edgeBlocked</span></span>|<span data-ttu-id="8a839-226">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-226">Boolean</span></span>|<span data-ttu-id="8a839-227">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="8a839-227">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="8a839-228">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="8a839-228">edgeCookiePolicy</span></span>|[<span data-ttu-id="8a839-229">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="8a839-229">edgeCookiePolicy</span></span>](../resources/intune_deviceconfig_edgecookiepolicy.md)|<span data-ttu-id="8a839-p110">指示要在 Edge 浏览器中阻止的 Cookie。 可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p110">Indicates which cookies to block in the Edge browser. The possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="8a839-232">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="8a839-232">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="8a839-233">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-233">Boolean</span></span>|<span data-ttu-id="8a839-234">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="8a839-234">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="8a839-235">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="8a839-235">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="8a839-236">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-236">Boolean</span></span>|<span data-ttu-id="8a839-237">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="8a839-237">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="8a839-238">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="8a839-238">edgeBlockExtensions</span></span>|<span data-ttu-id="8a839-239">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-239">Boolean</span></span>|<span data-ttu-id="8a839-240">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="8a839-240">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="8a839-241">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="8a839-241">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="8a839-242">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-242">Boolean</span></span>|<span data-ttu-id="8a839-243">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="8a839-243">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="8a839-244">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="8a839-244">edgeBlockJavaScript</span></span>|<span data-ttu-id="8a839-245">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-245">Boolean</span></span>|<span data-ttu-id="8a839-246">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="8a839-246">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="8a839-247">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="8a839-247">edgeBlockPasswordManager</span></span>|<span data-ttu-id="8a839-248">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-248">Boolean</span></span>|<span data-ttu-id="8a839-249">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="8a839-249">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="8a839-250">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="8a839-250">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="8a839-251">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-251">Boolean</span></span>|<span data-ttu-id="8a839-252">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="8a839-252">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="8a839-253">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="8a839-253">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="8a839-254">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="8a839-254">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="8a839-255">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-255">Boolean</span></span>|<span data-ttu-id="8a839-256">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="8a839-256">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="8a839-257">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="8a839-257">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="8a839-258">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="8a839-258">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="8a839-259">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-259">Boolean</span></span>|<span data-ttu-id="8a839-260">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="8a839-260">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="8a839-261">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="8a839-261">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="8a839-262">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-262">Boolean</span></span>|<span data-ttu-id="8a839-263">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="8a839-263">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="8a839-264">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="8a839-264">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="8a839-265">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="8a839-265">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="8a839-266">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-266">Boolean</span></span>|<span data-ttu-id="8a839-267">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="8a839-267">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="8a839-268">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="8a839-268">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="8a839-269">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="8a839-269">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="8a839-270">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-270">Boolean</span></span>|<span data-ttu-id="8a839-271">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="8a839-271">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="8a839-272">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="8a839-272">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="8a839-273">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-273">Boolean</span></span>|<span data-ttu-id="8a839-274">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="8a839-274">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="8a839-275">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="8a839-275">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="8a839-276">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="8a839-276">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="8a839-277">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-277">Boolean</span></span>|<span data-ttu-id="8a839-278">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="8a839-278">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="8a839-279">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="8a839-279">cellularBlockVpn</span></span>|<span data-ttu-id="8a839-280">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-280">Boolean</span></span>|<span data-ttu-id="8a839-281">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="8a839-281">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="8a839-282">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="8a839-282">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="8a839-283">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-283">Boolean</span></span>|<span data-ttu-id="8a839-284">是否阻止用户在通过手机网络漫游时使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="8a839-284">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="8a839-285">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="8a839-285">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="8a839-286">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-286">Boolean</span></span>|<span data-ttu-id="8a839-287">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="8a839-287">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="8a839-288">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="8a839-288">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="8a839-289">Int32</span><span class="sxs-lookup"><span data-stu-id="8a839-289">Int32</span></span>|<span data-ttu-id="8a839-290">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="8a839-290">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="8a839-291">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="8a839-291">Valid values 0 to 90</span></span>|
|<span data-ttu-id="8a839-292">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="8a839-292">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="8a839-293">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="8a839-293">defenderDetectedMalwareActions</span></span>](../resources/intune_deviceconfig_defenderdetectedmalwareactions.md)|<span data-ttu-id="8a839-294">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="8a839-294">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="8a839-295">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="8a839-295">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="8a839-296">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="8a839-296">weeklySchedule</span></span>](../resources/intune_deviceconfig_weeklyschedule.md)|<span data-ttu-id="8a839-p117">Defender 进行系统扫描的星期几。可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p117">Defender day of the week for the system scan. The possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="8a839-299">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="8a839-299">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="8a839-300">String 集合</span><span class="sxs-lookup"><span data-stu-id="8a839-300">String collection</span></span>|<span data-ttu-id="8a839-301">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="8a839-301">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="8a839-302">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="8a839-302">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="8a839-303">String 集合</span><span class="sxs-lookup"><span data-stu-id="8a839-303">String collection</span></span>|<span data-ttu-id="8a839-304">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="8a839-304">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="8a839-305">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="8a839-305">defenderScanMaxCpu</span></span>|<span data-ttu-id="8a839-306">Int32</span><span class="sxs-lookup"><span data-stu-id="8a839-306">Int32</span></span>|<span data-ttu-id="8a839-307">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="8a839-307">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="8a839-308">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="8a839-308">Valid values 0 to 100</span></span>|
|<span data-ttu-id="8a839-309">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="8a839-309">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="8a839-310">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="8a839-310">defenderMonitorFileActivity</span></span>](../resources/intune_deviceconfig_defendermonitorfileactivity.md)|<span data-ttu-id="8a839-p119">监视文件活动的值。可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p119">Value for monitoring file activity. The possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="8a839-313">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="8a839-313">defenderProcessesToExclude</span></span>|<span data-ttu-id="8a839-314">String 集合</span><span class="sxs-lookup"><span data-stu-id="8a839-314">String collection</span></span>|<span data-ttu-id="8a839-315">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="8a839-315">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="8a839-316">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="8a839-316">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="8a839-317">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="8a839-317">defenderPromptForSampleSubmission</span></span>](../resources/intune_deviceconfig_defenderpromptforsamplesubmission.md)|<span data-ttu-id="8a839-p120">用于提示用户提交样本的配置。可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p120">The configuration for how to prompt user for sample submission. The possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="8a839-320">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="8a839-320">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="8a839-321">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-321">Boolean</span></span>|<span data-ttu-id="8a839-322">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="8a839-322">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="8a839-323">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="8a839-323">defenderRequireCloudProtection</span></span>|<span data-ttu-id="8a839-324">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-324">Boolean</span></span>|<span data-ttu-id="8a839-325">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="8a839-325">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="8a839-326">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="8a839-326">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="8a839-327">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-327">Boolean</span></span>|<span data-ttu-id="8a839-328">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="8a839-328">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="8a839-329">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="8a839-329">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="8a839-330">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-330">Boolean</span></span>|<span data-ttu-id="8a839-331">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="8a839-331">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="8a839-332">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="8a839-332">defenderScanArchiveFiles</span></span>|<span data-ttu-id="8a839-333">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-333">Boolean</span></span>|<span data-ttu-id="8a839-334">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="8a839-334">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="8a839-335">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="8a839-335">defenderScanDownloads</span></span>|<span data-ttu-id="8a839-336">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-336">Boolean</span></span>|<span data-ttu-id="8a839-337">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="8a839-337">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="8a839-338">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="8a839-338">defenderScanNetworkFiles</span></span>|<span data-ttu-id="8a839-339">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-339">Boolean</span></span>|<span data-ttu-id="8a839-340">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="8a839-340">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="8a839-341">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="8a839-341">defenderScanIncomingMail</span></span>|<span data-ttu-id="8a839-342">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-342">Boolean</span></span>|<span data-ttu-id="8a839-343">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="8a839-343">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="8a839-344">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="8a839-344">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="8a839-345">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-345">Boolean</span></span>|<span data-ttu-id="8a839-346">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="8a839-346">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="8a839-347">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="8a839-347">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="8a839-348">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-348">Boolean</span></span>|<span data-ttu-id="8a839-349">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="8a839-349">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="8a839-350">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="8a839-350">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="8a839-351">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-351">Boolean</span></span>|<span data-ttu-id="8a839-352">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="8a839-352">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="8a839-353">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="8a839-353">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="8a839-354">Int32</span><span class="sxs-lookup"><span data-stu-id="8a839-354">Int32</span></span>|<span data-ttu-id="8a839-355">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="8a839-355">The signature update interval in hours.</span></span> <span data-ttu-id="8a839-356">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="8a839-356">Specify 0 not to check.</span></span> <span data-ttu-id="8a839-357">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="8a839-357">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8a839-358">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="8a839-358">defenderScanType</span></span>|[<span data-ttu-id="8a839-359">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="8a839-359">defenderScanType</span></span>](../resources/intune_deviceconfig_defenderscantype.md)|<span data-ttu-id="8a839-p122">防御系统扫描类型。 可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p122">The defender system scan type. The possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="8a839-362">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="8a839-362">defenderScheduledScanTime</span></span>|<span data-ttu-id="8a839-363">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8a839-363">TimeOfDay</span></span>|<span data-ttu-id="8a839-364">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="8a839-364">The defender time for the system scan.</span></span>|
|<span data-ttu-id="8a839-365">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="8a839-365">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="8a839-366">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8a839-366">TimeOfDay</span></span>|<span data-ttu-id="8a839-367">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="8a839-367">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="8a839-368">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="8a839-368">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="8a839-369">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="8a839-369">defenderCloudBlockLevelType</span></span>](../resources/intune_deviceconfig_defendercloudblockleveltype.md)|<span data-ttu-id="8a839-p123">指定云交付保护的级别。可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p123">Specifies the level of cloud-delivered protection. The possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="8a839-372">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a839-372">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="8a839-373">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-373">Boolean</span></span>|<span data-ttu-id="8a839-374">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="8a839-374">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="8a839-375">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="8a839-375">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="8a839-376">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="8a839-376">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="8a839-377">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-377">Boolean</span></span>|<span data-ttu-id="8a839-378">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="8a839-378">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="8a839-379">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="8a839-379">lockScreenBlockCortana</span></span>|<span data-ttu-id="8a839-380">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-380">Boolean</span></span>|<span data-ttu-id="8a839-381">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="8a839-381">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="8a839-382">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="8a839-382">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="8a839-383">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-383">Boolean</span></span>|<span data-ttu-id="8a839-384">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="8a839-384">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="8a839-385">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="8a839-385">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="8a839-386">Int32</span><span class="sxs-lookup"><span data-stu-id="8a839-386">Int32</span></span>|<span data-ttu-id="8a839-387">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="8a839-387">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="8a839-388">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="8a839-388">Supported values are 11-1800.</span></span> <span data-ttu-id="8a839-389">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="8a839-389">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="8a839-390">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="8a839-390">passwordBlockSimple</span></span>|<span data-ttu-id="8a839-391">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-391">Boolean</span></span>|<span data-ttu-id="8a839-392">指定是否允许 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="8a839-392">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="8a839-393">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="8a839-393">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="8a839-394">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8a839-394">passwordExpirationDays</span></span>|<span data-ttu-id="8a839-395">Int32</span><span class="sxs-lookup"><span data-stu-id="8a839-395">Int32</span></span>|<span data-ttu-id="8a839-396">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="8a839-396">The password expiration in days.</span></span> <span data-ttu-id="8a839-397">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="8a839-397">Valid values 0 to 730</span></span>|
|<span data-ttu-id="8a839-398">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8a839-398">passwordMinimumLength</span></span>|<span data-ttu-id="8a839-399">Int32</span><span class="sxs-lookup"><span data-stu-id="8a839-399">Int32</span></span>|<span data-ttu-id="8a839-400">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="8a839-400">The minimum password length.</span></span> <span data-ttu-id="8a839-401">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="8a839-401">Valid values 4 to 16</span></span>|
|<span data-ttu-id="8a839-402">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8a839-402">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8a839-403">Int32</span><span class="sxs-lookup"><span data-stu-id="8a839-403">Int32</span></span>|<span data-ttu-id="8a839-404">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="8a839-404">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8a839-405">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8a839-405">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8a839-406">Int32</span><span class="sxs-lookup"><span data-stu-id="8a839-406">Int32</span></span>|<span data-ttu-id="8a839-407">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="8a839-407">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8a839-408">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8a839-408">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8a839-409">Int32</span><span class="sxs-lookup"><span data-stu-id="8a839-409">Int32</span></span>|<span data-ttu-id="8a839-410">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="8a839-410">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="8a839-411">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="8a839-411">Valid values 0 to 50</span></span>|
|<span data-ttu-id="8a839-412">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8a839-412">passwordRequired</span></span>|<span data-ttu-id="8a839-413">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-413">Boolean</span></span>|<span data-ttu-id="8a839-414">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="8a839-414">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="8a839-415">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="8a839-415">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="8a839-416">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-416">Boolean</span></span>|<span data-ttu-id="8a839-417">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="8a839-417">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="8a839-418">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8a839-418">passwordRequiredType</span></span>|[<span data-ttu-id="8a839-419">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8a839-419">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="8a839-p130">所需的密码类型。可取值是：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p130">The required password type. The possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8a839-422">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="8a839-422">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="8a839-423">Int32</span><span class="sxs-lookup"><span data-stu-id="8a839-423">Int32</span></span>|<span data-ttu-id="8a839-424">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="8a839-424">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="8a839-425">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="8a839-425">Valid values 0 to 999</span></span>|
|<span data-ttu-id="8a839-426">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="8a839-426">privacyAdvertisingId</span></span>|[<span data-ttu-id="8a839-427">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="8a839-427">stateManagementSetting</span></span>](../resources/intune_deviceconfig_statemanagementsetting.md)|<span data-ttu-id="8a839-p132">启用或禁用广告 ID 的使用。 已添加到 Windows 10 版本 1607。 可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p132">Enables or disables the use of advertising ID. Added in Windows 10, version 1607. The possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="8a839-431">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="8a839-431">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="8a839-432">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-432">Boolean</span></span>|<span data-ttu-id="8a839-433">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="8a839-433">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="8a839-434">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="8a839-434">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="8a839-435">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-435">Boolean</span></span>|<span data-ttu-id="8a839-436">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="8a839-436">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="8a839-437">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="8a839-437">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="8a839-438">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-438">Boolean</span></span>|<span data-ttu-id="8a839-439">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="8a839-439">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="8a839-440">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="8a839-440">startMenuAppListVisibility</span></span>|[<span data-ttu-id="8a839-441">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="8a839-441">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune_deviceconfig_windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="8a839-p133">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p133">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app. The possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="8a839-444">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="8a839-444">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="8a839-445">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-445">Boolean</span></span>|<span data-ttu-id="8a839-446">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="8a839-446">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="8a839-447">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="8a839-447">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="8a839-448">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-448">Boolean</span></span>|<span data-ttu-id="8a839-449">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="8a839-449">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="8a839-450">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="8a839-450">startMenuHideHibernate</span></span>|<span data-ttu-id="8a839-451">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-451">Boolean</span></span>|<span data-ttu-id="8a839-452">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="8a839-452">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="8a839-453">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="8a839-453">startMenuHideLock</span></span>|<span data-ttu-id="8a839-454">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-454">Boolean</span></span>|<span data-ttu-id="8a839-455">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="8a839-455">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="8a839-456">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="8a839-456">startMenuHidePowerButton</span></span>|<span data-ttu-id="8a839-457">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-457">Boolean</span></span>|<span data-ttu-id="8a839-458">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="8a839-458">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="8a839-459">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="8a839-459">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="8a839-460">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-460">Boolean</span></span>|<span data-ttu-id="8a839-461">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="8a839-461">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="8a839-462">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="8a839-462">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="8a839-463">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-463">Boolean</span></span>|<span data-ttu-id="8a839-464">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="8a839-464">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="8a839-465">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="8a839-465">startMenuHideRestartOptions</span></span>|<span data-ttu-id="8a839-466">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-466">Boolean</span></span>|<span data-ttu-id="8a839-467">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="8a839-467">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="8a839-468">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="8a839-468">startMenuHideShutDown</span></span>|<span data-ttu-id="8a839-469">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-469">Boolean</span></span>|<span data-ttu-id="8a839-470">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="8a839-470">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="8a839-471">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="8a839-471">startMenuHideSignOut</span></span>|<span data-ttu-id="8a839-472">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-472">Boolean</span></span>|<span data-ttu-id="8a839-473">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="8a839-473">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="8a839-474">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="8a839-474">startMenuHideSleep</span></span>|<span data-ttu-id="8a839-475">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-475">Boolean</span></span>|<span data-ttu-id="8a839-476">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="8a839-476">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="8a839-477">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="8a839-477">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="8a839-478">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-478">Boolean</span></span>|<span data-ttu-id="8a839-479">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="8a839-479">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="8a839-480">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="8a839-480">startMenuHideUserTile</span></span>|<span data-ttu-id="8a839-481">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-481">Boolean</span></span>|<span data-ttu-id="8a839-482">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="8a839-482">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="8a839-483">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="8a839-483">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="8a839-484">二进制</span><span class="sxs-lookup"><span data-stu-id="8a839-484">Binary</span></span>|<span data-ttu-id="8a839-485">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="8a839-485">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="8a839-486">开始布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="8a839-486">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="8a839-487">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="8a839-487">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="8a839-488">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="8a839-488">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="8a839-489">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="8a839-489">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="8a839-490">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="8a839-490">startMenuLayoutXml</span></span>|<span data-ttu-id="8a839-491">二进制</span><span class="sxs-lookup"><span data-stu-id="8a839-491">Binary</span></span>|<span data-ttu-id="8a839-492">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="8a839-492">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="8a839-493">通过基于布局修改模式指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="8a839-493">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="8a839-494">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="8a839-494">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="8a839-495">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="8a839-495">startMenuMode</span></span>|[<span data-ttu-id="8a839-496">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="8a839-496">windowsStartMenuModeType</span></span>](../resources/intune_deviceconfig_windowsstartmenumodetype.md)|<span data-ttu-id="8a839-p136">允许管理员决定显示“开始”菜单的方式。可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p136">Allows admins to decide how the Start menu is displayed. The possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="8a839-499">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="8a839-499">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="8a839-500">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="8a839-500">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="8a839-p137">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p137">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="8a839-503">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="8a839-503">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="8a839-504">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="8a839-504">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="8a839-p138">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p138">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="8a839-507">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="8a839-507">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="8a839-508">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="8a839-508">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="8a839-p139">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。 可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p139">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="8a839-511">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="8a839-511">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="8a839-512">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="8a839-512">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="8a839-p140">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p140">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="8a839-515">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="8a839-515">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="8a839-516">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="8a839-516">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="8a839-p141">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p141">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="8a839-519">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="8a839-519">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="8a839-520">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="8a839-520">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="8a839-p142">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p142">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="8a839-523">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="8a839-523">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="8a839-524">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="8a839-524">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="8a839-p143">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p143">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="8a839-527">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="8a839-527">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="8a839-528">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="8a839-528">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="8a839-p144">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p144">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="8a839-531">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="8a839-531">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="8a839-532">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="8a839-532">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="8a839-p145">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p145">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="8a839-535">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="8a839-535">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="8a839-536">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="8a839-536">visibilitySetting</span></span>](../resources/intune_deviceconfig_visibilitysetting.md)|<span data-ttu-id="8a839-p146">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p146">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu. The possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="8a839-539">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="8a839-539">settingsBlockSettingsApp</span></span>|<span data-ttu-id="8a839-540">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-540">Boolean</span></span>|<span data-ttu-id="8a839-541">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="8a839-541">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="8a839-542">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="8a839-542">settingsBlockSystemPage</span></span>|<span data-ttu-id="8a839-543">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-543">Boolean</span></span>|<span data-ttu-id="8a839-544">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="8a839-544">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="8a839-545">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="8a839-545">settingsBlockDevicesPage</span></span>|<span data-ttu-id="8a839-546">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-546">Boolean</span></span>|<span data-ttu-id="8a839-547">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="8a839-547">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="8a839-548">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="8a839-548">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="8a839-549">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-549">Boolean</span></span>|<span data-ttu-id="8a839-550">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="8a839-550">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="8a839-551">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="8a839-551">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="8a839-552">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-552">Boolean</span></span>|<span data-ttu-id="8a839-553">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="8a839-553">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="8a839-554">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="8a839-554">settingsBlockAccountsPage</span></span>|<span data-ttu-id="8a839-555">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-555">Boolean</span></span>|<span data-ttu-id="8a839-556">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="8a839-556">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="8a839-557">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="8a839-557">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="8a839-558">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-558">Boolean</span></span>|<span data-ttu-id="8a839-559">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="8a839-559">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="8a839-560">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="8a839-560">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="8a839-561">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-561">Boolean</span></span>|<span data-ttu-id="8a839-562">指示是否阻止在“设置”应用中访问“辅助功能”。</span><span class="sxs-lookup"><span data-stu-id="8a839-562">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="8a839-563">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="8a839-563">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="8a839-564">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-564">Boolean</span></span>|<span data-ttu-id="8a839-565">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="8a839-565">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="8a839-566">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="8a839-566">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="8a839-567">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-567">Boolean</span></span>|<span data-ttu-id="8a839-568">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="8a839-568">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="8a839-569">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="8a839-569">settingsBlockAppsPage</span></span>|<span data-ttu-id="8a839-570">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-570">Boolean</span></span>|<span data-ttu-id="8a839-571">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="8a839-571">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="8a839-572">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="8a839-572">settingsBlockGamingPage</span></span>|<span data-ttu-id="8a839-573">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-573">Boolean</span></span>|<span data-ttu-id="8a839-574">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="8a839-574">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="8a839-575">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="8a839-575">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="8a839-576">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-576">Boolean</span></span>|<span data-ttu-id="8a839-577">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="8a839-577">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="8a839-578">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-578">windowsSpotlightBlocked</span></span>|<span data-ttu-id="8a839-579">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-579">Boolean</span></span>|<span data-ttu-id="8a839-580">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="8a839-580">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="8a839-581">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="8a839-581">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="8a839-582">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-582">Boolean</span></span>|<span data-ttu-id="8a839-583">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="8a839-583">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="8a839-584">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="8a839-584">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="8a839-585">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-585">Boolean</span></span>|<span data-ttu-id="8a839-586">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="8a839-586">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="8a839-587">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="8a839-587">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="8a839-588">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-588">Boolean</span></span>|<span data-ttu-id="8a839-589">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="8a839-589">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="8a839-590">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="8a839-590">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="8a839-591">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-591">Boolean</span></span>|<span data-ttu-id="8a839-592">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="8a839-592">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="8a839-593">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="8a839-593">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="8a839-594">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-594">Boolean</span></span>|<span data-ttu-id="8a839-595">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="8a839-595">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="8a839-596">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="8a839-596">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="8a839-597">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="8a839-597">windowsSpotlightEnablementSettings</span></span>](../resources/intune_deviceconfig_windowsspotlightenablementsettings.md)|<span data-ttu-id="8a839-p147">指定热点的类型。可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p147">Specifies the type of Spotlight Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="8a839-600">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="8a839-600">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="8a839-601">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-601">Boolean</span></span>|<span data-ttu-id="8a839-602">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="8a839-602">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="8a839-603">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="8a839-603">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="8a839-604">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="8a839-604">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="8a839-605">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-605">Boolean</span></span>|<span data-ttu-id="8a839-606">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="8a839-606">Disable automatic detection of settings.</span></span> <span data-ttu-id="8a839-607">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="8a839-607">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="8a839-608">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="8a839-608">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="8a839-609">字符串</span><span class="sxs-lookup"><span data-stu-id="8a839-609">String</span></span>|<span data-ttu-id="8a839-610">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="8a839-610">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="8a839-611">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="8a839-611">networkProxyServer</span></span>|[<span data-ttu-id="8a839-612">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="8a839-612">windows10NetworkProxyServer</span></span>](../resources/intune_deviceconfig_windows10networkproxyserver.md)|<span data-ttu-id="8a839-613">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="8a839-613">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="8a839-614">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="8a839-614">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="8a839-615">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-615">Boolean</span></span>|<span data-ttu-id="8a839-616">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="8a839-616">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="8a839-617">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-617">antiTheftModeBlocked</span></span>|<span data-ttu-id="8a839-618">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-618">Boolean</span></span>|<span data-ttu-id="8a839-619">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="8a839-619">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="8a839-620">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-620">bluetoothBlocked</span></span>|<span data-ttu-id="8a839-621">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-621">Boolean</span></span>|<span data-ttu-id="8a839-622">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="8a839-622">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="8a839-623">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-623">cameraBlocked</span></span>|<span data-ttu-id="8a839-624">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-624">Boolean</span></span>|<span data-ttu-id="8a839-625">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="8a839-625">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="8a839-626">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-626">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="8a839-627">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-627">Boolean</span></span>|<span data-ttu-id="8a839-628">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="8a839-628">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="8a839-629">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="8a839-629">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="8a839-630">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-630">Boolean</span></span>|<span data-ttu-id="8a839-631">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="8a839-631">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="8a839-632">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-632">copyPasteBlocked</span></span>|<span data-ttu-id="8a839-633">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-633">Boolean</span></span>|<span data-ttu-id="8a839-634">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="8a839-634">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="8a839-635">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-635">cortanaBlocked</span></span>|<span data-ttu-id="8a839-636">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-636">Boolean</span></span>|<span data-ttu-id="8a839-637">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="8a839-637">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="8a839-638">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="8a839-638">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="8a839-639">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-639">Boolean</span></span>|<span data-ttu-id="8a839-640">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="8a839-640">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="8a839-641">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="8a839-641">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="8a839-642">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-642">Boolean</span></span>|<span data-ttu-id="8a839-643">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="8a839-643">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="8a839-644">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="8a839-644">safeSearchFilter</span></span>|[<span data-ttu-id="8a839-645">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="8a839-645">safeSearchFilterType</span></span>](../resources/intune_deviceconfig_safesearchfiltertype.md)|<span data-ttu-id="8a839-p150">指定需要的安全搜索筛选级别。可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p150">Specifies what filter level of safe search is required. The possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="8a839-648">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="8a839-648">edgeBlockPopups</span></span>|<span data-ttu-id="8a839-649">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-649">Boolean</span></span>|<span data-ttu-id="8a839-650">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="8a839-650">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="8a839-651">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="8a839-651">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="8a839-652">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-652">Boolean</span></span>|<span data-ttu-id="8a839-653">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="8a839-653">Indicates whether or not to Block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="8a839-654">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="8a839-654">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="8a839-655">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-655">Boolean</span></span>|<span data-ttu-id="8a839-656">指示是否阻止用户将 Intranet 流量从 Edge 发送到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="8a839-656">Indicates whether or not to Block the user from sending Intranet traffic to Internet Explorer from Edge.</span></span>|
|<span data-ttu-id="8a839-657">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="8a839-657">edgeRequireSmartScreen</span></span>|<span data-ttu-id="8a839-658">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-658">Boolean</span></span>|<span data-ttu-id="8a839-659">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="8a839-659">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="8a839-660">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="8a839-660">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="8a839-661">字符串</span><span class="sxs-lookup"><span data-stu-id="8a839-661">String</span></span>|<span data-ttu-id="8a839-662">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="8a839-662">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="8a839-663">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="8a839-663">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="8a839-664">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="8a839-664">edgeFirstRunUrl</span></span>|<span data-ttu-id="8a839-665">字符串</span><span class="sxs-lookup"><span data-stu-id="8a839-665">String</span></span>|<span data-ttu-id="8a839-666">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="8a839-666">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="8a839-667">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="8a839-667">edgeSearchEngine</span></span>|[<span data-ttu-id="8a839-668">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="8a839-668">edgeSearchEngineBase</span></span>](../resources/intune_deviceconfig_edgesearchenginebase.md)|<span data-ttu-id="8a839-669">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="8a839-669">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="8a839-670">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="8a839-670">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="8a839-671">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="8a839-671">edgeHomepageUrls</span></span>|<span data-ttu-id="8a839-672">String 集合</span><span class="sxs-lookup"><span data-stu-id="8a839-672">String collection</span></span>|<span data-ttu-id="8a839-673">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="8a839-673">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="8a839-674">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="8a839-674">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="8a839-675">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-675">Boolean</span></span>|<span data-ttu-id="8a839-676">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="8a839-676">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="8a839-677">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="8a839-677">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="8a839-678">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-678">Boolean</span></span>|<span data-ttu-id="8a839-679">指示用户是否可以覆盖有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="8a839-679">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="8a839-680">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="8a839-680">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="8a839-681">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-681">Boolean</span></span>|<span data-ttu-id="8a839-682">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="8a839-682">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="8a839-683">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="8a839-683">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="8a839-684">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-684">Boolean</span></span>|<span data-ttu-id="8a839-685">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="8a839-685">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="8a839-686">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-686">internetSharingBlocked</span></span>|<span data-ttu-id="8a839-687">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-687">Boolean</span></span>|<span data-ttu-id="8a839-688">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="8a839-688">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="8a839-689">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="8a839-689">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="8a839-690">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-690">Boolean</span></span>|<span data-ttu-id="8a839-691">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="8a839-691">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="8a839-692">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="8a839-692">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="8a839-693">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-693">Boolean</span></span>|<span data-ttu-id="8a839-694">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="8a839-694">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="8a839-695">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="8a839-695">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="8a839-696">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-696">Boolean</span></span>|<span data-ttu-id="8a839-697">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="8a839-697">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="8a839-698">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="8a839-698">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="8a839-699">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-699">Boolean</span></span>|<span data-ttu-id="8a839-700">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="8a839-700">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="8a839-701">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="8a839-701">settingsBlockChangeRegion</span></span>|<span data-ttu-id="8a839-702">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-702">Boolean</span></span>|<span data-ttu-id="8a839-703">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="8a839-703">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="8a839-704">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="8a839-704">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="8a839-705">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-705">Boolean</span></span>|<span data-ttu-id="8a839-706">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="8a839-706">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="8a839-707">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="8a839-707">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="8a839-708">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-708">Boolean</span></span>|<span data-ttu-id="8a839-709">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="8a839-709">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="8a839-710">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-710">locationServicesBlocked</span></span>|<span data-ttu-id="8a839-711">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-711">Boolean</span></span>|<span data-ttu-id="8a839-712">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="8a839-712">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="8a839-713">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-713">microsoftAccountBlocked</span></span>|<span data-ttu-id="8a839-714">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-714">Boolean</span></span>|<span data-ttu-id="8a839-715">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="8a839-715">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="8a839-716">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="8a839-716">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="8a839-717">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-717">Boolean</span></span>|<span data-ttu-id="8a839-718">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="8a839-718">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="8a839-719">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-719">nfcBlocked</span></span>|<span data-ttu-id="8a839-720">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-720">Boolean</span></span>|<span data-ttu-id="8a839-721">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="8a839-721">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="8a839-722">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-722">resetProtectionModeBlocked</span></span>|<span data-ttu-id="8a839-723">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-723">Boolean</span></span>|<span data-ttu-id="8a839-724">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="8a839-724">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="8a839-725">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-725">screenCaptureBlocked</span></span>|<span data-ttu-id="8a839-726">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-726">Boolean</span></span>|<span data-ttu-id="8a839-727">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="8a839-727">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="8a839-728">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="8a839-728">storageBlockRemovableStorage</span></span>|<span data-ttu-id="8a839-729">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-729">Boolean</span></span>|<span data-ttu-id="8a839-730">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="8a839-730">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="8a839-731">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="8a839-731">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="8a839-732">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-732">Boolean</span></span>|<span data-ttu-id="8a839-733">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="8a839-733">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="8a839-734">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-734">usbBlocked</span></span>|<span data-ttu-id="8a839-735">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-735">Boolean</span></span>|<span data-ttu-id="8a839-736">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="8a839-736">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="8a839-737">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-737">voiceRecordingBlocked</span></span>|<span data-ttu-id="8a839-738">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-738">Boolean</span></span>|<span data-ttu-id="8a839-739">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="8a839-739">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="8a839-740">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="8a839-740">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="8a839-741">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-741">Boolean</span></span>|<span data-ttu-id="8a839-742">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="8a839-742">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="8a839-743">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="8a839-743">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="8a839-744">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-744">wiFiBlocked</span></span>|<span data-ttu-id="8a839-745">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-745">Boolean</span></span>|<span data-ttu-id="8a839-746">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="8a839-746">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="8a839-747">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a839-747">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="8a839-748">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-748">Boolean</span></span>|<span data-ttu-id="8a839-749">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="8a839-749">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="8a839-750">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="8a839-750">wiFiScanInterval</span></span>|<span data-ttu-id="8a839-751">Int32</span><span class="sxs-lookup"><span data-stu-id="8a839-751">Int32</span></span>|<span data-ttu-id="8a839-752">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="8a839-752">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="8a839-753">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="8a839-753">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="8a839-754">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="8a839-754">Valid values 1 to 500</span></span>|
|<span data-ttu-id="8a839-755">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="8a839-755">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="8a839-756">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-756">Boolean</span></span>|<span data-ttu-id="8a839-757">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="8a839-757">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="8a839-758">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="8a839-758">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="8a839-759">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-759">Boolean</span></span>|<span data-ttu-id="8a839-760">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="8a839-760">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="8a839-761">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="8a839-761">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="8a839-762">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-762">Boolean</span></span>|<span data-ttu-id="8a839-763">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="8a839-763">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="8a839-764">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-764">windowsStoreBlocked</span></span>|<span data-ttu-id="8a839-765">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-765">Boolean</span></span>|<span data-ttu-id="8a839-766">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="8a839-766">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="8a839-767">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="8a839-767">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="8a839-768">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="8a839-768">stateManagementSetting</span></span>](../resources/intune_deviceconfig_statemanagementsetting.md)|<span data-ttu-id="8a839-p155">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p155">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded. The possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="8a839-771">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="8a839-771">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="8a839-772">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-772">Boolean</span></span>|<span data-ttu-id="8a839-773">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="8a839-773">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="8a839-774">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="8a839-774">developerUnlockSetting</span></span>|[<span data-ttu-id="8a839-775">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="8a839-775">stateManagementSetting</span></span>](../resources/intune_deviceconfig_statemanagementsetting.md)|<span data-ttu-id="8a839-p156">指示是否允许开发人员解锁。可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="8a839-p156">Indicates whether or not to allow developer unlock. The possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="8a839-778">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="8a839-778">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="8a839-779">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-779">Boolean</span></span>|<span data-ttu-id="8a839-780">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="8a839-780">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="8a839-781">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="8a839-781">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="8a839-782">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-782">Boolean</span></span>|<span data-ttu-id="8a839-783">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="8a839-783">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="8a839-784">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="8a839-784">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="8a839-785">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-785">Boolean</span></span>|<span data-ttu-id="8a839-786">指示是否启用“仅限私人应用商店”。</span><span class="sxs-lookup"><span data-stu-id="8a839-786">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="8a839-787">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="8a839-787">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="8a839-788">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-788">Boolean</span></span>|<span data-ttu-id="8a839-789">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="8a839-789">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="8a839-790">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="8a839-790">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="8a839-791">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-791">Boolean</span></span>|<span data-ttu-id="8a839-792">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="8a839-792">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="8a839-793">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="8a839-793">gameDvrBlocked</span></span>|<span data-ttu-id="8a839-794">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-794">Boolean</span></span>|<span data-ttu-id="8a839-795">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="8a839-795">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="8a839-796">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="8a839-796">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="8a839-797">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-797">Boolean</span></span>|<span data-ttu-id="8a839-798">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="8a839-798">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="8a839-799">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="8a839-799">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="8a839-800">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-800">Boolean</span></span>|<span data-ttu-id="8a839-801">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="8a839-801">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="8a839-802">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="8a839-802">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="8a839-803">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-803">Boolean</span></span>|<span data-ttu-id="8a839-804">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="8a839-804">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="8a839-805">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="8a839-805">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="8a839-806">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a839-806">Boolean</span></span>|<span data-ttu-id="8a839-807">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="8a839-807">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|



## <a name="response"></a><span data-ttu-id="8a839-808">响应</span><span class="sxs-lookup"><span data-stu-id="8a839-808">Response</span></span>
<span data-ttu-id="8a839-809">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a839-809">If successful, this method returns a `201 Created` response code and a [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a839-810">示例</span><span class="sxs-lookup"><span data-stu-id="8a839-810">Example</span></span>
### <a name="request"></a><span data-ttu-id="8a839-811">请求</span><span class="sxs-lookup"><span data-stu-id="8a839-811">Request</span></span>
<span data-ttu-id="8a839-812">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a839-812">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8a839-813">响应</span><span class="sxs-lookup"><span data-stu-id="8a839-813">Response</span></span>
<span data-ttu-id="8a839-p157">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8a839-p157">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








