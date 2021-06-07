---
title: 创建 mdmWindowsInformationProtectionPolicy
description: 创建新的 mdmWindowsInformationProtectionPolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a11a5e87b57847febdb50c7ce31d82b5697d75b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759112"
---
# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="a2103-103">创建 mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a2103-103">Create mdmWindowsInformationProtectionPolicy</span></span>

<span data-ttu-id="a2103-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2103-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2103-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2103-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2103-106">创建新的 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a2103-106">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2103-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2103-107">Prerequisites</span></span>
<span data-ttu-id="a2103-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2103-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2103-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2103-110">Permission type</span></span>|<span data-ttu-id="a2103-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2103-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2103-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2103-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2103-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2103-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a2103-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2103-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2103-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2103-115">Not supported.</span></span>|
|<span data-ttu-id="a2103-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2103-116">Application</span></span>|<span data-ttu-id="a2103-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2103-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2103-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2103-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="a2103-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2103-119">Request headers</span></span>
|<span data-ttu-id="a2103-120">标头</span><span class="sxs-lookup"><span data-stu-id="a2103-120">Header</span></span>|<span data-ttu-id="a2103-121">值</span><span class="sxs-lookup"><span data-stu-id="a2103-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2103-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2103-122">Authorization</span></span>|<span data-ttu-id="a2103-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a2103-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2103-124">接受</span><span class="sxs-lookup"><span data-stu-id="a2103-124">Accept</span></span>|<span data-ttu-id="a2103-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2103-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2103-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2103-126">Request body</span></span>
<span data-ttu-id="a2103-127">在请求正文中，提供 mdmWindowsInformationProtectionPolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2103-127">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="a2103-128">下表显示创建 mdmWindowsInformationProtectionPolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a2103-128">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="a2103-129">属性</span><span class="sxs-lookup"><span data-stu-id="a2103-129">Property</span></span>|<span data-ttu-id="a2103-130">类型</span><span class="sxs-lookup"><span data-stu-id="a2103-130">Type</span></span>|<span data-ttu-id="a2103-131">说明</span><span class="sxs-lookup"><span data-stu-id="a2103-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2103-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a2103-132">displayName</span></span>|<span data-ttu-id="a2103-133">String</span><span class="sxs-lookup"><span data-stu-id="a2103-133">String</span></span>|<span data-ttu-id="a2103-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="a2103-134">Policy display name.</span></span> <span data-ttu-id="a2103-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a2103-136">description</span><span class="sxs-lookup"><span data-stu-id="a2103-136">description</span></span>|<span data-ttu-id="a2103-137">String</span><span class="sxs-lookup"><span data-stu-id="a2103-137">String</span></span>|<span data-ttu-id="a2103-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="a2103-138">The policy's description.</span></span> <span data-ttu-id="a2103-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a2103-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2103-140">createdDateTime</span></span>|<span data-ttu-id="a2103-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2103-141">DateTimeOffset</span></span>|<span data-ttu-id="a2103-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a2103-142">The date and time the policy was created.</span></span> <span data-ttu-id="a2103-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a2103-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2103-144">lastModifiedDateTime</span></span>|<span data-ttu-id="a2103-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2103-145">DateTimeOffset</span></span>|<span data-ttu-id="a2103-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="a2103-146">Last time the policy was modified.</span></span> <span data-ttu-id="a2103-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a2103-148">id</span><span class="sxs-lookup"><span data-stu-id="a2103-148">id</span></span>|<span data-ttu-id="a2103-149">String</span><span class="sxs-lookup"><span data-stu-id="a2103-149">String</span></span>|<span data-ttu-id="a2103-150">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a2103-150">Key of the entity.</span></span> <span data-ttu-id="a2103-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a2103-152">version</span><span class="sxs-lookup"><span data-stu-id="a2103-152">version</span></span>|<span data-ttu-id="a2103-153">String</span><span class="sxs-lookup"><span data-stu-id="a2103-153">String</span></span>|<span data-ttu-id="a2103-154">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="a2103-154">Version of the entity.</span></span> <span data-ttu-id="a2103-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a2103-156">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="a2103-156">enforcementLevel</span></span>|[<span data-ttu-id="a2103-157">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="a2103-157">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="a2103-158">WIP 强制级别。请参阅 Enum 定义了解受支持的值 继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="a2103-158">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="a2103-159">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="a2103-159">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="a2103-160">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="a2103-160">enterpriseDomain</span></span>|<span data-ttu-id="a2103-161">String</span><span class="sxs-lookup"><span data-stu-id="a2103-161">String</span></span>|<span data-ttu-id="a2103-162">主企业域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-162">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-163">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="a2103-163">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="a2103-164">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2103-164">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a2103-165">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-165">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-166">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="a2103-166">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="a2103-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2103-167">Boolean</span></span>|<span data-ttu-id="a2103-168">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-168">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-169">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a2103-169">dataRecoveryCertificate</span></span>|[<span data-ttu-id="a2103-170">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a2103-170">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="a2103-171">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="a2103-171">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="a2103-172">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-172">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-173">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="a2103-173">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="a2103-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2103-174">Boolean</span></span>|<span data-ttu-id="a2103-175">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="a2103-175">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="a2103-176">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="a2103-176">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="a2103-177">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="a2103-177">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="a2103-178">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-178">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-179">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="a2103-179">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="a2103-180">Guid</span><span class="sxs-lookup"><span data-stu-id="a2103-180">Guid</span></span>|<span data-ttu-id="a2103-181">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="a2103-181">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="a2103-182">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-182">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-183">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="a2103-183">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="a2103-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2103-184">Boolean</span></span>|<span data-ttu-id="a2103-185">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-185">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-186">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="a2103-186">iconsVisible</span></span>|<span data-ttu-id="a2103-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2103-187">Boolean</span></span>|<span data-ttu-id="a2103-188">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="a2103-188">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="a2103-189">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-189">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-190">protectedApps</span><span class="sxs-lookup"><span data-stu-id="a2103-190">protectedApps</span></span>|<span data-ttu-id="a2103-191">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2103-191">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="a2103-192">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-192">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-193">exemptApps</span><span class="sxs-lookup"><span data-stu-id="a2103-193">exemptApps</span></span>|<span data-ttu-id="a2103-194">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2103-194">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="a2103-195">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="a2103-195">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="a2103-196">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="a2103-196">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="a2103-197">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-197">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-198">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="a2103-198">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="a2103-199">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2103-199">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a2103-200">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="a2103-200">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="a2103-201">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-201">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-202">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="a2103-202">enterpriseProxiedDomains</span></span>|<span data-ttu-id="a2103-203">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2103-203">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="a2103-204">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="a2103-204">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="a2103-205">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="a2103-205">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="a2103-206">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="a2103-206">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="a2103-207">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-207">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-208">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="a2103-208">enterpriseIPRanges</span></span>|<span data-ttu-id="a2103-209">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2103-209">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="a2103-210">设置定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="a2103-210">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="a2103-211">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="a2103-211">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="a2103-212">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-212">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-213">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="a2103-213">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="a2103-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2103-214">Boolean</span></span>|<span data-ttu-id="a2103-215">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="a2103-215">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="a2103-216">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-216">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-217">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="a2103-217">enterpriseProxyServers</span></span>|<span data-ttu-id="a2103-218">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2103-218">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a2103-219">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="a2103-219">This is a list of proxy servers.</span></span> <span data-ttu-id="a2103-220">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-220">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-221">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="a2103-221">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="a2103-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2103-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a2103-223">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="a2103-223">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="a2103-224">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="a2103-224">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="a2103-225">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="a2103-225">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="a2103-226">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="a2103-226">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="a2103-227">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-227">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-228">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="a2103-228">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="a2103-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2103-229">Boolean</span></span>|<span data-ttu-id="a2103-230">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="a2103-230">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="a2103-231">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-231">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-232">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="a2103-232">neutralDomainResources</span></span>|<span data-ttu-id="a2103-233">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2103-233">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a2103-234">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-234">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-235">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="a2103-235">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="a2103-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2103-236">Boolean</span></span>|<span data-ttu-id="a2103-237">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-237">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-238">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="a2103-238">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="a2103-239">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2103-239">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a2103-240">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-240">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a2103-241">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a2103-241">isAssigned</span></span>|<span data-ttu-id="a2103-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2103-242">Boolean</span></span>|<span data-ttu-id="a2103-243">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="a2103-243">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="a2103-244">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a2103-244">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a2103-245">响应</span><span class="sxs-lookup"><span data-stu-id="a2103-245">Response</span></span>
<span data-ttu-id="a2103-246">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a2103-246">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2103-247">示例</span><span class="sxs-lookup"><span data-stu-id="a2103-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2103-248">请求</span><span class="sxs-lookup"><span data-stu-id="a2103-248">Request</span></span>
<span data-ttu-id="a2103-249">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2103-249">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies
Content-type: application/json
Content-length: 3905

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
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
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="a2103-250">响应</span><span class="sxs-lookup"><span data-stu-id="a2103-250">Response</span></span>
<span data-ttu-id="a2103-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2103-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




