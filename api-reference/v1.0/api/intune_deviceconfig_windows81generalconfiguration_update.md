# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="691fb-101">更新 windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="691fb-101">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="691fb-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="691fb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="691fb-103">更新 [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="691fb-103">Update the properties of a [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="691fb-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="691fb-104">Prerequisites</span></span>
<span data-ttu-id="691fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="691fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="691fb-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="691fb-107">Permission type</span></span>|<span data-ttu-id="691fb-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="691fb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="691fb-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="691fb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="691fb-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="691fb-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="691fb-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="691fb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="691fb-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="691fb-112">Not supported.</span></span>|
|<span data-ttu-id="691fb-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="691fb-113">Application</span></span>|<span data-ttu-id="691fb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="691fb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="691fb-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="691fb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="691fb-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="691fb-116">Request headers</span></span>
|<span data-ttu-id="691fb-117">标头</span><span class="sxs-lookup"><span data-stu-id="691fb-117">Header</span></span>|<span data-ttu-id="691fb-118">值</span><span class="sxs-lookup"><span data-stu-id="691fb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="691fb-119">授权</span><span class="sxs-lookup"><span data-stu-id="691fb-119">Authorization</span></span>|<span data-ttu-id="691fb-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="691fb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="691fb-121">接受</span><span class="sxs-lookup"><span data-stu-id="691fb-121">Accept</span></span>|<span data-ttu-id="691fb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="691fb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="691fb-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="691fb-123">Request body</span></span>
<span data-ttu-id="691fb-124">在请求正文中，提供 [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="691fb-124">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="691fb-125">下表显示了创建 [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="691fb-125">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="691fb-126">属性</span><span class="sxs-lookup"><span data-stu-id="691fb-126">Property</span></span>|<span data-ttu-id="691fb-127">类型</span><span class="sxs-lookup"><span data-stu-id="691fb-127">Type</span></span>|<span data-ttu-id="691fb-128">说明</span><span class="sxs-lookup"><span data-stu-id="691fb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="691fb-129">ID</span><span class="sxs-lookup"><span data-stu-id="691fb-129">id</span></span>|<span data-ttu-id="691fb-130">字符串</span><span class="sxs-lookup"><span data-stu-id="691fb-130">String</span></span>|<span data-ttu-id="691fb-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="691fb-131">Key of the entity.</span></span> <span data-ttu-id="691fb-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="691fb-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="691fb-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="691fb-133">lastModifiedDateTime</span></span>|<span data-ttu-id="691fb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="691fb-134">DateTimeOffset</span></span>|<span data-ttu-id="691fb-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="691fb-135">DateTime the object was last modified.</span></span> <span data-ttu-id="691fb-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="691fb-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="691fb-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="691fb-137">createdDateTime</span></span>|<span data-ttu-id="691fb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="691fb-138">DateTimeOffset</span></span>|<span data-ttu-id="691fb-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="691fb-139">DateTime the object was created.</span></span> <span data-ttu-id="691fb-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="691fb-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="691fb-141">描述</span><span class="sxs-lookup"><span data-stu-id="691fb-141">description</span></span>|<span data-ttu-id="691fb-142">字符串</span><span class="sxs-lookup"><span data-stu-id="691fb-142">String</span></span>|<span data-ttu-id="691fb-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="691fb-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="691fb-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="691fb-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="691fb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="691fb-145">displayName</span></span>|<span data-ttu-id="691fb-146">字符串</span><span class="sxs-lookup"><span data-stu-id="691fb-146">String</span></span>|<span data-ttu-id="691fb-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="691fb-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="691fb-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="691fb-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="691fb-149">版本</span><span class="sxs-lookup"><span data-stu-id="691fb-149">version</span></span>|<span data-ttu-id="691fb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="691fb-150">Int32</span></span>|<span data-ttu-id="691fb-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="691fb-151">Version of the device configuration.</span></span> <span data-ttu-id="691fb-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="691fb-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="691fb-153">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="691fb-153">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="691fb-154">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-154">Boolean</span></span>|<span data-ttu-id="691fb-155">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="691fb-155">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="691fb-156">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="691fb-156">applyOnlyToWindows81</span></span>|<span data-ttu-id="691fb-157">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-157">Boolean</span></span>|<span data-ttu-id="691fb-158">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="691fb-158">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="691fb-159">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="691fb-159">This property is read-only.</span></span>|
|<span data-ttu-id="691fb-160">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="691fb-160">browserBlockAutofill</span></span>|<span data-ttu-id="691fb-161">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-161">Boolean</span></span>|<span data-ttu-id="691fb-162">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="691fb-162">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="691fb-163">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="691fb-163">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="691fb-164">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-164">Boolean</span></span>|<span data-ttu-id="691fb-165">指示是否阻止自动检测 Intranet 站点。</span><span class="sxs-lookup"><span data-stu-id="691fb-165">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="691fb-166">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="691fb-166">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="691fb-167">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-167">Boolean</span></span>|<span data-ttu-id="691fb-168">指示是否阻止企业模式访问。</span><span class="sxs-lookup"><span data-stu-id="691fb-168">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="691fb-169">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="691fb-169">browserBlockJavaScript</span></span>|<span data-ttu-id="691fb-170">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-170">Boolean</span></span>|<span data-ttu-id="691fb-171">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="691fb-171">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="691fb-172">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="691fb-172">browserBlockPlugins</span></span>|<span data-ttu-id="691fb-173">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-173">Boolean</span></span>|<span data-ttu-id="691fb-174">指示是否阻止插件。</span><span class="sxs-lookup"><span data-stu-id="691fb-174">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="691fb-175">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="691fb-175">browserBlockPopups</span></span>|<span data-ttu-id="691fb-176">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-176">Boolean</span></span>|<span data-ttu-id="691fb-177">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="691fb-177">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="691fb-178">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="691fb-178">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="691fb-179">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-179">Boolean</span></span>|<span data-ttu-id="691fb-180">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="691fb-180">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="691fb-181">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="691fb-181">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="691fb-182">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-182">Boolean</span></span>|<span data-ttu-id="691fb-183">指示是否阻止在 Intranet 站点上使用单字条目。</span><span class="sxs-lookup"><span data-stu-id="691fb-183">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="691fb-184">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="691fb-184">browserRequireSmartScreen</span></span>|<span data-ttu-id="691fb-185">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-185">Boolean</span></span>|<span data-ttu-id="691fb-186">指示是否要求用户使用智能屏幕筛选器。</span><span class="sxs-lookup"><span data-stu-id="691fb-186">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="691fb-187">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="691fb-187">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="691fb-188">字符串</span><span class="sxs-lookup"><span data-stu-id="691fb-188">String</span></span>|<span data-ttu-id="691fb-189">企业模式网站列表位置。</span><span class="sxs-lookup"><span data-stu-id="691fb-189">The enterprise mode site list location.</span></span> <span data-ttu-id="691fb-190">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="691fb-190">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="691fb-191">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="691fb-191">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="691fb-192">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="691fb-192">internetSiteSecurityLevel</span></span>](../resources/intune_deviceconfig_internetsitesecuritylevel.md)|<span data-ttu-id="691fb-p110">互联网安全级别。可能的值是：`userDefined`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="691fb-p110">The internet security level. The possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="691fb-195">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="691fb-195">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="691fb-196">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="691fb-196">siteSecurityLevel</span></span>](../resources/intune_deviceconfig_sitesecuritylevel.md)|<span data-ttu-id="691fb-p111">互联网安全级别。可能的值是： `userDefined`, `low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="691fb-p111">The Intranet security level. The possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="691fb-199">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="691fb-199">browserLoggingReportLocation</span></span>|<span data-ttu-id="691fb-200">字符串</span><span class="sxs-lookup"><span data-stu-id="691fb-200">String</span></span>|<span data-ttu-id="691fb-201">日志记录报表位置。</span><span class="sxs-lookup"><span data-stu-id="691fb-201">The logging report location.</span></span>|
|<span data-ttu-id="691fb-202">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="691fb-202">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="691fb-203">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-203">Boolean</span></span>|<span data-ttu-id="691fb-204">指示是否要求受限站点具有高安全性。</span><span class="sxs-lookup"><span data-stu-id="691fb-204">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="691fb-205">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="691fb-205">browserRequireFirewall</span></span>|<span data-ttu-id="691fb-206">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-206">Boolean</span></span>|<span data-ttu-id="691fb-207">指示是否需要防火墙。</span><span class="sxs-lookup"><span data-stu-id="691fb-207">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="691fb-208">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="691fb-208">browserRequireFraudWarning</span></span>|<span data-ttu-id="691fb-209">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-209">Boolean</span></span>|<span data-ttu-id="691fb-210">指示是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="691fb-210">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="691fb-211">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="691fb-211">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="691fb-212">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="691fb-212">siteSecurityLevel</span></span>](../resources/intune_deviceconfig_sitesecuritylevel.md)|<span data-ttu-id="691fb-p112">受信任的站点安全级别。可能的值是：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="691fb-p112">The trusted sites security level. The possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="691fb-215">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="691fb-215">cellularBlockDataRoaming</span></span>|<span data-ttu-id="691fb-216">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-216">Boolean</span></span>|<span data-ttu-id="691fb-217">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="691fb-217">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="691fb-218">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="691fb-218">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="691fb-219">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-219">Boolean</span></span>|<span data-ttu-id="691fb-220">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="691fb-220">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="691fb-221">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="691fb-221">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="691fb-222">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-222">Boolean</span></span>|<span data-ttu-id="691fb-223">指示是否阻止用户使用图片密码和 PIN。</span><span class="sxs-lookup"><span data-stu-id="691fb-223">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="691fb-224">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="691fb-224">passwordExpirationDays</span></span>|<span data-ttu-id="691fb-225">Int32</span><span class="sxs-lookup"><span data-stu-id="691fb-225">Int32</span></span>|<span data-ttu-id="691fb-226">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="691fb-226">Password expiration in days.</span></span>|
|<span data-ttu-id="691fb-227">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="691fb-227">passwordMinimumLength</span></span>|<span data-ttu-id="691fb-228">Int32</span><span class="sxs-lookup"><span data-stu-id="691fb-228">Int32</span></span>|<span data-ttu-id="691fb-229">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="691fb-229">The minimum password length.</span></span>|
|<span data-ttu-id="691fb-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="691fb-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="691fb-231">Int32</span><span class="sxs-lookup"><span data-stu-id="691fb-231">Int32</span></span>|<span data-ttu-id="691fb-232">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="691fb-232">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="691fb-233">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="691fb-233">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="691fb-234">Int32</span><span class="sxs-lookup"><span data-stu-id="691fb-234">Int32</span></span>|<span data-ttu-id="691fb-235">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="691fb-235">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="691fb-236">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="691fb-236">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="691fb-237">Int32</span><span class="sxs-lookup"><span data-stu-id="691fb-237">Int32</span></span>|<span data-ttu-id="691fb-238">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="691fb-238">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="691fb-239">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="691fb-239">Valid values 0 to 24</span></span>|
|<span data-ttu-id="691fb-240">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="691fb-240">passwordRequiredType</span></span>|[<span data-ttu-id="691fb-241">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="691fb-241">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="691fb-p114">所需的密码类型。可取值是：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="691fb-p114">The required password type. The possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="691fb-244">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="691fb-244">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="691fb-245">Int32</span><span class="sxs-lookup"><span data-stu-id="691fb-245">Int32</span></span>|<span data-ttu-id="691fb-246">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="691fb-246">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="691fb-247">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="691fb-247">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="691fb-248">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-248">Boolean</span></span>|<span data-ttu-id="691fb-249">指示是否要求对移动设备加密。</span><span class="sxs-lookup"><span data-stu-id="691fb-249">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="691fb-250">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="691fb-250">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="691fb-251">布尔</span><span class="sxs-lookup"><span data-stu-id="691fb-251">Boolean</span></span>|<span data-ttu-id="691fb-252">指示是否需要自动更新。</span><span class="sxs-lookup"><span data-stu-id="691fb-252">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="691fb-253">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="691fb-253">userAccountControlSettings</span></span>|[<span data-ttu-id="691fb-254">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="691fb-254">windowsUserAccountControlSettings</span></span>](../resources/intune_deviceconfig_windowsuseraccountcontrolsettings.md)|<span data-ttu-id="691fb-p115">用户帐户控制设置。可能的值是：`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify`。</span><span class="sxs-lookup"><span data-stu-id="691fb-p115">The user account control settings. The possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="691fb-257">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="691fb-257">workFoldersUrl</span></span>|<span data-ttu-id="691fb-258">字符串</span><span class="sxs-lookup"><span data-stu-id="691fb-258">String</span></span>|<span data-ttu-id="691fb-259">工作文件夹 URL。</span><span class="sxs-lookup"><span data-stu-id="691fb-259">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="691fb-260">响应</span><span class="sxs-lookup"><span data-stu-id="691fb-260">Response</span></span>
<span data-ttu-id="691fb-261">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="691fb-261">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="691fb-262">示例</span><span class="sxs-lookup"><span data-stu-id="691fb-262">Example</span></span>
### <a name="request"></a><span data-ttu-id="691fb-263">请求</span><span class="sxs-lookup"><span data-stu-id="691fb-263">Request</span></span>
<span data-ttu-id="691fb-264">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="691fb-264">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1689

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="691fb-265">响应</span><span class="sxs-lookup"><span data-stu-id="691fb-265">Response</span></span>
<span data-ttu-id="691fb-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="691fb-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1865

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```








