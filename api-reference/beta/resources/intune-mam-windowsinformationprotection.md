---
title: windowsInformationProtection 资源类型
description: 用于配置详细管理设置的 Windows 信息保护策略
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41f288e360aaf7a086541fb483c93af5dc451942
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403159"
---
# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="499c9-103">windowsInformationProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="499c9-103">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="499c9-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="499c9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="499c9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="499c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="499c9-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="499c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="499c9-107">用于配置详细管理设置的 Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="499c9-107">Policy for Windows information protection to configure detailed management settings</span></span>


<span data-ttu-id="499c9-108">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="499c9-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="499c9-109">方法</span><span class="sxs-lookup"><span data-stu-id="499c9-109">Methods</span></span>
|<span data-ttu-id="499c9-110">方法</span><span class="sxs-lookup"><span data-stu-id="499c9-110">Method</span></span>|<span data-ttu-id="499c9-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="499c9-111">Return Type</span></span>|<span data-ttu-id="499c9-112">说明</span><span class="sxs-lookup"><span data-stu-id="499c9-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="499c9-113">List windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="499c9-113">List windowsInformationProtections</span></span>](../api/intune-mam-windowsinformationprotection-list.md)|<span data-ttu-id="499c9-114">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-114">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="499c9-115">列出 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="499c9-115">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="499c9-116">Get windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="499c9-116">Get windowsInformationProtection</span></span>](../api/intune-mam-windowsinformationprotection-get.md)|[<span data-ttu-id="499c9-117">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="499c9-117">windowsInformationProtection</span></span>](../resources/intune-mam-windowsinformationprotection.md)|<span data-ttu-id="499c9-118">读取 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="499c9-118">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="499c9-119">assign 操作</span><span class="sxs-lookup"><span data-stu-id="499c9-119">assign action</span></span>](../api/intune-mam-windowsinformationprotection-assign.md)|<span data-ttu-id="499c9-120">无</span><span class="sxs-lookup"><span data-stu-id="499c9-120">None</span></span>|<span data-ttu-id="499c9-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="499c9-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="499c9-122">属性</span><span class="sxs-lookup"><span data-stu-id="499c9-122">Properties</span></span>
|<span data-ttu-id="499c9-123">属性</span><span class="sxs-lookup"><span data-stu-id="499c9-123">Property</span></span>|<span data-ttu-id="499c9-124">类型</span><span class="sxs-lookup"><span data-stu-id="499c9-124">Type</span></span>|<span data-ttu-id="499c9-125">说明</span><span class="sxs-lookup"><span data-stu-id="499c9-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="499c9-126">displayName</span><span class="sxs-lookup"><span data-stu-id="499c9-126">displayName</span></span>|<span data-ttu-id="499c9-127">String</span><span class="sxs-lookup"><span data-stu-id="499c9-127">String</span></span>|<span data-ttu-id="499c9-128">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="499c9-128">Policy display name.</span></span> <span data-ttu-id="499c9-129">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="499c9-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="499c9-130">description</span><span class="sxs-lookup"><span data-stu-id="499c9-130">description</span></span>|<span data-ttu-id="499c9-131">String</span><span class="sxs-lookup"><span data-stu-id="499c9-131">String</span></span>|<span data-ttu-id="499c9-132">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="499c9-132">The policy's description.</span></span> <span data-ttu-id="499c9-133">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="499c9-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="499c9-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="499c9-134">createdDateTime</span></span>|<span data-ttu-id="499c9-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="499c9-135">DateTimeOffset</span></span>|<span data-ttu-id="499c9-136">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="499c9-136">The date and time the policy was created.</span></span> <span data-ttu-id="499c9-137">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="499c9-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="499c9-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="499c9-138">lastModifiedDateTime</span></span>|<span data-ttu-id="499c9-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="499c9-139">DateTimeOffset</span></span>|<span data-ttu-id="499c9-140">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="499c9-140">Last time the policy was modified.</span></span> <span data-ttu-id="499c9-141">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="499c9-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="499c9-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="499c9-142">roleScopeTagIds</span></span>|<span data-ttu-id="499c9-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-143">String collection</span></span>|<span data-ttu-id="499c9-144">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="499c9-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="499c9-145">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="499c9-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="499c9-146">id</span><span class="sxs-lookup"><span data-stu-id="499c9-146">id</span></span>|<span data-ttu-id="499c9-147">String</span><span class="sxs-lookup"><span data-stu-id="499c9-147">String</span></span>|<span data-ttu-id="499c9-148">实体的键。</span><span class="sxs-lookup"><span data-stu-id="499c9-148">Key of the entity.</span></span> <span data-ttu-id="499c9-149">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="499c9-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="499c9-150">version</span><span class="sxs-lookup"><span data-stu-id="499c9-150">version</span></span>|<span data-ttu-id="499c9-151">String</span><span class="sxs-lookup"><span data-stu-id="499c9-151">String</span></span>|<span data-ttu-id="499c9-152">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="499c9-152">Version of the entity.</span></span> <span data-ttu-id="499c9-153">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="499c9-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="499c9-154">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="499c9-154">enforcementLevel</span></span>|[<span data-ttu-id="499c9-155">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="499c9-155">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="499c9-156">WIP 实施级别。请参阅支持的值的枚举定义。</span><span class="sxs-lookup"><span data-stu-id="499c9-156">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="499c9-157">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="499c9-157">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="499c9-158">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="499c9-158">enterpriseDomain</span></span>|<span data-ttu-id="499c9-159">String</span><span class="sxs-lookup"><span data-stu-id="499c9-159">String</span></span>|<span data-ttu-id="499c9-160">主企业域</span><span class="sxs-lookup"><span data-stu-id="499c9-160">Primary enterprise domain</span></span>|
|<span data-ttu-id="499c9-161">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="499c9-161">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="499c9-162">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-162">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="499c9-163">要保护的企业域列表</span><span class="sxs-lookup"><span data-stu-id="499c9-163">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="499c9-164">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="499c9-164">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="499c9-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="499c9-165">Boolean</span></span>|<span data-ttu-id="499c9-166">指定是否应配置锁定功能下的保护（也称为 pin 下的加密）</span><span class="sxs-lookup"><span data-stu-id="499c9-166">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="499c9-167">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="499c9-167">dataRecoveryCertificate</span></span>|[<span data-ttu-id="499c9-168">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="499c9-168">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="499c9-169">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="499c9-169">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="499c9-170">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。</span><span class="sxs-lookup"><span data-stu-id="499c9-170">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="499c9-171">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="499c9-171">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="499c9-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="499c9-172">Boolean</span></span>|<span data-ttu-id="499c9-173">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="499c9-173">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="499c9-174">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="499c9-174">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="499c9-175">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="499c9-175">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="499c9-176">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="499c9-176">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="499c9-177">Guid</span><span class="sxs-lookup"><span data-stu-id="499c9-177">Guid</span></span>|<span data-ttu-id="499c9-178">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="499c9-178">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="499c9-179">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。</span><span class="sxs-lookup"><span data-stu-id="499c9-179">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="499c9-180">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="499c9-180">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="499c9-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="499c9-181">Boolean</span></span>|<span data-ttu-id="499c9-182">指定是否允许 Azure RMS 加密用于 WIP。</span><span class="sxs-lookup"><span data-stu-id="499c9-182">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="499c9-183">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="499c9-183">iconsVisible</span></span>|<span data-ttu-id="499c9-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="499c9-184">Boolean</span></span>|<span data-ttu-id="499c9-185">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="499c9-185">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="499c9-186">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性</span><span class="sxs-lookup"><span data-stu-id="499c9-186">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="499c9-187">protectedApps</span><span class="sxs-lookup"><span data-stu-id="499c9-187">protectedApps</span></span>|<span data-ttu-id="499c9-188">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-188">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="499c9-189">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护</span><span class="sxs-lookup"><span data-stu-id="499c9-189">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="499c9-190">exemptApps</span><span class="sxs-lookup"><span data-stu-id="499c9-190">exemptApps</span></span>|<span data-ttu-id="499c9-191">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-191">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="499c9-192">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="499c9-192">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="499c9-193">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="499c9-193">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="499c9-194">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="499c9-194">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="499c9-195">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-195">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="499c9-196">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="499c9-196">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="499c9-197">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。</span><span class="sxs-lookup"><span data-stu-id="499c9-197">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="499c9-198">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="499c9-198">enterpriseProxiedDomains</span></span>|<span data-ttu-id="499c9-199">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-199">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="499c9-200">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="499c9-200">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="499c9-201">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="499c9-201">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="499c9-202">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="499c9-202">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="499c9-203">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。</span><span class="sxs-lookup"><span data-stu-id="499c9-203">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="499c9-204">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="499c9-204">enterpriseIPRanges</span></span>|<span data-ttu-id="499c9-205">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-205">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="499c9-206">设置可定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="499c9-206">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="499c9-207">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="499c9-207">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="499c9-208">这些位置将被视为共享企业数据的安全目标</span><span class="sxs-lookup"><span data-stu-id="499c9-208">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="499c9-209">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="499c9-209">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="499c9-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="499c9-210">Boolean</span></span>|<span data-ttu-id="499c9-211">用于通知客户端接受已配置的列表，并且不使用试探法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="499c9-211">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="499c9-212">默认值为 false</span><span class="sxs-lookup"><span data-stu-id="499c9-212">Default is false</span></span>|
|<span data-ttu-id="499c9-213">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="499c9-213">enterpriseProxyServers</span></span>|<span data-ttu-id="499c9-214">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-214">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="499c9-215">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="499c9-215">This is a list of proxy servers.</span></span> <span data-ttu-id="499c9-216">任何不在此列表中的服务器都被视为非企业服务器</span><span class="sxs-lookup"><span data-stu-id="499c9-216">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="499c9-217">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="499c9-217">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="499c9-218">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-218">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="499c9-219">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="499c9-219">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="499c9-220">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="499c9-220">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="499c9-221">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="499c9-221">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="499c9-222">它们被视为是企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="499c9-222">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="499c9-223">代理仅在配置 EnterpriseProxiedDomains 策略时利用以强制流量通过这些代理传输到匹配的域</span><span class="sxs-lookup"><span data-stu-id="499c9-223">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="499c9-224">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="499c9-224">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="499c9-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="499c9-225">Boolean</span></span>|<span data-ttu-id="499c9-226">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="499c9-226">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="499c9-227">默认值为 false</span><span class="sxs-lookup"><span data-stu-id="499c9-227">Default is false</span></span>|
|<span data-ttu-id="499c9-228">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="499c9-228">neutralDomainResources</span></span>|<span data-ttu-id="499c9-229">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-229">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="499c9-230">可用于工作或个人资源的域名列表</span><span class="sxs-lookup"><span data-stu-id="499c9-230">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="499c9-231">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="499c9-231">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="499c9-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="499c9-232">Boolean</span></span>|<span data-ttu-id="499c9-233">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引</span><span class="sxs-lookup"><span data-stu-id="499c9-233">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="499c9-234">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="499c9-234">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="499c9-235">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-235">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="499c9-236">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件</span><span class="sxs-lookup"><span data-stu-id="499c9-236">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="499c9-237">isAssigned</span><span class="sxs-lookup"><span data-stu-id="499c9-237">isAssigned</span></span>|<span data-ttu-id="499c9-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="499c9-238">Boolean</span></span>|<span data-ttu-id="499c9-239">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="499c9-239">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="499c9-240">关系</span><span class="sxs-lookup"><span data-stu-id="499c9-240">Relationships</span></span>
|<span data-ttu-id="499c9-241">关系</span><span class="sxs-lookup"><span data-stu-id="499c9-241">Relationship</span></span>|<span data-ttu-id="499c9-242">类型</span><span class="sxs-lookup"><span data-stu-id="499c9-242">Type</span></span>|<span data-ttu-id="499c9-243">说明</span><span class="sxs-lookup"><span data-stu-id="499c9-243">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="499c9-244">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="499c9-244">protectedAppLockerFiles</span></span>|<span data-ttu-id="499c9-245">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-245">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="499c9-246">通过 xml 文件输入受保护应用的另一种方法</span><span class="sxs-lookup"><span data-stu-id="499c9-246">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="499c9-247">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="499c9-247">exemptAppLockerFiles</span></span>|<span data-ttu-id="499c9-248">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-248">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="499c9-249">通过 xml 文件输入豁免应用的另一种方法</span><span class="sxs-lookup"><span data-stu-id="499c9-249">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="499c9-250">assignments</span><span class="sxs-lookup"><span data-stu-id="499c9-250">assignments</span></span>|<span data-ttu-id="499c9-251">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="499c9-251">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="499c9-252">针对策略的安全组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="499c9-252">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="499c9-253">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="499c9-253">JSON Representation</span></span>
<span data-ttu-id="499c9-254">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="499c9-254">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
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
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
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




