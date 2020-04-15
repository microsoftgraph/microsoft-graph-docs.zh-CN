---
title: windowsInformationProtection 资源类型
description: 用于配置详细管理设置的 Windows 信息保护策略
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1b8deab3dfaebc87b95035ef9f474f27783aa507
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443511"
---
# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="ed8d1-103">windowsInformationProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed8d1-103">windowsInformationProtection resource type</span></span>

<span data-ttu-id="ed8d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed8d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed8d1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed8d1-106">用于配置详细管理设置的 Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="ed8d1-106">Policy for Windows information protection to configure detailed management settings</span></span>


<span data-ttu-id="ed8d1-107">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ed8d1-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ed8d1-108">方法</span><span class="sxs-lookup"><span data-stu-id="ed8d1-108">Methods</span></span>
|<span data-ttu-id="ed8d1-109">方法</span><span class="sxs-lookup"><span data-stu-id="ed8d1-109">Method</span></span>|<span data-ttu-id="ed8d1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ed8d1-110">Return Type</span></span>|<span data-ttu-id="ed8d1-111">说明</span><span class="sxs-lookup"><span data-stu-id="ed8d1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ed8d1-112">List windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="ed8d1-112">List windowsInformationProtections</span></span>](../api/intune-mam-windowsinformationprotection-list.md)|<span data-ttu-id="ed8d1-113">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed8d1-113">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="ed8d1-114">列出 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-114">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="ed8d1-115">Get windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="ed8d1-115">Get windowsInformationProtection</span></span>](../api/intune-mam-windowsinformationprotection-get.md)|[<span data-ttu-id="ed8d1-116">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="ed8d1-116">windowsInformationProtection</span></span>](../resources/intune-mam-windowsinformationprotection.md)|<span data-ttu-id="ed8d1-117">读取 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-117">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="ed8d1-118">assign 操作</span><span class="sxs-lookup"><span data-stu-id="ed8d1-118">assign action</span></span>](../api/intune-mam-windowsinformationprotection-assign.md)|<span data-ttu-id="ed8d1-119">无</span><span class="sxs-lookup"><span data-stu-id="ed8d1-119">None</span></span>|<span data-ttu-id="ed8d1-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ed8d1-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ed8d1-121">属性</span><span class="sxs-lookup"><span data-stu-id="ed8d1-121">Properties</span></span>
|<span data-ttu-id="ed8d1-122">属性</span><span class="sxs-lookup"><span data-stu-id="ed8d1-122">Property</span></span>|<span data-ttu-id="ed8d1-123">类型</span><span class="sxs-lookup"><span data-stu-id="ed8d1-123">Type</span></span>|<span data-ttu-id="ed8d1-124">说明</span><span class="sxs-lookup"><span data-stu-id="ed8d1-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed8d1-125">displayName</span><span class="sxs-lookup"><span data-stu-id="ed8d1-125">displayName</span></span>|<span data-ttu-id="ed8d1-126">字符串</span><span class="sxs-lookup"><span data-stu-id="ed8d1-126">String</span></span>|<span data-ttu-id="ed8d1-127">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-127">Policy display name.</span></span> <span data-ttu-id="ed8d1-128">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ed8d1-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ed8d1-129">description</span><span class="sxs-lookup"><span data-stu-id="ed8d1-129">description</span></span>|<span data-ttu-id="ed8d1-130">String</span><span class="sxs-lookup"><span data-stu-id="ed8d1-130">String</span></span>|<span data-ttu-id="ed8d1-131">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-131">The policy's description.</span></span> <span data-ttu-id="ed8d1-132">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ed8d1-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ed8d1-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed8d1-133">createdDateTime</span></span>|<span data-ttu-id="ed8d1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed8d1-134">DateTimeOffset</span></span>|<span data-ttu-id="ed8d1-135">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-135">The date and time the policy was created.</span></span> <span data-ttu-id="ed8d1-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ed8d1-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ed8d1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed8d1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ed8d1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed8d1-138">DateTimeOffset</span></span>|<span data-ttu-id="ed8d1-139">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-139">Last time the policy was modified.</span></span> <span data-ttu-id="ed8d1-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ed8d1-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ed8d1-141">id</span><span class="sxs-lookup"><span data-stu-id="ed8d1-141">id</span></span>|<span data-ttu-id="ed8d1-142">字符串</span><span class="sxs-lookup"><span data-stu-id="ed8d1-142">String</span></span>|<span data-ttu-id="ed8d1-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-143">Key of the entity.</span></span> <span data-ttu-id="ed8d1-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ed8d1-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ed8d1-145">version</span><span class="sxs-lookup"><span data-stu-id="ed8d1-145">version</span></span>|<span data-ttu-id="ed8d1-146">String</span><span class="sxs-lookup"><span data-stu-id="ed8d1-146">String</span></span>|<span data-ttu-id="ed8d1-147">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-147">Version of the entity.</span></span> <span data-ttu-id="ed8d1-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ed8d1-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ed8d1-149">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="ed8d1-149">enforcementLevel</span></span>|[<span data-ttu-id="ed8d1-150">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="ed8d1-150">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="ed8d1-151">WIP 强制等级。有关受支持的值，请参阅枚举定义。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-151">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="ed8d1-152">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-152">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="ed8d1-153">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="ed8d1-153">enterpriseDomain</span></span>|<span data-ttu-id="ed8d1-154">String</span><span class="sxs-lookup"><span data-stu-id="ed8d1-154">String</span></span>|<span data-ttu-id="ed8d1-155">主企业域</span><span class="sxs-lookup"><span data-stu-id="ed8d1-155">Primary enterprise domain</span></span>|
|<span data-ttu-id="ed8d1-156">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="ed8d1-156">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="ed8d1-157">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed8d1-157">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="ed8d1-158">要保护的企业域列表</span><span class="sxs-lookup"><span data-stu-id="ed8d1-158">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="ed8d1-159">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="ed8d1-159">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="ed8d1-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed8d1-160">Boolean</span></span>|<span data-ttu-id="ed8d1-161">指定是否应配置锁定功能下的保护（也称为 pin 下的加密）</span><span class="sxs-lookup"><span data-stu-id="ed8d1-161">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="ed8d1-162">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="ed8d1-162">dataRecoveryCertificate</span></span>|[<span data-ttu-id="ed8d1-163">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="ed8d1-163">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="ed8d1-164">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-164">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="ed8d1-165">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-165">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="ed8d1-166">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="ed8d1-166">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="ed8d1-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed8d1-167">Boolean</span></span>|<span data-ttu-id="ed8d1-168">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-168">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="ed8d1-169">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-169">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="ed8d1-170">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-170">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="ed8d1-171">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="ed8d1-171">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="ed8d1-172">Guid</span><span class="sxs-lookup"><span data-stu-id="ed8d1-172">Guid</span></span>|<span data-ttu-id="ed8d1-173">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-173">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="ed8d1-174">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-174">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="ed8d1-175">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="ed8d1-175">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="ed8d1-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed8d1-176">Boolean</span></span>|<span data-ttu-id="ed8d1-177">指定是否允许 Azure RMS 加密用于 WIP。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-177">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="ed8d1-178">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="ed8d1-178">iconsVisible</span></span>|<span data-ttu-id="ed8d1-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed8d1-179">Boolean</span></span>|<span data-ttu-id="ed8d1-180">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-180">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="ed8d1-181">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性</span><span class="sxs-lookup"><span data-stu-id="ed8d1-181">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="ed8d1-182">protectedApps</span><span class="sxs-lookup"><span data-stu-id="ed8d1-182">protectedApps</span></span>|<span data-ttu-id="ed8d1-183">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed8d1-183">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="ed8d1-184">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护</span><span class="sxs-lookup"><span data-stu-id="ed8d1-184">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="ed8d1-185">exemptApps</span><span class="sxs-lookup"><span data-stu-id="ed8d1-185">exemptApps</span></span>|<span data-ttu-id="ed8d1-186">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed8d1-186">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="ed8d1-187">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-187">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="ed8d1-188">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-188">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="ed8d1-189">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="ed8d1-189">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="ed8d1-190">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed8d1-190">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="ed8d1-191">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-191">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="ed8d1-192">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-192">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="ed8d1-193">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="ed8d1-193">enterpriseProxiedDomains</span></span>|<span data-ttu-id="ed8d1-194">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed8d1-194">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="ed8d1-195">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-195">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="ed8d1-196">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-196">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="ed8d1-197">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-197">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="ed8d1-198">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-198">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="ed8d1-199">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="ed8d1-199">enterpriseIPRanges</span></span>|<span data-ttu-id="ed8d1-200">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed8d1-200">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="ed8d1-201">设置定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-201">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="ed8d1-202">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-202">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="ed8d1-203">这些位置将被视为共享企业数据的安全目标</span><span class="sxs-lookup"><span data-stu-id="ed8d1-203">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="ed8d1-204">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="ed8d1-204">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="ed8d1-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed8d1-205">Boolean</span></span>|<span data-ttu-id="ed8d1-206">用于通知客户端接受已配置的列表，并且不使用试探法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-206">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="ed8d1-207">默认值为 false</span><span class="sxs-lookup"><span data-stu-id="ed8d1-207">Default is false</span></span>|
|<span data-ttu-id="ed8d1-208">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="ed8d1-208">enterpriseProxyServers</span></span>|<span data-ttu-id="ed8d1-209">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed8d1-209">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="ed8d1-210">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-210">This is a list of proxy servers.</span></span> <span data-ttu-id="ed8d1-211">任何不在此列表中的服务器都被视为非企业服务器</span><span class="sxs-lookup"><span data-stu-id="ed8d1-211">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="ed8d1-212">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="ed8d1-212">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="ed8d1-213">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed8d1-213">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="ed8d1-214">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-214">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="ed8d1-215">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-215">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="ed8d1-216">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-216">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="ed8d1-217">它们被视为是企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-217">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="ed8d1-218">代理仅在配置 EnterpriseProxiedDomains 策略时利用以强制流量通过这些代理传输到匹配的域</span><span class="sxs-lookup"><span data-stu-id="ed8d1-218">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="ed8d1-219">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="ed8d1-219">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="ed8d1-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed8d1-220">Boolean</span></span>|<span data-ttu-id="ed8d1-221">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-221">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="ed8d1-222">默认值为 false</span><span class="sxs-lookup"><span data-stu-id="ed8d1-222">Default is false</span></span>|
|<span data-ttu-id="ed8d1-223">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="ed8d1-223">neutralDomainResources</span></span>|<span data-ttu-id="ed8d1-224">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed8d1-224">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="ed8d1-225">可用于工作或个人资源的域名列表</span><span class="sxs-lookup"><span data-stu-id="ed8d1-225">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="ed8d1-226">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="ed8d1-226">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="ed8d1-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed8d1-227">Boolean</span></span>|<span data-ttu-id="ed8d1-228">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引</span><span class="sxs-lookup"><span data-stu-id="ed8d1-228">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="ed8d1-229">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="ed8d1-229">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="ed8d1-230">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed8d1-230">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="ed8d1-231">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件</span><span class="sxs-lookup"><span data-stu-id="ed8d1-231">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="ed8d1-232">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ed8d1-232">isAssigned</span></span>|<span data-ttu-id="ed8d1-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed8d1-233">Boolean</span></span>|<span data-ttu-id="ed8d1-234">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-234">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed8d1-235">关系</span><span class="sxs-lookup"><span data-stu-id="ed8d1-235">Relationships</span></span>
|<span data-ttu-id="ed8d1-236">关系</span><span class="sxs-lookup"><span data-stu-id="ed8d1-236">Relationship</span></span>|<span data-ttu-id="ed8d1-237">类型</span><span class="sxs-lookup"><span data-stu-id="ed8d1-237">Type</span></span>|<span data-ttu-id="ed8d1-238">说明</span><span class="sxs-lookup"><span data-stu-id="ed8d1-238">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed8d1-239">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="ed8d1-239">protectedAppLockerFiles</span></span>|<span data-ttu-id="ed8d1-240">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed8d1-240">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="ed8d1-241">通过 xml 文件输入受保护应用的另一种方法</span><span class="sxs-lookup"><span data-stu-id="ed8d1-241">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="ed8d1-242">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="ed8d1-242">exemptAppLockerFiles</span></span>|<span data-ttu-id="ed8d1-243">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed8d1-243">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="ed8d1-244">通过 xml 文件输入豁免应用的另一种方法</span><span class="sxs-lookup"><span data-stu-id="ed8d1-244">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="ed8d1-245">assignments</span><span class="sxs-lookup"><span data-stu-id="ed8d1-245">assignments</span></span>|<span data-ttu-id="ed8d1-246">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed8d1-246">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="ed8d1-247">针对策略的安全组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-247">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed8d1-248">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed8d1-248">JSON Representation</span></span>
<span data-ttu-id="ed8d1-249">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed8d1-249">Here is a JSON representation of the resource.</span></span>
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







