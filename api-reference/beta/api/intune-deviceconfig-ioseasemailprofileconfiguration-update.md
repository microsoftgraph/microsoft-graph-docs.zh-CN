---
title: 更新 iosEasEmailProfileConfiguration
description: 更新 iosEasEmailProfileConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ab410bc3fc5df4bd595287e35c633458617eab30
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448968"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="50188-103">更新 iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="50188-103">Update iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="50188-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="50188-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50188-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="50188-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50188-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="50188-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50188-107">更新[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="50188-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50188-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="50188-108">Prerequisites</span></span>
<span data-ttu-id="50188-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50188-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50188-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="50188-111">Permission type</span></span>|<span data-ttu-id="50188-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="50188-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50188-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50188-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50188-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50188-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50188-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50188-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50188-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="50188-116">Not supported.</span></span>|
|<span data-ttu-id="50188-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="50188-117">Application</span></span>|<span data-ttu-id="50188-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50188-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50188-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50188-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="50188-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="50188-120">Request headers</span></span>
|<span data-ttu-id="50188-121">标头</span><span class="sxs-lookup"><span data-stu-id="50188-121">Header</span></span>|<span data-ttu-id="50188-122">值</span><span class="sxs-lookup"><span data-stu-id="50188-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50188-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50188-123">Authorization</span></span>|<span data-ttu-id="50188-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="50188-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50188-125">接受</span><span class="sxs-lookup"><span data-stu-id="50188-125">Accept</span></span>|<span data-ttu-id="50188-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50188-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50188-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="50188-127">Request body</span></span>
<span data-ttu-id="50188-128">在请求正文中，提供[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50188-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="50188-129">下表显示创建[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="50188-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="50188-130">属性</span><span class="sxs-lookup"><span data-stu-id="50188-130">Property</span></span>|<span data-ttu-id="50188-131">类型</span><span class="sxs-lookup"><span data-stu-id="50188-131">Type</span></span>|<span data-ttu-id="50188-132">说明</span><span class="sxs-lookup"><span data-stu-id="50188-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50188-133">id</span><span class="sxs-lookup"><span data-stu-id="50188-133">id</span></span>|<span data-ttu-id="50188-134">字符串</span><span class="sxs-lookup"><span data-stu-id="50188-134">String</span></span>|<span data-ttu-id="50188-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="50188-135">Key of the entity.</span></span> <span data-ttu-id="50188-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50188-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50188-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50188-137">lastModifiedDateTime</span></span>|<span data-ttu-id="50188-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50188-138">DateTimeOffset</span></span>|<span data-ttu-id="50188-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="50188-139">DateTime the object was last modified.</span></span> <span data-ttu-id="50188-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50188-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50188-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50188-141">roleScopeTagIds</span></span>|<span data-ttu-id="50188-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="50188-142">String collection</span></span>|<span data-ttu-id="50188-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="50188-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="50188-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50188-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50188-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="50188-145">supportsScopeTags</span></span>|<span data-ttu-id="50188-146">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-146">Boolean</span></span>|<span data-ttu-id="50188-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="50188-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="50188-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="50188-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="50188-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="50188-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="50188-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="50188-150">This property is read-only.</span></span> <span data-ttu-id="50188-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50188-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50188-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="50188-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="50188-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="50188-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="50188-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="50188-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="50188-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50188-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50188-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="50188-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="50188-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="50188-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="50188-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="50188-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="50188-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50188-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50188-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="50188-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="50188-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="50188-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="50188-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="50188-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="50188-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50188-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50188-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50188-164">createdDateTime</span></span>|<span data-ttu-id="50188-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50188-165">DateTimeOffset</span></span>|<span data-ttu-id="50188-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="50188-166">DateTime the object was created.</span></span> <span data-ttu-id="50188-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50188-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50188-168">说明</span><span class="sxs-lookup"><span data-stu-id="50188-168">description</span></span>|<span data-ttu-id="50188-169">String</span><span class="sxs-lookup"><span data-stu-id="50188-169">String</span></span>|<span data-ttu-id="50188-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="50188-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="50188-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50188-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50188-172">displayName</span><span class="sxs-lookup"><span data-stu-id="50188-172">displayName</span></span>|<span data-ttu-id="50188-173">String</span><span class="sxs-lookup"><span data-stu-id="50188-173">String</span></span>|<span data-ttu-id="50188-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="50188-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="50188-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50188-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50188-176">version</span><span class="sxs-lookup"><span data-stu-id="50188-176">version</span></span>|<span data-ttu-id="50188-177">Int32</span><span class="sxs-lookup"><span data-stu-id="50188-177">Int32</span></span>|<span data-ttu-id="50188-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="50188-178">Version of the device configuration.</span></span> <span data-ttu-id="50188-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50188-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50188-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="50188-180">usernameSource</span></span>|[<span data-ttu-id="50188-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="50188-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="50188-182">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="50188-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="50188-183">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="50188-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="50188-184">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="50188-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="50188-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="50188-185">usernameAADSource</span></span>|[<span data-ttu-id="50188-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="50188-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="50188-187">AAD 字段的名称，将用于检索电子邮件配置文件的用户名。</span><span class="sxs-lookup"><span data-stu-id="50188-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="50188-188">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="50188-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="50188-189">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="50188-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="50188-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="50188-190">userDomainNameSource</span></span>|[<span data-ttu-id="50188-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="50188-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="50188-192">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="50188-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="50188-193">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="50188-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="50188-194">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="50188-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="50188-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="50188-195">customDomainName</span></span>|<span data-ttu-id="50188-196">String</span><span class="sxs-lookup"><span data-stu-id="50188-196">String</span></span>|<span data-ttu-id="50188-197">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="50188-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="50188-198">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="50188-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="50188-199">帐户</span><span class="sxs-lookup"><span data-stu-id="50188-199">accountName</span></span>|<span data-ttu-id="50188-200">String</span><span class="sxs-lookup"><span data-stu-id="50188-200">String</span></span>|<span data-ttu-id="50188-201">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="50188-201">Account name.</span></span>|
|<span data-ttu-id="50188-202">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="50188-202">authenticationMethod</span></span>|[<span data-ttu-id="50188-203">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="50188-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="50188-204">此电子邮件配置文件的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="50188-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="50188-205">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="50188-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="50188-206">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="50188-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="50188-207">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-207">Boolean</span></span>|<span data-ttu-id="50188-208">指示是否阻止将邮件移动到其他电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="50188-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="50188-209">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="50188-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="50188-210">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-210">Boolean</span></span>|<span data-ttu-id="50188-211">指示是否阻止来自第三方应用的发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="50188-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="50188-212">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="50188-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="50188-213">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-213">Boolean</span></span>|<span data-ttu-id="50188-214">指示是否阻止同步最近使用的电子邮件地址，例如，撰写新电子邮件时。</span><span class="sxs-lookup"><span data-stu-id="50188-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="50188-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="50188-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="50188-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="50188-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="50188-217">电子邮件的持续时间应同步回。</span><span class="sxs-lookup"><span data-stu-id="50188-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="50188-218">.</span><span class="sxs-lookup"><span data-stu-id="50188-218">.</span></span> <span data-ttu-id="50188-219">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="50188-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="50188-220">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="50188-220">emailAddressSource</span></span>|[<span data-ttu-id="50188-221">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="50188-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="50188-222">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="50188-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="50188-223">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="50188-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="50188-224">easServices</span><span class="sxs-lookup"><span data-stu-id="50188-224">easServices</span></span>|[<span data-ttu-id="50188-225">easServices</span><span class="sxs-lookup"><span data-stu-id="50188-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="50188-226">要同步的 Exchange 数据。可能的值为`none`： `calendars`、 `contacts`、 `email`、 `notes`、 `reminders`、。</span><span class="sxs-lookup"><span data-stu-id="50188-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="50188-227">easServicesUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="50188-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="50188-228">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-228">Boolean</span></span>|<span data-ttu-id="50188-229">允许用户更改同步设置。</span><span class="sxs-lookup"><span data-stu-id="50188-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="50188-230">hostName</span><span class="sxs-lookup"><span data-stu-id="50188-230">hostName</span></span>|<span data-ttu-id="50188-231">String</span><span class="sxs-lookup"><span data-stu-id="50188-231">String</span></span>|<span data-ttu-id="50188-232">本机邮件应用程序连接到的 Exchange 位置（URL）。</span><span class="sxs-lookup"><span data-stu-id="50188-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="50188-233">requireSmime</span><span class="sxs-lookup"><span data-stu-id="50188-233">requireSmime</span></span>|<span data-ttu-id="50188-234">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-234">Boolean</span></span>|<span data-ttu-id="50188-235">指示是否使用 S/MIME 证书。</span><span class="sxs-lookup"><span data-stu-id="50188-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="50188-236">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="50188-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="50188-237">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-237">Boolean</span></span>|<span data-ttu-id="50188-238">指示是否允许未加密的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="50188-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="50188-239">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="50188-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="50188-240">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-240">Boolean</span></span>|<span data-ttu-id="50188-241">如果设置为 "true S/MIME 加密"，则默认为启用。</span><span class="sxs-lookup"><span data-stu-id="50188-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="50188-242">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="50188-242">smimeSigningEnabled</span></span>|<span data-ttu-id="50188-243">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-243">Boolean</span></span>|<span data-ttu-id="50188-244">如果为此帐户启用了设置为 true S/MIME 签名</span><span class="sxs-lookup"><span data-stu-id="50188-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="50188-245">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="50188-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="50188-246">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-246">Boolean</span></span>|<span data-ttu-id="50188-247">如果设置为 true，则用户可以打开或关闭 S/MIME 签名。</span><span class="sxs-lookup"><span data-stu-id="50188-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="50188-248">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="50188-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="50188-249">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-249">Boolean</span></span>|<span data-ttu-id="50188-250">如果设置为 true，则用户可以默认切换加密设置。</span><span class="sxs-lookup"><span data-stu-id="50188-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="50188-251">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="50188-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="50188-252">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-252">Boolean</span></span>|<span data-ttu-id="50188-253">如果设置为 true，则用户可以选择签名标识。</span><span class="sxs-lookup"><span data-stu-id="50188-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="50188-254">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="50188-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="50188-255">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-255">Boolean</span></span>|<span data-ttu-id="50188-256">如果设置为 true，则用户可以选择 S/MIME 加密标识。</span><span class="sxs-lookup"><span data-stu-id="50188-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="50188-257">requireSsl</span><span class="sxs-lookup"><span data-stu-id="50188-257">requireSsl</span></span>|<span data-ttu-id="50188-258">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-258">Boolean</span></span>|<span data-ttu-id="50188-259">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="50188-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="50188-260">useOAuth</span><span class="sxs-lookup"><span data-stu-id="50188-260">useOAuth</span></span>|<span data-ttu-id="50188-261">布尔</span><span class="sxs-lookup"><span data-stu-id="50188-261">Boolean</span></span>|<span data-ttu-id="50188-262">指定连接是否应使用 OAuth 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="50188-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="50188-263">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="50188-263">signingCertificateType</span></span>|[<span data-ttu-id="50188-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="50188-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="50188-265">此电子邮件配置文件的签名证书类型。</span><span class="sxs-lookup"><span data-stu-id="50188-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="50188-266">可取值为：`none`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="50188-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="50188-267">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="50188-267">encryptionCertificateType</span></span>|[<span data-ttu-id="50188-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="50188-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="50188-269">此电子邮件配置文件的加密证书类型。</span><span class="sxs-lookup"><span data-stu-id="50188-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="50188-270">可取值为：`none`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="50188-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="50188-271">响应</span><span class="sxs-lookup"><span data-stu-id="50188-271">Response</span></span>
<span data-ttu-id="50188-272">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="50188-272">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50188-273">示例</span><span class="sxs-lookup"><span data-stu-id="50188-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="50188-274">请求</span><span class="sxs-lookup"><span data-stu-id="50188-274">Request</span></span>
<span data-ttu-id="50188-275">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50188-275">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="50188-276">响应</span><span class="sxs-lookup"><span data-stu-id="50188-276">Response</span></span>
<span data-ttu-id="50188-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50188-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





