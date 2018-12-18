---
title: windowsInformationProtection 资源类型
description: 用于配置详细管理设置的 Windows 信息保护策略
author: tfitzmac
ms.openlocfilehash: 86c1202636046320312cd12fb5d97b98937a2cec
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349222"
---
# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="81030-103">windowsInformationProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="81030-103">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="81030-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="81030-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81030-105">用于配置详细管理设置的 Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="81030-105">Policy for Windows information protection to configure detailed management settings</span></span>

<span data-ttu-id="81030-106">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81030-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="81030-107">方法</span><span class="sxs-lookup"><span data-stu-id="81030-107">Methods</span></span>
|<span data-ttu-id="81030-108">方法</span><span class="sxs-lookup"><span data-stu-id="81030-108">Method</span></span>|<span data-ttu-id="81030-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="81030-109">Return Type</span></span>|<span data-ttu-id="81030-110">说明</span><span class="sxs-lookup"><span data-stu-id="81030-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81030-111">List windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="81030-111">List windowsInformationProtections</span></span>](../api/intune-mam-windowsinformationprotection-list.md)|<span data-ttu-id="81030-112">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81030-112">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="81030-113">列出 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81030-113">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="81030-114">Get windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="81030-114">Get windowsInformationProtection</span></span>](../api/intune-mam-windowsinformationprotection-get.md)|[<span data-ttu-id="81030-115">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="81030-115">windowsInformationProtection</span></span>](../resources/intune-mam-windowsinformationprotection.md)|<span data-ttu-id="81030-116">读取 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81030-116">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="81030-117">assign 操作</span><span class="sxs-lookup"><span data-stu-id="81030-117">assign action</span></span>](../api/intune-mam-windowsinformationprotection-assign.md)|<span data-ttu-id="81030-118">无</span><span class="sxs-lookup"><span data-stu-id="81030-118">None</span></span>|<span data-ttu-id="81030-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="81030-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="81030-120">属性</span><span class="sxs-lookup"><span data-stu-id="81030-120">Properties</span></span>
|<span data-ttu-id="81030-121">属性</span><span class="sxs-lookup"><span data-stu-id="81030-121">Property</span></span>|<span data-ttu-id="81030-122">类型</span><span class="sxs-lookup"><span data-stu-id="81030-122">Type</span></span>|<span data-ttu-id="81030-123">说明</span><span class="sxs-lookup"><span data-stu-id="81030-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81030-124">displayName</span><span class="sxs-lookup"><span data-stu-id="81030-124">displayName</span></span>|<span data-ttu-id="81030-125">String</span><span class="sxs-lookup"><span data-stu-id="81030-125">String</span></span>|<span data-ttu-id="81030-126">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="81030-126">Policy display name.</span></span> <span data-ttu-id="81030-127">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81030-127">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81030-128">description</span><span class="sxs-lookup"><span data-stu-id="81030-128">description</span></span>|<span data-ttu-id="81030-129">String</span><span class="sxs-lookup"><span data-stu-id="81030-129">String</span></span>|<span data-ttu-id="81030-130">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="81030-130">The policy's description.</span></span> <span data-ttu-id="81030-131">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81030-131">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81030-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81030-132">createdDateTime</span></span>|<span data-ttu-id="81030-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81030-133">DateTimeOffset</span></span>|<span data-ttu-id="81030-134">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="81030-134">The date and time the policy was created.</span></span> <span data-ttu-id="81030-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81030-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81030-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81030-136">lastModifiedDateTime</span></span>|<span data-ttu-id="81030-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81030-137">DateTimeOffset</span></span>|<span data-ttu-id="81030-138">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="81030-138">Last time the policy was modified.</span></span> <span data-ttu-id="81030-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81030-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81030-140">id</span><span class="sxs-lookup"><span data-stu-id="81030-140">id</span></span>|<span data-ttu-id="81030-141">String</span><span class="sxs-lookup"><span data-stu-id="81030-141">String</span></span>|<span data-ttu-id="81030-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="81030-142">Key of the entity.</span></span> <span data-ttu-id="81030-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81030-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81030-144">version</span><span class="sxs-lookup"><span data-stu-id="81030-144">version</span></span>|<span data-ttu-id="81030-145">String</span><span class="sxs-lookup"><span data-stu-id="81030-145">String</span></span>|<span data-ttu-id="81030-146">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="81030-146">Version of the entity.</span></span> <span data-ttu-id="81030-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81030-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81030-148">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="81030-148">enforcementLevel</span></span>|[<span data-ttu-id="81030-149">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="81030-149">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="81030-150">WIP 实施级别。请参阅支持的值的枚举定义。</span><span class="sxs-lookup"><span data-stu-id="81030-150">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="81030-151">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="81030-151">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="81030-152">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="81030-152">enterpriseDomain</span></span>|<span data-ttu-id="81030-153">String</span><span class="sxs-lookup"><span data-stu-id="81030-153">String</span></span>|<span data-ttu-id="81030-154">主企业域</span><span class="sxs-lookup"><span data-stu-id="81030-154">Primary enterprise domain</span></span>|
|<span data-ttu-id="81030-155">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="81030-155">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="81030-156">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81030-156">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="81030-157">要保护的企业域列表</span><span class="sxs-lookup"><span data-stu-id="81030-157">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="81030-158">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="81030-158">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="81030-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="81030-159">Boolean</span></span>|<span data-ttu-id="81030-160">指定是否应配置锁定功能下的保护（也称为 pin 下的加密）</span><span class="sxs-lookup"><span data-stu-id="81030-160">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="81030-161">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="81030-161">dataRecoveryCertificate</span></span>|[<span data-ttu-id="81030-162">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="81030-162">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="81030-163">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="81030-163">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="81030-164">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。</span><span class="sxs-lookup"><span data-stu-id="81030-164">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="81030-165">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="81030-165">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="81030-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="81030-166">Boolean</span></span>|<span data-ttu-id="81030-167">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="81030-167">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="81030-168">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="81030-168">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="81030-169">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="81030-169">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="81030-170">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="81030-170">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="81030-171">Guid</span><span class="sxs-lookup"><span data-stu-id="81030-171">Guid</span></span>|<span data-ttu-id="81030-172">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="81030-172">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="81030-173">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。</span><span class="sxs-lookup"><span data-stu-id="81030-173">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="81030-174">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="81030-174">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="81030-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="81030-175">Boolean</span></span>|<span data-ttu-id="81030-176">指定是否允许 Azure RMS 加密用于 WIP。</span><span class="sxs-lookup"><span data-stu-id="81030-176">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="81030-177">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="81030-177">iconsVisible</span></span>|<span data-ttu-id="81030-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="81030-178">Boolean</span></span>|<span data-ttu-id="81030-179">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="81030-179">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="81030-180">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性</span><span class="sxs-lookup"><span data-stu-id="81030-180">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="81030-181">protectedApps</span><span class="sxs-lookup"><span data-stu-id="81030-181">protectedApps</span></span>|<span data-ttu-id="81030-182">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81030-182">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="81030-183">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护</span><span class="sxs-lookup"><span data-stu-id="81030-183">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="81030-184">exemptApps</span><span class="sxs-lookup"><span data-stu-id="81030-184">exemptApps</span></span>|<span data-ttu-id="81030-185">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81030-185">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="81030-186">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="81030-186">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="81030-187">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="81030-187">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="81030-188">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="81030-188">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="81030-189">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81030-189">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="81030-190">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="81030-190">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="81030-191">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。</span><span class="sxs-lookup"><span data-stu-id="81030-191">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="81030-192">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="81030-192">enterpriseProxiedDomains</span></span>|<span data-ttu-id="81030-193">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81030-193">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="81030-194">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="81030-194">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="81030-195">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="81030-195">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="81030-196">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="81030-196">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="81030-197">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。</span><span class="sxs-lookup"><span data-stu-id="81030-197">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="81030-198">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="81030-198">enterpriseIPRanges</span></span>|<span data-ttu-id="81030-199">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81030-199">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="81030-200">设置可定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="81030-200">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="81030-201">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="81030-201">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="81030-202">这些位置将被视为共享企业数据的安全目标</span><span class="sxs-lookup"><span data-stu-id="81030-202">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="81030-203">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="81030-203">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="81030-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="81030-204">Boolean</span></span>|<span data-ttu-id="81030-205">用于通知客户端接受已配置的列表，并且不使用试探法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="81030-205">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="81030-206">默认值为 false</span><span class="sxs-lookup"><span data-stu-id="81030-206">Default is false</span></span>|
|<span data-ttu-id="81030-207">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="81030-207">enterpriseProxyServers</span></span>|<span data-ttu-id="81030-208">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81030-208">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="81030-209">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="81030-209">This is a list of proxy servers.</span></span> <span data-ttu-id="81030-210">任何不在此列表中的服务器都被视为非企业服务器</span><span class="sxs-lookup"><span data-stu-id="81030-210">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="81030-211">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="81030-211">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="81030-212">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81030-212">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="81030-213">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="81030-213">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="81030-214">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="81030-214">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="81030-215">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="81030-215">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="81030-216">它们被视为是企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="81030-216">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="81030-217">代理仅在配置 EnterpriseProxiedDomains 策略时利用以强制流量通过这些代理传输到匹配的域</span><span class="sxs-lookup"><span data-stu-id="81030-217">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="81030-218">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="81030-218">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="81030-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="81030-219">Boolean</span></span>|<span data-ttu-id="81030-220">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="81030-220">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="81030-221">默认值为 false</span><span class="sxs-lookup"><span data-stu-id="81030-221">Default is false</span></span>|
|<span data-ttu-id="81030-222">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="81030-222">neutralDomainResources</span></span>|<span data-ttu-id="81030-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81030-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="81030-224">可用于工作或个人资源的域名列表</span><span class="sxs-lookup"><span data-stu-id="81030-224">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="81030-225">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="81030-225">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="81030-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="81030-226">Boolean</span></span>|<span data-ttu-id="81030-227">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引</span><span class="sxs-lookup"><span data-stu-id="81030-227">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="81030-228">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="81030-228">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="81030-229">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81030-229">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="81030-230">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件</span><span class="sxs-lookup"><span data-stu-id="81030-230">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="81030-231">isAssigned</span><span class="sxs-lookup"><span data-stu-id="81030-231">isAssigned</span></span>|<span data-ttu-id="81030-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="81030-232">Boolean</span></span>|<span data-ttu-id="81030-233">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="81030-233">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81030-234">关系</span><span class="sxs-lookup"><span data-stu-id="81030-234">Relationships</span></span>
|<span data-ttu-id="81030-235">关系</span><span class="sxs-lookup"><span data-stu-id="81030-235">Relationship</span></span>|<span data-ttu-id="81030-236">类型</span><span class="sxs-lookup"><span data-stu-id="81030-236">Type</span></span>|<span data-ttu-id="81030-237">说明</span><span class="sxs-lookup"><span data-stu-id="81030-237">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81030-238">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="81030-238">protectedAppLockerFiles</span></span>|<span data-ttu-id="81030-239">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81030-239">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="81030-240">通过 xml 文件输入受保护应用的另一种方法</span><span class="sxs-lookup"><span data-stu-id="81030-240">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="81030-241">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="81030-241">exemptAppLockerFiles</span></span>|<span data-ttu-id="81030-242">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81030-242">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="81030-243">通过 xml 文件输入豁免应用的另一种方法</span><span class="sxs-lookup"><span data-stu-id="81030-243">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="81030-244">assignments</span><span class="sxs-lookup"><span data-stu-id="81030-244">assignments</span></span>|<span data-ttu-id="81030-245">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81030-245">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="81030-246">针对策略的安全组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="81030-246">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81030-247">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81030-247">JSON Representation</span></span>
<span data-ttu-id="81030-248">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81030-248">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtection"
}
-->
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
  "rightsManagementServicesTemplateId": "Guid",
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



