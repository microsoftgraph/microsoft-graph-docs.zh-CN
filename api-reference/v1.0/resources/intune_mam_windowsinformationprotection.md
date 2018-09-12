# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="587c8-101">windowsInformationProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="587c8-101">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="587c8-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="587c8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="587c8-103">用于配置详细管理设置的 Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="587c8-103">Policy for Windows information protection to configure detailed management settings</span></span>

<span data-ttu-id="587c8-104">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="587c8-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="587c8-105">方法</span><span class="sxs-lookup"><span data-stu-id="587c8-105">Methods</span></span>
|<span data-ttu-id="587c8-106">方法</span><span class="sxs-lookup"><span data-stu-id="587c8-106">Method</span></span>|<span data-ttu-id="587c8-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="587c8-107">Return Type</span></span>|<span data-ttu-id="587c8-108">说明</span><span class="sxs-lookup"><span data-stu-id="587c8-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="587c8-109">列举 windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="587c8-109">List windowsInformationProtections</span></span>](../api/intune_mam_windowsinformationprotection_list.md)|<span data-ttu-id="587c8-110">[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="587c8-110">[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="587c8-111">列出 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="587c8-111">List properties and relationships of the [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="587c8-112">获取 windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="587c8-112">Get windowsInformationProtection</span></span>](../api/intune_mam_windowsinformationprotection_get.md)|[<span data-ttu-id="587c8-113">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="587c8-113">windowsInformationProtection</span></span>](../resources/intune_mam_windowsinformationprotection.md)|<span data-ttu-id="587c8-114">读取 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="587c8-114">Read properties and relationships of the [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="587c8-115">assign 操作</span><span class="sxs-lookup"><span data-stu-id="587c8-115">assign action</span></span>](../api/intune_mam_windowsinformationprotection_assign.md)|<span data-ttu-id="587c8-116">无</span><span class="sxs-lookup"><span data-stu-id="587c8-116">None</span></span>|<span data-ttu-id="587c8-117">尚未记录</span><span class="sxs-lookup"><span data-stu-id="587c8-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="587c8-118">属性</span><span class="sxs-lookup"><span data-stu-id="587c8-118">Properties</span></span>
|<span data-ttu-id="587c8-119">属性</span><span class="sxs-lookup"><span data-stu-id="587c8-119">Property</span></span>|<span data-ttu-id="587c8-120">类型</span><span class="sxs-lookup"><span data-stu-id="587c8-120">Type</span></span>|<span data-ttu-id="587c8-121">说明</span><span class="sxs-lookup"><span data-stu-id="587c8-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="587c8-122">displayName</span><span class="sxs-lookup"><span data-stu-id="587c8-122">displayName</span></span>|<span data-ttu-id="587c8-123">字符串</span><span class="sxs-lookup"><span data-stu-id="587c8-123">String</span></span>|<span data-ttu-id="587c8-124">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="587c8-124">Policy display name.</span></span> <span data-ttu-id="587c8-125">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="587c8-125">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="587c8-126">说明</span><span class="sxs-lookup"><span data-stu-id="587c8-126">description</span></span>|<span data-ttu-id="587c8-127">字符串</span><span class="sxs-lookup"><span data-stu-id="587c8-127">String</span></span>|<span data-ttu-id="587c8-128">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="587c8-128">The policy's description.</span></span> <span data-ttu-id="587c8-129">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="587c8-129">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="587c8-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="587c8-130">createdDateTime</span></span>|<span data-ttu-id="587c8-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="587c8-131">DateTimeOffset</span></span>|<span data-ttu-id="587c8-132">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="587c8-132">The date and time the policy was created.</span></span> <span data-ttu-id="587c8-133">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="587c8-133">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="587c8-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="587c8-134">lastModifiedDateTime</span></span>|<span data-ttu-id="587c8-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="587c8-135">DateTimeOffset</span></span>|<span data-ttu-id="587c8-136">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="587c8-136">Last time the policy was modified.</span></span> <span data-ttu-id="587c8-137">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="587c8-137">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="587c8-138">id</span><span class="sxs-lookup"><span data-stu-id="587c8-138">id</span></span>|<span data-ttu-id="587c8-139">字符串</span><span class="sxs-lookup"><span data-stu-id="587c8-139">String</span></span>|<span data-ttu-id="587c8-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="587c8-140">Key of the entity.</span></span> <span data-ttu-id="587c8-141">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="587c8-141">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="587c8-142">版本</span><span class="sxs-lookup"><span data-stu-id="587c8-142">version</span></span>|<span data-ttu-id="587c8-143">字符串</span><span class="sxs-lookup"><span data-stu-id="587c8-143">String</span></span>|<span data-ttu-id="587c8-144">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="587c8-144">Version of the entity.</span></span> <span data-ttu-id="587c8-145">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="587c8-145">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="587c8-146">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="587c8-146">enforcementLevel</span></span>|[<span data-ttu-id="587c8-147">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="587c8-147">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune_mam_windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="587c8-p107">WIP 强制级别。有关受支持的值，请参阅枚举定义。可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="587c8-p107">WIP enforcement level.See the Enum definition for supported values Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="587c8-150">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="587c8-150">enterpriseDomain</span></span>|<span data-ttu-id="587c8-151">字符串</span><span class="sxs-lookup"><span data-stu-id="587c8-151">String</span></span>|<span data-ttu-id="587c8-152">主企业域</span><span class="sxs-lookup"><span data-stu-id="587c8-152">Primary enterprise domain</span></span>|
|<span data-ttu-id="587c8-153">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="587c8-153">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="587c8-154">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="587c8-154">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="587c8-155">要保护的企业域列表</span><span class="sxs-lookup"><span data-stu-id="587c8-155">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="587c8-156">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="587c8-156">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="587c8-157">布尔值</span><span class="sxs-lookup"><span data-stu-id="587c8-157">Boolean</span></span>|<span data-ttu-id="587c8-158">指定是否应配置锁定功能下的保护（也称为 pin 下的加密）</span><span class="sxs-lookup"><span data-stu-id="587c8-158">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="587c8-159">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="587c8-159">dataRecoveryCertificate</span></span>|[<span data-ttu-id="587c8-160">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="587c8-160">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="587c8-161">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="587c8-161">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="587c8-162">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。</span><span class="sxs-lookup"><span data-stu-id="587c8-162">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="587c8-163">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="587c8-163">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="587c8-164">布尔值</span><span class="sxs-lookup"><span data-stu-id="587c8-164">Boolean</span></span>|<span data-ttu-id="587c8-165">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="587c8-165">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="587c8-166">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="587c8-166">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="587c8-167">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="587c8-167">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="587c8-168">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="587c8-168">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="587c8-169">全局唯一标识符</span><span class="sxs-lookup"><span data-stu-id="587c8-169">Guid</span></span>|<span data-ttu-id="587c8-170">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="587c8-170">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="587c8-171">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。</span><span class="sxs-lookup"><span data-stu-id="587c8-171">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="587c8-172">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="587c8-172">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="587c8-173">布尔值</span><span class="sxs-lookup"><span data-stu-id="587c8-173">Boolean</span></span>|<span data-ttu-id="587c8-174">指定是否允许 Azure RMS 加密用于 WIP。</span><span class="sxs-lookup"><span data-stu-id="587c8-174">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="587c8-175">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="587c8-175">iconsVisible</span></span>|<span data-ttu-id="587c8-176">布尔值</span><span class="sxs-lookup"><span data-stu-id="587c8-176">Boolean</span></span>|<span data-ttu-id="587c8-177">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="587c8-177">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="587c8-178">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性</span><span class="sxs-lookup"><span data-stu-id="587c8-178">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="587c8-179">protectedApps</span><span class="sxs-lookup"><span data-stu-id="587c8-179">protectedApps</span></span>|<span data-ttu-id="587c8-180">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="587c8-180">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="587c8-181">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护</span><span class="sxs-lookup"><span data-stu-id="587c8-181">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="587c8-182">exemptApps</span><span class="sxs-lookup"><span data-stu-id="587c8-182">exemptApps</span></span>|<span data-ttu-id="587c8-183">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="587c8-183">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="587c8-184">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="587c8-184">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="587c8-185">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="587c8-185">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="587c8-186">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="587c8-186">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="587c8-187">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="587c8-187">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="587c8-188">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="587c8-188">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="587c8-189">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。</span><span class="sxs-lookup"><span data-stu-id="587c8-189">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="587c8-190">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="587c8-190">enterpriseProxiedDomains</span></span>|<span data-ttu-id="587c8-191">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="587c8-191">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="587c8-192">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="587c8-192">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="587c8-193">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="587c8-193">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="587c8-194">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="587c8-194">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="587c8-195">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。</span><span class="sxs-lookup"><span data-stu-id="587c8-195">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="587c8-196">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="587c8-196">enterpriseIPRanges</span></span>|<span data-ttu-id="587c8-197">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="587c8-197">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="587c8-198">设置可定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="587c8-198">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="587c8-199">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="587c8-199">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="587c8-200">这些位置将被视为共享企业数据的安全目标</span><span class="sxs-lookup"><span data-stu-id="587c8-200">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="587c8-201">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="587c8-201">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="587c8-202">布尔值</span><span class="sxs-lookup"><span data-stu-id="587c8-202">Boolean</span></span>|<span data-ttu-id="587c8-203">用于通知客户端接受已配置的列表，并且不使用试探法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="587c8-203">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="587c8-204">默认值为 false</span><span class="sxs-lookup"><span data-stu-id="587c8-204">Default is false</span></span>|
|<span data-ttu-id="587c8-205">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="587c8-205">enterpriseProxyServers</span></span>|<span data-ttu-id="587c8-206">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="587c8-206">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="587c8-207">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="587c8-207">This is a list of proxy servers.</span></span> <span data-ttu-id="587c8-208">任何不在此列表中的服务器都被视为非企业服务器</span><span class="sxs-lookup"><span data-stu-id="587c8-208">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="587c8-209">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="587c8-209">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="587c8-210">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="587c8-210">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="587c8-211">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="587c8-211">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="587c8-212">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="587c8-212">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="587c8-213">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="587c8-213">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="587c8-214">它们被视为是企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="587c8-214">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="587c8-215">代理仅在配置 EnterpriseProxiedDomains 策略时利用以强制流量通过这些代理传输到匹配的域</span><span class="sxs-lookup"><span data-stu-id="587c8-215">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="587c8-216">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="587c8-216">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="587c8-217">布尔值</span><span class="sxs-lookup"><span data-stu-id="587c8-217">Boolean</span></span>|<span data-ttu-id="587c8-218">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="587c8-218">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="587c8-219">默认值为 false</span><span class="sxs-lookup"><span data-stu-id="587c8-219">Default is false</span></span>|
|<span data-ttu-id="587c8-220">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="587c8-220">neutralDomainResources</span></span>|<span data-ttu-id="587c8-221">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="587c8-221">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="587c8-222">可用于工作或个人资源的域名列表</span><span class="sxs-lookup"><span data-stu-id="587c8-222">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="587c8-223">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="587c8-223">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="587c8-224">布尔值</span><span class="sxs-lookup"><span data-stu-id="587c8-224">Boolean</span></span>|<span data-ttu-id="587c8-225">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引</span><span class="sxs-lookup"><span data-stu-id="587c8-225">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="587c8-226">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="587c8-226">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="587c8-227">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="587c8-227">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="587c8-228">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件</span><span class="sxs-lookup"><span data-stu-id="587c8-228">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="587c8-229">isAssigned</span><span class="sxs-lookup"><span data-stu-id="587c8-229">isAssigned</span></span>|<span data-ttu-id="587c8-230">布尔值</span><span class="sxs-lookup"><span data-stu-id="587c8-230">Boolean</span></span>|<span data-ttu-id="587c8-231">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="587c8-231">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="587c8-232">关系</span><span class="sxs-lookup"><span data-stu-id="587c8-232">Relationships</span></span>
|<span data-ttu-id="587c8-233">关系</span><span class="sxs-lookup"><span data-stu-id="587c8-233">Relationship</span></span>|<span data-ttu-id="587c8-234">类型</span><span class="sxs-lookup"><span data-stu-id="587c8-234">Type</span></span>|<span data-ttu-id="587c8-235">说明</span><span class="sxs-lookup"><span data-stu-id="587c8-235">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="587c8-236">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="587c8-236">protectedAppLockerFiles</span></span>|<span data-ttu-id="587c8-237">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="587c8-237">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="587c8-238">通过 xml 文件输入受保护应用的另一种方法</span><span class="sxs-lookup"><span data-stu-id="587c8-238">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="587c8-239">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="587c8-239">exemptAppLockerFiles</span></span>|<span data-ttu-id="587c8-240">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="587c8-240">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="587c8-241">通过 xml 文件输入豁免应用的另一种方法</span><span class="sxs-lookup"><span data-stu-id="587c8-241">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="587c8-242">赋值</span><span class="sxs-lookup"><span data-stu-id="587c8-242">assignments</span></span>|<span data-ttu-id="587c8-243">[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="587c8-243">[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="587c8-244">针对策略的安全组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="587c8-244">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="587c8-245">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="587c8-245">JSON Representation</span></span>
<span data-ttu-id="587c8-246">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="587c8-246">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedAppPolicy",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "description": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "String",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "String",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "isAssigned": true
}
```








