---
title: 更新 iosEasEmailProfileConfiguration
description: 更新 iosEasEmailProfileConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a965fa5e70c2182c54a9c67ba4aa9144e56ea4e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129991"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="4255f-103">更新 iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="4255f-103">Update iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="4255f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4255f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4255f-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4255f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4255f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4255f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4255f-107">更新 [iosEasEmailProfileConfiguration 对象](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="4255f-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4255f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4255f-108">Prerequisites</span></span>
<span data-ttu-id="4255f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4255f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4255f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4255f-111">Permission type</span></span>|<span data-ttu-id="4255f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4255f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4255f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4255f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4255f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4255f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4255f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4255f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4255f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4255f-116">Not supported.</span></span>|
|<span data-ttu-id="4255f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4255f-117">Application</span></span>|<span data-ttu-id="4255f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4255f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4255f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4255f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4255f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4255f-120">Request headers</span></span>
|<span data-ttu-id="4255f-121">标头</span><span class="sxs-lookup"><span data-stu-id="4255f-121">Header</span></span>|<span data-ttu-id="4255f-122">值</span><span class="sxs-lookup"><span data-stu-id="4255f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4255f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4255f-123">Authorization</span></span>|<span data-ttu-id="4255f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4255f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4255f-125">接受</span><span class="sxs-lookup"><span data-stu-id="4255f-125">Accept</span></span>|<span data-ttu-id="4255f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4255f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4255f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4255f-127">Request body</span></span>
<span data-ttu-id="4255f-128">在请求正文中，提供 [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4255f-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="4255f-129">下表显示创建 [iosEasEmailProfileConfiguration 时所需的属性](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="4255f-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="4255f-130">属性</span><span class="sxs-lookup"><span data-stu-id="4255f-130">Property</span></span>|<span data-ttu-id="4255f-131">类型</span><span class="sxs-lookup"><span data-stu-id="4255f-131">Type</span></span>|<span data-ttu-id="4255f-132">说明</span><span class="sxs-lookup"><span data-stu-id="4255f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4255f-133">id</span><span class="sxs-lookup"><span data-stu-id="4255f-133">id</span></span>|<span data-ttu-id="4255f-134">String</span><span class="sxs-lookup"><span data-stu-id="4255f-134">String</span></span>|<span data-ttu-id="4255f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4255f-135">Key of the entity.</span></span> <span data-ttu-id="4255f-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4255f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4255f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4255f-138">DateTimeOffset</span></span>|<span data-ttu-id="4255f-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4255f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4255f-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4255f-141">roleScopeTagIds</span></span>|<span data-ttu-id="4255f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="4255f-142">String collection</span></span>|<span data-ttu-id="4255f-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4255f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4255f-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4255f-145">supportsScopeTags</span></span>|<span data-ttu-id="4255f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-146">Boolean</span></span>|<span data-ttu-id="4255f-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="4255f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4255f-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="4255f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4255f-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="4255f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4255f-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4255f-150">This property is read-only.</span></span> <span data-ttu-id="4255f-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4255f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4255f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4255f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4255f-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="4255f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4255f-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4255f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4255f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4255f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4255f-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4255f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4255f-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4255f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4255f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4255f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4255f-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4255f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4255f-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4255f-164">createdDateTime</span></span>|<span data-ttu-id="4255f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4255f-165">DateTimeOffset</span></span>|<span data-ttu-id="4255f-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4255f-166">DateTime the object was created.</span></span> <span data-ttu-id="4255f-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-168">说明</span><span class="sxs-lookup"><span data-stu-id="4255f-168">description</span></span>|<span data-ttu-id="4255f-169">String</span><span class="sxs-lookup"><span data-stu-id="4255f-169">String</span></span>|<span data-ttu-id="4255f-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4255f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4255f-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4255f-172">displayName</span></span>|<span data-ttu-id="4255f-173">String</span><span class="sxs-lookup"><span data-stu-id="4255f-173">String</span></span>|<span data-ttu-id="4255f-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4255f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4255f-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-176">version</span><span class="sxs-lookup"><span data-stu-id="4255f-176">version</span></span>|<span data-ttu-id="4255f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4255f-177">Int32</span></span>|<span data-ttu-id="4255f-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4255f-178">Version of the device configuration.</span></span> <span data-ttu-id="4255f-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4255f-180">usernameSource</span></span>|[<span data-ttu-id="4255f-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="4255f-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4255f-182">在设备上安装之前从 AAD 中选取并注入到此配置文件中的用户名属性。</span><span class="sxs-lookup"><span data-stu-id="4255f-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4255f-183">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="4255f-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4255f-184">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="4255f-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4255f-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="4255f-185">usernameAADSource</span></span>|[<span data-ttu-id="4255f-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4255f-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="4255f-187">AAD 字段的名称，该字段将用于检索电子邮件配置文件的 UserName。</span><span class="sxs-lookup"><span data-stu-id="4255f-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="4255f-188">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="4255f-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4255f-189">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="4255f-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="4255f-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="4255f-190">userDomainNameSource</span></span>|[<span data-ttu-id="4255f-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="4255f-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="4255f-192">UserDomainname 属性，在设备上安装之前从 AAD 中选取并注入到此配置文件中。</span><span class="sxs-lookup"><span data-stu-id="4255f-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4255f-193">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="4255f-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4255f-194">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="4255f-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="4255f-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="4255f-195">customDomainName</span></span>|<span data-ttu-id="4255f-196">String</span><span class="sxs-lookup"><span data-stu-id="4255f-196">String</span></span>|<span data-ttu-id="4255f-197">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="4255f-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="4255f-198">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="4255f-199">accountName</span><span class="sxs-lookup"><span data-stu-id="4255f-199">accountName</span></span>|<span data-ttu-id="4255f-200">String</span><span class="sxs-lookup"><span data-stu-id="4255f-200">String</span></span>|<span data-ttu-id="4255f-201">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="4255f-201">Account name.</span></span>|
|<span data-ttu-id="4255f-202">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4255f-202">authenticationMethod</span></span>|[<span data-ttu-id="4255f-203">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4255f-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="4255f-204">此电子邮件配置文件的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="4255f-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="4255f-205">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="4255f-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="4255f-206">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="4255f-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="4255f-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-207">Boolean</span></span>|<span data-ttu-id="4255f-208">指示是否阻止将邮件移动到其他电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="4255f-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="4255f-209">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="4255f-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="4255f-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-210">Boolean</span></span>|<span data-ttu-id="4255f-211">指示是否阻止从第三方应用发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="4255f-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="4255f-212">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="4255f-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="4255f-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-213">Boolean</span></span>|<span data-ttu-id="4255f-214">指示是否阻止同步最近使用的电子邮件地址，例如 - 撰写新电子邮件时。</span><span class="sxs-lookup"><span data-stu-id="4255f-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="4255f-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="4255f-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="4255f-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="4255f-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="4255f-217">电子邮件应同步回的持续时间。</span><span class="sxs-lookup"><span data-stu-id="4255f-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="4255f-218">.</span><span class="sxs-lookup"><span data-stu-id="4255f-218">.</span></span> <span data-ttu-id="4255f-219">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="4255f-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="4255f-220">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="4255f-220">emailAddressSource</span></span>|[<span data-ttu-id="4255f-221">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="4255f-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4255f-222">从 AAD 中选取并注入到此配置文件中的电子邮件属性，在设备上安装之前。</span><span class="sxs-lookup"><span data-stu-id="4255f-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4255f-223">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="4255f-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4255f-224">easServices</span><span class="sxs-lookup"><span data-stu-id="4255f-224">easServices</span></span>|[<span data-ttu-id="4255f-225">easServices</span><span class="sxs-lookup"><span data-stu-id="4255f-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="4255f-226">要同步的 Exchange 数据。可能的值是 `none` `calendars` `contacts` ：、、、、、。 `email` `notes` `reminders`</span><span class="sxs-lookup"><span data-stu-id="4255f-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="4255f-227">easServicesUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="4255f-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="4255f-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-228">Boolean</span></span>|<span data-ttu-id="4255f-229">允许用户更改同步设置。</span><span class="sxs-lookup"><span data-stu-id="4255f-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="4255f-230">hostName</span><span class="sxs-lookup"><span data-stu-id="4255f-230">hostName</span></span>|<span data-ttu-id="4255f-231">String</span><span class="sxs-lookup"><span data-stu-id="4255f-231">String</span></span>|<span data-ttu-id="4255f-232">使用本机 (连接到) URL 的 Exchange 位置。</span><span class="sxs-lookup"><span data-stu-id="4255f-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="4255f-233">requireSmime</span><span class="sxs-lookup"><span data-stu-id="4255f-233">requireSmime</span></span>|<span data-ttu-id="4255f-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-234">Boolean</span></span>|<span data-ttu-id="4255f-235">指示是否使用 S/MIME 证书。</span><span class="sxs-lookup"><span data-stu-id="4255f-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="4255f-236">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="4255f-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="4255f-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-237">Boolean</span></span>|<span data-ttu-id="4255f-238">指示是否允许未加密的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="4255f-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="4255f-239">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="4255f-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="4255f-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-240">Boolean</span></span>|<span data-ttu-id="4255f-241">如果设置为 true，则默认启用 S/MIME 加密。</span><span class="sxs-lookup"><span data-stu-id="4255f-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="4255f-242">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="4255f-242">smimeSigningEnabled</span></span>|<span data-ttu-id="4255f-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-243">Boolean</span></span>|<span data-ttu-id="4255f-244">如果设置为 true，则为此帐户启用 S/MIME 签名</span><span class="sxs-lookup"><span data-stu-id="4255f-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="4255f-245">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="4255f-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="4255f-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-246">Boolean</span></span>|<span data-ttu-id="4255f-247">如果设置为 true，用户可以打开或关闭 S/MIME 签名。</span><span class="sxs-lookup"><span data-stu-id="4255f-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="4255f-248">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="4255f-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="4255f-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-249">Boolean</span></span>|<span data-ttu-id="4255f-250">如果设置为 true，用户可以默认切换加密设置。</span><span class="sxs-lookup"><span data-stu-id="4255f-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="4255f-251">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="4255f-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="4255f-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-252">Boolean</span></span>|<span data-ttu-id="4255f-253">如果设置为 true，则用户可以选择签名标识。</span><span class="sxs-lookup"><span data-stu-id="4255f-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="4255f-254">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="4255f-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="4255f-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-255">Boolean</span></span>|<span data-ttu-id="4255f-256">如果设置为 true，则用户可以选择 S/MIME 加密标识。</span><span class="sxs-lookup"><span data-stu-id="4255f-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="4255f-257">requireSsl</span><span class="sxs-lookup"><span data-stu-id="4255f-257">requireSsl</span></span>|<span data-ttu-id="4255f-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-258">Boolean</span></span>|<span data-ttu-id="4255f-259">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="4255f-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="4255f-260">useOAuth</span><span class="sxs-lookup"><span data-stu-id="4255f-260">useOAuth</span></span>|<span data-ttu-id="4255f-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-261">Boolean</span></span>|<span data-ttu-id="4255f-262">指定连接是否应该使用 OAuth 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="4255f-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="4255f-263">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="4255f-263">signingCertificateType</span></span>|[<span data-ttu-id="4255f-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="4255f-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="4255f-265">签署此电子邮件配置文件的证书类型。</span><span class="sxs-lookup"><span data-stu-id="4255f-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="4255f-266">可取值为：`none`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="4255f-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="4255f-267">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="4255f-267">encryptionCertificateType</span></span>|[<span data-ttu-id="4255f-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="4255f-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="4255f-269">加密 此电子邮件配置文件的证书类型。</span><span class="sxs-lookup"><span data-stu-id="4255f-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="4255f-270">可取值为：`none`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="4255f-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="4255f-271">perAppVPNProfileId</span><span class="sxs-lookup"><span data-stu-id="4255f-271">perAppVPNProfileId</span></span>|<span data-ttu-id="4255f-272">String</span><span class="sxs-lookup"><span data-stu-id="4255f-272">String</span></span>|<span data-ttu-id="4255f-273">用于从本机Per-App客户端访问电子邮件的邮箱 VPN 策略的配置文件 ID</span><span class="sxs-lookup"><span data-stu-id="4255f-273">Profile ID of the Per-App VPN policy to be used to access emails from the native Mail client</span></span>|



## <a name="response"></a><span data-ttu-id="4255f-274">响应</span><span class="sxs-lookup"><span data-stu-id="4255f-274">Response</span></span>
<span data-ttu-id="4255f-275">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4255f-275">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4255f-276">示例</span><span class="sxs-lookup"><span data-stu-id="4255f-276">Example</span></span>

### <a name="request"></a><span data-ttu-id="4255f-277">请求</span><span class="sxs-lookup"><span data-stu-id="4255f-277">Request</span></span>
<span data-ttu-id="4255f-278">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4255f-278">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2187

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "easServices": "calendars",
  "easServicesUserOverrideEnabled": true,
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "certificate",
  "encryptionCertificateType": "certificate",
  "perAppVPNProfileId": "Per App VPNProfile Id value"
}
```

### <a name="response"></a><span data-ttu-id="4255f-279">响应</span><span class="sxs-lookup"><span data-stu-id="4255f-279">Response</span></span>
<span data-ttu-id="4255f-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4255f-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2359

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "id": "e03086da-86da-e030-da86-30e0da8630e0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "easServices": "calendars",
  "easServicesUserOverrideEnabled": true,
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "certificate",
  "encryptionCertificateType": "certificate",
  "perAppVPNProfileId": "Per App VPNProfile Id value"
}
```




