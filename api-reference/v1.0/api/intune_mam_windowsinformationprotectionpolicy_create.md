# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="26a9c-101">创建 windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="26a9c-101">Create windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="26a9c-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="26a9c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26a9c-103">创建新的 [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="26a9c-103">Create a new [plannerBucket](../resources/intune_mam_windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="26a9c-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="26a9c-104">Prerequisites</span></span>
<span data-ttu-id="26a9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="26a9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="26a9c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="26a9c-107">Permission type</span></span>|<span data-ttu-id="26a9c-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="26a9c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26a9c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26a9c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="26a9c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26a9c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="26a9c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26a9c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26a9c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="26a9c-112">Not supported.</span></span>|
|<span data-ttu-id="26a9c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="26a9c-113">Application</span></span>|<span data-ttu-id="26a9c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="26a9c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26a9c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26a9c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="26a9c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="26a9c-116">Request headers</span></span>
|<span data-ttu-id="26a9c-117">标头</span><span class="sxs-lookup"><span data-stu-id="26a9c-117">Header</span></span>|<span data-ttu-id="26a9c-118">值</span><span class="sxs-lookup"><span data-stu-id="26a9c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26a9c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="26a9c-119">Authorization</span></span>|<span data-ttu-id="26a9c-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="26a9c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="26a9c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="26a9c-121">Accept</span></span>|<span data-ttu-id="26a9c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="26a9c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26a9c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="26a9c-123">Request body</span></span>
<span data-ttu-id="26a9c-124">在请求正文中，提供 windowsInformationProtectionPolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26a9c-124">In the request body, supply a JSON representation of calendar object.</span></span>

<span data-ttu-id="26a9c-125">下表显示创建 windowsInformationProtectionPolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="26a9c-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="26a9c-126">属性</span><span class="sxs-lookup"><span data-stu-id="26a9c-126">Property</span></span>|<span data-ttu-id="26a9c-127">类型</span><span class="sxs-lookup"><span data-stu-id="26a9c-127">Type</span></span>|<span data-ttu-id="26a9c-128">说明</span><span class="sxs-lookup"><span data-stu-id="26a9c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26a9c-129">displayName</span><span class="sxs-lookup"><span data-stu-id="26a9c-129">displayName</span></span>|<span data-ttu-id="26a9c-130">String</span><span class="sxs-lookup"><span data-stu-id="26a9c-130">String</span></span>|<span data-ttu-id="26a9c-131">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="26a9c-131">Policy display name.</span></span> <span data-ttu-id="26a9c-132">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="26a9c-133">description</span><span class="sxs-lookup"><span data-stu-id="26a9c-133">description</span></span>|<span data-ttu-id="26a9c-134">String</span><span class="sxs-lookup"><span data-stu-id="26a9c-134">String</span></span>|<span data-ttu-id="26a9c-135">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="26a9c-135">The policy's description.</span></span> <span data-ttu-id="26a9c-136">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="26a9c-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26a9c-137">createdDateTime</span></span>|<span data-ttu-id="26a9c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26a9c-138">DateTimeOffset</span></span>|<span data-ttu-id="26a9c-139">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="26a9c-139">The date and time when the page was created.</span></span> <span data-ttu-id="26a9c-140">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="26a9c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26a9c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="26a9c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26a9c-142">DateTimeOffset</span></span>|<span data-ttu-id="26a9c-143">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="26a9c-143">Last time the policy was modified.</span></span> <span data-ttu-id="26a9c-144">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="26a9c-145">id</span><span class="sxs-lookup"><span data-stu-id="26a9c-145">id</span></span>|<span data-ttu-id="26a9c-146">String</span><span class="sxs-lookup"><span data-stu-id="26a9c-146">String</span></span>|<span data-ttu-id="26a9c-147">实体的键。</span><span class="sxs-lookup"><span data-stu-id="26a9c-147">Key of the setting.</span></span> <span data-ttu-id="26a9c-148">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="26a9c-149">version</span><span class="sxs-lookup"><span data-stu-id="26a9c-149">version</span></span>|<span data-ttu-id="26a9c-150">String</span><span class="sxs-lookup"><span data-stu-id="26a9c-150">String</span></span>|<span data-ttu-id="26a9c-151">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="26a9c-151">Version of the entity.</span></span> <span data-ttu-id="26a9c-152">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="26a9c-153">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="26a9c-153">enforcementLevel</span></span>|<span data-ttu-id="26a9c-154">String</span><span class="sxs-lookup"><span data-stu-id="26a9c-154">String</span></span>|<span data-ttu-id="26a9c-155">WIP 强制级别。有关受支持的值，请参阅枚举定义。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)。可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="26a9c-155">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="26a9c-156">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="26a9c-156">enterpriseDomain</span></span>|<span data-ttu-id="26a9c-157">String</span><span class="sxs-lookup"><span data-stu-id="26a9c-157">String</span></span>|<span data-ttu-id="26a9c-158">主企业域。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-158">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-159">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="26a9c-159">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="26a9c-160">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26a9c-160">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="26a9c-161">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-161">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-162">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="26a9c-162">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="26a9c-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a9c-163">Boolean</span></span>|<span data-ttu-id="26a9c-164">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-164">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-165">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="26a9c-165">dataRecoveryCertificate</span></span>|[<span data-ttu-id="26a9c-166">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="26a9c-166">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="26a9c-167">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="26a9c-167">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="26a9c-168">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-168">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-169">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="26a9c-169">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="26a9c-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a9c-170">Boolean</span></span>|<span data-ttu-id="26a9c-171">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="26a9c-171">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="26a9c-172">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="26a9c-172">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="26a9c-173">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="26a9c-173">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="26a9c-174">继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-174">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-175">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="26a9c-175">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="26a9c-176">Guid</span><span class="sxs-lookup"><span data-stu-id="26a9c-176">Guid</span></span>|<span data-ttu-id="26a9c-177">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="26a9c-177">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="26a9c-178">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-178">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-179">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="26a9c-179">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="26a9c-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a9c-180">Boolean</span></span>|<span data-ttu-id="26a9c-181">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-181">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-182">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="26a9c-182">iconsVisible</span></span>|<span data-ttu-id="26a9c-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a9c-183">Boolean</span></span>|<span data-ttu-id="26a9c-184">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="26a9c-184">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="26a9c-185">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-185">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-186">protectedApps</span><span class="sxs-lookup"><span data-stu-id="26a9c-186">protectedApps</span></span>|<span data-ttu-id="26a9c-187">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26a9c-187">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="26a9c-188">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-188">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-189">exemptApps</span><span class="sxs-lookup"><span data-stu-id="26a9c-189">exemptApps</span></span>|<span data-ttu-id="26a9c-190">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26a9c-190">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="26a9c-191">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="26a9c-191">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="26a9c-192">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="26a9c-192">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="26a9c-193">继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-193">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-194">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="26a9c-194">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="26a9c-195">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26a9c-195">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="26a9c-196">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="26a9c-196">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="26a9c-197">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-197">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-198">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="26a9c-198">enterpriseProxiedDomains</span></span>|<span data-ttu-id="26a9c-199">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26a9c-199">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="26a9c-200">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="26a9c-200">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="26a9c-201">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="26a9c-201">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="26a9c-202">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="26a9c-202">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="26a9c-203">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-203">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-204">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="26a9c-204">enterpriseIPRanges</span></span>|<span data-ttu-id="26a9c-205">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26a9c-205">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="26a9c-206">设置定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="26a9c-206">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="26a9c-207">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="26a9c-207">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="26a9c-208">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-208">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-209">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="26a9c-209">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="26a9c-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a9c-210">Boolean</span></span>|<span data-ttu-id="26a9c-211">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="26a9c-211">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="26a9c-212">默认值为 false。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-212">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-213">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="26a9c-213">enterpriseProxyServers</span></span>|<span data-ttu-id="26a9c-214">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26a9c-214">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="26a9c-215">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="26a9c-215">This is a list of proxy servers.</span></span> <span data-ttu-id="26a9c-216">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-216">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-217">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="26a9c-217">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="26a9c-218">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26a9c-218">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="26a9c-219">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="26a9c-219">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="26a9c-220">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="26a9c-220">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="26a9c-221">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="26a9c-221">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="26a9c-222">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="26a9c-222">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="26a9c-223">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-223">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-224">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="26a9c-224">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="26a9c-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a9c-225">Boolean</span></span>|<span data-ttu-id="26a9c-226">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="26a9c-226">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="26a9c-227">默认值为 false。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-227">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-228">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="26a9c-228">neutralDomainResources</span></span>|<span data-ttu-id="26a9c-229">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26a9c-229">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="26a9c-230">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-230">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-231">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="26a9c-231">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="26a9c-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a9c-232">Boolean</span></span>|<span data-ttu-id="26a9c-233">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-233">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-234">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="26a9c-234">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="26a9c-235">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26a9c-235">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="26a9c-236">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-236">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-237">isAssigned</span><span class="sxs-lookup"><span data-stu-id="26a9c-237">isAssigned</span></span>|<span data-ttu-id="26a9c-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a9c-238">Boolean</span></span>|<span data-ttu-id="26a9c-239">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="26a9c-239">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="26a9c-240">继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="26a9c-240">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="26a9c-241">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="26a9c-241">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="26a9c-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a9c-242">Boolean</span></span>|<span data-ttu-id="26a9c-243">RS2 中的新属性，待定文档</span><span class="sxs-lookup"><span data-stu-id="26a9c-243">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="26a9c-244">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="26a9c-244">mdmEnrollmentUrl</span></span>|<span data-ttu-id="26a9c-245">String</span><span class="sxs-lookup"><span data-stu-id="26a9c-245">String</span></span>|<span data-ttu-id="26a9c-246">MDM 的注册 URL</span><span class="sxs-lookup"><span data-stu-id="26a9c-246">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="26a9c-247">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="26a9c-247">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="26a9c-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a9c-248">Boolean</span></span>|<span data-ttu-id="26a9c-249">将 Windows Hello 企业版设置为登录 Windows 的方法的布尔值。</span><span class="sxs-lookup"><span data-stu-id="26a9c-249">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="26a9c-250">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="26a9c-250">pinMinimumLength</span></span>|<span data-ttu-id="26a9c-251">Int32</span><span class="sxs-lookup"><span data-stu-id="26a9c-251">Int32</span></span>|<span data-ttu-id="26a9c-252">整数值，用于设置 PIN 所需的最少字符数。</span><span class="sxs-lookup"><span data-stu-id="26a9c-252">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="26a9c-253">默认值为 4。</span><span class="sxs-lookup"><span data-stu-id="26a9c-253">Default value is 4.</span></span> <span data-ttu-id="26a9c-254">可以为此策略设置配置的最小数量为 4。</span><span class="sxs-lookup"><span data-stu-id="26a9c-254">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="26a9c-255">可以配置的最大数量必须小于最大 PIN 长度策略设置中配置的数量或 127（以最低者为准）。</span><span class="sxs-lookup"><span data-stu-id="26a9c-255">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="26a9c-256">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="26a9c-256">pinUppercaseLetters</span></span>|<span data-ttu-id="26a9c-257">String</span><span class="sxs-lookup"><span data-stu-id="26a9c-257">String</span></span>|<span data-ttu-id="26a9c-258">整数值，用于配置 Windows Hello 企业版 PIN 中的大写字母的使用。</span><span class="sxs-lookup"><span data-stu-id="26a9c-258">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="26a9c-259">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="26a9c-259">Default is NotAllow.</span></span> <span data-ttu-id="26a9c-260">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="26a9c-260">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="26a9c-261">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="26a9c-261">pinLowercaseLetters</span></span>|<span data-ttu-id="26a9c-262">String</span><span class="sxs-lookup"><span data-stu-id="26a9c-262">String</span></span>|<span data-ttu-id="26a9c-263">整数值，用于配置 Windows Hello 企业版 PIN 中的小写字母的使用。</span><span class="sxs-lookup"><span data-stu-id="26a9c-263">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="26a9c-264">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="26a9c-264">Default is NotAllow.</span></span> <span data-ttu-id="26a9c-265">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="26a9c-265">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="26a9c-266">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="26a9c-266">pinSpecialCharacters</span></span>|<span data-ttu-id="26a9c-267">String</span><span class="sxs-lookup"><span data-stu-id="26a9c-267">String</span></span>|<span data-ttu-id="26a9c-268">整数值，用于配置 Windows Hello 企业版 PIN 中的特殊字母的使用。</span><span class="sxs-lookup"><span data-stu-id="26a9c-268">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="26a9c-269">Windows Hello 企业版 PIN 手势的有效特殊字符包括：!</span><span class="sxs-lookup"><span data-stu-id="26a9c-269">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="26a9c-270">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="26a9c-270">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="26a9c-271">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="26a9c-271">/ : ; < = > ?</span></span><span data-ttu-id="26a9c-272"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="26a9c-272"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="26a9c-273">} ~。</span><span class="sxs-lookup"><span data-stu-id="26a9c-273">=, ==</span></span> <span data-ttu-id="26a9c-274">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="26a9c-274">Default is NotAllow.</span></span> <span data-ttu-id="26a9c-275">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="26a9c-275">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="26a9c-276">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="26a9c-276">pinExpirationDays</span></span>|<span data-ttu-id="26a9c-277">Int32</span><span class="sxs-lookup"><span data-stu-id="26a9c-277">Int32</span></span>|<span data-ttu-id="26a9c-278">整数值指定在系统要求用户更改 PIN 之前可以使用 PIN 的时间段（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="26a9c-278">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="26a9c-279">可以为此策略设置配置的最大数量为 730。</span><span class="sxs-lookup"><span data-stu-id="26a9c-279">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="26a9c-280">可以为此策略设置配置的最小数量为 0。</span><span class="sxs-lookup"><span data-stu-id="26a9c-280">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="26a9c-281">如果此策略设置为 0，则用户的 PIN 永远不会过期。</span><span class="sxs-lookup"><span data-stu-id="26a9c-281">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="26a9c-282">此节点在 Windows 10 版本 1511 中添加。</span><span class="sxs-lookup"><span data-stu-id="26a9c-282">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="26a9c-283">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="26a9c-283">Default is 0.</span></span>|
|<span data-ttu-id="26a9c-284">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="26a9c-284">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="26a9c-285">Int32</span><span class="sxs-lookup"><span data-stu-id="26a9c-285">Int32</span></span>|<span data-ttu-id="26a9c-286">整数值，用于指定可以关联到无法重用的用户帐户的过去 PIN 的数量。</span><span class="sxs-lookup"><span data-stu-id="26a9c-286">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="26a9c-287">可以为此策略设置配置的最大数量为 50。</span><span class="sxs-lookup"><span data-stu-id="26a9c-287">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="26a9c-288">可以为此策略设置配置的最小数量为 0。</span><span class="sxs-lookup"><span data-stu-id="26a9c-288">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="26a9c-289">如果此策略设置为 0，则不需要存储以前的 PIN。</span><span class="sxs-lookup"><span data-stu-id="26a9c-289">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="26a9c-290">此节点在 Windows 10 版本 1511 中添加。</span><span class="sxs-lookup"><span data-stu-id="26a9c-290">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="26a9c-291">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="26a9c-291">Default is 0.</span></span>|
|<span data-ttu-id="26a9c-292">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="26a9c-292">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="26a9c-293">Int32</span><span class="sxs-lookup"><span data-stu-id="26a9c-293">Int32</span></span>|<span data-ttu-id="26a9c-294">在擦除设备之前允许的身份验证失败次数。</span><span class="sxs-lookup"><span data-stu-id="26a9c-294">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="26a9c-295">值为 0 将禁用设备擦除功能。</span><span class="sxs-lookup"><span data-stu-id="26a9c-295">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="26a9c-296">范围是一个整数 X，其中对于台式机 4 <= X <= 16，对于移动设备 0 <= X <= 999。</span><span class="sxs-lookup"><span data-stu-id="26a9c-296">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="26a9c-297">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="26a9c-297">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="26a9c-298">Int32</span><span class="sxs-lookup"><span data-stu-id="26a9c-298">Int32</span></span>|<span data-ttu-id="26a9c-299">指定设备闲置后将导致设备变为 PIN 或密码锁定的允许的最长时间（以分钟为单位）。</span><span class="sxs-lookup"><span data-stu-id="26a9c-299">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="26a9c-300">范围是整数 X，其中 0 < = X < = 999。</span><span class="sxs-lookup"><span data-stu-id="26a9c-300">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="26a9c-301">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="26a9c-301">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="26a9c-302">Int32</span><span class="sxs-lookup"><span data-stu-id="26a9c-302">Int32</span></span>|<span data-ttu-id="26a9c-303">擦除应用数据之前的脱机间隔时间（天）</span><span class="sxs-lookup"><span data-stu-id="26a9c-303">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="26a9c-304">响应</span><span class="sxs-lookup"><span data-stu-id="26a9c-304">Response</span></span>
<span data-ttu-id="26a9c-305">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="26a9c-305">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_mam_windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26a9c-306">示例</span><span class="sxs-lookup"><span data-stu-id="26a9c-306">Example</span></span>
### <a name="request"></a><span data-ttu-id="26a9c-307">请求</span><span class="sxs-lookup"><span data-stu-id="26a9c-307">Request</span></span>
<span data-ttu-id="26a9c-308">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="26a9c-308">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4466

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": "Version value",
  "enforcementLevel": "encryptAndAuditOnly",
  "enterpriseDomain": "Enterprise Domain value",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "Subject Name value",
    "description": "Description value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificate": "Y2VydGlmaWNhdGU="
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "Display Name value",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "Ip Address Or FQDN value",
          "proxy": "Proxy value"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "Display Name value",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 0,
  "pinUppercaseLetters": "requireAtLeastOne",
  "pinLowercaseLetters": "requireAtLeastOne",
  "pinSpecialCharacters": "requireAtLeastOne",
  "pinExpirationDays": 1,
  "numberOfPastPinsRemembered": 10,
  "passwordMaximumAttemptCount": 11,
  "minutesOfInactivityBeforeDeviceLock": 3,
  "daysWithoutContactBeforeUnenroll": 0
}
```

### <a name="response"></a><span data-ttu-id="26a9c-309">响应</span><span class="sxs-lookup"><span data-stu-id="26a9c-309">Response</span></span>
<span data-ttu-id="26a9c-p130">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="26a9c-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4574

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "6397be61-be61-6397-61be-976361be9763",
  "version": "Version value",
  "enforcementLevel": "encryptAndAuditOnly",
  "enterpriseDomain": "Enterprise Domain value",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "Subject Name value",
    "description": "Description value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificate": "Y2VydGlmaWNhdGU="
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "Display Name value",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "Ip Address Or FQDN value",
          "proxy": "Proxy value"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "Display Name value",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 0,
  "pinUppercaseLetters": "requireAtLeastOne",
  "pinLowercaseLetters": "requireAtLeastOne",
  "pinSpecialCharacters": "requireAtLeastOne",
  "pinExpirationDays": 1,
  "numberOfPastPinsRemembered": 10,
  "passwordMaximumAttemptCount": 11,
  "minutesOfInactivityBeforeDeviceLock": 3,
  "daysWithoutContactBeforeUnenroll": 0
}
```



