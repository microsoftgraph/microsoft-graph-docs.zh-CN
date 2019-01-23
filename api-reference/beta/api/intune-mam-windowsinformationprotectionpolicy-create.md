---
title: 创建 windowsInformationProtectionPolicy
description: 创建新的 windowsInformationProtectionPolicy 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74d9e4a8ddd9ae0979a6360eaf229396b2e107bb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416606"
---
# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="f5257-103">创建 windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="f5257-103">Create windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="f5257-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f5257-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f5257-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f5257-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5257-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5257-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5257-107">创建新的 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5257-107">Create a new [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5257-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f5257-108">Prerequisites</span></span>
<span data-ttu-id="f5257-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f5257-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f5257-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5257-111">Permission type</span></span>|<span data-ttu-id="f5257-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f5257-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5257-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5257-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5257-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5257-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f5257-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5257-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5257-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5257-116">Not supported.</span></span>|
|<span data-ttu-id="f5257-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5257-117">Application</span></span>|<span data-ttu-id="f5257-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5257-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5257-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5257-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f5257-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5257-120">Request headers</span></span>
|<span data-ttu-id="f5257-121">标头</span><span class="sxs-lookup"><span data-stu-id="f5257-121">Header</span></span>|<span data-ttu-id="f5257-122">值</span><span class="sxs-lookup"><span data-stu-id="f5257-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5257-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5257-123">Authorization</span></span>|<span data-ttu-id="f5257-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f5257-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5257-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f5257-125">Accept</span></span>|<span data-ttu-id="f5257-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5257-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5257-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5257-127">Request body</span></span>
<span data-ttu-id="f5257-128">在请求正文中，提供 windowsInformationProtectionPolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5257-128">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="f5257-129">下表显示创建 windowsInformationProtectionPolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f5257-129">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="f5257-130">属性</span><span class="sxs-lookup"><span data-stu-id="f5257-130">Property</span></span>|<span data-ttu-id="f5257-131">类型</span><span class="sxs-lookup"><span data-stu-id="f5257-131">Type</span></span>|<span data-ttu-id="f5257-132">说明</span><span class="sxs-lookup"><span data-stu-id="f5257-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5257-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f5257-133">displayName</span></span>|<span data-ttu-id="f5257-134">String</span><span class="sxs-lookup"><span data-stu-id="f5257-134">String</span></span>|<span data-ttu-id="f5257-135">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="f5257-135">Policy display name.</span></span> <span data-ttu-id="f5257-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f5257-137">description</span><span class="sxs-lookup"><span data-stu-id="f5257-137">description</span></span>|<span data-ttu-id="f5257-138">String</span><span class="sxs-lookup"><span data-stu-id="f5257-138">String</span></span>|<span data-ttu-id="f5257-139">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="f5257-139">The policy's description.</span></span> <span data-ttu-id="f5257-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f5257-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5257-141">createdDateTime</span></span>|<span data-ttu-id="f5257-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5257-142">DateTimeOffset</span></span>|<span data-ttu-id="f5257-143">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f5257-143">The date and time the policy was created.</span></span> <span data-ttu-id="f5257-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f5257-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5257-145">lastModifiedDateTime</span></span>|<span data-ttu-id="f5257-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5257-146">DateTimeOffset</span></span>|<span data-ttu-id="f5257-147">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="f5257-147">Last time the policy was modified.</span></span> <span data-ttu-id="f5257-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f5257-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f5257-149">roleScopeTagIds</span></span>|<span data-ttu-id="f5257-150">String 集合</span><span class="sxs-lookup"><span data-stu-id="f5257-150">String collection</span></span>|<span data-ttu-id="f5257-151">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="f5257-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f5257-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f5257-153">id</span><span class="sxs-lookup"><span data-stu-id="f5257-153">id</span></span>|<span data-ttu-id="f5257-154">String</span><span class="sxs-lookup"><span data-stu-id="f5257-154">String</span></span>|<span data-ttu-id="f5257-155">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f5257-155">Key of the entity.</span></span> <span data-ttu-id="f5257-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f5257-157">version</span><span class="sxs-lookup"><span data-stu-id="f5257-157">version</span></span>|<span data-ttu-id="f5257-158">String</span><span class="sxs-lookup"><span data-stu-id="f5257-158">String</span></span>|<span data-ttu-id="f5257-159">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="f5257-159">Version of the entity.</span></span> <span data-ttu-id="f5257-160">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f5257-161">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="f5257-161">enforcementLevel</span></span>|[<span data-ttu-id="f5257-162">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="f5257-162">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="f5257-163">WIP 实施级别。请参见支持值继承[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)枚举定义。</span><span class="sxs-lookup"><span data-stu-id="f5257-163">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="f5257-164">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="f5257-164">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="f5257-165">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="f5257-165">enterpriseDomain</span></span>|<span data-ttu-id="f5257-166">String</span><span class="sxs-lookup"><span data-stu-id="f5257-166">String</span></span>|<span data-ttu-id="f5257-167">主企业域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-167">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-168">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="f5257-168">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="f5257-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5257-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="f5257-170">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-170">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-171">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="f5257-171">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="f5257-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5257-172">Boolean</span></span>|<span data-ttu-id="f5257-173">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-173">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-174">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="f5257-174">dataRecoveryCertificate</span></span>|[<span data-ttu-id="f5257-175">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="f5257-175">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="f5257-176">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="f5257-176">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="f5257-177">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-177">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-178">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="f5257-178">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="f5257-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5257-179">Boolean</span></span>|<span data-ttu-id="f5257-180">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="f5257-180">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="f5257-181">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="f5257-181">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="f5257-182">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="f5257-182">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="f5257-183">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-183">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-184">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="f5257-184">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="f5257-185">Guid</span><span class="sxs-lookup"><span data-stu-id="f5257-185">Guid</span></span>|<span data-ttu-id="f5257-186">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="f5257-186">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="f5257-187">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-187">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-188">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="f5257-188">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="f5257-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5257-189">Boolean</span></span>|<span data-ttu-id="f5257-190">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-190">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-191">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="f5257-191">iconsVisible</span></span>|<span data-ttu-id="f5257-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5257-192">Boolean</span></span>|<span data-ttu-id="f5257-193">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="f5257-193">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="f5257-194">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-194">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-195">protectedApps</span><span class="sxs-lookup"><span data-stu-id="f5257-195">protectedApps</span></span>|<span data-ttu-id="f5257-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5257-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="f5257-197">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-197">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-198">exemptApps</span><span class="sxs-lookup"><span data-stu-id="f5257-198">exemptApps</span></span>|<span data-ttu-id="f5257-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5257-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="f5257-200">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="f5257-200">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="f5257-201">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="f5257-201">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="f5257-202">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-202">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-203">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="f5257-203">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="f5257-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5257-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="f5257-205">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="f5257-205">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="f5257-206">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-206">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-207">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="f5257-207">enterpriseProxiedDomains</span></span>|<span data-ttu-id="f5257-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5257-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="f5257-209">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="f5257-209">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="f5257-210">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="f5257-210">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="f5257-211">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="f5257-211">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="f5257-212">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-212">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-213">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="f5257-213">enterpriseIPRanges</span></span>|<span data-ttu-id="f5257-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5257-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="f5257-215">设置可定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="f5257-215">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="f5257-216">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="f5257-216">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="f5257-217">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-217">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-218">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="f5257-218">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="f5257-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5257-219">Boolean</span></span>|<span data-ttu-id="f5257-220">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="f5257-220">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="f5257-221">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-221">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-222">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="f5257-222">enterpriseProxyServers</span></span>|<span data-ttu-id="f5257-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5257-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="f5257-224">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="f5257-224">This is a list of proxy servers.</span></span> <span data-ttu-id="f5257-225">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-225">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-226">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="f5257-226">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="f5257-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5257-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="f5257-228">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="f5257-228">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="f5257-229">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="f5257-229">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="f5257-230">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="f5257-230">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="f5257-231">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="f5257-231">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="f5257-232">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-232">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-233">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="f5257-233">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="f5257-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5257-234">Boolean</span></span>|<span data-ttu-id="f5257-235">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="f5257-235">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="f5257-236">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-236">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-237">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="f5257-237">neutralDomainResources</span></span>|<span data-ttu-id="f5257-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5257-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="f5257-239">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-239">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-240">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="f5257-240">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="f5257-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5257-241">Boolean</span></span>|<span data-ttu-id="f5257-242">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-242">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-243">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="f5257-243">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="f5257-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5257-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="f5257-245">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-245">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-246">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f5257-246">isAssigned</span></span>|<span data-ttu-id="f5257-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5257-247">Boolean</span></span>|<span data-ttu-id="f5257-248">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="f5257-248">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="f5257-249">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f5257-249">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f5257-250">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="f5257-250">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="f5257-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5257-251">Boolean</span></span>|<span data-ttu-id="f5257-252">RS2 中的新属性，待定文档</span><span class="sxs-lookup"><span data-stu-id="f5257-252">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="f5257-253">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="f5257-253">mdmEnrollmentUrl</span></span>|<span data-ttu-id="f5257-254">String</span><span class="sxs-lookup"><span data-stu-id="f5257-254">String</span></span>|<span data-ttu-id="f5257-255">MDM 的注册 URL</span><span class="sxs-lookup"><span data-stu-id="f5257-255">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="f5257-256">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="f5257-256">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="f5257-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5257-257">Boolean</span></span>|<span data-ttu-id="f5257-258">将 Windows Hello 企业版设置为登录 Windows 的方法的布尔值。</span><span class="sxs-lookup"><span data-stu-id="f5257-258">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="f5257-259">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f5257-259">pinMinimumLength</span></span>|<span data-ttu-id="f5257-260">Int32</span><span class="sxs-lookup"><span data-stu-id="f5257-260">Int32</span></span>|<span data-ttu-id="f5257-261">整数值，用于设置 PIN 所需的最少字符数。</span><span class="sxs-lookup"><span data-stu-id="f5257-261">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="f5257-262">默认值为 4。</span><span class="sxs-lookup"><span data-stu-id="f5257-262">Default value is 4.</span></span> <span data-ttu-id="f5257-263">可以为此策略设置配置的最小数量为 4。</span><span class="sxs-lookup"><span data-stu-id="f5257-263">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="f5257-264">可以配置的最大数量必须小于最大 PIN 长度策略设置中配置的数量或 127（以最低者为准）。</span><span class="sxs-lookup"><span data-stu-id="f5257-264">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="f5257-265">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="f5257-265">pinUppercaseLetters</span></span>|[<span data-ttu-id="f5257-266">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="f5257-266">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="f5257-267">整数值，用于配置 Windows Hello 企业版 PIN 中的大写字母的使用。</span><span class="sxs-lookup"><span data-stu-id="f5257-267">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="f5257-268">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="f5257-268">Default is NotAllow.</span></span> <span data-ttu-id="f5257-269">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="f5257-269">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="f5257-270">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="f5257-270">pinLowercaseLetters</span></span>|[<span data-ttu-id="f5257-271">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="f5257-271">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="f5257-272">整数值，用于配置 Windows Hello 企业版 PIN 中的小写字母的使用。</span><span class="sxs-lookup"><span data-stu-id="f5257-272">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="f5257-273">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="f5257-273">Default is NotAllow.</span></span> <span data-ttu-id="f5257-274">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="f5257-274">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="f5257-275">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="f5257-275">pinSpecialCharacters</span></span>|[<span data-ttu-id="f5257-276">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="f5257-276">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="f5257-277">整数值，用于配置 Windows Hello 企业版 PIN 中的特殊字母的使用。</span><span class="sxs-lookup"><span data-stu-id="f5257-277">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="f5257-278">Windows Hello 企业版 PIN 手势的有效特殊字符包括：!</span><span class="sxs-lookup"><span data-stu-id="f5257-278">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="f5257-279">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="f5257-279">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="f5257-280">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="f5257-280">/ : ; < = > ?</span></span><span data-ttu-id="f5257-281"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="f5257-281"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="f5257-282">} ~。</span><span class="sxs-lookup"><span data-stu-id="f5257-282">} ~.</span></span> <span data-ttu-id="f5257-283">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="f5257-283">Default is NotAllow.</span></span> <span data-ttu-id="f5257-284">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="f5257-284">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="f5257-285">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f5257-285">pinExpirationDays</span></span>|<span data-ttu-id="f5257-286">Int32</span><span class="sxs-lookup"><span data-stu-id="f5257-286">Int32</span></span>|<span data-ttu-id="f5257-287">整数值指定在系统要求用户更改 PIN 之前可以使用 PIN 的时间段（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="f5257-287">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="f5257-288">可以为此策略设置配置的最大数量为 730。</span><span class="sxs-lookup"><span data-stu-id="f5257-288">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="f5257-289">可以为此策略设置配置的最小数量为 0。</span><span class="sxs-lookup"><span data-stu-id="f5257-289">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="f5257-290">如果此策略设置为 0，则用户的 PIN 永远不会过期。</span><span class="sxs-lookup"><span data-stu-id="f5257-290">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="f5257-291">此节点在 Windows 10 版本 1511 中添加。</span><span class="sxs-lookup"><span data-stu-id="f5257-291">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="f5257-292">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="f5257-292">Default is 0.</span></span>|
|<span data-ttu-id="f5257-293">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="f5257-293">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="f5257-294">Int32</span><span class="sxs-lookup"><span data-stu-id="f5257-294">Int32</span></span>|<span data-ttu-id="f5257-295">整数值，用于指定可以关联到无法重用的用户帐户的过去 PIN 的数量。</span><span class="sxs-lookup"><span data-stu-id="f5257-295">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="f5257-296">可以为此策略设置配置的最大数量为 50。</span><span class="sxs-lookup"><span data-stu-id="f5257-296">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="f5257-297">可以为此策略设置配置的最小数量为 0。</span><span class="sxs-lookup"><span data-stu-id="f5257-297">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="f5257-298">如果此策略设置为 0，则不需要存储以前的 PIN。</span><span class="sxs-lookup"><span data-stu-id="f5257-298">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="f5257-299">此节点在 Windows 10 版本 1511 中添加。</span><span class="sxs-lookup"><span data-stu-id="f5257-299">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="f5257-300">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="f5257-300">Default is 0.</span></span>|
|<span data-ttu-id="f5257-301">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="f5257-301">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="f5257-302">Int32</span><span class="sxs-lookup"><span data-stu-id="f5257-302">Int32</span></span>|<span data-ttu-id="f5257-303">在擦除设备之前允许的身份验证失败次数。</span><span class="sxs-lookup"><span data-stu-id="f5257-303">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="f5257-304">值为 0 将禁用设备擦除功能。</span><span class="sxs-lookup"><span data-stu-id="f5257-304">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="f5257-305">范围是一个整数 X，其中对于台式机 4 <= X <= 16，对于移动设备 0 <= X <= 999。</span><span class="sxs-lookup"><span data-stu-id="f5257-305">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="f5257-306">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="f5257-306">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="f5257-307">Int32</span><span class="sxs-lookup"><span data-stu-id="f5257-307">Int32</span></span>|<span data-ttu-id="f5257-308">指定设备闲置后将导致设备变为 PIN 或密码锁定的允许的最长时间（以分钟为单位）。</span><span class="sxs-lookup"><span data-stu-id="f5257-308">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="f5257-309">范围是整数 X，其中 0 < = X < = 999。</span><span class="sxs-lookup"><span data-stu-id="f5257-309">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="f5257-310">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="f5257-310">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="f5257-311">Int32</span><span class="sxs-lookup"><span data-stu-id="f5257-311">Int32</span></span>|<span data-ttu-id="f5257-312">擦除应用数据之前的脱机间隔时间（天）</span><span class="sxs-lookup"><span data-stu-id="f5257-312">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="f5257-313">响应</span><span class="sxs-lookup"><span data-stu-id="f5257-313">Response</span></span>
<span data-ttu-id="f5257-314">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5257-314">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5257-315">示例</span><span class="sxs-lookup"><span data-stu-id="f5257-315">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5257-316">请求</span><span class="sxs-lookup"><span data-stu-id="f5257-316">Request</span></span>
<span data-ttu-id="f5257-317">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5257-317">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4467

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

### <a name="response"></a><span data-ttu-id="f5257-318">响应</span><span class="sxs-lookup"><span data-stu-id="f5257-318">Response</span></span>
<span data-ttu-id="f5257-p133">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f5257-p133">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4639

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




