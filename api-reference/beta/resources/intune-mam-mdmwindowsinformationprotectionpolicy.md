---
title: mdmWindowsInformationProtectionPolicy 资源类型
description: 使用 MDM 进行 Windows 信息保护的策略
ms.openlocfilehash: f714b74a5fcb4c45c92ba262d1fa573647722336
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043852"
---
# <a name="mdmwindowsinformationprotectionpolicy-resource-type"></a><span data-ttu-id="faf54-103">mdmWindowsInformationProtectionPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="faf54-103">mdmWindowsInformationProtectionPolicy resource type</span></span>

> <span data-ttu-id="faf54-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="faf54-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="faf54-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="faf54-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="faf54-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="faf54-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="faf54-107">使用 MDM 进行 Windows 信息保护的策略</span><span class="sxs-lookup"><span data-stu-id="faf54-107">Policy for Windows information protection with MDM</span></span>

<span data-ttu-id="faf54-108">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-108">Inherits from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>

## <a name="methods"></a><span data-ttu-id="faf54-109">方法</span><span class="sxs-lookup"><span data-stu-id="faf54-109">Methods</span></span>
|<span data-ttu-id="faf54-110">方法</span><span class="sxs-lookup"><span data-stu-id="faf54-110">Method</span></span>|<span data-ttu-id="faf54-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="faf54-111">Return Type</span></span>|<span data-ttu-id="faf54-112">说明</span><span class="sxs-lookup"><span data-stu-id="faf54-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="faf54-113">List mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="faf54-113">List mdmWindowsInformationProtectionPolicies</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-list.md)|<span data-ttu-id="faf54-114">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faf54-114">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) collection</span></span>|<span data-ttu-id="faf54-115">列出 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="faf54-115">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>|
|[<span data-ttu-id="faf54-116">Get mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="faf54-116">Get mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-get.md)|[<span data-ttu-id="faf54-117">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="faf54-117">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="faf54-118">读取 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="faf54-118">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|[<span data-ttu-id="faf54-119">Create mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="faf54-119">Create mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-create.md)|[<span data-ttu-id="faf54-120">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="faf54-120">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="faf54-121">创建新的 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="faf54-121">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|[<span data-ttu-id="faf54-122">Delete mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="faf54-122">Delete mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-delete.md)|<span data-ttu-id="faf54-123">无</span><span class="sxs-lookup"><span data-stu-id="faf54-123">None</span></span>|<span data-ttu-id="faf54-124">删除 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="faf54-124">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>|
|[<span data-ttu-id="faf54-125">Update mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="faf54-125">Update mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-update.md)|[<span data-ttu-id="faf54-126">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="faf54-126">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="faf54-127">更新 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="faf54-127">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="faf54-128">属性</span><span class="sxs-lookup"><span data-stu-id="faf54-128">Properties</span></span>
|<span data-ttu-id="faf54-129">属性</span><span class="sxs-lookup"><span data-stu-id="faf54-129">Property</span></span>|<span data-ttu-id="faf54-130">类型</span><span class="sxs-lookup"><span data-stu-id="faf54-130">Type</span></span>|<span data-ttu-id="faf54-131">说明</span><span class="sxs-lookup"><span data-stu-id="faf54-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faf54-132">displayName</span><span class="sxs-lookup"><span data-stu-id="faf54-132">displayName</span></span>|<span data-ttu-id="faf54-133">String</span><span class="sxs-lookup"><span data-stu-id="faf54-133">String</span></span>|<span data-ttu-id="faf54-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="faf54-134">Policy display name.</span></span> <span data-ttu-id="faf54-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="faf54-136">description</span><span class="sxs-lookup"><span data-stu-id="faf54-136">description</span></span>|<span data-ttu-id="faf54-137">String</span><span class="sxs-lookup"><span data-stu-id="faf54-137">String</span></span>|<span data-ttu-id="faf54-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="faf54-138">The policy's description.</span></span> <span data-ttu-id="faf54-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="faf54-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="faf54-140">createdDateTime</span></span>|<span data-ttu-id="faf54-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faf54-141">DateTimeOffset</span></span>|<span data-ttu-id="faf54-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="faf54-142">The date and time the policy was created.</span></span> <span data-ttu-id="faf54-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="faf54-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="faf54-144">lastModifiedDateTime</span></span>|<span data-ttu-id="faf54-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faf54-145">DateTimeOffset</span></span>|<span data-ttu-id="faf54-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="faf54-146">Last time the policy was modified.</span></span> <span data-ttu-id="faf54-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="faf54-148">id</span><span class="sxs-lookup"><span data-stu-id="faf54-148">id</span></span>|<span data-ttu-id="faf54-149">String</span><span class="sxs-lookup"><span data-stu-id="faf54-149">String</span></span>|<span data-ttu-id="faf54-150">实体的键。</span><span class="sxs-lookup"><span data-stu-id="faf54-150">Key of the entity.</span></span> <span data-ttu-id="faf54-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="faf54-152">version</span><span class="sxs-lookup"><span data-stu-id="faf54-152">version</span></span>|<span data-ttu-id="faf54-153">String</span><span class="sxs-lookup"><span data-stu-id="faf54-153">String</span></span>|<span data-ttu-id="faf54-154">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="faf54-154">Version of the entity.</span></span> <span data-ttu-id="faf54-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="faf54-156">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="faf54-156">enforcementLevel</span></span>|[<span data-ttu-id="faf54-157">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="faf54-157">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="faf54-158">WIP 实施级别。请参见支持值继承[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)枚举定义。</span><span class="sxs-lookup"><span data-stu-id="faf54-158">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="faf54-159">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="faf54-159">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="faf54-160">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="faf54-160">enterpriseDomain</span></span>|<span data-ttu-id="faf54-161">String</span><span class="sxs-lookup"><span data-stu-id="faf54-161">String</span></span>|<span data-ttu-id="faf54-162">主企业域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-162">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-163">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="faf54-163">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="faf54-164">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faf54-164">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="faf54-165">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-165">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-166">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="faf54-166">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="faf54-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="faf54-167">Boolean</span></span>|<span data-ttu-id="faf54-168">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-168">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-169">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="faf54-169">dataRecoveryCertificate</span></span>|[<span data-ttu-id="faf54-170">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="faf54-170">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="faf54-171">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="faf54-171">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="faf54-172">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-172">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-173">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="faf54-173">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="faf54-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="faf54-174">Boolean</span></span>|<span data-ttu-id="faf54-175">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="faf54-175">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="faf54-176">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="faf54-176">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="faf54-177">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="faf54-177">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="faf54-178">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-178">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-179">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="faf54-179">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="faf54-180">Guid</span><span class="sxs-lookup"><span data-stu-id="faf54-180">Guid</span></span>|<span data-ttu-id="faf54-181">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="faf54-181">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="faf54-182">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-182">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-183">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="faf54-183">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="faf54-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="faf54-184">Boolean</span></span>|<span data-ttu-id="faf54-185">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-185">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-186">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="faf54-186">iconsVisible</span></span>|<span data-ttu-id="faf54-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="faf54-187">Boolean</span></span>|<span data-ttu-id="faf54-188">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="faf54-188">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="faf54-189">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-189">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-190">protectedApps</span><span class="sxs-lookup"><span data-stu-id="faf54-190">protectedApps</span></span>|<span data-ttu-id="faf54-191">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faf54-191">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="faf54-192">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-192">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-193">exemptApps</span><span class="sxs-lookup"><span data-stu-id="faf54-193">exemptApps</span></span>|<span data-ttu-id="faf54-194">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faf54-194">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="faf54-195">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="faf54-195">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="faf54-196">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="faf54-196">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="faf54-197">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-197">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-198">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="faf54-198">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="faf54-199">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faf54-199">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="faf54-200">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="faf54-200">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="faf54-201">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-201">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-202">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="faf54-202">enterpriseProxiedDomains</span></span>|<span data-ttu-id="faf54-203">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faf54-203">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="faf54-204">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="faf54-204">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="faf54-205">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="faf54-205">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="faf54-206">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="faf54-206">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="faf54-207">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-207">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-208">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="faf54-208">enterpriseIPRanges</span></span>|<span data-ttu-id="faf54-209">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faf54-209">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="faf54-210">设置可定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="faf54-210">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="faf54-211">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="faf54-211">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="faf54-212">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-212">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-213">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="faf54-213">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="faf54-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="faf54-214">Boolean</span></span>|<span data-ttu-id="faf54-215">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="faf54-215">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="faf54-216">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-216">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-217">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="faf54-217">enterpriseProxyServers</span></span>|<span data-ttu-id="faf54-218">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faf54-218">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="faf54-219">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="faf54-219">This is a list of proxy servers.</span></span> <span data-ttu-id="faf54-220">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-220">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-221">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="faf54-221">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="faf54-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faf54-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="faf54-223">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="faf54-223">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="faf54-224">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="faf54-224">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="faf54-225">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="faf54-225">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="faf54-226">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="faf54-226">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="faf54-227">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-227">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-228">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="faf54-228">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="faf54-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="faf54-229">Boolean</span></span>|<span data-ttu-id="faf54-230">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="faf54-230">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="faf54-231">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-231">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-232">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="faf54-232">neutralDomainResources</span></span>|<span data-ttu-id="faf54-233">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faf54-233">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="faf54-234">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-234">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-235">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="faf54-235">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="faf54-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="faf54-236">Boolean</span></span>|<span data-ttu-id="faf54-237">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-237">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-238">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="faf54-238">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="faf54-239">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faf54-239">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="faf54-240">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-240">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-241">isAssigned</span><span class="sxs-lookup"><span data-stu-id="faf54-241">isAssigned</span></span>|<span data-ttu-id="faf54-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="faf54-242">Boolean</span></span>|<span data-ttu-id="faf54-243">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="faf54-243">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="faf54-244">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-244">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="faf54-245">关系</span><span class="sxs-lookup"><span data-stu-id="faf54-245">Relationships</span></span>
|<span data-ttu-id="faf54-246">关系</span><span class="sxs-lookup"><span data-stu-id="faf54-246">Relationship</span></span>|<span data-ttu-id="faf54-247">类型</span><span class="sxs-lookup"><span data-stu-id="faf54-247">Type</span></span>|<span data-ttu-id="faf54-248">说明</span><span class="sxs-lookup"><span data-stu-id="faf54-248">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faf54-249">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="faf54-249">protectedAppLockerFiles</span></span>|<span data-ttu-id="faf54-250">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faf54-250">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="faf54-251">通过 xml 文件输入受保护应用的另一种方法 继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-251">Another way to input protected apps through xml files Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-252">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="faf54-252">exemptAppLockerFiles</span></span>|<span data-ttu-id="faf54-253">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faf54-253">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="faf54-254">通过 xml 文件输入豁免应用的另一种方法 继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-254">Another way to input exempt apps through xml files Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="faf54-255">assignments</span><span class="sxs-lookup"><span data-stu-id="faf54-255">assignments</span></span>|<span data-ttu-id="faf54-256">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faf54-256">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="faf54-257">针对策略的安全组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="faf54-257">Navigation property to list of security groups targeted for policy.</span></span> <span data-ttu-id="faf54-258">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="faf54-258">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="faf54-259">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="faf54-259">JSON Representation</span></span>
<span data-ttu-id="faf54-260">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="faf54-260">Here is a JSON representation of the resource.</span></span>
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





