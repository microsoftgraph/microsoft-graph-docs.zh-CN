---
title: 创建 mdmWindowsInformationProtectionPolicy
description: 创建新的 mdmWindowsInformationProtectionPolicy 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 88407774cf16f5225b5478ce1c70d414216c742f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994535"
---
# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="989e5-103">创建 mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="989e5-103">Create mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="989e5-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="989e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="989e5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="989e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="989e5-106">创建新的 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="989e5-106">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="989e5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="989e5-107">Prerequisites</span></span>
<span data-ttu-id="989e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="989e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="989e5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="989e5-110">Permission type</span></span>|<span data-ttu-id="989e5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="989e5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="989e5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="989e5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="989e5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="989e5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="989e5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="989e5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="989e5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="989e5-115">Not supported.</span></span>|
|<span data-ttu-id="989e5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="989e5-116">Application</span></span>|<span data-ttu-id="989e5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="989e5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="989e5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="989e5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="989e5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="989e5-119">Request headers</span></span>
|<span data-ttu-id="989e5-120">标头</span><span class="sxs-lookup"><span data-stu-id="989e5-120">Header</span></span>|<span data-ttu-id="989e5-121">值</span><span class="sxs-lookup"><span data-stu-id="989e5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="989e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="989e5-122">Authorization</span></span>|<span data-ttu-id="989e5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="989e5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="989e5-124">接受</span><span class="sxs-lookup"><span data-stu-id="989e5-124">Accept</span></span>|<span data-ttu-id="989e5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="989e5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="989e5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="989e5-126">Request body</span></span>
<span data-ttu-id="989e5-127">在请求正文中，提供 mdmWindowsInformationProtectionPolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="989e5-127">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="989e5-128">下表显示创建 mdmWindowsInformationProtectionPolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="989e5-128">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="989e5-129">属性</span><span class="sxs-lookup"><span data-stu-id="989e5-129">Property</span></span>|<span data-ttu-id="989e5-130">类型</span><span class="sxs-lookup"><span data-stu-id="989e5-130">Type</span></span>|<span data-ttu-id="989e5-131">说明</span><span class="sxs-lookup"><span data-stu-id="989e5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="989e5-132">displayName</span><span class="sxs-lookup"><span data-stu-id="989e5-132">displayName</span></span>|<span data-ttu-id="989e5-133">字符串</span><span class="sxs-lookup"><span data-stu-id="989e5-133">String</span></span>|<span data-ttu-id="989e5-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="989e5-134">Policy display name.</span></span> <span data-ttu-id="989e5-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="989e5-136">说明</span><span class="sxs-lookup"><span data-stu-id="989e5-136">description</span></span>|<span data-ttu-id="989e5-137">String</span><span class="sxs-lookup"><span data-stu-id="989e5-137">String</span></span>|<span data-ttu-id="989e5-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="989e5-138">The policy's description.</span></span> <span data-ttu-id="989e5-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="989e5-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="989e5-140">createdDateTime</span></span>|<span data-ttu-id="989e5-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="989e5-141">DateTimeOffset</span></span>|<span data-ttu-id="989e5-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="989e5-142">The date and time the policy was created.</span></span> <span data-ttu-id="989e5-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="989e5-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="989e5-144">lastModifiedDateTime</span></span>|<span data-ttu-id="989e5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="989e5-145">DateTimeOffset</span></span>|<span data-ttu-id="989e5-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="989e5-146">Last time the policy was modified.</span></span> <span data-ttu-id="989e5-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="989e5-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="989e5-148">roleScopeTagIds</span></span>|<span data-ttu-id="989e5-149">String collection</span><span class="sxs-lookup"><span data-stu-id="989e5-149">String collection</span></span>|<span data-ttu-id="989e5-150">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="989e5-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="989e5-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="989e5-152">id</span><span class="sxs-lookup"><span data-stu-id="989e5-152">id</span></span>|<span data-ttu-id="989e5-153">字符串</span><span class="sxs-lookup"><span data-stu-id="989e5-153">String</span></span>|<span data-ttu-id="989e5-154">实体的键。</span><span class="sxs-lookup"><span data-stu-id="989e5-154">Key of the entity.</span></span> <span data-ttu-id="989e5-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="989e5-156">version</span><span class="sxs-lookup"><span data-stu-id="989e5-156">version</span></span>|<span data-ttu-id="989e5-157">String</span><span class="sxs-lookup"><span data-stu-id="989e5-157">String</span></span>|<span data-ttu-id="989e5-158">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="989e5-158">Version of the entity.</span></span> <span data-ttu-id="989e5-159">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="989e5-160">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="989e5-160">enforcementLevel</span></span>|[<span data-ttu-id="989e5-161">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="989e5-161">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="989e5-162">WIP 强制等级。若要获取从[WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)继承的受支持值的枚举定义, 请参阅。</span><span class="sxs-lookup"><span data-stu-id="989e5-162">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="989e5-163">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="989e5-163">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="989e5-164">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="989e5-164">enterpriseDomain</span></span>|<span data-ttu-id="989e5-165">String</span><span class="sxs-lookup"><span data-stu-id="989e5-165">String</span></span>|<span data-ttu-id="989e5-166">主企业域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-166">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-167">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="989e5-167">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="989e5-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989e5-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="989e5-169">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-169">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-170">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="989e5-170">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="989e5-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="989e5-171">Boolean</span></span>|<span data-ttu-id="989e5-172">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-172">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-173">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="989e5-173">dataRecoveryCertificate</span></span>|[<span data-ttu-id="989e5-174">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="989e5-174">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="989e5-175">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="989e5-175">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="989e5-176">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-176">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-177">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="989e5-177">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="989e5-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="989e5-178">Boolean</span></span>|<span data-ttu-id="989e5-179">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="989e5-179">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="989e5-180">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="989e5-180">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="989e5-181">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="989e5-181">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="989e5-182">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-182">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-183">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="989e5-183">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="989e5-184">Guid</span><span class="sxs-lookup"><span data-stu-id="989e5-184">Guid</span></span>|<span data-ttu-id="989e5-185">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="989e5-185">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="989e5-186">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-186">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-187">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="989e5-187">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="989e5-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="989e5-188">Boolean</span></span>|<span data-ttu-id="989e5-189">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-189">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-190">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="989e5-190">iconsVisible</span></span>|<span data-ttu-id="989e5-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="989e5-191">Boolean</span></span>|<span data-ttu-id="989e5-192">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="989e5-192">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="989e5-193">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-193">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-194">protectedApps</span><span class="sxs-lookup"><span data-stu-id="989e5-194">protectedApps</span></span>|<span data-ttu-id="989e5-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989e5-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="989e5-196">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-196">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-197">exemptApps</span><span class="sxs-lookup"><span data-stu-id="989e5-197">exemptApps</span></span>|<span data-ttu-id="989e5-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989e5-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="989e5-199">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="989e5-199">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="989e5-200">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="989e5-200">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="989e5-201">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-201">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-202">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="989e5-202">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="989e5-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989e5-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="989e5-204">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="989e5-204">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="989e5-205">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-205">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-206">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="989e5-206">enterpriseProxiedDomains</span></span>|<span data-ttu-id="989e5-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989e5-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="989e5-208">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="989e5-208">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="989e5-209">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="989e5-209">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="989e5-210">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="989e5-210">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="989e5-211">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-211">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-212">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="989e5-212">enterpriseIPRanges</span></span>|<span data-ttu-id="989e5-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989e5-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="989e5-214">设置定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="989e5-214">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="989e5-215">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="989e5-215">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="989e5-216">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-216">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-217">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="989e5-217">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="989e5-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="989e5-218">Boolean</span></span>|<span data-ttu-id="989e5-219">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="989e5-219">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="989e5-220">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-220">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-221">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="989e5-221">enterpriseProxyServers</span></span>|<span data-ttu-id="989e5-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989e5-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="989e5-223">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="989e5-223">This is a list of proxy servers.</span></span> <span data-ttu-id="989e5-224">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-224">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-225">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="989e5-225">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="989e5-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989e5-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="989e5-227">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="989e5-227">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="989e5-228">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="989e5-228">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="989e5-229">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="989e5-229">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="989e5-230">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="989e5-230">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="989e5-231">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-231">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-232">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="989e5-232">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="989e5-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="989e5-233">Boolean</span></span>|<span data-ttu-id="989e5-234">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="989e5-234">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="989e5-235">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-235">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-236">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="989e5-236">neutralDomainResources</span></span>|<span data-ttu-id="989e5-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989e5-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="989e5-238">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-238">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-239">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="989e5-239">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="989e5-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="989e5-240">Boolean</span></span>|<span data-ttu-id="989e5-241">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-241">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-242">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="989e5-242">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="989e5-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989e5-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="989e5-244">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-244">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="989e5-245">isAssigned</span><span class="sxs-lookup"><span data-stu-id="989e5-245">isAssigned</span></span>|<span data-ttu-id="989e5-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="989e5-246">Boolean</span></span>|<span data-ttu-id="989e5-247">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="989e5-247">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="989e5-248">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="989e5-248">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="989e5-249">响应</span><span class="sxs-lookup"><span data-stu-id="989e5-249">Response</span></span>
<span data-ttu-id="989e5-250">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="989e5-250">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="989e5-251">示例</span><span class="sxs-lookup"><span data-stu-id="989e5-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="989e5-252">请求</span><span class="sxs-lookup"><span data-stu-id="989e5-252">Request</span></span>
<span data-ttu-id="989e5-253">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="989e5-253">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies
Content-type: application/json
Content-length: 3967

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
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
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="989e5-254">响应</span><span class="sxs-lookup"><span data-stu-id="989e5-254">Response</span></span>
<span data-ttu-id="989e5-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="989e5-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4139

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "8efb0c35-0c35-8efb-350c-fb8e350cfb8e",
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
  "isAssigned": true
}
```





