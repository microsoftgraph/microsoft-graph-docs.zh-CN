---
title: 创建 iosEasEmailProfileConfiguration
description: 创建新的 iosEasEmailProfileConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eb8a26779255430cf000e7047ef871d8da96b1a4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130012"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="a8503-103">创建 iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8503-103">Create iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="a8503-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8503-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8503-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a8503-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8503-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a8503-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8503-107">创建新的 [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a8503-107">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8503-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a8503-108">Prerequisites</span></span>
<span data-ttu-id="a8503-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8503-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8503-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8503-111">Permission type</span></span>|<span data-ttu-id="a8503-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8503-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8503-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8503-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8503-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8503-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8503-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8503-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8503-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8503-116">Not supported.</span></span>|
|<span data-ttu-id="a8503-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8503-117">Application</span></span>|<span data-ttu-id="a8503-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8503-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8503-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8503-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a8503-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8503-120">Request headers</span></span>
|<span data-ttu-id="a8503-121">标头</span><span class="sxs-lookup"><span data-stu-id="a8503-121">Header</span></span>|<span data-ttu-id="a8503-122">值</span><span class="sxs-lookup"><span data-stu-id="a8503-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8503-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8503-123">Authorization</span></span>|<span data-ttu-id="a8503-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a8503-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8503-125">接受</span><span class="sxs-lookup"><span data-stu-id="a8503-125">Accept</span></span>|<span data-ttu-id="a8503-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8503-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8503-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8503-127">Request body</span></span>
<span data-ttu-id="a8503-128">在请求正文中，提供 iosEasEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8503-128">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="a8503-129">下表显示创建 iosEasEmailProfileConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a8503-129">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="a8503-130">属性</span><span class="sxs-lookup"><span data-stu-id="a8503-130">Property</span></span>|<span data-ttu-id="a8503-131">类型</span><span class="sxs-lookup"><span data-stu-id="a8503-131">Type</span></span>|<span data-ttu-id="a8503-132">说明</span><span class="sxs-lookup"><span data-stu-id="a8503-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8503-133">id</span><span class="sxs-lookup"><span data-stu-id="a8503-133">id</span></span>|<span data-ttu-id="a8503-134">String</span><span class="sxs-lookup"><span data-stu-id="a8503-134">String</span></span>|<span data-ttu-id="a8503-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a8503-135">Key of the entity.</span></span> <span data-ttu-id="a8503-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8503-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8503-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8503-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a8503-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8503-138">DateTimeOffset</span></span>|<span data-ttu-id="a8503-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a8503-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a8503-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8503-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8503-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a8503-141">roleScopeTagIds</span></span>|<span data-ttu-id="a8503-142">String collection</span><span class="sxs-lookup"><span data-stu-id="a8503-142">String collection</span></span>|<span data-ttu-id="a8503-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a8503-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a8503-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8503-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8503-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a8503-145">supportsScopeTags</span></span>|<span data-ttu-id="a8503-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-146">Boolean</span></span>|<span data-ttu-id="a8503-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="a8503-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a8503-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="a8503-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a8503-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="a8503-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a8503-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a8503-150">This property is read-only.</span></span> <span data-ttu-id="a8503-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8503-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8503-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a8503-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a8503-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a8503-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a8503-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="a8503-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a8503-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8503-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8503-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a8503-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a8503-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a8503-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a8503-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a8503-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a8503-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8503-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8503-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a8503-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a8503-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a8503-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a8503-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a8503-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a8503-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8503-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8503-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8503-164">createdDateTime</span></span>|<span data-ttu-id="a8503-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8503-165">DateTimeOffset</span></span>|<span data-ttu-id="a8503-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a8503-166">DateTime the object was created.</span></span> <span data-ttu-id="a8503-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8503-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8503-168">说明</span><span class="sxs-lookup"><span data-stu-id="a8503-168">description</span></span>|<span data-ttu-id="a8503-169">String</span><span class="sxs-lookup"><span data-stu-id="a8503-169">String</span></span>|<span data-ttu-id="a8503-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a8503-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a8503-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8503-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8503-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a8503-172">displayName</span></span>|<span data-ttu-id="a8503-173">String</span><span class="sxs-lookup"><span data-stu-id="a8503-173">String</span></span>|<span data-ttu-id="a8503-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a8503-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a8503-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8503-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8503-176">version</span><span class="sxs-lookup"><span data-stu-id="a8503-176">version</span></span>|<span data-ttu-id="a8503-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a8503-177">Int32</span></span>|<span data-ttu-id="a8503-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a8503-178">Version of the device configuration.</span></span> <span data-ttu-id="a8503-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8503-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8503-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a8503-180">usernameSource</span></span>|[<span data-ttu-id="a8503-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="a8503-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a8503-182">在设备上安装之前从 AAD 中选取并注入到此配置文件中的用户名属性。</span><span class="sxs-lookup"><span data-stu-id="a8503-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a8503-183">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="a8503-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a8503-184">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="a8503-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a8503-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="a8503-185">usernameAADSource</span></span>|[<span data-ttu-id="a8503-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a8503-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="a8503-187">AAD 字段的名称，该字段将用于检索电子邮件配置文件的 UserName。</span><span class="sxs-lookup"><span data-stu-id="a8503-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="a8503-188">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="a8503-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a8503-189">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="a8503-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="a8503-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="a8503-190">userDomainNameSource</span></span>|[<span data-ttu-id="a8503-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="a8503-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="a8503-192">UserDomainname 属性，在设备上安装之前从 AAD 中选取并注入到此配置文件中。</span><span class="sxs-lookup"><span data-stu-id="a8503-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a8503-193">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="a8503-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a8503-194">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="a8503-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="a8503-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="a8503-195">customDomainName</span></span>|<span data-ttu-id="a8503-196">String</span><span class="sxs-lookup"><span data-stu-id="a8503-196">String</span></span>|<span data-ttu-id="a8503-197">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="a8503-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="a8503-198">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="a8503-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="a8503-199">accountName</span><span class="sxs-lookup"><span data-stu-id="a8503-199">accountName</span></span>|<span data-ttu-id="a8503-200">String</span><span class="sxs-lookup"><span data-stu-id="a8503-200">String</span></span>|<span data-ttu-id="a8503-201">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="a8503-201">Account name.</span></span>|
|<span data-ttu-id="a8503-202">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a8503-202">authenticationMethod</span></span>|[<span data-ttu-id="a8503-203">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a8503-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="a8503-204">此电子邮件配置文件的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="a8503-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="a8503-205">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="a8503-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a8503-206">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="a8503-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="a8503-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-207">Boolean</span></span>|<span data-ttu-id="a8503-208">指示是否阻止将邮件移动到其他电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="a8503-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="a8503-209">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="a8503-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="a8503-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-210">Boolean</span></span>|<span data-ttu-id="a8503-211">指示是否阻止从第三方应用发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="a8503-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="a8503-212">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="a8503-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="a8503-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-213">Boolean</span></span>|<span data-ttu-id="a8503-214">指示是否阻止同步最近使用的电子邮件地址，例如 - 撰写新电子邮件时。</span><span class="sxs-lookup"><span data-stu-id="a8503-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="a8503-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="a8503-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="a8503-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="a8503-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="a8503-217">电子邮件应同步回的持续时间。</span><span class="sxs-lookup"><span data-stu-id="a8503-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="a8503-218">.</span><span class="sxs-lookup"><span data-stu-id="a8503-218">.</span></span> <span data-ttu-id="a8503-219">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="a8503-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="a8503-220">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="a8503-220">emailAddressSource</span></span>|[<span data-ttu-id="a8503-221">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="a8503-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a8503-222">从 AAD 中选取并注入到此配置文件中的电子邮件属性，在设备上安装之前。</span><span class="sxs-lookup"><span data-stu-id="a8503-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a8503-223">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="a8503-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a8503-224">easServices</span><span class="sxs-lookup"><span data-stu-id="a8503-224">easServices</span></span>|[<span data-ttu-id="a8503-225">easServices</span><span class="sxs-lookup"><span data-stu-id="a8503-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="a8503-226">要同步的 Exchange 数据。可能的值是 `none` `calendars` `contacts` ：、、、、、。 `email` `notes` `reminders`</span><span class="sxs-lookup"><span data-stu-id="a8503-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="a8503-227">easServicesUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a8503-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="a8503-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-228">Boolean</span></span>|<span data-ttu-id="a8503-229">允许用户更改同步设置。</span><span class="sxs-lookup"><span data-stu-id="a8503-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="a8503-230">hostName</span><span class="sxs-lookup"><span data-stu-id="a8503-230">hostName</span></span>|<span data-ttu-id="a8503-231">String</span><span class="sxs-lookup"><span data-stu-id="a8503-231">String</span></span>|<span data-ttu-id="a8503-232">使用本机 (连接到) URL 的 Exchange 位置。</span><span class="sxs-lookup"><span data-stu-id="a8503-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="a8503-233">requireSmime</span><span class="sxs-lookup"><span data-stu-id="a8503-233">requireSmime</span></span>|<span data-ttu-id="a8503-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-234">Boolean</span></span>|<span data-ttu-id="a8503-235">指示是否使用 S/MIME 证书。</span><span class="sxs-lookup"><span data-stu-id="a8503-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="a8503-236">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="a8503-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="a8503-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-237">Boolean</span></span>|<span data-ttu-id="a8503-238">指示是否允许未加密的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="a8503-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="a8503-239">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="a8503-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="a8503-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-240">Boolean</span></span>|<span data-ttu-id="a8503-241">如果设置为 true，则默认启用 S/MIME 加密。</span><span class="sxs-lookup"><span data-stu-id="a8503-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="a8503-242">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="a8503-242">smimeSigningEnabled</span></span>|<span data-ttu-id="a8503-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-243">Boolean</span></span>|<span data-ttu-id="a8503-244">如果设置为 true，则为此帐户启用 S/MIME 签名</span><span class="sxs-lookup"><span data-stu-id="a8503-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="a8503-245">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a8503-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="a8503-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-246">Boolean</span></span>|<span data-ttu-id="a8503-247">如果设置为 true，用户可以打开或关闭 S/MIME 签名。</span><span class="sxs-lookup"><span data-stu-id="a8503-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="a8503-248">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a8503-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="a8503-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-249">Boolean</span></span>|<span data-ttu-id="a8503-250">如果设置为 true，用户可以默认切换加密设置。</span><span class="sxs-lookup"><span data-stu-id="a8503-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="a8503-251">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a8503-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="a8503-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-252">Boolean</span></span>|<span data-ttu-id="a8503-253">如果设置为 true，则用户可以选择签名标识。</span><span class="sxs-lookup"><span data-stu-id="a8503-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="a8503-254">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a8503-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="a8503-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-255">Boolean</span></span>|<span data-ttu-id="a8503-256">如果设置为 true，则用户可以选择 S/MIME 加密标识。</span><span class="sxs-lookup"><span data-stu-id="a8503-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="a8503-257">requireSsl</span><span class="sxs-lookup"><span data-stu-id="a8503-257">requireSsl</span></span>|<span data-ttu-id="a8503-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-258">Boolean</span></span>|<span data-ttu-id="a8503-259">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="a8503-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="a8503-260">useOAuth</span><span class="sxs-lookup"><span data-stu-id="a8503-260">useOAuth</span></span>|<span data-ttu-id="a8503-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8503-261">Boolean</span></span>|<span data-ttu-id="a8503-262">指定连接是否应该使用 OAuth 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="a8503-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="a8503-263">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="a8503-263">signingCertificateType</span></span>|[<span data-ttu-id="a8503-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="a8503-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="a8503-265">签署此电子邮件配置文件的证书类型。</span><span class="sxs-lookup"><span data-stu-id="a8503-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="a8503-266">可取值为：`none`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="a8503-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a8503-267">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="a8503-267">encryptionCertificateType</span></span>|[<span data-ttu-id="a8503-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="a8503-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="a8503-269">加密 此电子邮件配置文件的证书类型。</span><span class="sxs-lookup"><span data-stu-id="a8503-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="a8503-270">可取值为：`none`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="a8503-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a8503-271">perAppVPNProfileId</span><span class="sxs-lookup"><span data-stu-id="a8503-271">perAppVPNProfileId</span></span>|<span data-ttu-id="a8503-272">String</span><span class="sxs-lookup"><span data-stu-id="a8503-272">String</span></span>|<span data-ttu-id="a8503-273">用于从本机Per-App客户端访问电子邮件的邮箱 VPN 策略的配置文件 ID</span><span class="sxs-lookup"><span data-stu-id="a8503-273">Profile ID of the Per-App VPN policy to be used to access emails from the native Mail client</span></span>|



## <a name="response"></a><span data-ttu-id="a8503-274">响应</span><span class="sxs-lookup"><span data-stu-id="a8503-274">Response</span></span>
<span data-ttu-id="a8503-275">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a8503-275">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8503-276">示例</span><span class="sxs-lookup"><span data-stu-id="a8503-276">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8503-277">请求</span><span class="sxs-lookup"><span data-stu-id="a8503-277">Request</span></span>
<span data-ttu-id="a8503-278">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8503-278">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="a8503-279">响应</span><span class="sxs-lookup"><span data-stu-id="a8503-279">Response</span></span>
<span data-ttu-id="a8503-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a8503-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




