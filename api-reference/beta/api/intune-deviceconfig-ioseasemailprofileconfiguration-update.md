---
title: 更新 iosEasEmailProfileConfiguration
description: 更新 iosEasEmailProfileConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8e9f1fc9dd8f7a7344edd568ae3bcd1b26aecaee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36339356"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="e7ae5-103">更新 iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="e7ae5-103">Update iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="e7ae5-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7ae5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7ae5-106">更新[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-106">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7ae5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e7ae5-107">Prerequisites</span></span>
<span data-ttu-id="e7ae5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7ae5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7ae5-110">Permission type</span></span>|<span data-ttu-id="e7ae5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e7ae5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7ae5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7ae5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7ae5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7ae5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7ae5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7ae5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7ae5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-115">Not supported.</span></span>|
|<span data-ttu-id="e7ae5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7ae5-116">Application</span></span>|<span data-ttu-id="e7ae5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7ae5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7ae5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7ae5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e7ae5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7ae5-119">Request headers</span></span>
|<span data-ttu-id="e7ae5-120">标头</span><span class="sxs-lookup"><span data-stu-id="e7ae5-120">Header</span></span>|<span data-ttu-id="e7ae5-121">值</span><span class="sxs-lookup"><span data-stu-id="e7ae5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7ae5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7ae5-122">Authorization</span></span>|<span data-ttu-id="e7ae5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7ae5-124">接受</span><span class="sxs-lookup"><span data-stu-id="e7ae5-124">Accept</span></span>|<span data-ttu-id="e7ae5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7ae5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7ae5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7ae5-126">Request body</span></span>
<span data-ttu-id="e7ae5-127">在请求正文中, 提供[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-127">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="e7ae5-128">下表显示创建[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-128">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="e7ae5-129">属性</span><span class="sxs-lookup"><span data-stu-id="e7ae5-129">Property</span></span>|<span data-ttu-id="e7ae5-130">类型</span><span class="sxs-lookup"><span data-stu-id="e7ae5-130">Type</span></span>|<span data-ttu-id="e7ae5-131">说明</span><span class="sxs-lookup"><span data-stu-id="e7ae5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7ae5-132">id</span><span class="sxs-lookup"><span data-stu-id="e7ae5-132">id</span></span>|<span data-ttu-id="e7ae5-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e7ae5-133">String</span></span>|<span data-ttu-id="e7ae5-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-134">Key of the entity.</span></span> <span data-ttu-id="e7ae5-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7ae5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ae5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7ae5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e7ae5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7ae5-137">DateTimeOffset</span></span>|<span data-ttu-id="e7ae5-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e7ae5-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7ae5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ae5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e7ae5-140">roleScopeTagIds</span></span>|<span data-ttu-id="e7ae5-141">String collection</span><span class="sxs-lookup"><span data-stu-id="e7ae5-141">String collection</span></span>|<span data-ttu-id="e7ae5-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e7ae5-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7ae5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ae5-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e7ae5-144">supportsScopeTags</span></span>|<span data-ttu-id="e7ae5-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ae5-145">Boolean</span></span>|<span data-ttu-id="e7ae5-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e7ae5-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e7ae5-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e7ae5-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-149">This property is read-only.</span></span> <span data-ttu-id="e7ae5-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7ae5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ae5-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e7ae5-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e7ae5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e7ae5-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e7ae5-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e7ae5-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7ae5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ae5-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e7ae5-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e7ae5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e7ae5-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e7ae5-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e7ae5-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7ae5-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ae5-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e7ae5-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e7ae5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e7ae5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e7ae5-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e7ae5-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7ae5-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ae5-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7ae5-163">createdDateTime</span></span>|<span data-ttu-id="e7ae5-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7ae5-164">DateTimeOffset</span></span>|<span data-ttu-id="e7ae5-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-165">DateTime the object was created.</span></span> <span data-ttu-id="e7ae5-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7ae5-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ae5-167">说明</span><span class="sxs-lookup"><span data-stu-id="e7ae5-167">description</span></span>|<span data-ttu-id="e7ae5-168">String</span><span class="sxs-lookup"><span data-stu-id="e7ae5-168">String</span></span>|<span data-ttu-id="e7ae5-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e7ae5-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7ae5-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ae5-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e7ae5-171">displayName</span></span>|<span data-ttu-id="e7ae5-172">String</span><span class="sxs-lookup"><span data-stu-id="e7ae5-172">String</span></span>|<span data-ttu-id="e7ae5-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e7ae5-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7ae5-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ae5-175">version</span><span class="sxs-lookup"><span data-stu-id="e7ae5-175">version</span></span>|<span data-ttu-id="e7ae5-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e7ae5-176">Int32</span></span>|<span data-ttu-id="e7ae5-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-177">Version of the device configuration.</span></span> <span data-ttu-id="e7ae5-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7ae5-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7ae5-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="e7ae5-179">usernameSource</span></span>|[<span data-ttu-id="e7ae5-180">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="e7ae5-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="e7ae5-181">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e7ae5-182">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e7ae5-183">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="e7ae5-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="e7ae5-184">usernameAADSource</span></span>|[<span data-ttu-id="e7ae5-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="e7ae5-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="e7ae5-186">AAD 字段的名称, 将用于检索电子邮件配置文件的用户名。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="e7ae5-187">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e7ae5-188">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="e7ae5-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="e7ae5-189">userDomainNameSource</span></span>|[<span data-ttu-id="e7ae5-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="e7ae5-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="e7ae5-191">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e7ae5-192">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e7ae5-193">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="e7ae5-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="e7ae5-194">customDomainName</span></span>|<span data-ttu-id="e7ae5-195">String</span><span class="sxs-lookup"><span data-stu-id="e7ae5-195">String</span></span>|<span data-ttu-id="e7ae5-196">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="e7ae5-197">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="e7ae5-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="e7ae5-198">帐户</span><span class="sxs-lookup"><span data-stu-id="e7ae5-198">accountName</span></span>|<span data-ttu-id="e7ae5-199">String</span><span class="sxs-lookup"><span data-stu-id="e7ae5-199">String</span></span>|<span data-ttu-id="e7ae5-200">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-200">Account name.</span></span>|
|<span data-ttu-id="e7ae5-201">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e7ae5-201">authenticationMethod</span></span>|[<span data-ttu-id="e7ae5-202">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e7ae5-202">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="e7ae5-203">此电子邮件配置文件的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-203">Authentication method for this Email profile.</span></span> <span data-ttu-id="e7ae5-204">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-204">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e7ae5-205">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="e7ae5-205">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="e7ae5-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ae5-206">Boolean</span></span>|<span data-ttu-id="e7ae5-207">指示是否阻止将邮件移动到其他电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-207">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="e7ae5-208">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="e7ae5-208">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="e7ae5-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ae5-209">Boolean</span></span>|<span data-ttu-id="e7ae5-210">指示是否阻止来自第三方应用的发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-210">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="e7ae5-211">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="e7ae5-211">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="e7ae5-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ae5-212">Boolean</span></span>|<span data-ttu-id="e7ae5-213">指示是否阻止同步最近使用的电子邮件地址, 例如, 撰写新电子邮件时。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-213">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="e7ae5-214">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="e7ae5-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="e7ae5-215">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="e7ae5-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="e7ae5-216">电子邮件的持续时间应同步回。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-216">Duration of time email should be synced back to.</span></span> <span data-ttu-id="e7ae5-217">.</span><span class="sxs-lookup"><span data-stu-id="e7ae5-217"></span></span> <span data-ttu-id="e7ae5-218">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-218">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="e7ae5-219">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="e7ae5-219">emailAddressSource</span></span>|[<span data-ttu-id="e7ae5-220">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="e7ae5-220">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="e7ae5-221">在设备上安装之前, 从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-221">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e7ae5-222">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-222">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="e7ae5-223">hostName</span><span class="sxs-lookup"><span data-stu-id="e7ae5-223">hostName</span></span>|<span data-ttu-id="e7ae5-224">String</span><span class="sxs-lookup"><span data-stu-id="e7ae5-224">String</span></span>|<span data-ttu-id="e7ae5-225">本机邮件应用程序连接到的 Exchange 位置 (URL)。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-225">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="e7ae5-226">requireSmime</span><span class="sxs-lookup"><span data-stu-id="e7ae5-226">requireSmime</span></span>|<span data-ttu-id="e7ae5-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ae5-227">Boolean</span></span>|<span data-ttu-id="e7ae5-228">指示是否使用 S/MIME 证书。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-228">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="e7ae5-229">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="e7ae5-229">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="e7ae5-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ae5-230">Boolean</span></span>|<span data-ttu-id="e7ae5-231">指示是否允许未加密的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-231">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="e7ae5-232">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="e7ae5-232">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="e7ae5-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ae5-233">Boolean</span></span>|<span data-ttu-id="e7ae5-234">如果设置为 "true S/MIME 加密", 则默认为启用。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-234">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="e7ae5-235">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="e7ae5-235">smimeSigningEnabled</span></span>|<span data-ttu-id="e7ae5-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ae5-236">Boolean</span></span>|<span data-ttu-id="e7ae5-237">如果为此帐户启用了设置为 true S/MIME 签名</span><span class="sxs-lookup"><span data-stu-id="e7ae5-237">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="e7ae5-238">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="e7ae5-238">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="e7ae5-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ae5-239">Boolean</span></span>|<span data-ttu-id="e7ae5-240">如果设置为 true, 则用户可以打开或关闭 S/MIME 签名。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-240">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="e7ae5-241">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="e7ae5-241">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="e7ae5-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ae5-242">Boolean</span></span>|<span data-ttu-id="e7ae5-243">如果设置为 true, 则用户可以默认切换加密设置。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-243">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="e7ae5-244">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="e7ae5-244">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="e7ae5-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ae5-245">Boolean</span></span>|<span data-ttu-id="e7ae5-246">如果设置为 true, 则用户可以选择签名标识。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-246">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="e7ae5-247">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="e7ae5-247">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="e7ae5-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ae5-248">Boolean</span></span>|<span data-ttu-id="e7ae5-249">如果设置为 true, 则用户可以选择 S/MIME 加密标识。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-249">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="e7ae5-250">requireSsl</span><span class="sxs-lookup"><span data-stu-id="e7ae5-250">requireSsl</span></span>|<span data-ttu-id="e7ae5-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ae5-251">Boolean</span></span>|<span data-ttu-id="e7ae5-252">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-252">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="e7ae5-253">useOAuth</span><span class="sxs-lookup"><span data-stu-id="e7ae5-253">useOAuth</span></span>|<span data-ttu-id="e7ae5-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ae5-254">Boolean</span></span>|<span data-ttu-id="e7ae5-255">指定连接是否应使用 OAuth 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-255">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="e7ae5-256">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="e7ae5-256">signingCertificateType</span></span>|[<span data-ttu-id="e7ae5-257">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="e7ae5-257">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="e7ae5-258">此电子邮件配置文件的签名证书类型。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-258">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="e7ae5-259">可取值为：`none`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-259">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e7ae5-260">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="e7ae5-260">encryptionCertificateType</span></span>|[<span data-ttu-id="e7ae5-261">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="e7ae5-261">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="e7ae5-262">此电子邮件配置文件的加密证书类型。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-262">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="e7ae5-263">可取值为：`none`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-263">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="e7ae5-264">响应</span><span class="sxs-lookup"><span data-stu-id="e7ae5-264">Response</span></span>
<span data-ttu-id="e7ae5-265">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-265">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7ae5-266">示例</span><span class="sxs-lookup"><span data-stu-id="e7ae5-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7ae5-267">请求</span><span class="sxs-lookup"><span data-stu-id="e7ae5-267">Request</span></span>
<span data-ttu-id="e7ae5-268">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-268">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="e7ae5-269">响应</span><span class="sxs-lookup"><span data-stu-id="e7ae5-269">Response</span></span>
<span data-ttu-id="e7ae5-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e7ae5-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






