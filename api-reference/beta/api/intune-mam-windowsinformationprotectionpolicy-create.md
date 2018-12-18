---
title: 创建 windowsInformationProtectionPolicy
description: 创建新的 windowsInformationProtectionPolicy 对象。
author: tfitzmac
ms.openlocfilehash: 80615563dcc85b74a7f8d40f9c6752d4c16fdae8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323777"
---
# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="de0e5-103">创建 windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="de0e5-103">Create windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="de0e5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="de0e5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de0e5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="de0e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de0e5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="de0e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de0e5-107">创建新的 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="de0e5-107">Create a new [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de0e5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="de0e5-108">Prerequisites</span></span>
<span data-ttu-id="de0e5-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="de0e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de0e5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="de0e5-111">Permission type</span></span>|<span data-ttu-id="de0e5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="de0e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de0e5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de0e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de0e5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de0e5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="de0e5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de0e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de0e5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="de0e5-116">Not supported.</span></span>|
|<span data-ttu-id="de0e5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="de0e5-117">Application</span></span>|<span data-ttu-id="de0e5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="de0e5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de0e5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de0e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="de0e5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="de0e5-120">Request headers</span></span>
|<span data-ttu-id="de0e5-121">标头</span><span class="sxs-lookup"><span data-stu-id="de0e5-121">Header</span></span>|<span data-ttu-id="de0e5-122">值</span><span class="sxs-lookup"><span data-stu-id="de0e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de0e5-123">授权</span><span class="sxs-lookup"><span data-stu-id="de0e5-123">Authorization</span></span>|<span data-ttu-id="de0e5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="de0e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de0e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de0e5-125">Accept</span></span>|<span data-ttu-id="de0e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de0e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de0e5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="de0e5-127">Request body</span></span>
<span data-ttu-id="de0e5-128">在请求正文中，提供 windowsInformationProtectionPolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de0e5-128">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="de0e5-129">下表显示创建 windowsInformationProtectionPolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="de0e5-129">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="de0e5-130">属性</span><span class="sxs-lookup"><span data-stu-id="de0e5-130">Property</span></span>|<span data-ttu-id="de0e5-131">类型</span><span class="sxs-lookup"><span data-stu-id="de0e5-131">Type</span></span>|<span data-ttu-id="de0e5-132">说明</span><span class="sxs-lookup"><span data-stu-id="de0e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de0e5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="de0e5-133">displayName</span></span>|<span data-ttu-id="de0e5-134">String</span><span class="sxs-lookup"><span data-stu-id="de0e5-134">String</span></span>|<span data-ttu-id="de0e5-135">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="de0e5-135">Policy display name.</span></span> <span data-ttu-id="de0e5-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="de0e5-137">description</span><span class="sxs-lookup"><span data-stu-id="de0e5-137">description</span></span>|<span data-ttu-id="de0e5-138">String</span><span class="sxs-lookup"><span data-stu-id="de0e5-138">String</span></span>|<span data-ttu-id="de0e5-139">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="de0e5-139">The policy's description.</span></span> <span data-ttu-id="de0e5-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="de0e5-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de0e5-141">createdDateTime</span></span>|<span data-ttu-id="de0e5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de0e5-142">DateTimeOffset</span></span>|<span data-ttu-id="de0e5-143">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="de0e5-143">The date and time the policy was created.</span></span> <span data-ttu-id="de0e5-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="de0e5-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de0e5-145">lastModifiedDateTime</span></span>|<span data-ttu-id="de0e5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de0e5-146">DateTimeOffset</span></span>|<span data-ttu-id="de0e5-147">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="de0e5-147">Last time the policy was modified.</span></span> <span data-ttu-id="de0e5-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="de0e5-149">id</span><span class="sxs-lookup"><span data-stu-id="de0e5-149">id</span></span>|<span data-ttu-id="de0e5-150">String</span><span class="sxs-lookup"><span data-stu-id="de0e5-150">String</span></span>|<span data-ttu-id="de0e5-151">实体的键。</span><span class="sxs-lookup"><span data-stu-id="de0e5-151">Key of the entity.</span></span> <span data-ttu-id="de0e5-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="de0e5-153">version</span><span class="sxs-lookup"><span data-stu-id="de0e5-153">version</span></span>|<span data-ttu-id="de0e5-154">String</span><span class="sxs-lookup"><span data-stu-id="de0e5-154">String</span></span>|<span data-ttu-id="de0e5-155">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="de0e5-155">Version of the entity.</span></span> <span data-ttu-id="de0e5-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="de0e5-157">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="de0e5-157">enforcementLevel</span></span>|[<span data-ttu-id="de0e5-158">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="de0e5-158">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="de0e5-159">WIP 实施级别。请参见支持值继承[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)枚举定义。</span><span class="sxs-lookup"><span data-stu-id="de0e5-159">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="de0e5-160">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="de0e5-160">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="de0e5-161">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="de0e5-161">enterpriseDomain</span></span>|<span data-ttu-id="de0e5-162">String</span><span class="sxs-lookup"><span data-stu-id="de0e5-162">String</span></span>|<span data-ttu-id="de0e5-163">主企业域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-163">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-164">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="de0e5-164">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="de0e5-165">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de0e5-165">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="de0e5-166">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-166">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-167">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="de0e5-167">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="de0e5-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="de0e5-168">Boolean</span></span>|<span data-ttu-id="de0e5-169">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-169">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-170">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="de0e5-170">dataRecoveryCertificate</span></span>|[<span data-ttu-id="de0e5-171">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="de0e5-171">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="de0e5-172">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="de0e5-172">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="de0e5-173">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-173">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-174">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="de0e5-174">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="de0e5-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="de0e5-175">Boolean</span></span>|<span data-ttu-id="de0e5-176">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="de0e5-176">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="de0e5-177">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="de0e5-177">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="de0e5-178">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="de0e5-178">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="de0e5-179">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-179">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-180">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="de0e5-180">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="de0e5-181">Guid</span><span class="sxs-lookup"><span data-stu-id="de0e5-181">Guid</span></span>|<span data-ttu-id="de0e5-182">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="de0e5-182">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="de0e5-183">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-183">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-184">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="de0e5-184">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="de0e5-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="de0e5-185">Boolean</span></span>|<span data-ttu-id="de0e5-186">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-186">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-187">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="de0e5-187">iconsVisible</span></span>|<span data-ttu-id="de0e5-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="de0e5-188">Boolean</span></span>|<span data-ttu-id="de0e5-189">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="de0e5-189">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="de0e5-190">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-190">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-191">protectedApps</span><span class="sxs-lookup"><span data-stu-id="de0e5-191">protectedApps</span></span>|<span data-ttu-id="de0e5-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de0e5-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="de0e5-193">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-193">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-194">exemptApps</span><span class="sxs-lookup"><span data-stu-id="de0e5-194">exemptApps</span></span>|<span data-ttu-id="de0e5-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de0e5-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="de0e5-196">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="de0e5-196">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="de0e5-197">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="de0e5-197">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="de0e5-198">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-198">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-199">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="de0e5-199">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="de0e5-200">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de0e5-200">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="de0e5-201">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="de0e5-201">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="de0e5-202">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-202">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-203">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="de0e5-203">enterpriseProxiedDomains</span></span>|<span data-ttu-id="de0e5-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de0e5-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="de0e5-205">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="de0e5-205">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="de0e5-206">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="de0e5-206">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="de0e5-207">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="de0e5-207">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="de0e5-208">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-208">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-209">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="de0e5-209">enterpriseIPRanges</span></span>|<span data-ttu-id="de0e5-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de0e5-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="de0e5-211">设置可定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="de0e5-211">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="de0e5-212">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="de0e5-212">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="de0e5-213">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-213">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-214">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="de0e5-214">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="de0e5-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="de0e5-215">Boolean</span></span>|<span data-ttu-id="de0e5-216">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="de0e5-216">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="de0e5-217">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-217">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-218">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="de0e5-218">enterpriseProxyServers</span></span>|<span data-ttu-id="de0e5-219">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de0e5-219">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="de0e5-220">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="de0e5-220">This is a list of proxy servers.</span></span> <span data-ttu-id="de0e5-221">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-221">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-222">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="de0e5-222">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="de0e5-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de0e5-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="de0e5-224">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="de0e5-224">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="de0e5-225">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="de0e5-225">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="de0e5-226">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="de0e5-226">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="de0e5-227">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="de0e5-227">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="de0e5-228">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-228">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-229">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="de0e5-229">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="de0e5-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="de0e5-230">Boolean</span></span>|<span data-ttu-id="de0e5-231">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="de0e5-231">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="de0e5-232">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-232">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-233">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="de0e5-233">neutralDomainResources</span></span>|<span data-ttu-id="de0e5-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de0e5-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="de0e5-235">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-235">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-236">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="de0e5-236">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="de0e5-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="de0e5-237">Boolean</span></span>|<span data-ttu-id="de0e5-238">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-238">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-239">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="de0e5-239">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="de0e5-240">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de0e5-240">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="de0e5-241">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-241">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-242">isAssigned</span><span class="sxs-lookup"><span data-stu-id="de0e5-242">isAssigned</span></span>|<span data-ttu-id="de0e5-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="de0e5-243">Boolean</span></span>|<span data-ttu-id="de0e5-244">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="de0e5-244">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="de0e5-245">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="de0e5-245">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="de0e5-246">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="de0e5-246">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="de0e5-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="de0e5-247">Boolean</span></span>|<span data-ttu-id="de0e5-248">RS2 中的新属性，待定文档</span><span class="sxs-lookup"><span data-stu-id="de0e5-248">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="de0e5-249">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="de0e5-249">mdmEnrollmentUrl</span></span>|<span data-ttu-id="de0e5-250">String</span><span class="sxs-lookup"><span data-stu-id="de0e5-250">String</span></span>|<span data-ttu-id="de0e5-251">MDM 的注册 URL</span><span class="sxs-lookup"><span data-stu-id="de0e5-251">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="de0e5-252">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="de0e5-252">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="de0e5-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="de0e5-253">Boolean</span></span>|<span data-ttu-id="de0e5-254">将 Windows Hello 企业版设置为登录 Windows 的方法的布尔值。</span><span class="sxs-lookup"><span data-stu-id="de0e5-254">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="de0e5-255">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="de0e5-255">pinMinimumLength</span></span>|<span data-ttu-id="de0e5-256">Int32</span><span class="sxs-lookup"><span data-stu-id="de0e5-256">Int32</span></span>|<span data-ttu-id="de0e5-257">整数值，用于设置 PIN 所需的最少字符数。</span><span class="sxs-lookup"><span data-stu-id="de0e5-257">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="de0e5-258">默认值为 4。</span><span class="sxs-lookup"><span data-stu-id="de0e5-258">Default value is 4.</span></span> <span data-ttu-id="de0e5-259">可以为此策略设置配置的最小数量为 4。</span><span class="sxs-lookup"><span data-stu-id="de0e5-259">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="de0e5-260">可以配置的最大数量必须小于最大 PIN 长度策略设置中配置的数量或 127（以最低者为准）。</span><span class="sxs-lookup"><span data-stu-id="de0e5-260">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="de0e5-261">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="de0e5-261">pinUppercaseLetters</span></span>|[<span data-ttu-id="de0e5-262">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="de0e5-262">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="de0e5-263">整数值，用于配置 Windows Hello 企业版 PIN 中的大写字母的使用。</span><span class="sxs-lookup"><span data-stu-id="de0e5-263">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="de0e5-264">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="de0e5-264">Default is NotAllow.</span></span> <span data-ttu-id="de0e5-265">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="de0e5-265">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="de0e5-266">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="de0e5-266">pinLowercaseLetters</span></span>|[<span data-ttu-id="de0e5-267">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="de0e5-267">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="de0e5-268">整数值，用于配置 Windows Hello 企业版 PIN 中的小写字母的使用。</span><span class="sxs-lookup"><span data-stu-id="de0e5-268">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="de0e5-269">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="de0e5-269">Default is NotAllow.</span></span> <span data-ttu-id="de0e5-270">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="de0e5-270">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="de0e5-271">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="de0e5-271">pinSpecialCharacters</span></span>|[<span data-ttu-id="de0e5-272">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="de0e5-272">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="de0e5-273">整数值，用于配置 Windows Hello 企业版 PIN 中的特殊字母的使用。</span><span class="sxs-lookup"><span data-stu-id="de0e5-273">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="de0e5-274">Windows Hello 企业版 PIN 手势的有效特殊字符包括：!</span><span class="sxs-lookup"><span data-stu-id="de0e5-274">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="de0e5-275">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="de0e5-275">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="de0e5-276">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="de0e5-276">/ : ; < = > ?</span></span><span data-ttu-id="de0e5-277"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="de0e5-277"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="de0e5-278">} ~。</span><span class="sxs-lookup"><span data-stu-id="de0e5-278">} ~.</span></span> <span data-ttu-id="de0e5-279">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="de0e5-279">Default is NotAllow.</span></span> <span data-ttu-id="de0e5-280">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="de0e5-280">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="de0e5-281">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="de0e5-281">pinExpirationDays</span></span>|<span data-ttu-id="de0e5-282">Int32</span><span class="sxs-lookup"><span data-stu-id="de0e5-282">Int32</span></span>|<span data-ttu-id="de0e5-283">整数值指定在系统要求用户更改 PIN 之前可以使用 PIN 的时间段（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="de0e5-283">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="de0e5-284">可以为此策略设置配置的最大数量为 730。</span><span class="sxs-lookup"><span data-stu-id="de0e5-284">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="de0e5-285">可以为此策略设置配置的最小数量为 0。</span><span class="sxs-lookup"><span data-stu-id="de0e5-285">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="de0e5-286">如果此策略设置为 0，则用户的 PIN 永远不会过期。</span><span class="sxs-lookup"><span data-stu-id="de0e5-286">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="de0e5-287">此节点在 Windows 10 版本 1511 中添加。</span><span class="sxs-lookup"><span data-stu-id="de0e5-287">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="de0e5-288">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="de0e5-288">Default is 0.</span></span>|
|<span data-ttu-id="de0e5-289">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="de0e5-289">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="de0e5-290">Int32</span><span class="sxs-lookup"><span data-stu-id="de0e5-290">Int32</span></span>|<span data-ttu-id="de0e5-291">整数值，用于指定可以关联到无法重用的用户帐户的过去 PIN 的数量。</span><span class="sxs-lookup"><span data-stu-id="de0e5-291">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="de0e5-292">可以为此策略设置配置的最大数量为 50。</span><span class="sxs-lookup"><span data-stu-id="de0e5-292">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="de0e5-293">可以为此策略设置配置的最小数量为 0。</span><span class="sxs-lookup"><span data-stu-id="de0e5-293">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="de0e5-294">如果此策略设置为 0，则不需要存储以前的 PIN。</span><span class="sxs-lookup"><span data-stu-id="de0e5-294">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="de0e5-295">此节点在 Windows 10 版本 1511 中添加。</span><span class="sxs-lookup"><span data-stu-id="de0e5-295">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="de0e5-296">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="de0e5-296">Default is 0.</span></span>|
|<span data-ttu-id="de0e5-297">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="de0e5-297">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="de0e5-298">Int32</span><span class="sxs-lookup"><span data-stu-id="de0e5-298">Int32</span></span>|<span data-ttu-id="de0e5-299">在擦除设备之前允许的身份验证失败次数。</span><span class="sxs-lookup"><span data-stu-id="de0e5-299">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="de0e5-300">值为 0 将禁用设备擦除功能。</span><span class="sxs-lookup"><span data-stu-id="de0e5-300">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="de0e5-301">范围是一个整数 X，其中对于台式机 4 <= X <= 16，对于移动设备 0 <= X <= 999。</span><span class="sxs-lookup"><span data-stu-id="de0e5-301">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="de0e5-302">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="de0e5-302">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="de0e5-303">Int32</span><span class="sxs-lookup"><span data-stu-id="de0e5-303">Int32</span></span>|<span data-ttu-id="de0e5-304">指定设备闲置后将导致设备变为 PIN 或密码锁定的允许的最长时间（以分钟为单位）。</span><span class="sxs-lookup"><span data-stu-id="de0e5-304">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="de0e5-305">范围是整数 X，其中 0 < = X < = 999。</span><span class="sxs-lookup"><span data-stu-id="de0e5-305">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="de0e5-306">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="de0e5-306">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="de0e5-307">Int32</span><span class="sxs-lookup"><span data-stu-id="de0e5-307">Int32</span></span>|<span data-ttu-id="de0e5-308">擦除应用数据之前的脱机间隔时间（天）</span><span class="sxs-lookup"><span data-stu-id="de0e5-308">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="de0e5-309">响应</span><span class="sxs-lookup"><span data-stu-id="de0e5-309">Response</span></span>
<span data-ttu-id="de0e5-310">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="de0e5-310">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de0e5-311">示例</span><span class="sxs-lookup"><span data-stu-id="de0e5-311">Example</span></span>
### <a name="request"></a><span data-ttu-id="de0e5-312">请求</span><span class="sxs-lookup"><span data-stu-id="de0e5-312">Request</span></span>
<span data-ttu-id="de0e5-313">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de0e5-313">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4469

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="de0e5-314">响应</span><span class="sxs-lookup"><span data-stu-id="de0e5-314">Response</span></span>
<span data-ttu-id="de0e5-p132">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="de0e5-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4577

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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





