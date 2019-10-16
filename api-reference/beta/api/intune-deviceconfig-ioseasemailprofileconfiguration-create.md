---
title: 创建 iosEasEmailProfileConfiguration
description: 创建新的 iosEasEmailProfileConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9e5802363997edd7f5cfb16efd444dc5a5bd95b0
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533894"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="0b6d9-103">创建 iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b6d9-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="0b6d9-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b6d9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b6d9-106">创建新的[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-106">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b6d9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b6d9-107">Prerequisites</span></span>
<span data-ttu-id="0b6d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b6d9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b6d9-110">Permission type</span></span>|<span data-ttu-id="0b6d9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0b6d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b6d9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b6d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b6d9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b6d9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b6d9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b6d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b6d9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-115">Not supported.</span></span>|
|<span data-ttu-id="0b6d9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b6d9-116">Application</span></span>|<span data-ttu-id="0b6d9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b6d9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b6d9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b6d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0b6d9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b6d9-119">Request headers</span></span>
|<span data-ttu-id="0b6d9-120">标头</span><span class="sxs-lookup"><span data-stu-id="0b6d9-120">Header</span></span>|<span data-ttu-id="0b6d9-121">值</span><span class="sxs-lookup"><span data-stu-id="0b6d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b6d9-122">授权</span><span class="sxs-lookup"><span data-stu-id="0b6d9-122">Authorization</span></span>|<span data-ttu-id="0b6d9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b6d9-124">接受</span><span class="sxs-lookup"><span data-stu-id="0b6d9-124">Accept</span></span>|<span data-ttu-id="0b6d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b6d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b6d9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b6d9-126">Request body</span></span>
<span data-ttu-id="0b6d9-127">在请求正文中，提供 iosEasEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-127">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="0b6d9-128">下表显示创建 iosEasEmailProfileConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-128">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="0b6d9-129">属性</span><span class="sxs-lookup"><span data-stu-id="0b6d9-129">Property</span></span>|<span data-ttu-id="0b6d9-130">类型</span><span class="sxs-lookup"><span data-stu-id="0b6d9-130">Type</span></span>|<span data-ttu-id="0b6d9-131">说明</span><span class="sxs-lookup"><span data-stu-id="0b6d9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b6d9-132">id</span><span class="sxs-lookup"><span data-stu-id="0b6d9-132">id</span></span>|<span data-ttu-id="0b6d9-133">字符串</span><span class="sxs-lookup"><span data-stu-id="0b6d9-133">String</span></span>|<span data-ttu-id="0b6d9-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-134">Key of the entity.</span></span> <span data-ttu-id="0b6d9-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b6d9-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b6d9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b6d9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0b6d9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b6d9-137">DateTimeOffset</span></span>|<span data-ttu-id="0b6d9-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0b6d9-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b6d9-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b6d9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0b6d9-140">roleScopeTagIds</span></span>|<span data-ttu-id="0b6d9-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="0b6d9-141">String collection</span></span>|<span data-ttu-id="0b6d9-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0b6d9-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b6d9-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b6d9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0b6d9-144">supportsScopeTags</span></span>|<span data-ttu-id="0b6d9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6d9-145">Boolean</span></span>|<span data-ttu-id="0b6d9-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0b6d9-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0b6d9-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0b6d9-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-149">This property is read-only.</span></span> <span data-ttu-id="0b6d9-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b6d9-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b6d9-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0b6d9-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0b6d9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0b6d9-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0b6d9-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0b6d9-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b6d9-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b6d9-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0b6d9-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0b6d9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0b6d9-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0b6d9-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0b6d9-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b6d9-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b6d9-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0b6d9-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0b6d9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0b6d9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0b6d9-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0b6d9-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b6d9-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b6d9-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b6d9-163">createdDateTime</span></span>|<span data-ttu-id="0b6d9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b6d9-164">DateTimeOffset</span></span>|<span data-ttu-id="0b6d9-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-165">DateTime the object was created.</span></span> <span data-ttu-id="0b6d9-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b6d9-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b6d9-167">说明</span><span class="sxs-lookup"><span data-stu-id="0b6d9-167">description</span></span>|<span data-ttu-id="0b6d9-168">String</span><span class="sxs-lookup"><span data-stu-id="0b6d9-168">String</span></span>|<span data-ttu-id="0b6d9-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0b6d9-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b6d9-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b6d9-171">displayName</span><span class="sxs-lookup"><span data-stu-id="0b6d9-171">displayName</span></span>|<span data-ttu-id="0b6d9-172">String</span><span class="sxs-lookup"><span data-stu-id="0b6d9-172">String</span></span>|<span data-ttu-id="0b6d9-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0b6d9-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b6d9-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b6d9-175">version</span><span class="sxs-lookup"><span data-stu-id="0b6d9-175">version</span></span>|<span data-ttu-id="0b6d9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0b6d9-176">Int32</span></span>|<span data-ttu-id="0b6d9-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-177">Version of the device configuration.</span></span> <span data-ttu-id="0b6d9-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b6d9-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b6d9-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="0b6d9-179">usernameSource</span></span>|[<span data-ttu-id="0b6d9-180">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="0b6d9-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="0b6d9-181">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0b6d9-182">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="0b6d9-183">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0b6d9-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="0b6d9-184">usernameAADSource</span></span>|[<span data-ttu-id="0b6d9-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="0b6d9-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="0b6d9-186">AAD 字段的名称，将用于检索电子邮件配置文件的用户名。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="0b6d9-187">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="0b6d9-188">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="0b6d9-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="0b6d9-189">userDomainNameSource</span></span>|[<span data-ttu-id="0b6d9-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="0b6d9-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="0b6d9-191">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0b6d9-192">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="0b6d9-193">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="0b6d9-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="0b6d9-194">customDomainName</span></span>|<span data-ttu-id="0b6d9-195">字符串</span><span class="sxs-lookup"><span data-stu-id="0b6d9-195">String</span></span>|<span data-ttu-id="0b6d9-196">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="0b6d9-197">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="0b6d9-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="0b6d9-198">帐户</span><span class="sxs-lookup"><span data-stu-id="0b6d9-198">accountName</span></span>|<span data-ttu-id="0b6d9-199">字符串</span><span class="sxs-lookup"><span data-stu-id="0b6d9-199">String</span></span>|<span data-ttu-id="0b6d9-200">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-200">Account name.</span></span>|
|<span data-ttu-id="0b6d9-201">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0b6d9-201">authenticationMethod</span></span>|[<span data-ttu-id="0b6d9-202">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0b6d9-202">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="0b6d9-203">此电子邮件配置文件的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-203">Authentication method for this Email profile.</span></span> <span data-ttu-id="0b6d9-204">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-204">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="0b6d9-205">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="0b6d9-205">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="0b6d9-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6d9-206">Boolean</span></span>|<span data-ttu-id="0b6d9-207">指示是否阻止将邮件移动到其他电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-207">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="0b6d9-208">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="0b6d9-208">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="0b6d9-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6d9-209">Boolean</span></span>|<span data-ttu-id="0b6d9-210">指示是否阻止来自第三方应用的发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-210">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="0b6d9-211">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="0b6d9-211">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="0b6d9-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6d9-212">Boolean</span></span>|<span data-ttu-id="0b6d9-213">指示是否阻止同步最近使用的电子邮件地址，例如，撰写新电子邮件时。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-213">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="0b6d9-214">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="0b6d9-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="0b6d9-215">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="0b6d9-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="0b6d9-216">电子邮件的持续时间应同步回。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-216">Duration of time email should be synced back to.</span></span> <span data-ttu-id="0b6d9-217">.</span><span class="sxs-lookup"><span data-stu-id="0b6d9-217"></span></span> <span data-ttu-id="0b6d9-218">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-218">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="0b6d9-219">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="0b6d9-219">emailAddressSource</span></span>|[<span data-ttu-id="0b6d9-220">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="0b6d9-220">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="0b6d9-221">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-221">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0b6d9-222">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-222">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0b6d9-223">hostName</span><span class="sxs-lookup"><span data-stu-id="0b6d9-223">hostName</span></span>|<span data-ttu-id="0b6d9-224">String</span><span class="sxs-lookup"><span data-stu-id="0b6d9-224">String</span></span>|<span data-ttu-id="0b6d9-225">本机邮件应用程序连接到的 Exchange 位置（URL）。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-225">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="0b6d9-226">requireSmime</span><span class="sxs-lookup"><span data-stu-id="0b6d9-226">requireSmime</span></span>|<span data-ttu-id="0b6d9-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6d9-227">Boolean</span></span>|<span data-ttu-id="0b6d9-228">指示是否使用 S/MIME 证书。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-228">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="0b6d9-229">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="0b6d9-229">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="0b6d9-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6d9-230">Boolean</span></span>|<span data-ttu-id="0b6d9-231">指示是否允许未加密的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-231">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="0b6d9-232">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="0b6d9-232">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="0b6d9-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6d9-233">Boolean</span></span>|<span data-ttu-id="0b6d9-234">如果设置为 "true S/MIME 加密"，则默认为启用。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-234">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="0b6d9-235">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="0b6d9-235">smimeSigningEnabled</span></span>|<span data-ttu-id="0b6d9-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6d9-236">Boolean</span></span>|<span data-ttu-id="0b6d9-237">如果为此帐户启用了设置为 true S/MIME 签名</span><span class="sxs-lookup"><span data-stu-id="0b6d9-237">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="0b6d9-238">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="0b6d9-238">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="0b6d9-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6d9-239">Boolean</span></span>|<span data-ttu-id="0b6d9-240">如果设置为 true，则用户可以打开或关闭 S/MIME 签名。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-240">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="0b6d9-241">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="0b6d9-241">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="0b6d9-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6d9-242">Boolean</span></span>|<span data-ttu-id="0b6d9-243">如果设置为 true，则用户可以默认切换加密设置。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-243">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="0b6d9-244">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="0b6d9-244">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="0b6d9-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6d9-245">Boolean</span></span>|<span data-ttu-id="0b6d9-246">如果设置为 true，则用户可以选择签名标识。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-246">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="0b6d9-247">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="0b6d9-247">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="0b6d9-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6d9-248">Boolean</span></span>|<span data-ttu-id="0b6d9-249">如果设置为 true，则用户可以选择 S/MIME 加密标识。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-249">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="0b6d9-250">requireSsl</span><span class="sxs-lookup"><span data-stu-id="0b6d9-250">requireSsl</span></span>|<span data-ttu-id="0b6d9-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6d9-251">Boolean</span></span>|<span data-ttu-id="0b6d9-252">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-252">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="0b6d9-253">useOAuth</span><span class="sxs-lookup"><span data-stu-id="0b6d9-253">useOAuth</span></span>|<span data-ttu-id="0b6d9-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6d9-254">Boolean</span></span>|<span data-ttu-id="0b6d9-255">指定连接是否应使用 OAuth 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-255">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="0b6d9-256">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="0b6d9-256">signingCertificateType</span></span>|[<span data-ttu-id="0b6d9-257">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="0b6d9-257">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="0b6d9-258">此电子邮件配置文件的签名证书类型。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-258">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="0b6d9-259">可取值为：`none`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-259">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="0b6d9-260">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="0b6d9-260">encryptionCertificateType</span></span>|[<span data-ttu-id="0b6d9-261">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="0b6d9-261">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="0b6d9-262">此电子邮件配置文件的加密证书类型。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-262">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="0b6d9-263">可取值为：`none`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-263">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="0b6d9-264">响应</span><span class="sxs-lookup"><span data-stu-id="0b6d9-264">Response</span></span>
<span data-ttu-id="0b6d9-265">如果成功，此方法在响应`201 Created`正文中返回响应代码和[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-265">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b6d9-266">示例</span><span class="sxs-lookup"><span data-stu-id="0b6d9-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b6d9-267">请求</span><span class="sxs-lookup"><span data-stu-id="0b6d9-267">Request</span></span>
<span data-ttu-id="0b6d9-268">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-268">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2057

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

### <a name="response"></a><span data-ttu-id="0b6d9-269">响应</span><span class="sxs-lookup"><span data-stu-id="0b6d9-269">Response</span></span>
<span data-ttu-id="0b6d9-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b6d9-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2229

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






