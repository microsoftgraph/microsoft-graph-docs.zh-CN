---
title: 更新 mdmWindowsInformationProtectionPolicy
description: 更新 mdmWindowsInformationProtectionPolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 361b1fde8a04f5a28f2a682647f59fc7a1c85b47
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996586"
---
# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="183d8-103">更新 mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="183d8-103">Update mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="183d8-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="183d8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="183d8-105">更新 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="183d8-105">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="183d8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="183d8-106">Prerequisites</span></span>
<span data-ttu-id="183d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="183d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="183d8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="183d8-109">Permission type</span></span>|<span data-ttu-id="183d8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="183d8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="183d8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="183d8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="183d8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="183d8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="183d8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="183d8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="183d8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="183d8-114">Not supported.</span></span>|
|<span data-ttu-id="183d8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="183d8-115">Application</span></span>|<span data-ttu-id="183d8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="183d8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="183d8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="183d8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="183d8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="183d8-118">Request headers</span></span>
|<span data-ttu-id="183d8-119">标头</span><span class="sxs-lookup"><span data-stu-id="183d8-119">Header</span></span>|<span data-ttu-id="183d8-120">值</span><span class="sxs-lookup"><span data-stu-id="183d8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="183d8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="183d8-121">Authorization</span></span>|<span data-ttu-id="183d8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="183d8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="183d8-123">接受</span><span class="sxs-lookup"><span data-stu-id="183d8-123">Accept</span></span>|<span data-ttu-id="183d8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="183d8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="183d8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="183d8-125">Request body</span></span>
<span data-ttu-id="183d8-126">在请求正文中，提供 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="183d8-126">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="183d8-127">下表显示创建 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="183d8-127">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="183d8-128">属性</span><span class="sxs-lookup"><span data-stu-id="183d8-128">Property</span></span>|<span data-ttu-id="183d8-129">类型</span><span class="sxs-lookup"><span data-stu-id="183d8-129">Type</span></span>|<span data-ttu-id="183d8-130">说明</span><span class="sxs-lookup"><span data-stu-id="183d8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="183d8-131">displayName</span><span class="sxs-lookup"><span data-stu-id="183d8-131">displayName</span></span>|<span data-ttu-id="183d8-132">字符串</span><span class="sxs-lookup"><span data-stu-id="183d8-132">String</span></span>|<span data-ttu-id="183d8-133">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="183d8-133">Policy display name.</span></span> <span data-ttu-id="183d8-134">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="183d8-135">说明</span><span class="sxs-lookup"><span data-stu-id="183d8-135">description</span></span>|<span data-ttu-id="183d8-136">String</span><span class="sxs-lookup"><span data-stu-id="183d8-136">String</span></span>|<span data-ttu-id="183d8-137">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="183d8-137">The policy's description.</span></span> <span data-ttu-id="183d8-138">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="183d8-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="183d8-139">createdDateTime</span></span>|<span data-ttu-id="183d8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="183d8-140">DateTimeOffset</span></span>|<span data-ttu-id="183d8-141">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="183d8-141">The date and time the policy was created.</span></span> <span data-ttu-id="183d8-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="183d8-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="183d8-143">lastModifiedDateTime</span></span>|<span data-ttu-id="183d8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="183d8-144">DateTimeOffset</span></span>|<span data-ttu-id="183d8-145">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="183d8-145">Last time the policy was modified.</span></span> <span data-ttu-id="183d8-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="183d8-147">id</span><span class="sxs-lookup"><span data-stu-id="183d8-147">id</span></span>|<span data-ttu-id="183d8-148">字符串</span><span class="sxs-lookup"><span data-stu-id="183d8-148">String</span></span>|<span data-ttu-id="183d8-149">实体的键。</span><span class="sxs-lookup"><span data-stu-id="183d8-149">Key of the entity.</span></span> <span data-ttu-id="183d8-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="183d8-151">version</span><span class="sxs-lookup"><span data-stu-id="183d8-151">version</span></span>|<span data-ttu-id="183d8-152">String</span><span class="sxs-lookup"><span data-stu-id="183d8-152">String</span></span>|<span data-ttu-id="183d8-153">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="183d8-153">Version of the entity.</span></span> <span data-ttu-id="183d8-154">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="183d8-155">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="183d8-155">enforcementLevel</span></span>|[<span data-ttu-id="183d8-156">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="183d8-156">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="183d8-157">WIP 强制等级。若要获取从[WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)继承的受支持值的枚举定义, 请参阅。</span><span class="sxs-lookup"><span data-stu-id="183d8-157">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="183d8-158">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="183d8-158">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="183d8-159">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="183d8-159">enterpriseDomain</span></span>|<span data-ttu-id="183d8-160">String</span><span class="sxs-lookup"><span data-stu-id="183d8-160">String</span></span>|<span data-ttu-id="183d8-161">主企业域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-161">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-162">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="183d8-162">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="183d8-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="183d8-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="183d8-164">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-164">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-165">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="183d8-165">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="183d8-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="183d8-166">Boolean</span></span>|<span data-ttu-id="183d8-167">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-167">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-168">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="183d8-168">dataRecoveryCertificate</span></span>|[<span data-ttu-id="183d8-169">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="183d8-169">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="183d8-170">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="183d8-170">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="183d8-171">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-171">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-172">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="183d8-172">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="183d8-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="183d8-173">Boolean</span></span>|<span data-ttu-id="183d8-174">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="183d8-174">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="183d8-175">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="183d8-175">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="183d8-176">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="183d8-176">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="183d8-177">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-177">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-178">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="183d8-178">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="183d8-179">Guid</span><span class="sxs-lookup"><span data-stu-id="183d8-179">Guid</span></span>|<span data-ttu-id="183d8-180">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="183d8-180">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="183d8-181">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-181">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-182">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="183d8-182">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="183d8-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="183d8-183">Boolean</span></span>|<span data-ttu-id="183d8-184">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-184">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-185">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="183d8-185">iconsVisible</span></span>|<span data-ttu-id="183d8-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="183d8-186">Boolean</span></span>|<span data-ttu-id="183d8-187">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="183d8-187">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="183d8-188">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-188">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-189">protectedApps</span><span class="sxs-lookup"><span data-stu-id="183d8-189">protectedApps</span></span>|<span data-ttu-id="183d8-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="183d8-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="183d8-191">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-191">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-192">exemptApps</span><span class="sxs-lookup"><span data-stu-id="183d8-192">exemptApps</span></span>|<span data-ttu-id="183d8-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="183d8-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="183d8-194">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="183d8-194">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="183d8-195">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="183d8-195">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="183d8-196">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-196">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-197">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="183d8-197">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="183d8-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="183d8-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="183d8-199">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="183d8-199">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="183d8-200">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-200">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-201">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="183d8-201">enterpriseProxiedDomains</span></span>|<span data-ttu-id="183d8-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="183d8-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="183d8-203">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="183d8-203">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="183d8-204">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="183d8-204">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="183d8-205">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="183d8-205">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="183d8-206">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-206">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-207">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="183d8-207">enterpriseIPRanges</span></span>|<span data-ttu-id="183d8-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="183d8-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="183d8-209">设置定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="183d8-209">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="183d8-210">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="183d8-210">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="183d8-211">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-211">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-212">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="183d8-212">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="183d8-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="183d8-213">Boolean</span></span>|<span data-ttu-id="183d8-214">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="183d8-214">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="183d8-215">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-215">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-216">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="183d8-216">enterpriseProxyServers</span></span>|<span data-ttu-id="183d8-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="183d8-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="183d8-218">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="183d8-218">This is a list of proxy servers.</span></span> <span data-ttu-id="183d8-219">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-219">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-220">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="183d8-220">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="183d8-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="183d8-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="183d8-222">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="183d8-222">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="183d8-223">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="183d8-223">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="183d8-224">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="183d8-224">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="183d8-225">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="183d8-225">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="183d8-226">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-226">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-227">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="183d8-227">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="183d8-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="183d8-228">Boolean</span></span>|<span data-ttu-id="183d8-229">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="183d8-229">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="183d8-230">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-230">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-231">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="183d8-231">neutralDomainResources</span></span>|<span data-ttu-id="183d8-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="183d8-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="183d8-233">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-233">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-234">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="183d8-234">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="183d8-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="183d8-235">Boolean</span></span>|<span data-ttu-id="183d8-236">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-236">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-237">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="183d8-237">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="183d8-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="183d8-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="183d8-239">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-239">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="183d8-240">isAssigned</span><span class="sxs-lookup"><span data-stu-id="183d8-240">isAssigned</span></span>|<span data-ttu-id="183d8-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="183d8-241">Boolean</span></span>|<span data-ttu-id="183d8-242">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="183d8-242">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="183d8-243">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="183d8-243">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="183d8-244">响应</span><span class="sxs-lookup"><span data-stu-id="183d8-244">Response</span></span>
<span data-ttu-id="183d8-245">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="183d8-245">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="183d8-246">示例</span><span class="sxs-lookup"><span data-stu-id="183d8-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="183d8-247">请求</span><span class="sxs-lookup"><span data-stu-id="183d8-247">Request</span></span>
<span data-ttu-id="183d8-248">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="183d8-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
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

### <a name="response"></a><span data-ttu-id="183d8-249">响应</span><span class="sxs-lookup"><span data-stu-id="183d8-249">Response</span></span>
<span data-ttu-id="183d8-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="183d8-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



