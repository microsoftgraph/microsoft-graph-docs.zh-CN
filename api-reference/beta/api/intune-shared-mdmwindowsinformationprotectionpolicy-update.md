---
title: 更新 mdmWindowsInformationProtectionPolicy
description: 更新 mdmWindowsInformationProtectionPolicy 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e7d336c4fea513a594a5886cdc73e0b7a0f7ed1e
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085813"
---
# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="1c1f4-103">更新 mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="1c1f4-103">Update mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="1c1f4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c1f4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c1f4-106">更新 [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-106">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c1f4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1c1f4-107">Prerequisites</span></span>
<span data-ttu-id="1c1f4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c1f4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c1f4-110">Permission type</span></span>|<span data-ttu-id="1c1f4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1c1f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c1f4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c1f4-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1c1f4-113">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="1c1f4-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="1c1f4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c1f4-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="1c1f4-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="1c1f4-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1c1f4-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c1f4-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1c1f4-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c1f4-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c1f4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-118">Not supported.</span></span>|
|<span data-ttu-id="1c1f4-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c1f4-119">Application</span></span>||
| <span data-ttu-id="1c1f4-120">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="1c1f4-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="1c1f4-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c1f4-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="1c1f4-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="1c1f4-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1c1f4-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c1f4-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c1f4-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c1f4-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="1c1f4-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c1f4-125">Request headers</span></span>
|<span data-ttu-id="1c1f4-126">标头</span><span class="sxs-lookup"><span data-stu-id="1c1f4-126">Header</span></span>|<span data-ttu-id="1c1f4-127">值</span><span class="sxs-lookup"><span data-stu-id="1c1f4-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c1f4-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c1f4-128">Authorization</span></span>|<span data-ttu-id="1c1f4-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c1f4-130">接受</span><span class="sxs-lookup"><span data-stu-id="1c1f4-130">Accept</span></span>|<span data-ttu-id="1c1f4-131">application/json</span><span class="sxs-lookup"><span data-stu-id="1c1f4-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c1f4-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c1f4-132">Request body</span></span>
<span data-ttu-id="1c1f4-133">在请求正文中，提供 [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-133">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="1c1f4-134">下表显示创建 [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-134">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="1c1f4-135">属性</span><span class="sxs-lookup"><span data-stu-id="1c1f4-135">Property</span></span>|<span data-ttu-id="1c1f4-136">类型</span><span class="sxs-lookup"><span data-stu-id="1c1f4-136">Type</span></span>|<span data-ttu-id="1c1f4-137">说明</span><span class="sxs-lookup"><span data-stu-id="1c1f4-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c1f4-138">displayName</span><span class="sxs-lookup"><span data-stu-id="1c1f4-138">displayName</span></span>|<span data-ttu-id="1c1f4-139">字符串</span><span class="sxs-lookup"><span data-stu-id="1c1f4-139">String</span></span>|<span data-ttu-id="1c1f4-140">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-140">Policy display name.</span></span> <span data-ttu-id="1c1f4-141">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1c1f4-142">说明</span><span class="sxs-lookup"><span data-stu-id="1c1f4-142">description</span></span>|<span data-ttu-id="1c1f4-143">String</span><span class="sxs-lookup"><span data-stu-id="1c1f4-143">String</span></span>|<span data-ttu-id="1c1f4-144">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-144">The policy's description.</span></span> <span data-ttu-id="1c1f4-145">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1c1f4-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c1f4-146">createdDateTime</span></span>|<span data-ttu-id="1c1f4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c1f4-147">DateTimeOffset</span></span>|<span data-ttu-id="1c1f4-148">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-148">The date and time the policy was created.</span></span> <span data-ttu-id="1c1f4-149">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1c1f4-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c1f4-150">lastModifiedDateTime</span></span>|<span data-ttu-id="1c1f4-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c1f4-151">DateTimeOffset</span></span>|<span data-ttu-id="1c1f4-152">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-152">Last time the policy was modified.</span></span> <span data-ttu-id="1c1f4-153">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1c1f4-154">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1c1f4-154">roleScopeTagIds</span></span>|<span data-ttu-id="1c1f4-155">String collection</span><span class="sxs-lookup"><span data-stu-id="1c1f4-155">String collection</span></span>|<span data-ttu-id="1c1f4-156">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-156">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1c1f4-157">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-157">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1c1f4-158">id</span><span class="sxs-lookup"><span data-stu-id="1c1f4-158">id</span></span>|<span data-ttu-id="1c1f4-159">字符串</span><span class="sxs-lookup"><span data-stu-id="1c1f4-159">String</span></span>|<span data-ttu-id="1c1f4-160">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-160">Key of the entity.</span></span> <span data-ttu-id="1c1f4-161">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-161">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1c1f4-162">version</span><span class="sxs-lookup"><span data-stu-id="1c1f4-162">version</span></span>|<span data-ttu-id="1c1f4-163">String</span><span class="sxs-lookup"><span data-stu-id="1c1f4-163">String</span></span>|<span data-ttu-id="1c1f4-164">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-164">Version of the entity.</span></span> <span data-ttu-id="1c1f4-165">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-165">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1c1f4-166">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="1c1f4-166">enforcementLevel</span></span>|[<span data-ttu-id="1c1f4-167">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="1c1f4-167">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="1c1f4-168">WIP 强制等级。若要获取从[WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)继承的受支持值的枚举定义，请参阅。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-168">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="1c1f4-169">可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-169">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="1c1f4-170">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="1c1f4-170">enterpriseDomain</span></span>|<span data-ttu-id="1c1f4-171">String</span><span class="sxs-lookup"><span data-stu-id="1c1f4-171">String</span></span>|<span data-ttu-id="1c1f4-172">主企业域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-172">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-173">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="1c1f4-173">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="1c1f4-174">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c1f4-174">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="1c1f4-175">要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-175">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-176">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="1c1f4-176">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="1c1f4-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c1f4-177">Boolean</span></span>|<span data-ttu-id="1c1f4-178">指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-178">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-179">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="1c1f4-179">dataRecoveryCertificate</span></span>|[<span data-ttu-id="1c1f4-180">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="1c1f4-180">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="1c1f4-181">指定可用于加密文件数据恢复的恢复证书。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-181">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="1c1f4-182">这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-182">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-183">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="1c1f4-183">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="1c1f4-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c1f4-184">Boolean</span></span>|<span data-ttu-id="1c1f4-185">此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-185">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="1c1f4-186">如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-186">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="1c1f4-187">如果未撤销密钥，随后将不会撤销文件清除。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-187">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="1c1f4-188">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-188">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-189">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="1c1f4-189">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="1c1f4-190">Guid</span><span class="sxs-lookup"><span data-stu-id="1c1f4-190">Guid</span></span>|<span data-ttu-id="1c1f4-191">用于 RMS 加密的 TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-191">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="1c1f4-192">RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-192">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-193">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="1c1f4-193">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="1c1f4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c1f4-194">Boolean</span></span>|<span data-ttu-id="1c1f4-195">指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-195">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-196">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="1c1f4-196">iconsVisible</span></span>|<span data-ttu-id="1c1f4-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c1f4-197">Boolean</span></span>|<span data-ttu-id="1c1f4-198">确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-198">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="1c1f4-199">从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-199">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-200">protectedApps</span><span class="sxs-lookup"><span data-stu-id="1c1f4-200">protectedApps</span></span>|<span data-ttu-id="1c1f4-201">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c1f4-201">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="1c1f4-202">受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-202">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-203">exemptApps</span><span class="sxs-lookup"><span data-stu-id="1c1f4-203">exemptApps</span></span>|<span data-ttu-id="1c1f4-204">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c1f4-204">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="1c1f4-205">豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-205">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="1c1f4-206">这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-206">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="1c1f4-207">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-207">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-208">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="1c1f4-208">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="1c1f4-209">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c1f4-209">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="1c1f4-210">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-210">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="1c1f4-211">发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-211">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-212">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="1c1f4-212">enterpriseProxiedDomains</span></span>|<span data-ttu-id="1c1f4-213">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c1f4-213">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="1c1f4-214">包含需要保护的托管在云中的企业资源域列表。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-214">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="1c1f4-215">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-215">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="1c1f4-216">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-216">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="1c1f4-217">用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-217">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-218">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="1c1f4-218">enterpriseIPRanges</span></span>|<span data-ttu-id="1c1f4-219">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c1f4-219">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="1c1f4-220">设置定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-220">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="1c1f4-221">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-221">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="1c1f4-222">这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-222">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-223">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="1c1f4-223">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="1c1f4-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c1f4-224">Boolean</span></span>|<span data-ttu-id="1c1f4-225">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-225">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="1c1f4-226">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-226">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-227">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="1c1f4-227">enterpriseProxyServers</span></span>|<span data-ttu-id="1c1f4-228">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c1f4-228">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="1c1f4-229">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-229">This is a list of proxy servers.</span></span> <span data-ttu-id="1c1f4-230">任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-230">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-231">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="1c1f4-231">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="1c1f4-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c1f4-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="1c1f4-233">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-233">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="1c1f4-234">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-234">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="1c1f4-235">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-235">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="1c1f4-236">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-236">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="1c1f4-237">仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-237">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-238">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="1c1f4-238">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="1c1f4-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c1f4-239">Boolean</span></span>|<span data-ttu-id="1c1f4-240">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-240">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="1c1f4-241">默认值为 false。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-241">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-242">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="1c1f4-242">neutralDomainResources</span></span>|<span data-ttu-id="1c1f4-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c1f4-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="1c1f4-244">可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-244">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-245">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="1c1f4-245">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="1c1f4-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c1f4-246">Boolean</span></span>|<span data-ttu-id="1c1f4-247">此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-247">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-248">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="1c1f4-248">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="1c1f4-249">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c1f4-249">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="1c1f4-250">指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-250">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="1c1f4-251">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1c1f4-251">isAssigned</span></span>|<span data-ttu-id="1c1f4-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c1f4-252">Boolean</span></span>|<span data-ttu-id="1c1f4-253">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-253">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="1c1f4-254">继承自 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1c1f4-254">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1c1f4-255">响应</span><span class="sxs-lookup"><span data-stu-id="1c1f4-255">Response</span></span>
<span data-ttu-id="1c1f4-256">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-256">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c1f4-257">示例</span><span class="sxs-lookup"><span data-stu-id="1c1f4-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c1f4-258">请求</span><span class="sxs-lookup"><span data-stu-id="1c1f4-258">Request</span></span>
<span data-ttu-id="1c1f4-259">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-259">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
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

### <a name="response"></a><span data-ttu-id="1c1f4-260">响应</span><span class="sxs-lookup"><span data-stu-id="1c1f4-260">Response</span></span>
<span data-ttu-id="1c1f4-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1c1f4-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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









