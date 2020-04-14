---
title: 更新 iosEasEmailProfileConfiguration
description: 更新 iosEasEmailProfileConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a2a8d3ca3a8a61bdcb957f2ea7be867906bb4275
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439329"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="cd0e0-103">更新 iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd0e0-103">Update iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="cd0e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd0e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd0e0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd0e0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd0e0-107">更新[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd0e0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cd0e0-108">Prerequisites</span></span>
<span data-ttu-id="cd0e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd0e0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd0e0-111">Permission type</span></span>|<span data-ttu-id="cd0e0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cd0e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd0e0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd0e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cd0e0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd0e0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cd0e0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd0e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd0e0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-116">Not supported.</span></span>|
|<span data-ttu-id="cd0e0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd0e0-117">Application</span></span>|<span data-ttu-id="cd0e0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd0e0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd0e0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd0e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cd0e0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd0e0-120">Request headers</span></span>
|<span data-ttu-id="cd0e0-121">标头</span><span class="sxs-lookup"><span data-stu-id="cd0e0-121">Header</span></span>|<span data-ttu-id="cd0e0-122">值</span><span class="sxs-lookup"><span data-stu-id="cd0e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd0e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd0e0-123">Authorization</span></span>|<span data-ttu-id="cd0e0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd0e0-125">接受</span><span class="sxs-lookup"><span data-stu-id="cd0e0-125">Accept</span></span>|<span data-ttu-id="cd0e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cd0e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd0e0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd0e0-127">Request body</span></span>
<span data-ttu-id="cd0e0-128">在请求正文中，提供[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="cd0e0-129">下表显示创建[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="cd0e0-130">属性</span><span class="sxs-lookup"><span data-stu-id="cd0e0-130">Property</span></span>|<span data-ttu-id="cd0e0-131">类型</span><span class="sxs-lookup"><span data-stu-id="cd0e0-131">Type</span></span>|<span data-ttu-id="cd0e0-132">说明</span><span class="sxs-lookup"><span data-stu-id="cd0e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd0e0-133">id</span><span class="sxs-lookup"><span data-stu-id="cd0e0-133">id</span></span>|<span data-ttu-id="cd0e0-134">字符串</span><span class="sxs-lookup"><span data-stu-id="cd0e0-134">String</span></span>|<span data-ttu-id="cd0e0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-135">Key of the entity.</span></span> <span data-ttu-id="cd0e0-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd0e0-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd0e0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd0e0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="cd0e0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd0e0-138">DateTimeOffset</span></span>|<span data-ttu-id="cd0e0-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="cd0e0-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd0e0-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd0e0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cd0e0-141">roleScopeTagIds</span></span>|<span data-ttu-id="cd0e0-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="cd0e0-142">String collection</span></span>|<span data-ttu-id="cd0e0-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cd0e0-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd0e0-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd0e0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cd0e0-145">supportsScopeTags</span></span>|<span data-ttu-id="cd0e0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-146">Boolean</span></span>|<span data-ttu-id="cd0e0-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cd0e0-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cd0e0-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cd0e0-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-150">This property is read-only.</span></span> <span data-ttu-id="cd0e0-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd0e0-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd0e0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cd0e0-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="cd0e0-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cd0e0-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="cd0e0-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="cd0e0-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd0e0-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd0e0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cd0e0-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="cd0e0-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cd0e0-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="cd0e0-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="cd0e0-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd0e0-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd0e0-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="cd0e0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="cd0e0-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="cd0e0-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="cd0e0-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="cd0e0-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd0e0-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd0e0-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd0e0-164">createdDateTime</span></span>|<span data-ttu-id="cd0e0-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd0e0-165">DateTimeOffset</span></span>|<span data-ttu-id="cd0e0-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-166">DateTime the object was created.</span></span> <span data-ttu-id="cd0e0-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd0e0-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd0e0-168">description</span><span class="sxs-lookup"><span data-stu-id="cd0e0-168">description</span></span>|<span data-ttu-id="cd0e0-169">String</span><span class="sxs-lookup"><span data-stu-id="cd0e0-169">String</span></span>|<span data-ttu-id="cd0e0-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cd0e0-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd0e0-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd0e0-172">displayName</span><span class="sxs-lookup"><span data-stu-id="cd0e0-172">displayName</span></span>|<span data-ttu-id="cd0e0-173">String</span><span class="sxs-lookup"><span data-stu-id="cd0e0-173">String</span></span>|<span data-ttu-id="cd0e0-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cd0e0-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd0e0-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd0e0-176">version</span><span class="sxs-lookup"><span data-stu-id="cd0e0-176">version</span></span>|<span data-ttu-id="cd0e0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="cd0e0-177">Int32</span></span>|<span data-ttu-id="cd0e0-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-178">Version of the device configuration.</span></span> <span data-ttu-id="cd0e0-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd0e0-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd0e0-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="cd0e0-180">usernameSource</span></span>|[<span data-ttu-id="cd0e0-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="cd0e0-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="cd0e0-182">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="cd0e0-183">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="cd0e0-184">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="cd0e0-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="cd0e0-185">usernameAADSource</span></span>|[<span data-ttu-id="cd0e0-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="cd0e0-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="cd0e0-187">AAD 字段的名称，将用于检索电子邮件配置文件的用户名。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="cd0e0-188">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="cd0e0-189">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="cd0e0-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="cd0e0-190">userDomainNameSource</span></span>|[<span data-ttu-id="cd0e0-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="cd0e0-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="cd0e0-192">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="cd0e0-193">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="cd0e0-194">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="cd0e0-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="cd0e0-195">customDomainName</span></span>|<span data-ttu-id="cd0e0-196">String</span><span class="sxs-lookup"><span data-stu-id="cd0e0-196">String</span></span>|<span data-ttu-id="cd0e0-197">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="cd0e0-198">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="cd0e0-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="cd0e0-199">帐户</span><span class="sxs-lookup"><span data-stu-id="cd0e0-199">accountName</span></span>|<span data-ttu-id="cd0e0-200">String</span><span class="sxs-lookup"><span data-stu-id="cd0e0-200">String</span></span>|<span data-ttu-id="cd0e0-201">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-201">Account name.</span></span>|
|<span data-ttu-id="cd0e0-202">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cd0e0-202">authenticationMethod</span></span>|[<span data-ttu-id="cd0e0-203">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cd0e0-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="cd0e0-204">此电子邮件配置文件的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="cd0e0-205">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="cd0e0-206">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="cd0e0-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="cd0e0-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-207">Boolean</span></span>|<span data-ttu-id="cd0e0-208">指示是否阻止将邮件移动到其他电子邮件帐户。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="cd0e0-209">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="cd0e0-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="cd0e0-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-210">Boolean</span></span>|<span data-ttu-id="cd0e0-211">指示是否阻止来自第三方应用的发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="cd0e0-212">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="cd0e0-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="cd0e0-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-213">Boolean</span></span>|<span data-ttu-id="cd0e0-214">指示是否阻止同步最近使用的电子邮件地址，例如，撰写新电子邮件时。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="cd0e0-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="cd0e0-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="cd0e0-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="cd0e0-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="cd0e0-217">电子邮件的持续时间应同步回。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="cd0e0-218">.</span><span class="sxs-lookup"><span data-stu-id="cd0e0-218">.</span></span> <span data-ttu-id="cd0e0-219">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="cd0e0-220">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="cd0e0-220">emailAddressSource</span></span>|[<span data-ttu-id="cd0e0-221">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="cd0e0-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="cd0e0-222">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="cd0e0-223">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="cd0e0-224">easServices</span><span class="sxs-lookup"><span data-stu-id="cd0e0-224">easServices</span></span>|[<span data-ttu-id="cd0e0-225">easServices</span><span class="sxs-lookup"><span data-stu-id="cd0e0-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="cd0e0-226">要同步的 Exchange 数据。可能的值为`none`： `calendars`、 `contacts`、 `email`、 `notes`、 `reminders`、。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="cd0e0-227">easServicesUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="cd0e0-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="cd0e0-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-228">Boolean</span></span>|<span data-ttu-id="cd0e0-229">允许用户更改同步设置。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="cd0e0-230">hostName</span><span class="sxs-lookup"><span data-stu-id="cd0e0-230">hostName</span></span>|<span data-ttu-id="cd0e0-231">String</span><span class="sxs-lookup"><span data-stu-id="cd0e0-231">String</span></span>|<span data-ttu-id="cd0e0-232">本机邮件应用程序连接到的 Exchange 位置（URL）。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="cd0e0-233">requireSmime</span><span class="sxs-lookup"><span data-stu-id="cd0e0-233">requireSmime</span></span>|<span data-ttu-id="cd0e0-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-234">Boolean</span></span>|<span data-ttu-id="cd0e0-235">指示是否使用 S/MIME 证书。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="cd0e0-236">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="cd0e0-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="cd0e0-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-237">Boolean</span></span>|<span data-ttu-id="cd0e0-238">指示是否允许未加密的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="cd0e0-239">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="cd0e0-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="cd0e0-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-240">Boolean</span></span>|<span data-ttu-id="cd0e0-241">如果设置为 "true S/MIME 加密"，则默认为启用。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="cd0e0-242">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="cd0e0-242">smimeSigningEnabled</span></span>|<span data-ttu-id="cd0e0-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-243">Boolean</span></span>|<span data-ttu-id="cd0e0-244">如果为此帐户启用了设置为 true S/MIME 签名</span><span class="sxs-lookup"><span data-stu-id="cd0e0-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="cd0e0-245">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="cd0e0-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="cd0e0-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-246">Boolean</span></span>|<span data-ttu-id="cd0e0-247">如果设置为 true，则用户可以打开或关闭 S/MIME 签名。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="cd0e0-248">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="cd0e0-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="cd0e0-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-249">Boolean</span></span>|<span data-ttu-id="cd0e0-250">如果设置为 true，则用户可以默认切换加密设置。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="cd0e0-251">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="cd0e0-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="cd0e0-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-252">Boolean</span></span>|<span data-ttu-id="cd0e0-253">如果设置为 true，则用户可以选择签名标识。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="cd0e0-254">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="cd0e0-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="cd0e0-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-255">Boolean</span></span>|<span data-ttu-id="cd0e0-256">如果设置为 true，则用户可以选择 S/MIME 加密标识。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="cd0e0-257">requireSsl</span><span class="sxs-lookup"><span data-stu-id="cd0e0-257">requireSsl</span></span>|<span data-ttu-id="cd0e0-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-258">Boolean</span></span>|<span data-ttu-id="cd0e0-259">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="cd0e0-260">useOAuth</span><span class="sxs-lookup"><span data-stu-id="cd0e0-260">useOAuth</span></span>|<span data-ttu-id="cd0e0-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd0e0-261">Boolean</span></span>|<span data-ttu-id="cd0e0-262">指定连接是否应使用 OAuth 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="cd0e0-263">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="cd0e0-263">signingCertificateType</span></span>|[<span data-ttu-id="cd0e0-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="cd0e0-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="cd0e0-265">此电子邮件配置文件的签名证书类型。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="cd0e0-266">可取值为：`none`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="cd0e0-267">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="cd0e0-267">encryptionCertificateType</span></span>|[<span data-ttu-id="cd0e0-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="cd0e0-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="cd0e0-269">此电子邮件配置文件的加密证书类型。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="cd0e0-270">可取值为：`none`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="cd0e0-271">响应</span><span class="sxs-lookup"><span data-stu-id="cd0e0-271">Response</span></span>
<span data-ttu-id="cd0e0-272">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-272">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd0e0-273">示例</span><span class="sxs-lookup"><span data-stu-id="cd0e0-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd0e0-274">请求</span><span class="sxs-lookup"><span data-stu-id="cd0e0-274">Request</span></span>
<span data-ttu-id="cd0e0-275">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-275">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cd0e0-276">响应</span><span class="sxs-lookup"><span data-stu-id="cd0e0-276">Response</span></span>
<span data-ttu-id="cd0e0-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd0e0-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



