---
title: 创建 mdmWindowsInformationProtectionPolicy
description: 创建新的 mdmWindowsInformationProtectionPolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dafc641d0af7f45332c2785ae387b20265ca82e9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926265"
---
# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="3d0d4-103">创建 mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="3d0d4-103">Create mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="3d0d4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d0d4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d0d4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d0d4-107">创建新的 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-107">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3d0d4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d0d4-108">Prerequisites</span></span>
<span data-ttu-id="3d0d4-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="3d0d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d0d4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d0d4-111">Permission type</span></span>|<span data-ttu-id="3d0d4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3d0d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d0d4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d0d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d0d4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d0d4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3d0d4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d0d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d0d4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-116">Not supported.</span></span>|
|<span data-ttu-id="3d0d4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d0d4-117">Application</span></span>|<span data-ttu-id="3d0d4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d0d4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d0d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="3d0d4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d0d4-120">Request headers</span></span>
|<span data-ttu-id="3d0d4-121">标头</span><span class="sxs-lookup"><span data-stu-id="3d0d4-121">Header</span></span>|<span data-ttu-id="3d0d4-122">值</span><span class="sxs-lookup"><span data-stu-id="3d0d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d0d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d0d4-123">Authorization</span></span>|<span data-ttu-id="3d0d4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d0d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d0d4-125">Accept</span></span>|<span data-ttu-id="3d0d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d0d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d0d4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d0d4-127">Request body</span></span>
<span data-ttu-id="3d0d4-128">在请求正文中，提供 mdmWindowsInformationProtectionPolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-128">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="3d0d4-129">下表显示创建 mdmWindowsInformationProtectionPolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-129">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="3d0d4-130">属性</span><span class="sxs-lookup"><span data-stu-id="3d0d4-130">Property</span></span>|<span data-ttu-id="3d0d4-131">类型</span><span class="sxs-lookup"><span data-stu-id="3d0d4-131">Type</span></span>|<span data-ttu-id="3d0d4-132">说明</span><span class="sxs-lookup"><span data-stu-id="3d0d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d0d4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3d0d4-133">displayName</span></span>|<span data-ttu-id="3d0d4-134">String</span><span class="sxs-lookup"><span data-stu-id="3d0d4-134">String</span></span>|<span data-ttu-id="3d0d4-135">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-135">Policy display name.</span></span> <span data-ttu-id="3d0d4-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3d0d4-137">description</span><span class="sxs-lookup"><span data-stu-id="3d0d4-137">description</span></span>|<span data-ttu-id="3d0d4-138">String</span><span class="sxs-lookup"><span data-stu-id="3d0d4-138">String</span></span>|<span data-ttu-id="3d0d4-139">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-139">The policy's description.</span></span> <span data-ttu-id="3d0d4-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3d0d4-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d0d4-141">createdDateTime</span></span>|<span data-ttu-id="3d0d4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d0d4-142">DateTimeOffset</span></span>|<span data-ttu-id="3d0d4-143">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-143">The date and time the policy was created.</span></span> <span data-ttu-id="3d0d4-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3d0d4-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d0d4-145">lastModifiedDateTime</span></span>|<span data-ttu-id="3d0d4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d0d4-146">DateTimeOffset</span></span>|<span data-ttu-id="3d0d4-147">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-147">Last time the policy was modified.</span></span> <span data-ttu-id="3d0d4-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3d0d4-149">id</span><span class="sxs-lookup"><span data-stu-id="3d0d4-149">id</span></span>|<span data-ttu-id="3d0d4-150">String</span><span class="sxs-lookup"><span data-stu-id="3d0d4-150">String</span></span>|<span data-ttu-id="3d0d4-151">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-151">Key of the entity.</span></span> <span data-ttu-id="3d0d4-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3d0d4-153">version</span><span class="sxs-lookup"><span data-stu-id="3d0d4-153">version</span></span>|<span data-ttu-id="3d0d4-154">String</span><span class="sxs-lookup"><span data-stu-id="3d0d4-154">String</span></span>|<span data-ttu-id="3d0d4-155">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-155">Version of the entity.</span></span> <span data-ttu-id="3d0d4-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3d0d4-157">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="3d0d4-157">enforcementLevel</span></span>|[<span data-ttu-id="3d0d4-158">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="3d0d4-158">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="3d0d4-159">WIP 实施级别。请参见支持值继承[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)枚举定义。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-159">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="3d0d4-160">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-160">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="3d0d4-161">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="3d0d4-161">enterpriseDomain</span></span>|<span data-ttu-id="3d0d4-162">String</span><span class="sxs-lookup"><span data-stu-id="3d0d4-162">String</span></span>|<span data-ttu-id="3d0d4-163">主企业域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-163">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-164">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="3d0d4-164">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="3d0d4-165">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3d0d4-165">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="3d0d4-166">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-166">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-167">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="3d0d4-167">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="3d0d4-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d0d4-168">Boolean</span></span>|<span data-ttu-id="3d0d4-169">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-169">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-170">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="3d0d4-170">dataRecoveryCertificate</span></span>|[<span data-ttu-id="3d0d4-171">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="3d0d4-171">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="3d0d4-172">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-172">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="3d0d4-173">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-173">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-174">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="3d0d4-174">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="3d0d4-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d0d4-175">Boolean</span></span>|<span data-ttu-id="3d0d4-176">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-176">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="3d0d4-177">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-177">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="3d0d4-178">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-178">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="3d0d4-179">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-179">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-180">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="3d0d4-180">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="3d0d4-181">Guid</span><span class="sxs-lookup"><span data-stu-id="3d0d4-181">Guid</span></span>|<span data-ttu-id="3d0d4-182">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-182">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="3d0d4-183">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-183">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-184">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="3d0d4-184">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="3d0d4-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d0d4-185">Boolean</span></span>|<span data-ttu-id="3d0d4-186">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-186">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-187">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="3d0d4-187">iconsVisible</span></span>|<span data-ttu-id="3d0d4-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d0d4-188">Boolean</span></span>|<span data-ttu-id="3d0d4-189">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-189">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="3d0d4-190">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-190">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-191">protectedApps</span><span class="sxs-lookup"><span data-stu-id="3d0d4-191">protectedApps</span></span>|<span data-ttu-id="3d0d4-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3d0d4-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="3d0d4-193">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-193">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-194">exemptApps</span><span class="sxs-lookup"><span data-stu-id="3d0d4-194">exemptApps</span></span>|<span data-ttu-id="3d0d4-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3d0d4-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="3d0d4-196">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-196">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="3d0d4-197">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-197">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="3d0d4-198">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-198">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-199">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="3d0d4-199">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="3d0d4-200">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3d0d4-200">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="3d0d4-201">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-201">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="3d0d4-202">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-202">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-203">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="3d0d4-203">enterpriseProxiedDomains</span></span>|<span data-ttu-id="3d0d4-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3d0d4-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="3d0d4-205">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-205">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="3d0d4-206">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-206">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="3d0d4-207">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-207">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="3d0d4-208">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-208">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-209">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="3d0d4-209">enterpriseIPRanges</span></span>|<span data-ttu-id="3d0d4-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3d0d4-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="3d0d4-211">设置可定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-211">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="3d0d4-212">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-212">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="3d0d4-213">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-213">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-214">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="3d0d4-214">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="3d0d4-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d0d4-215">Boolean</span></span>|<span data-ttu-id="3d0d4-216">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-216">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="3d0d4-217">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-217">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-218">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="3d0d4-218">enterpriseProxyServers</span></span>|<span data-ttu-id="3d0d4-219">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3d0d4-219">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="3d0d4-220">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-220">This is a list of proxy servers.</span></span> <span data-ttu-id="3d0d4-221">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-221">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-222">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="3d0d4-222">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="3d0d4-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3d0d4-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="3d0d4-224">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-224">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="3d0d4-225">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-225">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="3d0d4-226">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-226">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="3d0d4-227">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-227">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="3d0d4-228">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-228">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-229">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="3d0d4-229">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="3d0d4-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d0d4-230">Boolean</span></span>|<span data-ttu-id="3d0d4-231">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-231">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="3d0d4-232">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-232">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-233">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="3d0d4-233">neutralDomainResources</span></span>|<span data-ttu-id="3d0d4-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3d0d4-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="3d0d4-235">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-235">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-236">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="3d0d4-236">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="3d0d4-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d0d4-237">Boolean</span></span>|<span data-ttu-id="3d0d4-238">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-238">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-239">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="3d0d4-239">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="3d0d4-240">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3d0d4-240">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="3d0d4-241">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-241">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="3d0d4-242">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3d0d4-242">isAssigned</span></span>|<span data-ttu-id="3d0d4-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d0d4-243">Boolean</span></span>|<span data-ttu-id="3d0d4-244">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-244">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="3d0d4-245">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3d0d4-245">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3d0d4-246">响应</span><span class="sxs-lookup"><span data-stu-id="3d0d4-246">Response</span></span>
<span data-ttu-id="3d0d4-247">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-247">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d0d4-248">示例</span><span class="sxs-lookup"><span data-stu-id="3d0d4-248">Example</span></span>
### <a name="request"></a><span data-ttu-id="3d0d4-249">请求</span><span class="sxs-lookup"><span data-stu-id="3d0d4-249">Request</span></span>
<span data-ttu-id="3d0d4-250">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-250">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies
Content-type: application/json
Content-length: 3969

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
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
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="3d0d4-251">响应</span><span class="sxs-lookup"><span data-stu-id="3d0d4-251">Response</span></span>
<span data-ttu-id="3d0d4-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d0d4-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4077

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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





