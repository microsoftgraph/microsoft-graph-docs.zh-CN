---
title: 更新 windowsPhoneEASEmailProfileConfiguration
description: 更新 windowsPhoneEASEmailProfileConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45042dbccbc6ef9d465a554c8de339e9d8b6cc91
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154712"
---
# <a name="update-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="c1138-103">更新 windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="c1138-103">Update windowsPhoneEASEmailProfileConfiguration</span></span>

<span data-ttu-id="c1138-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1138-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1138-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c1138-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1138-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1138-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1138-107">更新 [windowsPhoneEASEmailProfileConfiguration 对象](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="c1138-107">Update the properties of a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1138-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1138-108">Prerequisites</span></span>
<span data-ttu-id="c1138-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1138-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1138-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1138-111">Permission type</span></span>|<span data-ttu-id="c1138-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1138-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1138-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1138-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1138-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1138-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1138-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1138-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1138-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1138-116">Not supported.</span></span>|
|<span data-ttu-id="c1138-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1138-117">Application</span></span>|<span data-ttu-id="c1138-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1138-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1138-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1138-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c1138-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1138-120">Request headers</span></span>
|<span data-ttu-id="c1138-121">标头</span><span class="sxs-lookup"><span data-stu-id="c1138-121">Header</span></span>|<span data-ttu-id="c1138-122">值</span><span class="sxs-lookup"><span data-stu-id="c1138-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1138-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1138-123">Authorization</span></span>|<span data-ttu-id="c1138-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1138-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1138-125">接受</span><span class="sxs-lookup"><span data-stu-id="c1138-125">Accept</span></span>|<span data-ttu-id="c1138-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1138-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1138-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1138-127">Request body</span></span>
<span data-ttu-id="c1138-128">在请求正文中，提供 [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1138-128">In the request body, supply a JSON representation for the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="c1138-129">下表显示创建 [windowsPhoneEASEmailProfileConfiguration 时所需的属性](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c1138-129">The following table shows the properties that are required when you create the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="c1138-130">属性</span><span class="sxs-lookup"><span data-stu-id="c1138-130">Property</span></span>|<span data-ttu-id="c1138-131">类型</span><span class="sxs-lookup"><span data-stu-id="c1138-131">Type</span></span>|<span data-ttu-id="c1138-132">说明</span><span class="sxs-lookup"><span data-stu-id="c1138-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1138-133">id</span><span class="sxs-lookup"><span data-stu-id="c1138-133">id</span></span>|<span data-ttu-id="c1138-134">String</span><span class="sxs-lookup"><span data-stu-id="c1138-134">String</span></span>|<span data-ttu-id="c1138-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c1138-135">Key of the entity.</span></span> <span data-ttu-id="c1138-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1138-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1138-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1138-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c1138-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1138-138">DateTimeOffset</span></span>|<span data-ttu-id="c1138-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c1138-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c1138-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1138-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1138-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1138-141">roleScopeTagIds</span></span>|<span data-ttu-id="c1138-142">String collection</span><span class="sxs-lookup"><span data-stu-id="c1138-142">String collection</span></span>|<span data-ttu-id="c1138-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c1138-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c1138-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1138-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1138-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c1138-145">supportsScopeTags</span></span>|<span data-ttu-id="c1138-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1138-146">Boolean</span></span>|<span data-ttu-id="c1138-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="c1138-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c1138-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="c1138-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c1138-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="c1138-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c1138-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c1138-150">This property is read-only.</span></span> <span data-ttu-id="c1138-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1138-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1138-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c1138-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c1138-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c1138-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c1138-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="c1138-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c1138-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1138-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1138-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c1138-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c1138-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c1138-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c1138-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c1138-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c1138-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1138-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1138-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c1138-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c1138-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c1138-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c1138-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c1138-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c1138-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1138-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1138-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1138-164">createdDateTime</span></span>|<span data-ttu-id="c1138-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1138-165">DateTimeOffset</span></span>|<span data-ttu-id="c1138-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c1138-166">DateTime the object was created.</span></span> <span data-ttu-id="c1138-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1138-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1138-168">说明</span><span class="sxs-lookup"><span data-stu-id="c1138-168">description</span></span>|<span data-ttu-id="c1138-169">String</span><span class="sxs-lookup"><span data-stu-id="c1138-169">String</span></span>|<span data-ttu-id="c1138-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c1138-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c1138-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1138-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1138-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c1138-172">displayName</span></span>|<span data-ttu-id="c1138-173">String</span><span class="sxs-lookup"><span data-stu-id="c1138-173">String</span></span>|<span data-ttu-id="c1138-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c1138-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c1138-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1138-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1138-176">version</span><span class="sxs-lookup"><span data-stu-id="c1138-176">version</span></span>|<span data-ttu-id="c1138-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c1138-177">Int32</span></span>|<span data-ttu-id="c1138-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c1138-178">Version of the device configuration.</span></span> <span data-ttu-id="c1138-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1138-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1138-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c1138-180">usernameSource</span></span>|[<span data-ttu-id="c1138-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="c1138-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c1138-182">在设备上安装之前从 AAD 中选取并注入到此配置文件中的用户名属性。</span><span class="sxs-lookup"><span data-stu-id="c1138-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c1138-183">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="c1138-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c1138-184">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="c1138-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c1138-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="c1138-185">usernameAADSource</span></span>|[<span data-ttu-id="c1138-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c1138-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="c1138-187">AAD 字段的名称，该字段将用于检索电子邮件配置文件的 UserName。</span><span class="sxs-lookup"><span data-stu-id="c1138-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="c1138-188">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="c1138-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c1138-189">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="c1138-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="c1138-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="c1138-190">userDomainNameSource</span></span>|[<span data-ttu-id="c1138-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="c1138-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="c1138-192">UserDomainname 属性，在设备上安装之前从 AAD 中选取并注入到此配置文件中。</span><span class="sxs-lookup"><span data-stu-id="c1138-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c1138-193">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="c1138-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c1138-194">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="c1138-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="c1138-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="c1138-195">customDomainName</span></span>|<span data-ttu-id="c1138-196">String</span><span class="sxs-lookup"><span data-stu-id="c1138-196">String</span></span>|<span data-ttu-id="c1138-197">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="c1138-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="c1138-198">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="c1138-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="c1138-199">accountName</span><span class="sxs-lookup"><span data-stu-id="c1138-199">accountName</span></span>|<span data-ttu-id="c1138-200">String</span><span class="sxs-lookup"><span data-stu-id="c1138-200">String</span></span>|<span data-ttu-id="c1138-201">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="c1138-201">Account name.</span></span>|
|<span data-ttu-id="c1138-202">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="c1138-202">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="c1138-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1138-203">Boolean</span></span>|<span data-ttu-id="c1138-204">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="c1138-204">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="c1138-205">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c1138-205">This property is read-only.</span></span>|
|<span data-ttu-id="c1138-206">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="c1138-206">syncCalendar</span></span>|<span data-ttu-id="c1138-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1138-207">Boolean</span></span>|<span data-ttu-id="c1138-208">是否同步日历。</span><span class="sxs-lookup"><span data-stu-id="c1138-208">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="c1138-209">syncContacts</span><span class="sxs-lookup"><span data-stu-id="c1138-209">syncContacts</span></span>|<span data-ttu-id="c1138-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1138-210">Boolean</span></span>|<span data-ttu-id="c1138-211">是否同步联系人。</span><span class="sxs-lookup"><span data-stu-id="c1138-211">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="c1138-212">syncTasks</span><span class="sxs-lookup"><span data-stu-id="c1138-212">syncTasks</span></span>|<span data-ttu-id="c1138-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1138-213">Boolean</span></span>|<span data-ttu-id="c1138-214">是否同步任务。</span><span class="sxs-lookup"><span data-stu-id="c1138-214">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="c1138-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="c1138-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="c1138-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="c1138-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="c1138-217">要同步的电子邮件的持续时间。可能的值是 `userDefined` `oneDay` `threeDays` ：、、、、、、。 `oneWeek` `twoWeeks` `oneMonth` `unlimited`</span><span class="sxs-lookup"><span data-stu-id="c1138-217">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="c1138-218">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="c1138-218">emailAddressSource</span></span>|[<span data-ttu-id="c1138-219">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="c1138-219">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c1138-220">从 AAD 中选取并注入到此配置文件中的电子邮件属性，在设备上安装之前。</span><span class="sxs-lookup"><span data-stu-id="c1138-220">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c1138-221">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="c1138-221">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c1138-222">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="c1138-222">emailSyncSchedule</span></span>|[<span data-ttu-id="c1138-223">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="c1138-223">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="c1138-224">电子邮件同步计划。</span><span class="sxs-lookup"><span data-stu-id="c1138-224">Email sync schedule.</span></span> <span data-ttu-id="c1138-225">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes` 或 `basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="c1138-225">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="c1138-226">hostName</span><span class="sxs-lookup"><span data-stu-id="c1138-226">hostName</span></span>|<span data-ttu-id="c1138-227">String</span><span class="sxs-lookup"><span data-stu-id="c1138-227">String</span></span>|<span data-ttu-id="c1138-228">使用本机 (连接到) URL 的 Exchange 位置。</span><span class="sxs-lookup"><span data-stu-id="c1138-228">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="c1138-229">requireSsl</span><span class="sxs-lookup"><span data-stu-id="c1138-229">requireSsl</span></span>|<span data-ttu-id="c1138-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1138-230">Boolean</span></span>|<span data-ttu-id="c1138-231">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="c1138-231">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="c1138-232">响应</span><span class="sxs-lookup"><span data-stu-id="c1138-232">Response</span></span>
<span data-ttu-id="c1138-233">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1138-233">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1138-234">示例</span><span class="sxs-lookup"><span data-stu-id="c1138-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1138-235">请求</span><span class="sxs-lookup"><span data-stu-id="c1138-235">Request</span></span>
<span data-ttu-id="c1138-236">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1138-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1567

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
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
  "applyOnlyToWindowsPhone81": true,
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```

### <a name="response"></a><span data-ttu-id="c1138-237">响应</span><span class="sxs-lookup"><span data-stu-id="c1138-237">Response</span></span>
<span data-ttu-id="c1138-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1138-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1739

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
  "id": "554f402a-402a-554f-2a40-4f552a404f55",
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
  "applyOnlyToWindowsPhone81": true,
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```




