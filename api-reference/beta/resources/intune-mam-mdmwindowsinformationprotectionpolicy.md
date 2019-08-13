---
title: mdmWindowsInformationProtectionPolicy 资源类型
description: 使用 MDM 进行 Windows 信息保护的策略
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 05e2c56fffd7c804038f77b60f20c2b1ccb17f3d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372998"
---
# <a name="mdmwindowsinformationprotectionpolicy-resource-type"></a><span data-ttu-id="e1819-103">mdmWindowsInformationProtectionPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1819-103">mdmWindowsInformationProtectionPolicy resource type</span></span>

> <span data-ttu-id="e1819-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e1819-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1819-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1819-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1819-106">使用 MDM 进行 Windows 信息保护的策略</span><span class="sxs-lookup"><span data-stu-id="e1819-106">Policy for Windows information protection with MDM</span></span>


<span data-ttu-id="e1819-107">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-107">Inherits from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e1819-108">方法</span><span class="sxs-lookup"><span data-stu-id="e1819-108">Methods</span></span>
|<span data-ttu-id="e1819-109">方法</span><span class="sxs-lookup"><span data-stu-id="e1819-109">Method</span></span>|<span data-ttu-id="e1819-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e1819-110">Return Type</span></span>|<span data-ttu-id="e1819-111">说明</span><span class="sxs-lookup"><span data-stu-id="e1819-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e1819-112">List mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="e1819-112">List mdmWindowsInformationProtectionPolicies</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-list.md)|<span data-ttu-id="e1819-113">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1819-113">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) collection</span></span>|<span data-ttu-id="e1819-114">列出 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e1819-114">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>|
|[<span data-ttu-id="e1819-115">Get mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e1819-115">Get mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-get.md)|[<span data-ttu-id="e1819-116">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e1819-116">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="e1819-117">读取 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e1819-117">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|[<span data-ttu-id="e1819-118">Create mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e1819-118">Create mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-create.md)|[<span data-ttu-id="e1819-119">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e1819-119">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="e1819-120">创建新的 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e1819-120">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|[<span data-ttu-id="e1819-121">Delete mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e1819-121">Delete mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-delete.md)|<span data-ttu-id="e1819-122">无</span><span class="sxs-lookup"><span data-stu-id="e1819-122">None</span></span>|<span data-ttu-id="e1819-123">删除 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="e1819-123">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>|
|[<span data-ttu-id="e1819-124">Update mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e1819-124">Update mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-update.md)|[<span data-ttu-id="e1819-125">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e1819-125">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="e1819-126">更新 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e1819-126">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1819-127">属性</span><span class="sxs-lookup"><span data-stu-id="e1819-127">Properties</span></span>
|<span data-ttu-id="e1819-128">属性</span><span class="sxs-lookup"><span data-stu-id="e1819-128">Property</span></span>|<span data-ttu-id="e1819-129">类型</span><span class="sxs-lookup"><span data-stu-id="e1819-129">Type</span></span>|<span data-ttu-id="e1819-130">说明</span><span class="sxs-lookup"><span data-stu-id="e1819-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1819-131">displayName</span><span class="sxs-lookup"><span data-stu-id="e1819-131">displayName</span></span>|<span data-ttu-id="e1819-132">字符串</span><span class="sxs-lookup"><span data-stu-id="e1819-132">String</span></span>|<span data-ttu-id="e1819-133">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="e1819-133">Policy display name.</span></span> <span data-ttu-id="e1819-134">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e1819-135">说明</span><span class="sxs-lookup"><span data-stu-id="e1819-135">description</span></span>|<span data-ttu-id="e1819-136">String</span><span class="sxs-lookup"><span data-stu-id="e1819-136">String</span></span>|<span data-ttu-id="e1819-137">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="e1819-137">The policy's description.</span></span> <span data-ttu-id="e1819-138">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e1819-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1819-139">createdDateTime</span></span>|<span data-ttu-id="e1819-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1819-140">DateTimeOffset</span></span>|<span data-ttu-id="e1819-141">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e1819-141">The date and time the policy was created.</span></span> <span data-ttu-id="e1819-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e1819-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1819-143">lastModifiedDateTime</span></span>|<span data-ttu-id="e1819-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1819-144">DateTimeOffset</span></span>|<span data-ttu-id="e1819-145">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="e1819-145">Last time the policy was modified.</span></span> <span data-ttu-id="e1819-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e1819-147">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e1819-147">roleScopeTagIds</span></span>|<span data-ttu-id="e1819-148">String collection</span><span class="sxs-lookup"><span data-stu-id="e1819-148">String collection</span></span>|<span data-ttu-id="e1819-149">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e1819-149">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e1819-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e1819-151">id</span><span class="sxs-lookup"><span data-stu-id="e1819-151">id</span></span>|<span data-ttu-id="e1819-152">字符串</span><span class="sxs-lookup"><span data-stu-id="e1819-152">String</span></span>|<span data-ttu-id="e1819-153">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e1819-153">Key of the entity.</span></span> <span data-ttu-id="e1819-154">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e1819-155">version</span><span class="sxs-lookup"><span data-stu-id="e1819-155">version</span></span>|<span data-ttu-id="e1819-156">String</span><span class="sxs-lookup"><span data-stu-id="e1819-156">String</span></span>|<span data-ttu-id="e1819-157">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="e1819-157">Version of the entity.</span></span> <span data-ttu-id="e1819-158">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e1819-159">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="e1819-159">enforcementLevel</span></span>|[<span data-ttu-id="e1819-160">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="e1819-160">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="e1819-161">WIP 强制等级。若要获取从[WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)继承的受支持值的枚举定义, 请参阅。</span><span class="sxs-lookup"><span data-stu-id="e1819-161">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="e1819-162">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="e1819-162">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="e1819-163">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="e1819-163">enterpriseDomain</span></span>|<span data-ttu-id="e1819-164">String</span><span class="sxs-lookup"><span data-stu-id="e1819-164">String</span></span>|<span data-ttu-id="e1819-165">主企业域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-165">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-166">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="e1819-166">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="e1819-167">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1819-167">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e1819-168">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-168">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-169">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="e1819-169">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="e1819-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1819-170">Boolean</span></span>|<span data-ttu-id="e1819-171">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-171">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-172">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="e1819-172">dataRecoveryCertificate</span></span>|[<span data-ttu-id="e1819-173">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="e1819-173">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="e1819-174">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="e1819-174">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="e1819-175">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-175">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-176">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="e1819-176">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="e1819-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1819-177">Boolean</span></span>|<span data-ttu-id="e1819-178">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="e1819-178">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="e1819-179">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="e1819-179">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="e1819-180">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="e1819-180">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="e1819-181">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-181">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-182">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="e1819-182">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="e1819-183">Guid</span><span class="sxs-lookup"><span data-stu-id="e1819-183">Guid</span></span>|<span data-ttu-id="e1819-184">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="e1819-184">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="e1819-185">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-185">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-186">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="e1819-186">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="e1819-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1819-187">Boolean</span></span>|<span data-ttu-id="e1819-188">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-188">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-189">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="e1819-189">iconsVisible</span></span>|<span data-ttu-id="e1819-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1819-190">Boolean</span></span>|<span data-ttu-id="e1819-191">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="e1819-191">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="e1819-192">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-192">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-193">protectedApps</span><span class="sxs-lookup"><span data-stu-id="e1819-193">protectedApps</span></span>|<span data-ttu-id="e1819-194">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1819-194">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="e1819-195">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-195">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-196">exemptApps</span><span class="sxs-lookup"><span data-stu-id="e1819-196">exemptApps</span></span>|<span data-ttu-id="e1819-197">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1819-197">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="e1819-198">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="e1819-198">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="e1819-199">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="e1819-199">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="e1819-200">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-200">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-201">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="e1819-201">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="e1819-202">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1819-202">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e1819-203">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="e1819-203">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="e1819-204">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-204">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-205">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="e1819-205">enterpriseProxiedDomains</span></span>|<span data-ttu-id="e1819-206">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1819-206">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="e1819-207">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="e1819-207">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="e1819-208">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="e1819-208">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="e1819-209">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="e1819-209">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="e1819-210">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-210">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-211">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="e1819-211">enterpriseIPRanges</span></span>|<span data-ttu-id="e1819-212">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1819-212">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="e1819-213">设置定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="e1819-213">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="e1819-214">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="e1819-214">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="e1819-215">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-215">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-216">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="e1819-216">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="e1819-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1819-217">Boolean</span></span>|<span data-ttu-id="e1819-218">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="e1819-218">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="e1819-219">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-219">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-220">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="e1819-220">enterpriseProxyServers</span></span>|<span data-ttu-id="e1819-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1819-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e1819-222">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="e1819-222">This is a list of proxy servers.</span></span> <span data-ttu-id="e1819-223">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-223">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-224">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="e1819-224">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="e1819-225">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1819-225">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e1819-226">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="e1819-226">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="e1819-227">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="e1819-227">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="e1819-228">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="e1819-228">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="e1819-229">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="e1819-229">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="e1819-230">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-230">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-231">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="e1819-231">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="e1819-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1819-232">Boolean</span></span>|<span data-ttu-id="e1819-233">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="e1819-233">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="e1819-234">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-234">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-235">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="e1819-235">neutralDomainResources</span></span>|<span data-ttu-id="e1819-236">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1819-236">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e1819-237">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-237">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-238">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="e1819-238">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="e1819-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1819-239">Boolean</span></span>|<span data-ttu-id="e1819-240">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-240">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-241">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="e1819-241">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="e1819-242">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1819-242">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="e1819-243">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-243">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-244">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e1819-244">isAssigned</span></span>|<span data-ttu-id="e1819-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1819-245">Boolean</span></span>|<span data-ttu-id="e1819-246">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="e1819-246">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="e1819-247">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-247">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1819-248">关系</span><span class="sxs-lookup"><span data-stu-id="e1819-248">Relationships</span></span>
|<span data-ttu-id="e1819-249">关系</span><span class="sxs-lookup"><span data-stu-id="e1819-249">Relationship</span></span>|<span data-ttu-id="e1819-250">类型</span><span class="sxs-lookup"><span data-stu-id="e1819-250">Type</span></span>|<span data-ttu-id="e1819-251">说明</span><span class="sxs-lookup"><span data-stu-id="e1819-251">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1819-252">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="e1819-252">protectedAppLockerFiles</span></span>|<span data-ttu-id="e1819-253">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1819-253">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="e1819-254">通过 xml 文件输入受保护应用的另一种方法 继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-254">Another way to input protected apps through xml files Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-255">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="e1819-255">exemptAppLockerFiles</span></span>|<span data-ttu-id="e1819-256">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1819-256">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="e1819-257">通过 xml 文件输入豁免应用的另一种方法 继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-257">Another way to input exempt apps through xml files Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="e1819-258">assignments</span><span class="sxs-lookup"><span data-stu-id="e1819-258">assignments</span></span>|<span data-ttu-id="e1819-259">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1819-259">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="e1819-260">针对策略的安全组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="e1819-260">Navigation property to list of security groups targeted for policy.</span></span> <span data-ttu-id="e1819-261">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e1819-261">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1819-262">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1819-262">JSON Representation</span></span>
<span data-ttu-id="e1819-263">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1819-263">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mdmWindowsInformationProtectionPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
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



