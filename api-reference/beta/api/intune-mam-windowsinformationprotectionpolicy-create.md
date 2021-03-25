---
title: 创建 windowsInformationProtectionPolicy
description: 创建新的 windowsInformationProtectionPolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d47fda8bddc9b27fac610f841918670c6c61a24f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153165"
---
# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="6bafd-103">创建 windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="6bafd-103">Create windowsInformationProtectionPolicy</span></span>

<span data-ttu-id="6bafd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bafd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6bafd-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6bafd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bafd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6bafd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bafd-107">创建新的 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6bafd-107">Create a new [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6bafd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6bafd-108">Prerequisites</span></span>
<span data-ttu-id="6bafd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6bafd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bafd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6bafd-111">Permission type</span></span>|<span data-ttu-id="6bafd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6bafd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bafd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6bafd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6bafd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bafd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6bafd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6bafd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bafd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6bafd-116">Not supported.</span></span>|
|<span data-ttu-id="6bafd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6bafd-117">Application</span></span>|<span data-ttu-id="6bafd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bafd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bafd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6bafd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="6bafd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6bafd-120">Request headers</span></span>
|<span data-ttu-id="6bafd-121">标头</span><span class="sxs-lookup"><span data-stu-id="6bafd-121">Header</span></span>|<span data-ttu-id="6bafd-122">值</span><span class="sxs-lookup"><span data-stu-id="6bafd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bafd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bafd-123">Authorization</span></span>|<span data-ttu-id="6bafd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6bafd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bafd-125">接受</span><span class="sxs-lookup"><span data-stu-id="6bafd-125">Accept</span></span>|<span data-ttu-id="6bafd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6bafd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bafd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6bafd-127">Request body</span></span>
<span data-ttu-id="6bafd-128">在请求正文中，提供 windowsInformationProtectionPolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bafd-128">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="6bafd-129">下表显示创建 windowsInformationProtectionPolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6bafd-129">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="6bafd-130">属性</span><span class="sxs-lookup"><span data-stu-id="6bafd-130">Property</span></span>|<span data-ttu-id="6bafd-131">类型</span><span class="sxs-lookup"><span data-stu-id="6bafd-131">Type</span></span>|<span data-ttu-id="6bafd-132">说明</span><span class="sxs-lookup"><span data-stu-id="6bafd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bafd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6bafd-133">displayName</span></span>|<span data-ttu-id="6bafd-134">String</span><span class="sxs-lookup"><span data-stu-id="6bafd-134">String</span></span>|<span data-ttu-id="6bafd-135">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="6bafd-135">Policy display name.</span></span> <span data-ttu-id="6bafd-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6bafd-137">说明</span><span class="sxs-lookup"><span data-stu-id="6bafd-137">description</span></span>|<span data-ttu-id="6bafd-138">String</span><span class="sxs-lookup"><span data-stu-id="6bafd-138">String</span></span>|<span data-ttu-id="6bafd-139">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="6bafd-139">The policy's description.</span></span> <span data-ttu-id="6bafd-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6bafd-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6bafd-141">createdDateTime</span></span>|<span data-ttu-id="6bafd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bafd-142">DateTimeOffset</span></span>|<span data-ttu-id="6bafd-143">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6bafd-143">The date and time the policy was created.</span></span> <span data-ttu-id="6bafd-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6bafd-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bafd-145">lastModifiedDateTime</span></span>|<span data-ttu-id="6bafd-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bafd-146">DateTimeOffset</span></span>|<span data-ttu-id="6bafd-147">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="6bafd-147">Last time the policy was modified.</span></span> <span data-ttu-id="6bafd-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6bafd-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6bafd-149">roleScopeTagIds</span></span>|<span data-ttu-id="6bafd-150">String collection</span><span class="sxs-lookup"><span data-stu-id="6bafd-150">String collection</span></span>|<span data-ttu-id="6bafd-151">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6bafd-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6bafd-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6bafd-153">id</span><span class="sxs-lookup"><span data-stu-id="6bafd-153">id</span></span>|<span data-ttu-id="6bafd-154">String</span><span class="sxs-lookup"><span data-stu-id="6bafd-154">String</span></span>|<span data-ttu-id="6bafd-155">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6bafd-155">Key of the entity.</span></span> <span data-ttu-id="6bafd-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6bafd-157">version</span><span class="sxs-lookup"><span data-stu-id="6bafd-157">version</span></span>|<span data-ttu-id="6bafd-158">String</span><span class="sxs-lookup"><span data-stu-id="6bafd-158">String</span></span>|<span data-ttu-id="6bafd-159">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="6bafd-159">Version of the entity.</span></span> <span data-ttu-id="6bafd-160">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6bafd-161">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="6bafd-161">enforcementLevel</span></span>|[<span data-ttu-id="6bafd-162">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="6bafd-162">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="6bafd-163">WIP 强制级别。请参阅 Enum 定义了解受支持的值 继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="6bafd-163">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="6bafd-164">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="6bafd-164">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="6bafd-165">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="6bafd-165">enterpriseDomain</span></span>|<span data-ttu-id="6bafd-166">String</span><span class="sxs-lookup"><span data-stu-id="6bafd-166">String</span></span>|<span data-ttu-id="6bafd-167">主企业域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-167">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-168">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="6bafd-168">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="6bafd-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bafd-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6bafd-170">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-170">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-171">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="6bafd-171">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="6bafd-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bafd-172">Boolean</span></span>|<span data-ttu-id="6bafd-173">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-173">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-174">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="6bafd-174">dataRecoveryCertificate</span></span>|[<span data-ttu-id="6bafd-175">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="6bafd-175">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="6bafd-176">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="6bafd-176">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="6bafd-177">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-177">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-178">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="6bafd-178">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="6bafd-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bafd-179">Boolean</span></span>|<span data-ttu-id="6bafd-180">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="6bafd-180">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="6bafd-181">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="6bafd-181">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="6bafd-182">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="6bafd-182">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="6bafd-183">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-183">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-184">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="6bafd-184">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="6bafd-185">Guid</span><span class="sxs-lookup"><span data-stu-id="6bafd-185">Guid</span></span>|<span data-ttu-id="6bafd-186">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="6bafd-186">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="6bafd-187">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-187">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-188">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="6bafd-188">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="6bafd-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bafd-189">Boolean</span></span>|<span data-ttu-id="6bafd-190">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-190">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-191">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="6bafd-191">iconsVisible</span></span>|<span data-ttu-id="6bafd-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bafd-192">Boolean</span></span>|<span data-ttu-id="6bafd-193">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="6bafd-193">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="6bafd-194">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-194">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-195">protectedApps</span><span class="sxs-lookup"><span data-stu-id="6bafd-195">protectedApps</span></span>|<span data-ttu-id="6bafd-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bafd-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="6bafd-197">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-197">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-198">exemptApps</span><span class="sxs-lookup"><span data-stu-id="6bafd-198">exemptApps</span></span>|<span data-ttu-id="6bafd-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bafd-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="6bafd-200">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="6bafd-200">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="6bafd-201">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="6bafd-201">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="6bafd-202">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-202">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-203">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="6bafd-203">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="6bafd-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bafd-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6bafd-205">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="6bafd-205">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="6bafd-206">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-206">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-207">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="6bafd-207">enterpriseProxiedDomains</span></span>|<span data-ttu-id="6bafd-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bafd-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="6bafd-209">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="6bafd-209">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="6bafd-210">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="6bafd-210">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="6bafd-211">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="6bafd-211">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="6bafd-212">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-212">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-213">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="6bafd-213">enterpriseIPRanges</span></span>|<span data-ttu-id="6bafd-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bafd-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="6bafd-215">设置定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="6bafd-215">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="6bafd-216">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="6bafd-216">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="6bafd-217">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-217">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-218">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="6bafd-218">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="6bafd-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bafd-219">Boolean</span></span>|<span data-ttu-id="6bafd-220">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="6bafd-220">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="6bafd-221">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-221">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-222">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="6bafd-222">enterpriseProxyServers</span></span>|<span data-ttu-id="6bafd-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bafd-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6bafd-224">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="6bafd-224">This is a list of proxy servers.</span></span> <span data-ttu-id="6bafd-225">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-225">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-226">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="6bafd-226">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="6bafd-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bafd-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6bafd-228">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="6bafd-228">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="6bafd-229">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="6bafd-229">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="6bafd-230">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="6bafd-230">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="6bafd-231">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="6bafd-231">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="6bafd-232">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-232">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-233">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="6bafd-233">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="6bafd-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bafd-234">Boolean</span></span>|<span data-ttu-id="6bafd-235">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="6bafd-235">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="6bafd-236">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-236">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-237">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="6bafd-237">neutralDomainResources</span></span>|<span data-ttu-id="6bafd-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bafd-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6bafd-239">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-239">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-240">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="6bafd-240">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="6bafd-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bafd-241">Boolean</span></span>|<span data-ttu-id="6bafd-242">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-242">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-243">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="6bafd-243">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="6bafd-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bafd-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6bafd-245">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-245">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-246">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6bafd-246">isAssigned</span></span>|<span data-ttu-id="6bafd-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bafd-247">Boolean</span></span>|<span data-ttu-id="6bafd-248">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="6bafd-248">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="6bafd-249">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6bafd-249">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6bafd-250">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="6bafd-250">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="6bafd-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bafd-251">Boolean</span></span>|<span data-ttu-id="6bafd-252">RS2 中的新属性，待定文档</span><span class="sxs-lookup"><span data-stu-id="6bafd-252">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="6bafd-253">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="6bafd-253">mdmEnrollmentUrl</span></span>|<span data-ttu-id="6bafd-254">String</span><span class="sxs-lookup"><span data-stu-id="6bafd-254">String</span></span>|<span data-ttu-id="6bafd-255">MDM 的注册 URL</span><span class="sxs-lookup"><span data-stu-id="6bafd-255">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="6bafd-256">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="6bafd-256">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="6bafd-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bafd-257">Boolean</span></span>|<span data-ttu-id="6bafd-258">将 Windows Hello 企业版设置为登录 Windows 的方法的布尔值。</span><span class="sxs-lookup"><span data-stu-id="6bafd-258">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="6bafd-259">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6bafd-259">pinMinimumLength</span></span>|<span data-ttu-id="6bafd-260">Int32</span><span class="sxs-lookup"><span data-stu-id="6bafd-260">Int32</span></span>|<span data-ttu-id="6bafd-261">整数值，用于设置 PIN 所需的最少字符数。</span><span class="sxs-lookup"><span data-stu-id="6bafd-261">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="6bafd-262">默认值为 4。</span><span class="sxs-lookup"><span data-stu-id="6bafd-262">Default value is 4.</span></span> <span data-ttu-id="6bafd-263">可以为此策略设置配置的最小数量为 4。</span><span class="sxs-lookup"><span data-stu-id="6bafd-263">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="6bafd-264">可以配置的最大数量必须小于最大 PIN 长度策略设置中配置的数量或 127（以最低者为准）。</span><span class="sxs-lookup"><span data-stu-id="6bafd-264">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="6bafd-265">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="6bafd-265">pinUppercaseLetters</span></span>|[<span data-ttu-id="6bafd-266">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="6bafd-266">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="6bafd-267">整数值，用于配置 Windows Hello 企业版 PIN 中的大写字母的使用。</span><span class="sxs-lookup"><span data-stu-id="6bafd-267">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="6bafd-268">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="6bafd-268">Default is NotAllow.</span></span> <span data-ttu-id="6bafd-269">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="6bafd-269">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="6bafd-270">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="6bafd-270">pinLowercaseLetters</span></span>|[<span data-ttu-id="6bafd-271">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="6bafd-271">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="6bafd-272">整数值，用于配置 Windows Hello 企业版 PIN 中的小写字母的使用。</span><span class="sxs-lookup"><span data-stu-id="6bafd-272">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="6bafd-273">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="6bafd-273">Default is NotAllow.</span></span> <span data-ttu-id="6bafd-274">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="6bafd-274">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="6bafd-275">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="6bafd-275">pinSpecialCharacters</span></span>|[<span data-ttu-id="6bafd-276">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="6bafd-276">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="6bafd-277">整数值，用于配置 Windows Hello 企业版 PIN 中的特殊字母的使用。</span><span class="sxs-lookup"><span data-stu-id="6bafd-277">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="6bafd-278">Windows Hello 企业版 PIN 手势的有效特殊字符包括：!</span><span class="sxs-lookup"><span data-stu-id="6bafd-278">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="6bafd-279">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="6bafd-279">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="6bafd-280">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="6bafd-280">/ : ; < = > ?</span></span><span data-ttu-id="6bafd-281"> @ \[ \ \] ^ _ ` { | } ~. Default is NotAllow. Possible values are: ` notAllow `, ` requireAtLeastOne `, ` allow'.</span><span class="sxs-lookup"><span data-stu-id="6bafd-281"> @ \[ \ \] ^ _ ` { | } ~. Default is NotAllow. Possible values are: `notAllow`, `requireAtLeastOne`, `allo\w`.</span></span>|
|<span data-ttu-id="6bafd-282">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6bafd-282">pinExpirationDays</span></span>|<span data-ttu-id="6bafd-283">Int32</span><span class="sxs-lookup"><span data-stu-id="6bafd-283">Int32</span></span>|<span data-ttu-id="6bafd-284">整数值指定在系统要求用户更改 PIN 之前可以使用 PIN 的时间段（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="6bafd-284">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="6bafd-285">可以为此策略设置配置的最大数量为 730。</span><span class="sxs-lookup"><span data-stu-id="6bafd-285">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="6bafd-286">可以为此策略设置配置的最小数量为 0。</span><span class="sxs-lookup"><span data-stu-id="6bafd-286">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="6bafd-287">如果此策略设置为 0，则用户的 PIN 永远不会过期。</span><span class="sxs-lookup"><span data-stu-id="6bafd-287">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="6bafd-288">此节点在 Windows 10 版本 1511 中添加。</span><span class="sxs-lookup"><span data-stu-id="6bafd-288">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="6bafd-289">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="6bafd-289">Default is 0.</span></span>|
|<span data-ttu-id="6bafd-290">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="6bafd-290">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="6bafd-291">Int32</span><span class="sxs-lookup"><span data-stu-id="6bafd-291">Int32</span></span>|<span data-ttu-id="6bafd-292">整数值，用于指定可以关联到无法重用的用户帐户的过去 PIN 的数量。</span><span class="sxs-lookup"><span data-stu-id="6bafd-292">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="6bafd-293">可以为此策略设置配置的最大数量为 50。</span><span class="sxs-lookup"><span data-stu-id="6bafd-293">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="6bafd-294">可以为此策略设置配置的最小数量为 0。</span><span class="sxs-lookup"><span data-stu-id="6bafd-294">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="6bafd-295">如果此策略设置为 0，则不需要存储以前的 PIN。</span><span class="sxs-lookup"><span data-stu-id="6bafd-295">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="6bafd-296">此节点在 Windows 10 版本 1511 中添加。</span><span class="sxs-lookup"><span data-stu-id="6bafd-296">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="6bafd-297">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="6bafd-297">Default is 0.</span></span>|
|<span data-ttu-id="6bafd-298">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="6bafd-298">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="6bafd-299">Int32</span><span class="sxs-lookup"><span data-stu-id="6bafd-299">Int32</span></span>|<span data-ttu-id="6bafd-300">在擦除设备之前允许的身份验证失败次数。</span><span class="sxs-lookup"><span data-stu-id="6bafd-300">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="6bafd-301">值为 0 将禁用设备擦除功能。</span><span class="sxs-lookup"><span data-stu-id="6bafd-301">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="6bafd-302">范围是一个整数 X，其中对于台式机 4 <= X <= 16，对于移动设备 0 <= X <= 999。</span><span class="sxs-lookup"><span data-stu-id="6bafd-302">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="6bafd-303">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="6bafd-303">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="6bafd-304">Int32</span><span class="sxs-lookup"><span data-stu-id="6bafd-304">Int32</span></span>|<span data-ttu-id="6bafd-305">指定设备闲置后将导致设备变为 PIN 或密码锁定的允许的最长时间（以分钟为单位）。</span><span class="sxs-lookup"><span data-stu-id="6bafd-305">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="6bafd-306">范围是整数 X，其中 0 < = X < = 999。</span><span class="sxs-lookup"><span data-stu-id="6bafd-306">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="6bafd-307">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="6bafd-307">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="6bafd-308">Int32</span><span class="sxs-lookup"><span data-stu-id="6bafd-308">Int32</span></span>|<span data-ttu-id="6bafd-309">擦除应用数据之前的脱机间隔时间（天）</span><span class="sxs-lookup"><span data-stu-id="6bafd-309">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="6bafd-310">响应</span><span class="sxs-lookup"><span data-stu-id="6bafd-310">Response</span></span>
<span data-ttu-id="6bafd-311">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6bafd-311">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bafd-312">示例</span><span class="sxs-lookup"><span data-stu-id="6bafd-312">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bafd-313">请求</span><span class="sxs-lookup"><span data-stu-id="6bafd-313">Request</span></span>
<span data-ttu-id="6bafd-314">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6bafd-314">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4365

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
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
          "@odata.type": "microsoft.graph.ipRange"
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

### <a name="response"></a><span data-ttu-id="6bafd-315">响应</span><span class="sxs-lookup"><span data-stu-id="6bafd-315">Response</span></span>
<span data-ttu-id="6bafd-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6bafd-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4537

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
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
          "@odata.type": "microsoft.graph.ipRange"
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




