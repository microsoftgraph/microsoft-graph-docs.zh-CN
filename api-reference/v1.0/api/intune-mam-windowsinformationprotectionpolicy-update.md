---
title: 更新 windowsInformationProtectionPolicy
description: 更新 windowsInformationProtectionPolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b378150fff4a2860a3e74cc0e99e09368200cad4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835320"
---
# <a name="update-windowsinformationprotectionpolicy"></a><span data-ttu-id="eb664-103">更新 windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="eb664-103">Update windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="eb664-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eb664-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb664-105">更新 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eb664-105">Update the properties of a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb664-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="eb664-106">Prerequisites</span></span>
<span data-ttu-id="eb664-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="eb664-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb664-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb664-109">Permission type</span></span>|<span data-ttu-id="eb664-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eb664-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb664-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb664-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eb664-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb664-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eb664-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb664-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb664-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb664-114">Not supported.</span></span>|
|<span data-ttu-id="eb664-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb664-115">Application</span></span>|<span data-ttu-id="eb664-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb664-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb664-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb664-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="eb664-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb664-118">Request headers</span></span>
|<span data-ttu-id="eb664-119">标头</span><span class="sxs-lookup"><span data-stu-id="eb664-119">Header</span></span>|<span data-ttu-id="eb664-120">值</span><span class="sxs-lookup"><span data-stu-id="eb664-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb664-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb664-121">Authorization</span></span>|<span data-ttu-id="eb664-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eb664-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb664-123">Accept</span><span class="sxs-lookup"><span data-stu-id="eb664-123">Accept</span></span>|<span data-ttu-id="eb664-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eb664-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb664-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb664-125">Request body</span></span>
<span data-ttu-id="eb664-126">在请求正文中，提供 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb664-126">In the request body, supply a JSON representation for the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="eb664-127">下表显示创建 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eb664-127">The following table shows the properties that are required when you create the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="eb664-128">属性</span><span class="sxs-lookup"><span data-stu-id="eb664-128">Property</span></span>|<span data-ttu-id="eb664-129">类型</span><span class="sxs-lookup"><span data-stu-id="eb664-129">Type</span></span>|<span data-ttu-id="eb664-130">说明</span><span class="sxs-lookup"><span data-stu-id="eb664-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb664-131">displayName</span><span class="sxs-lookup"><span data-stu-id="eb664-131">displayName</span></span>|<span data-ttu-id="eb664-132">String</span><span class="sxs-lookup"><span data-stu-id="eb664-132">String</span></span>|<span data-ttu-id="eb664-133">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="eb664-133">Policy display name.</span></span> <span data-ttu-id="eb664-134">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="eb664-135">description</span><span class="sxs-lookup"><span data-stu-id="eb664-135">description</span></span>|<span data-ttu-id="eb664-136">String</span><span class="sxs-lookup"><span data-stu-id="eb664-136">String</span></span>|<span data-ttu-id="eb664-137">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="eb664-137">The policy's description.</span></span> <span data-ttu-id="eb664-138">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="eb664-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb664-139">createdDateTime</span></span>|<span data-ttu-id="eb664-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb664-140">DateTimeOffset</span></span>|<span data-ttu-id="eb664-141">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="eb664-141">The date and time the policy was created.</span></span> <span data-ttu-id="eb664-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="eb664-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb664-143">lastModifiedDateTime</span></span>|<span data-ttu-id="eb664-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb664-144">DateTimeOffset</span></span>|<span data-ttu-id="eb664-145">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="eb664-145">Last time the policy was modified.</span></span> <span data-ttu-id="eb664-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="eb664-147">id</span><span class="sxs-lookup"><span data-stu-id="eb664-147">id</span></span>|<span data-ttu-id="eb664-148">String</span><span class="sxs-lookup"><span data-stu-id="eb664-148">String</span></span>|<span data-ttu-id="eb664-149">实体的键。</span><span class="sxs-lookup"><span data-stu-id="eb664-149">Key of the entity.</span></span> <span data-ttu-id="eb664-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="eb664-151">version</span><span class="sxs-lookup"><span data-stu-id="eb664-151">version</span></span>|<span data-ttu-id="eb664-152">String</span><span class="sxs-lookup"><span data-stu-id="eb664-152">String</span></span>|<span data-ttu-id="eb664-153">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="eb664-153">Version of the entity.</span></span> <span data-ttu-id="eb664-154">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="eb664-155">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="eb664-155">enforcementLevel</span></span>|[<span data-ttu-id="eb664-156">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="eb664-156">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="eb664-157">WIP 实施级别。请参见支持值继承[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)枚举定义。</span><span class="sxs-lookup"><span data-stu-id="eb664-157">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="eb664-158">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="eb664-158">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="eb664-159">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="eb664-159">enterpriseDomain</span></span>|<span data-ttu-id="eb664-160">String</span><span class="sxs-lookup"><span data-stu-id="eb664-160">String</span></span>|<span data-ttu-id="eb664-161">主企业域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-161">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-162">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="eb664-162">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="eb664-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb664-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="eb664-164">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-164">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-165">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="eb664-165">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="eb664-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb664-166">Boolean</span></span>|<span data-ttu-id="eb664-167">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-167">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-168">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="eb664-168">dataRecoveryCertificate</span></span>|[<span data-ttu-id="eb664-169">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="eb664-169">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="eb664-170">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="eb664-170">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="eb664-171">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-171">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-172">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="eb664-172">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="eb664-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb664-173">Boolean</span></span>|<span data-ttu-id="eb664-174">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="eb664-174">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="eb664-175">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="eb664-175">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="eb664-176">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="eb664-176">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="eb664-177">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-177">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-178">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="eb664-178">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="eb664-179">Guid</span><span class="sxs-lookup"><span data-stu-id="eb664-179">Guid</span></span>|<span data-ttu-id="eb664-180">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="eb664-180">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="eb664-181">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-181">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-182">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="eb664-182">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="eb664-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb664-183">Boolean</span></span>|<span data-ttu-id="eb664-184">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-184">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-185">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="eb664-185">iconsVisible</span></span>|<span data-ttu-id="eb664-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb664-186">Boolean</span></span>|<span data-ttu-id="eb664-187">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="eb664-187">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="eb664-188">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-188">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-189">protectedApps</span><span class="sxs-lookup"><span data-stu-id="eb664-189">protectedApps</span></span>|<span data-ttu-id="eb664-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb664-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="eb664-191">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-191">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-192">exemptApps</span><span class="sxs-lookup"><span data-stu-id="eb664-192">exemptApps</span></span>|<span data-ttu-id="eb664-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb664-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="eb664-194">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="eb664-194">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="eb664-195">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="eb664-195">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="eb664-196">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-196">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-197">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="eb664-197">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="eb664-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb664-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="eb664-199">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="eb664-199">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="eb664-200">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-200">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-201">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="eb664-201">enterpriseProxiedDomains</span></span>|<span data-ttu-id="eb664-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb664-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="eb664-203">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="eb664-203">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="eb664-204">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="eb664-204">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="eb664-205">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="eb664-205">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="eb664-206">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-206">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-207">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="eb664-207">enterpriseIPRanges</span></span>|<span data-ttu-id="eb664-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb664-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="eb664-209">设置可定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="eb664-209">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="eb664-210">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="eb664-210">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="eb664-211">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-211">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-212">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="eb664-212">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="eb664-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb664-213">Boolean</span></span>|<span data-ttu-id="eb664-214">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="eb664-214">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="eb664-215">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-215">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-216">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="eb664-216">enterpriseProxyServers</span></span>|<span data-ttu-id="eb664-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb664-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="eb664-218">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="eb664-218">This is a list of proxy servers.</span></span> <span data-ttu-id="eb664-219">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-219">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-220">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="eb664-220">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="eb664-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb664-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="eb664-222">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="eb664-222">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="eb664-223">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="eb664-223">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="eb664-224">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="eb664-224">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="eb664-225">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="eb664-225">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="eb664-226">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-226">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-227">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="eb664-227">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="eb664-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb664-228">Boolean</span></span>|<span data-ttu-id="eb664-229">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="eb664-229">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="eb664-230">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-230">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-231">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="eb664-231">neutralDomainResources</span></span>|<span data-ttu-id="eb664-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb664-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="eb664-233">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-233">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-234">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="eb664-234">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="eb664-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb664-235">Boolean</span></span>|<span data-ttu-id="eb664-236">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-236">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-237">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="eb664-237">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="eb664-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb664-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="eb664-239">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-239">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-240">isAssigned</span><span class="sxs-lookup"><span data-stu-id="eb664-240">isAssigned</span></span>|<span data-ttu-id="eb664-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb664-241">Boolean</span></span>|<span data-ttu-id="eb664-242">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="eb664-242">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="eb664-243">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-243">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="eb664-244">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="eb664-244">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="eb664-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb664-245">Boolean</span></span>|<span data-ttu-id="eb664-246">RS2 中的新属性，待定文档</span><span class="sxs-lookup"><span data-stu-id="eb664-246">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="eb664-247">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="eb664-247">mdmEnrollmentUrl</span></span>|<span data-ttu-id="eb664-248">String</span><span class="sxs-lookup"><span data-stu-id="eb664-248">String</span></span>|<span data-ttu-id="eb664-249">MDM 的注册 URL</span><span class="sxs-lookup"><span data-stu-id="eb664-249">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="eb664-250">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="eb664-250">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="eb664-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb664-251">Boolean</span></span>|<span data-ttu-id="eb664-252">将 Windows Hello 企业版设置为登录 Windows 的方法的布尔值。</span><span class="sxs-lookup"><span data-stu-id="eb664-252">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="eb664-253">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="eb664-253">pinMinimumLength</span></span>|<span data-ttu-id="eb664-254">Int32</span><span class="sxs-lookup"><span data-stu-id="eb664-254">Int32</span></span>|<span data-ttu-id="eb664-255">整数值，用于设置 PIN 所需的最少字符数。</span><span class="sxs-lookup"><span data-stu-id="eb664-255">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="eb664-256">默认值为 4。</span><span class="sxs-lookup"><span data-stu-id="eb664-256">Default value is 4.</span></span> <span data-ttu-id="eb664-257">可以为此策略设置配置的最小数量为 4。</span><span class="sxs-lookup"><span data-stu-id="eb664-257">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="eb664-258">可以配置的最大数量必须小于最大 PIN 长度策略设置中配置的数量或 127（以最低者为准）。</span><span class="sxs-lookup"><span data-stu-id="eb664-258">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="eb664-259">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="eb664-259">pinUppercaseLetters</span></span>|[<span data-ttu-id="eb664-260">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="eb664-260">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="eb664-261">整数值，用于配置 Windows Hello 企业版 PIN 中的大写字母的使用。</span><span class="sxs-lookup"><span data-stu-id="eb664-261">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="eb664-262">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="eb664-262">Default is NotAllow.</span></span> <span data-ttu-id="eb664-263">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="eb664-263">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="eb664-264">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="eb664-264">pinLowercaseLetters</span></span>|[<span data-ttu-id="eb664-265">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="eb664-265">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="eb664-266">整数值，用于配置 Windows Hello 企业版 PIN 中的小写字母的使用。</span><span class="sxs-lookup"><span data-stu-id="eb664-266">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="eb664-267">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="eb664-267">Default is NotAllow.</span></span> <span data-ttu-id="eb664-268">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="eb664-268">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="eb664-269">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="eb664-269">pinSpecialCharacters</span></span>|[<span data-ttu-id="eb664-270">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="eb664-270">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="eb664-271">整数值，用于配置 Windows Hello 企业版 PIN 中的特殊字母的使用。</span><span class="sxs-lookup"><span data-stu-id="eb664-271">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="eb664-272">Windows Hello 企业版 PIN 手势的有效特殊字符包括：!</span><span class="sxs-lookup"><span data-stu-id="eb664-272">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="eb664-273">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="eb664-273">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="eb664-274">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="eb664-274">/ : ; < = > ?</span></span><span data-ttu-id="eb664-275"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="eb664-275"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="eb664-276">} ~。</span><span class="sxs-lookup"><span data-stu-id="eb664-276">} ~.</span></span> <span data-ttu-id="eb664-277">默认值为 NotAllow。</span><span class="sxs-lookup"><span data-stu-id="eb664-277">Default is NotAllow.</span></span> <span data-ttu-id="eb664-278">可取值为：`notAllow`、`requireAtLeastOne`、`allow`。</span><span class="sxs-lookup"><span data-stu-id="eb664-278">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="eb664-279">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="eb664-279">pinExpirationDays</span></span>|<span data-ttu-id="eb664-280">Int32</span><span class="sxs-lookup"><span data-stu-id="eb664-280">Int32</span></span>|<span data-ttu-id="eb664-281">整数值指定在系统要求用户更改 PIN 之前可以使用 PIN 的时间段（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="eb664-281">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="eb664-282">可以为此策略设置配置的最大数量为 730。</span><span class="sxs-lookup"><span data-stu-id="eb664-282">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="eb664-283">可以为此策略设置配置的最小数量为 0。</span><span class="sxs-lookup"><span data-stu-id="eb664-283">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="eb664-284">如果此策略设置为 0，则用户的 PIN 永远不会过期。</span><span class="sxs-lookup"><span data-stu-id="eb664-284">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="eb664-285">此节点在 Windows 10 版本 1511 中添加。</span><span class="sxs-lookup"><span data-stu-id="eb664-285">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="eb664-286">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="eb664-286">Default is 0.</span></span>|
|<span data-ttu-id="eb664-287">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="eb664-287">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="eb664-288">Int32</span><span class="sxs-lookup"><span data-stu-id="eb664-288">Int32</span></span>|<span data-ttu-id="eb664-289">整数值，用于指定可以关联到无法重用的用户帐户的过去 PIN 的数量。</span><span class="sxs-lookup"><span data-stu-id="eb664-289">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="eb664-290">可以为此策略设置配置的最大数量为 50。</span><span class="sxs-lookup"><span data-stu-id="eb664-290">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="eb664-291">可以为此策略设置配置的最小数量为 0。</span><span class="sxs-lookup"><span data-stu-id="eb664-291">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="eb664-292">如果此策略设置为 0，则不需要存储以前的 PIN。</span><span class="sxs-lookup"><span data-stu-id="eb664-292">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="eb664-293">此节点在 Windows 10 版本 1511 中添加。</span><span class="sxs-lookup"><span data-stu-id="eb664-293">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="eb664-294">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="eb664-294">Default is 0.</span></span>|
|<span data-ttu-id="eb664-295">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="eb664-295">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="eb664-296">Int32</span><span class="sxs-lookup"><span data-stu-id="eb664-296">Int32</span></span>|<span data-ttu-id="eb664-297">在擦除设备之前允许的身份验证失败次数。</span><span class="sxs-lookup"><span data-stu-id="eb664-297">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="eb664-298">值为 0 将禁用设备擦除功能。</span><span class="sxs-lookup"><span data-stu-id="eb664-298">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="eb664-299">范围是一个整数 X，其中对于台式机 4 <= X <= 16，对于移动设备 0 <= X <= 999。</span><span class="sxs-lookup"><span data-stu-id="eb664-299">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="eb664-300">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="eb664-300">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="eb664-301">Int32</span><span class="sxs-lookup"><span data-stu-id="eb664-301">Int32</span></span>|<span data-ttu-id="eb664-302">指定设备闲置后将导致设备变为 PIN 或密码锁定的允许的最长时间（以分钟为单位）。</span><span class="sxs-lookup"><span data-stu-id="eb664-302">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="eb664-303">范围是整数 X，其中 0 < = X < = 999。</span><span class="sxs-lookup"><span data-stu-id="eb664-303">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="eb664-304">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="eb664-304">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="eb664-305">Int32</span><span class="sxs-lookup"><span data-stu-id="eb664-305">Int32</span></span>|<span data-ttu-id="eb664-306">擦除应用数据之前的脱机间隔时间（天）</span><span class="sxs-lookup"><span data-stu-id="eb664-306">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="eb664-307">响应</span><span class="sxs-lookup"><span data-stu-id="eb664-307">Response</span></span>
<span data-ttu-id="eb664-308">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb664-308">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb664-309">示例</span><span class="sxs-lookup"><span data-stu-id="eb664-309">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb664-310">请求</span><span class="sxs-lookup"><span data-stu-id="eb664-310">Request</span></span>
<span data-ttu-id="eb664-311">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb664-311">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 4405

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="eb664-312">响应</span><span class="sxs-lookup"><span data-stu-id="eb664-312">Response</span></span>
<span data-ttu-id="eb664-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eb664-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



