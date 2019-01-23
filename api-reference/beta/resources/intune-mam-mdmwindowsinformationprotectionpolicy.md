---
title: mdmWindowsInformationProtectionPolicy 资源类型
description: 使用 MDM 进行 Windows 信息保护的策略
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 60bd38174777342436095d222a36dadeb2d67437
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424782"
---
# <a name="mdmwindowsinformationprotectionpolicy-resource-type"></a><span data-ttu-id="fd973-103">mdmWindowsInformationProtectionPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd973-103">mdmWindowsInformationProtectionPolicy resource type</span></span>

> <span data-ttu-id="fd973-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="fd973-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fd973-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fd973-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd973-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd973-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd973-107">使用 MDM 进行 Windows 信息保护的策略</span><span class="sxs-lookup"><span data-stu-id="fd973-107">Policy for Windows information protection with MDM</span></span>


<span data-ttu-id="fd973-108">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-108">Inherits from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>

## <a name="methods"></a><span data-ttu-id="fd973-109">方法</span><span class="sxs-lookup"><span data-stu-id="fd973-109">Methods</span></span>
|<span data-ttu-id="fd973-110">方法</span><span class="sxs-lookup"><span data-stu-id="fd973-110">Method</span></span>|<span data-ttu-id="fd973-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="fd973-111">Return Type</span></span>|<span data-ttu-id="fd973-112">说明</span><span class="sxs-lookup"><span data-stu-id="fd973-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fd973-113">List mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="fd973-113">List mdmWindowsInformationProtectionPolicies</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-list.md)|<span data-ttu-id="fd973-114">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-114">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) collection</span></span>|<span data-ttu-id="fd973-115">列出 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fd973-115">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>|
|[<span data-ttu-id="fd973-116">Get mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fd973-116">Get mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-get.md)|[<span data-ttu-id="fd973-117">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fd973-117">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="fd973-118">读取 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fd973-118">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|[<span data-ttu-id="fd973-119">Create mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fd973-119">Create mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-create.md)|[<span data-ttu-id="fd973-120">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fd973-120">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="fd973-121">创建新的 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fd973-121">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|[<span data-ttu-id="fd973-122">Delete mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fd973-122">Delete mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-delete.md)|<span data-ttu-id="fd973-123">无</span><span class="sxs-lookup"><span data-stu-id="fd973-123">None</span></span>|<span data-ttu-id="fd973-124">删除 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="fd973-124">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>|
|[<span data-ttu-id="fd973-125">Update mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fd973-125">Update mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-update.md)|[<span data-ttu-id="fd973-126">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fd973-126">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="fd973-127">更新 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fd973-127">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fd973-128">属性</span><span class="sxs-lookup"><span data-stu-id="fd973-128">Properties</span></span>
|<span data-ttu-id="fd973-129">属性</span><span class="sxs-lookup"><span data-stu-id="fd973-129">Property</span></span>|<span data-ttu-id="fd973-130">类型</span><span class="sxs-lookup"><span data-stu-id="fd973-130">Type</span></span>|<span data-ttu-id="fd973-131">说明</span><span class="sxs-lookup"><span data-stu-id="fd973-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd973-132">displayName</span><span class="sxs-lookup"><span data-stu-id="fd973-132">displayName</span></span>|<span data-ttu-id="fd973-133">String</span><span class="sxs-lookup"><span data-stu-id="fd973-133">String</span></span>|<span data-ttu-id="fd973-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="fd973-134">Policy display name.</span></span> <span data-ttu-id="fd973-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fd973-136">description</span><span class="sxs-lookup"><span data-stu-id="fd973-136">description</span></span>|<span data-ttu-id="fd973-137">String</span><span class="sxs-lookup"><span data-stu-id="fd973-137">String</span></span>|<span data-ttu-id="fd973-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="fd973-138">The policy's description.</span></span> <span data-ttu-id="fd973-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fd973-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd973-140">createdDateTime</span></span>|<span data-ttu-id="fd973-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd973-141">DateTimeOffset</span></span>|<span data-ttu-id="fd973-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fd973-142">The date and time the policy was created.</span></span> <span data-ttu-id="fd973-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fd973-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd973-144">lastModifiedDateTime</span></span>|<span data-ttu-id="fd973-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd973-145">DateTimeOffset</span></span>|<span data-ttu-id="fd973-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="fd973-146">Last time the policy was modified.</span></span> <span data-ttu-id="fd973-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fd973-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fd973-148">roleScopeTagIds</span></span>|<span data-ttu-id="fd973-149">String 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-149">String collection</span></span>|<span data-ttu-id="fd973-150">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="fd973-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fd973-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fd973-152">id</span><span class="sxs-lookup"><span data-stu-id="fd973-152">id</span></span>|<span data-ttu-id="fd973-153">String</span><span class="sxs-lookup"><span data-stu-id="fd973-153">String</span></span>|<span data-ttu-id="fd973-154">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fd973-154">Key of the entity.</span></span> <span data-ttu-id="fd973-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fd973-156">version</span><span class="sxs-lookup"><span data-stu-id="fd973-156">version</span></span>|<span data-ttu-id="fd973-157">String</span><span class="sxs-lookup"><span data-stu-id="fd973-157">String</span></span>|<span data-ttu-id="fd973-158">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="fd973-158">Version of the entity.</span></span> <span data-ttu-id="fd973-159">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fd973-160">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="fd973-160">enforcementLevel</span></span>|[<span data-ttu-id="fd973-161">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="fd973-161">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="fd973-162">WIP 实施级别。请参见支持值继承[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)枚举定义。</span><span class="sxs-lookup"><span data-stu-id="fd973-162">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="fd973-163">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="fd973-163">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="fd973-164">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="fd973-164">enterpriseDomain</span></span>|<span data-ttu-id="fd973-165">String</span><span class="sxs-lookup"><span data-stu-id="fd973-165">String</span></span>|<span data-ttu-id="fd973-166">主企业域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-166">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-167">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="fd973-167">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="fd973-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fd973-169">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-169">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-170">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="fd973-170">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="fd973-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd973-171">Boolean</span></span>|<span data-ttu-id="fd973-172">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-172">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-173">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="fd973-173">dataRecoveryCertificate</span></span>|[<span data-ttu-id="fd973-174">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="fd973-174">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="fd973-175">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="fd973-175">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="fd973-176">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-176">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-177">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="fd973-177">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="fd973-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd973-178">Boolean</span></span>|<span data-ttu-id="fd973-179">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="fd973-179">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="fd973-180">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="fd973-180">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="fd973-181">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="fd973-181">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="fd973-182">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-182">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-183">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="fd973-183">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="fd973-184">Guid</span><span class="sxs-lookup"><span data-stu-id="fd973-184">Guid</span></span>|<span data-ttu-id="fd973-185">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="fd973-185">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="fd973-186">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-186">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-187">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="fd973-187">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="fd973-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd973-188">Boolean</span></span>|<span data-ttu-id="fd973-189">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-189">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-190">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="fd973-190">iconsVisible</span></span>|<span data-ttu-id="fd973-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd973-191">Boolean</span></span>|<span data-ttu-id="fd973-192">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="fd973-192">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="fd973-193">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-193">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-194">protectedApps</span><span class="sxs-lookup"><span data-stu-id="fd973-194">protectedApps</span></span>|<span data-ttu-id="fd973-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="fd973-196">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-196">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-197">exemptApps</span><span class="sxs-lookup"><span data-stu-id="fd973-197">exemptApps</span></span>|<span data-ttu-id="fd973-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="fd973-199">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="fd973-199">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="fd973-200">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="fd973-200">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="fd973-201">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-201">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-202">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="fd973-202">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="fd973-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fd973-204">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="fd973-204">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="fd973-205">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-205">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-206">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="fd973-206">enterpriseProxiedDomains</span></span>|<span data-ttu-id="fd973-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="fd973-208">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="fd973-208">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="fd973-209">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="fd973-209">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="fd973-210">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="fd973-210">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="fd973-211">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-211">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-212">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="fd973-212">enterpriseIPRanges</span></span>|<span data-ttu-id="fd973-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="fd973-214">设置可定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="fd973-214">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="fd973-215">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="fd973-215">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="fd973-216">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-216">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-217">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="fd973-217">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="fd973-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd973-218">Boolean</span></span>|<span data-ttu-id="fd973-219">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="fd973-219">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="fd973-220">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-220">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-221">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="fd973-221">enterpriseProxyServers</span></span>|<span data-ttu-id="fd973-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fd973-223">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="fd973-223">This is a list of proxy servers.</span></span> <span data-ttu-id="fd973-224">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-224">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-225">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="fd973-225">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="fd973-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fd973-227">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="fd973-227">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="fd973-228">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="fd973-228">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="fd973-229">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="fd973-229">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="fd973-230">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="fd973-230">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="fd973-231">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-231">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-232">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="fd973-232">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="fd973-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd973-233">Boolean</span></span>|<span data-ttu-id="fd973-234">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="fd973-234">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="fd973-235">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-235">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-236">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="fd973-236">neutralDomainResources</span></span>|<span data-ttu-id="fd973-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fd973-238">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-238">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-239">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="fd973-239">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="fd973-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd973-240">Boolean</span></span>|<span data-ttu-id="fd973-241">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-241">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-242">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="fd973-242">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="fd973-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fd973-244">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-244">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-245">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fd973-245">isAssigned</span></span>|<span data-ttu-id="fd973-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd973-246">Boolean</span></span>|<span data-ttu-id="fd973-247">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="fd973-247">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="fd973-248">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-248">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd973-249">关系</span><span class="sxs-lookup"><span data-stu-id="fd973-249">Relationships</span></span>
|<span data-ttu-id="fd973-250">关系</span><span class="sxs-lookup"><span data-stu-id="fd973-250">Relationship</span></span>|<span data-ttu-id="fd973-251">类型</span><span class="sxs-lookup"><span data-stu-id="fd973-251">Type</span></span>|<span data-ttu-id="fd973-252">说明</span><span class="sxs-lookup"><span data-stu-id="fd973-252">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd973-253">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="fd973-253">protectedAppLockerFiles</span></span>|<span data-ttu-id="fd973-254">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-254">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="fd973-255">通过 xml 文件输入受保护应用的另一种方法 继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-255">Another way to input protected apps through xml files Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-256">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="fd973-256">exemptAppLockerFiles</span></span>|<span data-ttu-id="fd973-257">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-257">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="fd973-258">通过 xml 文件输入豁免应用的另一种方法 继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-258">Another way to input exempt apps through xml files Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd973-259">assignments</span><span class="sxs-lookup"><span data-stu-id="fd973-259">assignments</span></span>|<span data-ttu-id="fd973-260">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd973-260">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="fd973-261">针对策略的安全组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="fd973-261">Navigation property to list of security groups targeted for policy.</span></span> <span data-ttu-id="fd973-262">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fd973-262">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd973-263">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd973-263">JSON Representation</span></span>
<span data-ttu-id="fd973-264">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd973-264">Here is a JSON representation of the resource.</span></span>
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




