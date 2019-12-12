---
title: 创建 iosEasEmailProfileConfiguration
description: 创建新的 iosEasEmailProfileConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26d62ae6ee81b69121dd0cd5d76b110a26347cd3
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949031"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="e7dab-103">创建 iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="e7dab-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="e7dab-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e7dab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7dab-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e7dab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7dab-106">创建新的[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e7dab-106">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7dab-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e7dab-107">Prerequisites</span></span>
<span data-ttu-id="e7dab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7dab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7dab-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7dab-110">Permission type</span></span>|<span data-ttu-id="e7dab-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e7dab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7dab-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7dab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7dab-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7dab-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7dab-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7dab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7dab-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7dab-115">Not supported.</span></span>|
|<span data-ttu-id="e7dab-116">Application</span><span class="sxs-lookup"><span data-stu-id="e7dab-116">Application</span></span>|<span data-ttu-id="e7dab-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7dab-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7dab-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7dab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e7dab-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7dab-119">Request headers</span></span>
|<span data-ttu-id="e7dab-120">标头</span><span class="sxs-lookup"><span data-stu-id="e7dab-120">Header</span></span>|<span data-ttu-id="e7dab-121">值</span><span class="sxs-lookup"><span data-stu-id="e7dab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7dab-122">授权</span><span class="sxs-lookup"><span data-stu-id="e7dab-122">Authorization</span></span>|<span data-ttu-id="e7dab-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e7dab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7dab-124">接受</span><span class="sxs-lookup"><span data-stu-id="e7dab-124">Accept</span></span>|<span data-ttu-id="e7dab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7dab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7dab-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7dab-126">Request body</span></span>
<span data-ttu-id="e7dab-127">在请求正文中，提供 iosEasEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7dab-127">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="e7dab-128">下表显示创建 iosEasEmailProfileConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e7dab-128">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="e7dab-129">属性</span><span class="sxs-lookup"><span data-stu-id="e7dab-129">Property</span></span>|<span data-ttu-id="e7dab-130">类型</span><span class="sxs-lookup"><span data-stu-id="e7dab-130">Type</span></span>|<span data-ttu-id="e7dab-131">说明</span><span class="sxs-lookup"><span data-stu-id="e7dab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7dab-132">id</span><span class="sxs-lookup"><span data-stu-id="e7dab-132">id</span></span>|<span data-ttu-id="e7dab-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e7dab-133">String</span></span>|<span data-ttu-id="e7dab-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e7dab-134">Key of the entity.</span></span> <span data-ttu-id="e7dab-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7dab-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7dab-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7dab-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e7dab-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7dab-137">DateTimeOffset</span></span>|<span data-ttu-id="e7dab-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e7dab-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e7dab-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7dab-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7dab-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e7dab-140">roleScopeTagIds</span></span>|<span data-ttu-id="e7dab-141">String collection</span><span class="sxs-lookup"><span data-stu-id="e7dab-141">String collection</span></span>|<span data-ttu-id="e7dab-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e7dab-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e7dab-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7dab-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7dab-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e7dab-144">supportsScopeTags</span></span>|<span data-ttu-id="e7dab-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-145">Boolean</span></span>|<span data-ttu-id="e7dab-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="e7dab-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e7dab-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="e7dab-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e7dab-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="e7dab-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e7dab-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e7dab-149">This property is read-only.</span></span> <span data-ttu-id="e7dab-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7dab-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7dab-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e7dab-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e7dab-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e7dab-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e7dab-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="e7dab-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e7dab-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7dab-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7dab-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e7dab-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e7dab-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e7dab-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e7dab-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e7dab-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e7dab-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7dab-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7dab-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e7dab-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e7dab-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e7dab-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e7dab-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e7dab-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e7dab-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7dab-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7dab-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7dab-163">createdDateTime</span></span>|<span data-ttu-id="e7dab-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7dab-164">DateTimeOffset</span></span>|<span data-ttu-id="e7dab-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e7dab-165">DateTime the object was created.</span></span> <span data-ttu-id="e7dab-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7dab-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7dab-167">说明</span><span class="sxs-lookup"><span data-stu-id="e7dab-167">description</span></span>|<span data-ttu-id="e7dab-168">String</span><span class="sxs-lookup"><span data-stu-id="e7dab-168">String</span></span>|<span data-ttu-id="e7dab-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e7dab-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e7dab-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7dab-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7dab-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e7dab-171">displayName</span></span>|<span data-ttu-id="e7dab-172">String</span><span class="sxs-lookup"><span data-stu-id="e7dab-172">String</span></span>|<span data-ttu-id="e7dab-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e7dab-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e7dab-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7dab-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7dab-175">version</span><span class="sxs-lookup"><span data-stu-id="e7dab-175">version</span></span>|<span data-ttu-id="e7dab-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e7dab-176">Int32</span></span>|<span data-ttu-id="e7dab-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e7dab-177">Version of the device configuration.</span></span> <span data-ttu-id="e7dab-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7dab-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7dab-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="e7dab-179">usernameSource</span></span>|[<span data-ttu-id="e7dab-180">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="e7dab-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="e7dab-181">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="e7dab-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e7dab-182">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="e7dab-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e7dab-183">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="e7dab-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="e7dab-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="e7dab-184">usernameAADSource</span></span>|[<span data-ttu-id="e7dab-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="e7dab-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="e7dab-186">AAD 字段的名称，将用于检索电子邮件配置文件的用户名。</span><span class="sxs-lookup"><span data-stu-id="e7dab-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="e7dab-187">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="e7dab-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e7dab-188">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="e7dab-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="e7dab-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="e7dab-189">userDomainNameSource</span></span>|[<span data-ttu-id="e7dab-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="e7dab-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="e7dab-191">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="e7dab-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e7dab-192">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="e7dab-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e7dab-193">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="e7dab-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="e7dab-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="e7dab-194">customDomainName</span></span>|<span data-ttu-id="e7dab-195">字符串</span><span class="sxs-lookup"><span data-stu-id="e7dab-195">String</span></span>|<span data-ttu-id="e7dab-196">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="e7dab-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="e7dab-197">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="e7dab-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="e7dab-198">帐户</span><span class="sxs-lookup"><span data-stu-id="e7dab-198">accountName</span></span>|<span data-ttu-id="e7dab-199">字符串</span><span class="sxs-lookup"><span data-stu-id="e7dab-199">String</span></span>|<span data-ttu-id="e7dab-200">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="e7dab-200">Account name.</span></span>|
|<span data-ttu-id="e7dab-201">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e7dab-201">authenticationMethod</span></span>|[<span data-ttu-id="e7dab-202">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e7dab-202">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="e7dab-203">此电子邮件配置文件的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="e7dab-203">Authentication method for this Email profile.</span></span> <span data-ttu-id="e7dab-204">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="e7dab-204">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e7dab-205">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="e7dab-205">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="e7dab-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-206">Boolean</span></span>|<span data-ttu-id="e7dab-207">指示是否阻止将邮件移动到其他电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="e7dab-207">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="e7dab-208">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="e7dab-208">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="e7dab-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-209">Boolean</span></span>|<span data-ttu-id="e7dab-210">指示是否阻止来自第三方应用的发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="e7dab-210">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="e7dab-211">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="e7dab-211">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="e7dab-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-212">Boolean</span></span>|<span data-ttu-id="e7dab-213">指示是否阻止同步最近使用的电子邮件地址，例如，撰写新电子邮件时。</span><span class="sxs-lookup"><span data-stu-id="e7dab-213">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="e7dab-214">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="e7dab-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="e7dab-215">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="e7dab-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="e7dab-216">电子邮件的持续时间应同步回。</span><span class="sxs-lookup"><span data-stu-id="e7dab-216">Duration of time email should be synced back to.</span></span> <span data-ttu-id="e7dab-217">.</span><span class="sxs-lookup"><span data-stu-id="e7dab-217"></span></span> <span data-ttu-id="e7dab-218">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="e7dab-218">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="e7dab-219">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="e7dab-219">emailAddressSource</span></span>|[<span data-ttu-id="e7dab-220">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="e7dab-220">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="e7dab-221">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="e7dab-221">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e7dab-222">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="e7dab-222">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="e7dab-223">easServices</span><span class="sxs-lookup"><span data-stu-id="e7dab-223">easServices</span></span>|[<span data-ttu-id="e7dab-224">easServices</span><span class="sxs-lookup"><span data-stu-id="e7dab-224">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="e7dab-225">要同步的 Exchange 数据。可能的值为`none`： `calendars`、 `contacts`、 `email`、 `notes`、 `reminders`、。</span><span class="sxs-lookup"><span data-stu-id="e7dab-225">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="e7dab-226">easServicesUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="e7dab-226">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="e7dab-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-227">Boolean</span></span>|<span data-ttu-id="e7dab-228">允许用户更改同步设置。</span><span class="sxs-lookup"><span data-stu-id="e7dab-228">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="e7dab-229">hostName</span><span class="sxs-lookup"><span data-stu-id="e7dab-229">hostName</span></span>|<span data-ttu-id="e7dab-230">String</span><span class="sxs-lookup"><span data-stu-id="e7dab-230">String</span></span>|<span data-ttu-id="e7dab-231">本机邮件应用程序连接到的 Exchange 位置（URL）。</span><span class="sxs-lookup"><span data-stu-id="e7dab-231">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="e7dab-232">requireSmime</span><span class="sxs-lookup"><span data-stu-id="e7dab-232">requireSmime</span></span>|<span data-ttu-id="e7dab-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-233">Boolean</span></span>|<span data-ttu-id="e7dab-234">指示是否使用 S/MIME 证书。</span><span class="sxs-lookup"><span data-stu-id="e7dab-234">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="e7dab-235">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="e7dab-235">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="e7dab-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-236">Boolean</span></span>|<span data-ttu-id="e7dab-237">指示是否允许未加密的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="e7dab-237">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="e7dab-238">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="e7dab-238">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="e7dab-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-239">Boolean</span></span>|<span data-ttu-id="e7dab-240">如果设置为 "true S/MIME 加密"，则默认为启用。</span><span class="sxs-lookup"><span data-stu-id="e7dab-240">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="e7dab-241">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="e7dab-241">smimeSigningEnabled</span></span>|<span data-ttu-id="e7dab-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-242">Boolean</span></span>|<span data-ttu-id="e7dab-243">如果为此帐户启用了设置为 true S/MIME 签名</span><span class="sxs-lookup"><span data-stu-id="e7dab-243">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="e7dab-244">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="e7dab-244">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="e7dab-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-245">Boolean</span></span>|<span data-ttu-id="e7dab-246">如果设置为 true，则用户可以打开或关闭 S/MIME 签名。</span><span class="sxs-lookup"><span data-stu-id="e7dab-246">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="e7dab-247">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="e7dab-247">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="e7dab-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-248">Boolean</span></span>|<span data-ttu-id="e7dab-249">如果设置为 true，则用户可以默认切换加密设置。</span><span class="sxs-lookup"><span data-stu-id="e7dab-249">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="e7dab-250">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="e7dab-250">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="e7dab-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-251">Boolean</span></span>|<span data-ttu-id="e7dab-252">如果设置为 true，则用户可以选择签名标识。</span><span class="sxs-lookup"><span data-stu-id="e7dab-252">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="e7dab-253">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="e7dab-253">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="e7dab-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-254">Boolean</span></span>|<span data-ttu-id="e7dab-255">如果设置为 true，则用户可以选择 S/MIME 加密标识。</span><span class="sxs-lookup"><span data-stu-id="e7dab-255">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="e7dab-256">requireSsl</span><span class="sxs-lookup"><span data-stu-id="e7dab-256">requireSsl</span></span>|<span data-ttu-id="e7dab-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-257">Boolean</span></span>|<span data-ttu-id="e7dab-258">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="e7dab-258">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="e7dab-259">useOAuth</span><span class="sxs-lookup"><span data-stu-id="e7dab-259">useOAuth</span></span>|<span data-ttu-id="e7dab-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7dab-260">Boolean</span></span>|<span data-ttu-id="e7dab-261">指定连接是否应使用 OAuth 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e7dab-261">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="e7dab-262">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="e7dab-262">signingCertificateType</span></span>|[<span data-ttu-id="e7dab-263">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="e7dab-263">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="e7dab-264">此电子邮件配置文件的签名证书类型。</span><span class="sxs-lookup"><span data-stu-id="e7dab-264">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="e7dab-265">可取值为：`none`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="e7dab-265">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e7dab-266">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="e7dab-266">encryptionCertificateType</span></span>|[<span data-ttu-id="e7dab-267">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="e7dab-267">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="e7dab-268">此电子邮件配置文件的加密证书类型。</span><span class="sxs-lookup"><span data-stu-id="e7dab-268">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="e7dab-269">可取值为：`none`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="e7dab-269">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="e7dab-270">响应</span><span class="sxs-lookup"><span data-stu-id="e7dab-270">Response</span></span>
<span data-ttu-id="e7dab-271">如果成功，此方法在响应`201 Created`正文中返回响应代码和[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e7dab-271">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7dab-272">示例</span><span class="sxs-lookup"><span data-stu-id="e7dab-272">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7dab-273">请求</span><span class="sxs-lookup"><span data-stu-id="e7dab-273">Request</span></span>
<span data-ttu-id="e7dab-274">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7dab-274">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2131

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
  "encryptionCertificateType": "certificate"
}
```

### <a name="response"></a><span data-ttu-id="e7dab-275">响应</span><span class="sxs-lookup"><span data-stu-id="e7dab-275">Response</span></span>
<span data-ttu-id="e7dab-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e7dab-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2303

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
  "encryptionCertificateType": "certificate"
}
```





