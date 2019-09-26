---
title: 更新 windowsInformationProtectionPolicy
description: 更新 windowsInformationProtectionPolicy 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a8c28dcbaecefa5eabda4ecdd9777c051fdf85ae
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191335"
---
# <a name="update-windowsinformationprotectionpolicy"></a><span data-ttu-id="41626-103">更新 windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="41626-103">Update windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="41626-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="41626-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41626-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41626-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41626-106">更新 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="41626-106">Update the properties of a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41626-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="41626-107">Prerequisites</span></span>
<span data-ttu-id="41626-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41626-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41626-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="41626-110">Permission type</span></span>|<span data-ttu-id="41626-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41626-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41626-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41626-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41626-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41626-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41626-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41626-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41626-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="41626-115">Not supported.</span></span>|
|<span data-ttu-id="41626-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="41626-116">Application</span></span>|<span data-ttu-id="41626-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41626-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41626-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41626-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="41626-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="41626-119">Request headers</span></span>
|<span data-ttu-id="41626-120">标头</span><span class="sxs-lookup"><span data-stu-id="41626-120">Header</span></span>|<span data-ttu-id="41626-121">值</span><span class="sxs-lookup"><span data-stu-id="41626-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41626-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41626-122">Authorization</span></span>|<span data-ttu-id="41626-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41626-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41626-124">接受</span><span class="sxs-lookup"><span data-stu-id="41626-124">Accept</span></span>|<span data-ttu-id="41626-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41626-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41626-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="41626-126">Request body</span></span>
<span data-ttu-id="41626-127">在请求正文中，提供 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41626-127">In the request body, supply a JSON representation for the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="41626-128">下表显示创建 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="41626-128">The following table shows the properties that are required when you create the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="41626-129">属性</span><span class="sxs-lookup"><span data-stu-id="41626-129">Property</span></span>|<span data-ttu-id="41626-130">类型</span><span class="sxs-lookup"><span data-stu-id="41626-130">Type</span></span>|<span data-ttu-id="41626-131">说明</span><span class="sxs-lookup"><span data-stu-id="41626-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41626-132">displayName</span><span class="sxs-lookup"><span data-stu-id="41626-132">displayName</span></span>|<span data-ttu-id="41626-133">字符串</span><span class="sxs-lookup"><span data-stu-id="41626-133">String</span></span>|<span data-ttu-id="41626-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="41626-134">Policy display name.</span></span> <span data-ttu-id="41626-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41626-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="41626-136">说明</span><span class="sxs-lookup"><span data-stu-id="41626-136">description</span></span>|<span data-ttu-id="41626-137">String</span><span class="sxs-lookup"><span data-stu-id="41626-137">String</span></span>|<span data-ttu-id="41626-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="41626-138">The policy's description.</span></span> <span data-ttu-id="41626-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41626-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="41626-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41626-140">createdDateTime</span></span>|<span data-ttu-id="41626-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41626-141">DateTimeOffset</span></span>|<span data-ttu-id="41626-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="41626-142">The date and time the policy was created.</span></span> <span data-ttu-id="41626-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41626-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="41626-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41626-144">lastModifiedDateTime</span></span>|<span data-ttu-id="41626-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41626-145">DateTimeOffset</span></span>|<span data-ttu-id="41626-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="41626-146">Last time the policy was modified.</span></span> <span data-ttu-id="41626-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41626-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="41626-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="41626-148">roleScopeTagIds</span></span>|<span data-ttu-id="41626-149">String collection</span><span class="sxs-lookup"><span data-stu-id="41626-149">String collection</span></span>|<span data-ttu-id="41626-150">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="41626-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="41626-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41626-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="41626-152">id</span><span class="sxs-lookup"><span data-stu-id="41626-152">id</span></span>|<span data-ttu-id="41626-153">字符串</span><span class="sxs-lookup"><span data-stu-id="41626-153">String</span></span>|<span data-ttu-id="41626-154">实体的键。</span><span class="sxs-lookup"><span data-stu-id="41626-154">Key of the entity.</span></span> <span data-ttu-id="41626-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41626-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="41626-156">version</span><span class="sxs-lookup"><span data-stu-id="41626-156">version</span></span>|<span data-ttu-id="41626-157">String</span><span class="sxs-lookup"><span data-stu-id="41626-157">String</span></span>|<span data-ttu-id="41626-158">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="41626-158">Version of the entity.</span></span> <span data-ttu-id="41626-159">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41626-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="41626-160">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="41626-160">enforcementLevel</span></span>|[<span data-ttu-id="41626-161">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="41626-161">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="41626-162">WIP 强制等级。若要获取从[WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)继承的受支持值的枚举定义，请参阅。</span><span class="sxs-lookup"><span data-stu-id="41626-162">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="41626-163">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="41626-163">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="41626-164">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="41626-164">enterpriseDomain</span></span>|<span data-ttu-id="41626-165">String</span><span class="sxs-lookup"><span data-stu-id="41626-165">String</span></span>|<span data-ttu-id="41626-166">主企业域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-166">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-167">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="41626-167">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="41626-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41626-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="41626-169">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-169">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-170">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="41626-170">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="41626-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="41626-171">Boolean</span></span>|<span data-ttu-id="41626-172">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-172">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-173">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="41626-173">dataRecoveryCertificate</span></span>|[<span data-ttu-id="41626-174">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="41626-174">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="41626-175">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="41626-175">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="41626-176">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-176">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-177">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="41626-177">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="41626-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="41626-178">Boolean</span></span>|<span data-ttu-id="41626-179">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="41626-179">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="41626-180">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="41626-180">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="41626-181">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="41626-181">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="41626-182">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-182">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-183">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="41626-183">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="41626-184">Guid</span><span class="sxs-lookup"><span data-stu-id="41626-184">Guid</span></span>|<span data-ttu-id="41626-185">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="41626-185">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="41626-186">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-186">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-187">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="41626-187">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="41626-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="41626-188">Boolean</span></span>|<span data-ttu-id="41626-189">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-189">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-190">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="41626-190">iconsVisible</span></span>|<span data-ttu-id="41626-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="41626-191">Boolean</span></span>|<span data-ttu-id="41626-192">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="41626-192">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="41626-193">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-193">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-194">protectedApps</span><span class="sxs-lookup"><span data-stu-id="41626-194">protectedApps</span></span>|<span data-ttu-id="41626-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41626-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="41626-196">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-196">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-197">exemptApps</span><span class="sxs-lookup"><span data-stu-id="41626-197">exemptApps</span></span>|<span data-ttu-id="41626-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41626-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="41626-199">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="41626-199">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="41626-200">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="41626-200">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="41626-201">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-201">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-202">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="41626-202">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="41626-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41626-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="41626-204">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="41626-204">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="41626-205">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-205">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-206">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="41626-206">enterpriseProxiedDomains</span></span>|<span data-ttu-id="41626-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41626-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="41626-208">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="41626-208">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="41626-209">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="41626-209">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="41626-210">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="41626-210">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="41626-211">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-211">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-212">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="41626-212">enterpriseIPRanges</span></span>|<span data-ttu-id="41626-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41626-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="41626-214">设置定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="41626-214">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="41626-215">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="41626-215">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="41626-216">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-216">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-217">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="41626-217">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="41626-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="41626-218">Boolean</span></span>|<span data-ttu-id="41626-219">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="41626-219">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="41626-220">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-220">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-221">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="41626-221">enterpriseProxyServers</span></span>|<span data-ttu-id="41626-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41626-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="41626-223">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="41626-223">This is a list of proxy servers.</span></span> <span data-ttu-id="41626-224">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-224">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-225">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="41626-225">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="41626-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41626-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="41626-227">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="41626-227">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="41626-228">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="41626-228">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="41626-229">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="41626-229">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="41626-230">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="41626-230">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="41626-231">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-231">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-232">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="41626-232">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="41626-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="41626-233">Boolean</span></span>|<span data-ttu-id="41626-234">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="41626-234">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="41626-235">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-235">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-236">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="41626-236">neutralDomainResources</span></span>|<span data-ttu-id="41626-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41626-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="41626-238">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-238">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-239">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="41626-239">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="41626-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="41626-240">Boolean</span></span>|<span data-ttu-id="41626-241">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-241">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-242">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="41626-242">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="41626-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41626-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="41626-244">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-244">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-245">isAssigned</span><span class="sxs-lookup"><span data-stu-id="41626-245">isAssigned</span></span>|<span data-ttu-id="41626-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="41626-246">Boolean</span></span>|<span data-ttu-id="41626-247">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="41626-247">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="41626-248">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41626-248">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41626-249">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="41626-249">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="41626-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="41626-250">Boolean</span></span>|<span data-ttu-id="41626-251">RS2 中的新属性，待定文档</span><span class="sxs-lookup"><span data-stu-id="41626-251">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="41626-252">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="41626-252">mdmEnrollmentUrl</span></span>|<span data-ttu-id="41626-253">String</span><span class="sxs-lookup"><span data-stu-id="41626-253">String</span></span>|<span data-ttu-id="41626-254">MDM 的注册 URL</span><span class="sxs-lookup"><span data-stu-id="41626-254">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="41626-255">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="41626-255">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="41626-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="41626-256">Boolean</span></span>|<span data-ttu-id="41626-257">将 Windows Hello 企业版设置为登录 Windows 的方法的布尔值。</span><span class="sxs-lookup"><span data-stu-id="41626-257">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="41626-258">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="41626-258">pinMinimumLength</span></span>|<span data-ttu-id="41626-259">Int32</span><span class="sxs-lookup"><span data-stu-id="41626-259">Int32</span></span>|<span data-ttu-id="41626-260">整数值，用于设置 PIN 所需的最少字符数。</span><span class="sxs-lookup"><span data-stu-id="41626-260">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="41626-261">默认值为 4。</span><span class="sxs-lookup"><span data-stu-id="41626-261">Default value is 4.</span></span> <span data-ttu-id="41626-262">可以为此策略设置配置的最小数量为 4。</span><span class="sxs-lookup"><span data-stu-id="41626-262">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="41626-263">可以配置的最大数量必须小于最大 PIN 长度策略设置中配置的数量或 127（以最低者为准）。</span><span class="sxs-lookup"><span data-stu-id="41626-263">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="41626-264">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="41626-264">pinUppercaseLetters</span></span>|[<span data-ttu-id="41626-265">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="41626-265">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="41626-266">整数值，用于配置 Windows Hello 企业版 PIN 中的大写字母的使用。</span><span class="sxs-lookup"><span data-stu-id="41626-266">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="41626-267">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="41626-267">Default is NotAllow.</span></span> <span data-ttu-id="41626-268">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="41626-268">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="41626-269">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="41626-269">pinLowercaseLetters</span></span>|[<span data-ttu-id="41626-270">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="41626-270">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="41626-271">整数值，用于配置 Windows Hello 企业版 PIN 中的小写字母的使用。</span><span class="sxs-lookup"><span data-stu-id="41626-271">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="41626-272">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="41626-272">Default is NotAllow.</span></span> <span data-ttu-id="41626-273">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="41626-273">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="41626-274">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="41626-274">pinSpecialCharacters</span></span>|[<span data-ttu-id="41626-275">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="41626-275">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="41626-276">整数值，用于配置 Windows Hello 企业版 PIN 中的特殊字母的使用。</span><span class="sxs-lookup"><span data-stu-id="41626-276">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="41626-277">Windows Hello 企业版 PIN 手势的有效特殊字符包括：!</span><span class="sxs-lookup"><span data-stu-id="41626-277">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="41626-278">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="41626-278">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="41626-279">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="41626-279">/ : ; < = > ?</span></span><span data-ttu-id="41626-280"> @ \[ \ \]^ _ ` { | } ~. Default is NotAllow. Possible values are: `notAllow`, `requireAtLeastOne`, `允许 "。</span><span class="sxs-lookup"><span data-stu-id="41626-280"> @ \[ \ \] ^ _ ` { | } ~. Default is NotAllow. Possible values are: `notAllow`, `requireAtLeastOne`, `allo\w`.</span></span>|
|<span data-ttu-id="41626-281">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="41626-281">pinExpirationDays</span></span>|<span data-ttu-id="41626-282">Int32</span><span class="sxs-lookup"><span data-stu-id="41626-282">Int32</span></span>|<span data-ttu-id="41626-283">整数值指定在系统要求用户更改 PIN 之前可以使用 PIN 的时间段（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="41626-283">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="41626-284">可以为此策略设置配置的最大数量为 730。</span><span class="sxs-lookup"><span data-stu-id="41626-284">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="41626-285">可以为此策略设置配置的最小数量为 0。</span><span class="sxs-lookup"><span data-stu-id="41626-285">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="41626-286">如果此策略设置为 0，则用户的 PIN 永远不会过期。</span><span class="sxs-lookup"><span data-stu-id="41626-286">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="41626-287">此节点在 Windows 10 版本 1511 中添加。</span><span class="sxs-lookup"><span data-stu-id="41626-287">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="41626-288">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="41626-288">Default is 0.</span></span>|
|<span data-ttu-id="41626-289">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="41626-289">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="41626-290">Int32</span><span class="sxs-lookup"><span data-stu-id="41626-290">Int32</span></span>|<span data-ttu-id="41626-291">整数值，用于指定可以关联到无法重用的用户帐户的过去 PIN 的数量。</span><span class="sxs-lookup"><span data-stu-id="41626-291">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="41626-292">可以为此策略设置配置的最大数量为 50。</span><span class="sxs-lookup"><span data-stu-id="41626-292">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="41626-293">可以为此策略设置配置的最小数量为 0。</span><span class="sxs-lookup"><span data-stu-id="41626-293">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="41626-294">如果此策略设置为 0，则不需要存储以前的 PIN。</span><span class="sxs-lookup"><span data-stu-id="41626-294">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="41626-295">此节点在 Windows 10 版本 1511 中添加。</span><span class="sxs-lookup"><span data-stu-id="41626-295">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="41626-296">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="41626-296">Default is 0.</span></span>|
|<span data-ttu-id="41626-297">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="41626-297">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="41626-298">Int32</span><span class="sxs-lookup"><span data-stu-id="41626-298">Int32</span></span>|<span data-ttu-id="41626-299">在擦除设备之前允许的身份验证失败次数。</span><span class="sxs-lookup"><span data-stu-id="41626-299">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="41626-300">值为 0 将禁用设备擦除功能。</span><span class="sxs-lookup"><span data-stu-id="41626-300">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="41626-301">范围是一个整数 X，其中对于台式机 4 <= X <= 16，对于移动设备 0 <= X <= 999。</span><span class="sxs-lookup"><span data-stu-id="41626-301">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="41626-302">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="41626-302">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="41626-303">Int32</span><span class="sxs-lookup"><span data-stu-id="41626-303">Int32</span></span>|<span data-ttu-id="41626-304">指定设备闲置后将导致设备变为 PIN 或密码锁定的允许的最长时间（以分钟为单位）。</span><span class="sxs-lookup"><span data-stu-id="41626-304">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="41626-305">范围是整数 X，其中 0 < = X < = 999。</span><span class="sxs-lookup"><span data-stu-id="41626-305">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="41626-306">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="41626-306">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="41626-307">Int32</span><span class="sxs-lookup"><span data-stu-id="41626-307">Int32</span></span>|<span data-ttu-id="41626-308">擦除应用数据之前的脱机间隔时间（天）</span><span class="sxs-lookup"><span data-stu-id="41626-308">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="41626-309">响应</span><span class="sxs-lookup"><span data-stu-id="41626-309">Response</span></span>
<span data-ttu-id="41626-310">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41626-310">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41626-311">示例</span><span class="sxs-lookup"><span data-stu-id="41626-311">Example</span></span>

### <a name="request"></a><span data-ttu-id="41626-312">请求</span><span class="sxs-lookup"><span data-stu-id="41626-312">Request</span></span>
<span data-ttu-id="41626-313">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41626-313">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
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

### <a name="response"></a><span data-ttu-id="41626-314">响应</span><span class="sxs-lookup"><span data-stu-id="41626-314">Response</span></span>
<span data-ttu-id="41626-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41626-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




