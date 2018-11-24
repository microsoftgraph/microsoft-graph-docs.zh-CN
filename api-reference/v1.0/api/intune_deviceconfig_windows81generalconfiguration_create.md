# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="68993-101">创建 windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="68993-101">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="68993-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="68993-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68993-103">创建新的 [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="68993-103">Create a new [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68993-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="68993-104">Prerequisites</span></span>
<span data-ttu-id="68993-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="68993-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="68993-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="68993-107">Permission type</span></span>|<span data-ttu-id="68993-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="68993-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68993-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68993-109">Delegated (work or school account)</span></span>|<span data-ttu-id="68993-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68993-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="68993-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68993-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68993-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="68993-112">Not supported.</span></span>|
|<span data-ttu-id="68993-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="68993-113">Application</span></span>|<span data-ttu-id="68993-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="68993-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68993-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68993-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="68993-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="68993-116">Request headers</span></span>
|<span data-ttu-id="68993-117">标头</span><span class="sxs-lookup"><span data-stu-id="68993-117">Header</span></span>|<span data-ttu-id="68993-118">值</span><span class="sxs-lookup"><span data-stu-id="68993-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68993-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="68993-119">Authorization</span></span>|<span data-ttu-id="68993-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="68993-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68993-121">Accept</span><span class="sxs-lookup"><span data-stu-id="68993-121">Accept</span></span>|<span data-ttu-id="68993-122">application/json</span><span class="sxs-lookup"><span data-stu-id="68993-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68993-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="68993-123">Request body</span></span>
<span data-ttu-id="68993-124">在请求正文中，提供 windows81GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68993-124">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="68993-125">下表显示了创建 windows81GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="68993-125">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="68993-126">属性</span><span class="sxs-lookup"><span data-stu-id="68993-126">Property</span></span>|<span data-ttu-id="68993-127">类型</span><span class="sxs-lookup"><span data-stu-id="68993-127">Type</span></span>|<span data-ttu-id="68993-128">说明</span><span class="sxs-lookup"><span data-stu-id="68993-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68993-129">id</span><span class="sxs-lookup"><span data-stu-id="68993-129">id</span></span>|<span data-ttu-id="68993-130">String</span><span class="sxs-lookup"><span data-stu-id="68993-130">String</span></span>|<span data-ttu-id="68993-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="68993-131">Key of the entity.</span></span> <span data-ttu-id="68993-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68993-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68993-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68993-133">lastModifiedDateTime</span></span>|<span data-ttu-id="68993-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68993-134">DateTimeOffset</span></span>|<span data-ttu-id="68993-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="68993-135">DateTime the object was last modified.</span></span> <span data-ttu-id="68993-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68993-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68993-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="68993-137">createdDateTime</span></span>|<span data-ttu-id="68993-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68993-138">DateTimeOffset</span></span>|<span data-ttu-id="68993-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="68993-139">DateTime the object was created.</span></span> <span data-ttu-id="68993-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68993-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68993-141">description</span><span class="sxs-lookup"><span data-stu-id="68993-141">description</span></span>|<span data-ttu-id="68993-142">String</span><span class="sxs-lookup"><span data-stu-id="68993-142">String</span></span>|<span data-ttu-id="68993-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="68993-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="68993-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68993-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68993-145">displayName</span><span class="sxs-lookup"><span data-stu-id="68993-145">displayName</span></span>|<span data-ttu-id="68993-146">String</span><span class="sxs-lookup"><span data-stu-id="68993-146">String</span></span>|<span data-ttu-id="68993-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="68993-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="68993-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68993-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68993-149">version</span><span class="sxs-lookup"><span data-stu-id="68993-149">version</span></span>|<span data-ttu-id="68993-150">Int32</span><span class="sxs-lookup"><span data-stu-id="68993-150">Int32</span></span>|<span data-ttu-id="68993-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="68993-151">Version of the device configuration.</span></span> <span data-ttu-id="68993-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="68993-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68993-153">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="68993-153">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="68993-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-154">Boolean</span></span>|<span data-ttu-id="68993-155">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="68993-155">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="68993-156">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="68993-156">applyOnlyToWindows81</span></span>|<span data-ttu-id="68993-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-157">Boolean</span></span>|<span data-ttu-id="68993-158">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="68993-158">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="68993-159">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="68993-159">This property is read-only.</span></span>|
|<span data-ttu-id="68993-160">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="68993-160">browserBlockAutofill</span></span>|<span data-ttu-id="68993-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-161">Boolean</span></span>|<span data-ttu-id="68993-162">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="68993-162">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="68993-163">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="68993-163">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="68993-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-164">Boolean</span></span>|<span data-ttu-id="68993-165">指示是否阻止自动检测 Intranet 站点。</span><span class="sxs-lookup"><span data-stu-id="68993-165">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="68993-166">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="68993-166">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="68993-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-167">Boolean</span></span>|<span data-ttu-id="68993-168">指示是否阻止企业模式访问。</span><span class="sxs-lookup"><span data-stu-id="68993-168">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="68993-169">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="68993-169">browserBlockJavaScript</span></span>|<span data-ttu-id="68993-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-170">Boolean</span></span>|<span data-ttu-id="68993-171">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="68993-171">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="68993-172">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="68993-172">browserBlockPlugins</span></span>|<span data-ttu-id="68993-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-173">Boolean</span></span>|<span data-ttu-id="68993-174">指示是否阻止插件。</span><span class="sxs-lookup"><span data-stu-id="68993-174">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="68993-175">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="68993-175">browserBlockPopups</span></span>|<span data-ttu-id="68993-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-176">Boolean</span></span>|<span data-ttu-id="68993-177">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="68993-177">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="68993-178">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="68993-178">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="68993-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-179">Boolean</span></span>|<span data-ttu-id="68993-180">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="68993-180">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="68993-181">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="68993-181">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="68993-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-182">Boolean</span></span>|<span data-ttu-id="68993-183">指示是否阻止在 Intranet 站点上使用单字条目。</span><span class="sxs-lookup"><span data-stu-id="68993-183">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="68993-184">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="68993-184">browserRequireSmartScreen</span></span>|<span data-ttu-id="68993-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-185">Boolean</span></span>|<span data-ttu-id="68993-186">指示是否要求用户使用智能屏幕筛选器。</span><span class="sxs-lookup"><span data-stu-id="68993-186">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="68993-187">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="68993-187">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="68993-188">String</span><span class="sxs-lookup"><span data-stu-id="68993-188">String</span></span>|<span data-ttu-id="68993-189">企业模式网站列表位置。</span><span class="sxs-lookup"><span data-stu-id="68993-189">The enterprise mode site list location.</span></span> <span data-ttu-id="68993-190">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="68993-190">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="68993-191">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="68993-191">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="68993-192">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="68993-192">internetSiteSecurityLevel</span></span>](../resources/intune_deviceconfig_internetsitesecuritylevel.md)|<span data-ttu-id="68993-193">Internet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="68993-193">The internet security level.</span></span> <span data-ttu-id="68993-194">可取值为：`userDefined`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="68993-194">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="68993-195">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="68993-195">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="68993-196">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="68993-196">siteSecurityLevel</span></span>](../resources/intune_deviceconfig_sitesecuritylevel.md)|<span data-ttu-id="68993-197">Intranet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="68993-197">The Intranet security level.</span></span> <span data-ttu-id="68993-198">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="68993-198">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="68993-199">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="68993-199">browserLoggingReportLocation</span></span>|<span data-ttu-id="68993-200">String</span><span class="sxs-lookup"><span data-stu-id="68993-200">String</span></span>|<span data-ttu-id="68993-201">日志记录报表位置。</span><span class="sxs-lookup"><span data-stu-id="68993-201">The logging report location.</span></span>|
|<span data-ttu-id="68993-202">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="68993-202">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="68993-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-203">Boolean</span></span>|<span data-ttu-id="68993-204">指示是否要求受限站点具有高安全性。</span><span class="sxs-lookup"><span data-stu-id="68993-204">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="68993-205">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="68993-205">browserRequireFirewall</span></span>|<span data-ttu-id="68993-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-206">Boolean</span></span>|<span data-ttu-id="68993-207">指示是否需要防火墙。</span><span class="sxs-lookup"><span data-stu-id="68993-207">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="68993-208">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="68993-208">browserRequireFraudWarning</span></span>|<span data-ttu-id="68993-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-209">Boolean</span></span>|<span data-ttu-id="68993-210">指示是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="68993-210">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="68993-211">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="68993-211">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="68993-212">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="68993-212">siteSecurityLevel</span></span>](../resources/intune_deviceconfig_sitesecuritylevel.md)|<span data-ttu-id="68993-213">受信任的站点安全级别。</span><span class="sxs-lookup"><span data-stu-id="68993-213">The trusted sites security level.</span></span> <span data-ttu-id="68993-214">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="68993-214">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="68993-215">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="68993-215">cellularBlockDataRoaming</span></span>|<span data-ttu-id="68993-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-216">Boolean</span></span>|<span data-ttu-id="68993-217">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="68993-217">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="68993-218">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="68993-218">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="68993-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-219">Boolean</span></span>|<span data-ttu-id="68993-220">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="68993-220">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="68993-221">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="68993-221">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="68993-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-222">Boolean</span></span>|<span data-ttu-id="68993-223">指示是否阻止用户使用图片密码和 PIN。</span><span class="sxs-lookup"><span data-stu-id="68993-223">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="68993-224">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="68993-224">passwordExpirationDays</span></span>|<span data-ttu-id="68993-225">Int32</span><span class="sxs-lookup"><span data-stu-id="68993-225">Int32</span></span>|<span data-ttu-id="68993-226">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="68993-226">Password expiration in days.</span></span>|
|<span data-ttu-id="68993-227">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="68993-227">passwordMinimumLength</span></span>|<span data-ttu-id="68993-228">Int32</span><span class="sxs-lookup"><span data-stu-id="68993-228">Int32</span></span>|<span data-ttu-id="68993-229">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="68993-229">The minimum password length.</span></span>|
|<span data-ttu-id="68993-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="68993-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="68993-231">Int32</span><span class="sxs-lookup"><span data-stu-id="68993-231">Int32</span></span>|<span data-ttu-id="68993-232">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="68993-232">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="68993-233">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="68993-233">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="68993-234">Int32</span><span class="sxs-lookup"><span data-stu-id="68993-234">Int32</span></span>|<span data-ttu-id="68993-235">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="68993-235">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="68993-236">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="68993-236">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="68993-237">Int32</span><span class="sxs-lookup"><span data-stu-id="68993-237">Int32</span></span>|<span data-ttu-id="68993-238">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="68993-238">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="68993-239">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="68993-239">Valid values 0 to 24</span></span>|
|<span data-ttu-id="68993-240">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="68993-240">passwordRequiredType</span></span>|[<span data-ttu-id="68993-241">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="68993-241">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="68993-242">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="68993-242">The required password type.</span></span> <span data-ttu-id="68993-243">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="68993-243">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="68993-244">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="68993-244">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="68993-245">Int32</span><span class="sxs-lookup"><span data-stu-id="68993-245">Int32</span></span>|<span data-ttu-id="68993-246">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="68993-246">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="68993-247">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="68993-247">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="68993-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-248">Boolean</span></span>|<span data-ttu-id="68993-249">指示是否要求对移动设备加密。</span><span class="sxs-lookup"><span data-stu-id="68993-249">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="68993-250">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="68993-250">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="68993-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="68993-251">Boolean</span></span>|<span data-ttu-id="68993-252">指示是否需要自动更新。</span><span class="sxs-lookup"><span data-stu-id="68993-252">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="68993-253">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="68993-253">userAccountControlSettings</span></span>|[<span data-ttu-id="68993-254">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="68993-254">windowsUserAccountControlSettings</span></span>](../resources/intune_deviceconfig_windowsuseraccountcontrolsettings.md)|<span data-ttu-id="68993-255">用户帐户控制设置。</span><span class="sxs-lookup"><span data-stu-id="68993-255">The user account control settings.</span></span> <span data-ttu-id="68993-256">可取值为：`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify`。</span><span class="sxs-lookup"><span data-stu-id="68993-256">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="68993-257">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="68993-257">workFoldersUrl</span></span>|<span data-ttu-id="68993-258">String</span><span class="sxs-lookup"><span data-stu-id="68993-258">String</span></span>|<span data-ttu-id="68993-259">工作文件夹 URL。</span><span class="sxs-lookup"><span data-stu-id="68993-259">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="68993-260">响应</span><span class="sxs-lookup"><span data-stu-id="68993-260">Response</span></span>
<span data-ttu-id="68993-261">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="68993-261">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68993-262">示例</span><span class="sxs-lookup"><span data-stu-id="68993-262">Example</span></span>
### <a name="request"></a><span data-ttu-id="68993-263">请求</span><span class="sxs-lookup"><span data-stu-id="68993-263">Request</span></span>
<span data-ttu-id="68993-264">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="68993-264">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1693

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="68993-265">响应</span><span class="sxs-lookup"><span data-stu-id="68993-265">Response</span></span>
<span data-ttu-id="68993-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="68993-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



