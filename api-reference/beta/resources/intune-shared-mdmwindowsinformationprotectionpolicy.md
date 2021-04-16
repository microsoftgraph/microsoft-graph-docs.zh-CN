---
title: mdmWindowsInformationProtectionPolicy 资源类型
description: 使用 MDM 进行 Windows 信息保护的策略
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7c1a5db2eebcd44a4fecaee2e763539832e2ef02
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866536"
---
# <a name="mdmwindowsinformationprotectionpolicy-resource-type"></a><span data-ttu-id="a783b-103">mdmWindowsInformationProtectionPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="a783b-103">mdmWindowsInformationProtectionPolicy resource type</span></span>

<span data-ttu-id="a783b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a783b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a783b-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a783b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a783b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a783b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a783b-107">使用 MDM 进行 Windows 信息保护的策略</span><span class="sxs-lookup"><span data-stu-id="a783b-107">Policy for Windows information protection with MDM</span></span>


<span data-ttu-id="a783b-108">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-108">Inherits from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a783b-109">方法</span><span class="sxs-lookup"><span data-stu-id="a783b-109">Methods</span></span>
|<span data-ttu-id="a783b-110">方法</span><span class="sxs-lookup"><span data-stu-id="a783b-110">Method</span></span>|<span data-ttu-id="a783b-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="a783b-111">Return Type</span></span>|<span data-ttu-id="a783b-112">说明</span><span class="sxs-lookup"><span data-stu-id="a783b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a783b-113">List mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="a783b-113">List mdmWindowsInformationProtectionPolicies</span></span>](../api/intune-shared-mdmwindowsinformationprotectionpolicy-list.md)|<span data-ttu-id="a783b-114">[mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-114">[mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) collection</span></span>|<span data-ttu-id="a783b-115">列出 [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a783b-115">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>|
|[<span data-ttu-id="a783b-116">Get mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a783b-116">Get mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-shared-mdmwindowsinformationprotectionpolicy-get.md)|[<span data-ttu-id="a783b-117">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a783b-117">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="a783b-118">读取 [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a783b-118">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|[<span data-ttu-id="a783b-119">Create mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a783b-119">Create mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-shared-mdmwindowsinformationprotectionpolicy-create.md)|[<span data-ttu-id="a783b-120">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a783b-120">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="a783b-121">创建新的 [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a783b-121">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|[<span data-ttu-id="a783b-122">Delete mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a783b-122">Delete mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-shared-mdmwindowsinformationprotectionpolicy-delete.md)|<span data-ttu-id="a783b-123">无</span><span class="sxs-lookup"><span data-stu-id="a783b-123">None</span></span>|<span data-ttu-id="a783b-124">删除 [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="a783b-124">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span></span>|
|[<span data-ttu-id="a783b-125">Update mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a783b-125">Update mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-shared-mdmwindowsinformationprotectionpolicy-update.md)|[<span data-ttu-id="a783b-126">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a783b-126">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="a783b-127">更新 [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a783b-127">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|<span data-ttu-id="a783b-128">**策略集**</span><span class="sxs-lookup"><span data-stu-id="a783b-128">**Policy Set**</span></span>|
|[<span data-ttu-id="a783b-129">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="a783b-129">hasPayloadLinks action</span></span>](../api/intune-shared-mdmwindowsinformationprotectionpolicy-haspayloadlinks.md)|<span data-ttu-id="a783b-130">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-130">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="a783b-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a783b-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a783b-132">属性</span><span class="sxs-lookup"><span data-stu-id="a783b-132">Properties</span></span>
|<span data-ttu-id="a783b-133">属性</span><span class="sxs-lookup"><span data-stu-id="a783b-133">Property</span></span>|<span data-ttu-id="a783b-134">类型</span><span class="sxs-lookup"><span data-stu-id="a783b-134">Type</span></span>|<span data-ttu-id="a783b-135">说明</span><span class="sxs-lookup"><span data-stu-id="a783b-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a783b-136">id</span><span class="sxs-lookup"><span data-stu-id="a783b-136">id</span></span>|<span data-ttu-id="a783b-137">String</span><span class="sxs-lookup"><span data-stu-id="a783b-137">String</span></span>|<span data-ttu-id="a783b-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a783b-138">Key of the entity.</span></span> <span data-ttu-id="a783b-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a783b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="a783b-140">displayName</span></span>|<span data-ttu-id="a783b-141">String</span><span class="sxs-lookup"><span data-stu-id="a783b-141">String</span></span>|<span data-ttu-id="a783b-142">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="a783b-142">Policy display name.</span></span> <span data-ttu-id="a783b-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a783b-144">说明</span><span class="sxs-lookup"><span data-stu-id="a783b-144">description</span></span>|<span data-ttu-id="a783b-145">String</span><span class="sxs-lookup"><span data-stu-id="a783b-145">String</span></span>|<span data-ttu-id="a783b-146">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="a783b-146">The policy's description.</span></span> <span data-ttu-id="a783b-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a783b-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a783b-148">createdDateTime</span></span>|<span data-ttu-id="a783b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a783b-149">DateTimeOffset</span></span>|<span data-ttu-id="a783b-150">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a783b-150">The date and time the policy was created.</span></span> <span data-ttu-id="a783b-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a783b-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a783b-152">lastModifiedDateTime</span></span>|<span data-ttu-id="a783b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a783b-153">DateTimeOffset</span></span>|<span data-ttu-id="a783b-154">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="a783b-154">Last time the policy was modified.</span></span> <span data-ttu-id="a783b-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a783b-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a783b-156">roleScopeTagIds</span></span>|<span data-ttu-id="a783b-157">String 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-157">String collection</span></span>|<span data-ttu-id="a783b-158">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a783b-158">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a783b-159">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a783b-160">version</span><span class="sxs-lookup"><span data-stu-id="a783b-160">version</span></span>|<span data-ttu-id="a783b-161">String</span><span class="sxs-lookup"><span data-stu-id="a783b-161">String</span></span>|<span data-ttu-id="a783b-162">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="a783b-162">Version of the entity.</span></span> <span data-ttu-id="a783b-163">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-163">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a783b-164">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="a783b-164">enforcementLevel</span></span>|[<span data-ttu-id="a783b-165">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="a783b-165">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="a783b-166">WIP 强制级别。请参阅 Enum 定义了解受支持的值 继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="a783b-166">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="a783b-167">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="a783b-167">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="a783b-168">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="a783b-168">enterpriseDomain</span></span>|<span data-ttu-id="a783b-169">String</span><span class="sxs-lookup"><span data-stu-id="a783b-169">String</span></span>|<span data-ttu-id="a783b-170">主企业域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-170">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-171">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="a783b-171">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="a783b-172">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-172">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a783b-173">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-173">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-174">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="a783b-174">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="a783b-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="a783b-175">Boolean</span></span>|<span data-ttu-id="a783b-176">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-176">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-177">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a783b-177">dataRecoveryCertificate</span></span>|[<span data-ttu-id="a783b-178">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a783b-178">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="a783b-179">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="a783b-179">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="a783b-180">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-180">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-181">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="a783b-181">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="a783b-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="a783b-182">Boolean</span></span>|<span data-ttu-id="a783b-183">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="a783b-183">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="a783b-184">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="a783b-184">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="a783b-185">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="a783b-185">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="a783b-186">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-186">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-187">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="a783b-187">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="a783b-188">Guid</span><span class="sxs-lookup"><span data-stu-id="a783b-188">Guid</span></span>|<span data-ttu-id="a783b-189">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="a783b-189">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="a783b-190">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-190">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-191">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="a783b-191">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="a783b-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="a783b-192">Boolean</span></span>|<span data-ttu-id="a783b-193">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-193">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-194">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="a783b-194">iconsVisible</span></span>|<span data-ttu-id="a783b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="a783b-195">Boolean</span></span>|<span data-ttu-id="a783b-196">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="a783b-196">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="a783b-197">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-197">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-198">protectedApps</span><span class="sxs-lookup"><span data-stu-id="a783b-198">protectedApps</span></span>|<span data-ttu-id="a783b-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="a783b-200">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-200">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-201">exemptApps</span><span class="sxs-lookup"><span data-stu-id="a783b-201">exemptApps</span></span>|<span data-ttu-id="a783b-202">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-202">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="a783b-203">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="a783b-203">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="a783b-204">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="a783b-204">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="a783b-205">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-205">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-206">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="a783b-206">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="a783b-207">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-207">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a783b-208">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="a783b-208">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="a783b-209">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-209">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-210">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="a783b-210">enterpriseProxiedDomains</span></span>|<span data-ttu-id="a783b-211">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-211">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="a783b-212">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="a783b-212">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="a783b-213">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="a783b-213">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="a783b-214">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="a783b-214">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="a783b-215">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-215">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-216">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="a783b-216">enterpriseIPRanges</span></span>|<span data-ttu-id="a783b-217">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-217">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="a783b-218">设置定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="a783b-218">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="a783b-219">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="a783b-219">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="a783b-220">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-220">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-221">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="a783b-221">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="a783b-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="a783b-222">Boolean</span></span>|<span data-ttu-id="a783b-223">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="a783b-223">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="a783b-224">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-224">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-225">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="a783b-225">enterpriseProxyServers</span></span>|<span data-ttu-id="a783b-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a783b-227">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="a783b-227">This is a list of proxy servers.</span></span> <span data-ttu-id="a783b-228">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-228">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-229">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="a783b-229">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="a783b-230">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-230">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a783b-231">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="a783b-231">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="a783b-232">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="a783b-232">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="a783b-233">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="a783b-233">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="a783b-234">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="a783b-234">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="a783b-235">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-235">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-236">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="a783b-236">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="a783b-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="a783b-237">Boolean</span></span>|<span data-ttu-id="a783b-238">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="a783b-238">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="a783b-239">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-239">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-240">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="a783b-240">neutralDomainResources</span></span>|<span data-ttu-id="a783b-241">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-241">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a783b-242">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-242">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-243">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="a783b-243">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="a783b-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="a783b-244">Boolean</span></span>|<span data-ttu-id="a783b-245">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-245">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-246">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="a783b-246">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="a783b-247">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-247">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a783b-248">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-248">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-249">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a783b-249">isAssigned</span></span>|<span data-ttu-id="a783b-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="a783b-250">Boolean</span></span>|<span data-ttu-id="a783b-251">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="a783b-251">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="a783b-252">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-252">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a783b-253">关系</span><span class="sxs-lookup"><span data-stu-id="a783b-253">Relationships</span></span>
|<span data-ttu-id="a783b-254">关系</span><span class="sxs-lookup"><span data-stu-id="a783b-254">Relationship</span></span>|<span data-ttu-id="a783b-255">类型</span><span class="sxs-lookup"><span data-stu-id="a783b-255">Type</span></span>|<span data-ttu-id="a783b-256">说明</span><span class="sxs-lookup"><span data-stu-id="a783b-256">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a783b-257">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="a783b-257">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="a783b-258">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="a783b-258">protectedAppLockerFiles</span></span>|<span data-ttu-id="a783b-259">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-259">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="a783b-260">通过 xml 文件输入受保护应用的另一种方法 继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-260">Another way to input protected apps through xml files Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-261">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="a783b-261">exemptAppLockerFiles</span></span>|<span data-ttu-id="a783b-262">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-262">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="a783b-263">通过 xml 文件输入豁免应用的另一种方法 继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-263">Another way to input exempt apps through xml files Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a783b-264">assignments</span><span class="sxs-lookup"><span data-stu-id="a783b-264">assignments</span></span>|<span data-ttu-id="a783b-265">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a783b-265">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="a783b-266">针对策略的安全组列表的导航属性。</span><span class="sxs-lookup"><span data-stu-id="a783b-266">Navigation property to list of security groups targeted for policy.</span></span> <span data-ttu-id="a783b-267">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a783b-267">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a783b-268">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a783b-268">JSON Representation</span></span>
<span data-ttu-id="a783b-269">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a783b-269">Here is a JSON representation of the resource.</span></span>
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




