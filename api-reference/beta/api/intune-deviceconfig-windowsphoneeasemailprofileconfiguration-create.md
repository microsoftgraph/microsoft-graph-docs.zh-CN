---
title: 创建 windowsPhoneEASEmailProfileConfiguration
description: 创建新的 windowsPhoneEASEmailProfileConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 512ff04cb2c4eda2539f91b627070f45480cb72b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147124"
---
# <a name="create-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="6eeaa-103">创建 windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="6eeaa-103">Create windowsPhoneEASEmailProfileConfiguration</span></span>

<span data-ttu-id="6eeaa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6eeaa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6eeaa-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6eeaa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6eeaa-107">创建新的 [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-107">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6eeaa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6eeaa-108">Prerequisites</span></span>
<span data-ttu-id="6eeaa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6eeaa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6eeaa-111">Permission type</span></span>|<span data-ttu-id="6eeaa-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6eeaa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6eeaa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6eeaa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6eeaa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6eeaa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6eeaa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6eeaa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6eeaa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-116">Not supported.</span></span>|
|<span data-ttu-id="6eeaa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6eeaa-117">Application</span></span>|<span data-ttu-id="6eeaa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6eeaa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6eeaa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6eeaa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6eeaa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6eeaa-120">Request headers</span></span>
|<span data-ttu-id="6eeaa-121">标头</span><span class="sxs-lookup"><span data-stu-id="6eeaa-121">Header</span></span>|<span data-ttu-id="6eeaa-122">值</span><span class="sxs-lookup"><span data-stu-id="6eeaa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6eeaa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6eeaa-123">Authorization</span></span>|<span data-ttu-id="6eeaa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6eeaa-125">接受</span><span class="sxs-lookup"><span data-stu-id="6eeaa-125">Accept</span></span>|<span data-ttu-id="6eeaa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6eeaa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6eeaa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6eeaa-127">Request body</span></span>
<span data-ttu-id="6eeaa-128">在请求正文中，提供 windowsPhoneEASEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-128">In the request body, supply a JSON representation for the windowsPhoneEASEmailProfileConfiguration object.</span></span>

<span data-ttu-id="6eeaa-129">下表显示创建 windowsPhoneEASEmailProfileConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-129">The following table shows the properties that are required when you create the windowsPhoneEASEmailProfileConfiguration.</span></span>

|<span data-ttu-id="6eeaa-130">属性</span><span class="sxs-lookup"><span data-stu-id="6eeaa-130">Property</span></span>|<span data-ttu-id="6eeaa-131">类型</span><span class="sxs-lookup"><span data-stu-id="6eeaa-131">Type</span></span>|<span data-ttu-id="6eeaa-132">说明</span><span class="sxs-lookup"><span data-stu-id="6eeaa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6eeaa-133">id</span><span class="sxs-lookup"><span data-stu-id="6eeaa-133">id</span></span>|<span data-ttu-id="6eeaa-134">String</span><span class="sxs-lookup"><span data-stu-id="6eeaa-134">String</span></span>|<span data-ttu-id="6eeaa-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-135">Key of the entity.</span></span> <span data-ttu-id="6eeaa-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6eeaa-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6eeaa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6eeaa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6eeaa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6eeaa-138">DateTimeOffset</span></span>|<span data-ttu-id="6eeaa-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6eeaa-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6eeaa-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6eeaa-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6eeaa-141">roleScopeTagIds</span></span>|<span data-ttu-id="6eeaa-142">String collection</span><span class="sxs-lookup"><span data-stu-id="6eeaa-142">String collection</span></span>|<span data-ttu-id="6eeaa-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6eeaa-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6eeaa-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6eeaa-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6eeaa-145">supportsScopeTags</span></span>|<span data-ttu-id="6eeaa-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6eeaa-146">Boolean</span></span>|<span data-ttu-id="6eeaa-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6eeaa-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6eeaa-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6eeaa-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-150">This property is read-only.</span></span> <span data-ttu-id="6eeaa-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6eeaa-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6eeaa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6eeaa-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6eeaa-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6eeaa-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6eeaa-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6eeaa-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6eeaa-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6eeaa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6eeaa-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6eeaa-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6eeaa-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6eeaa-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6eeaa-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6eeaa-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6eeaa-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6eeaa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6eeaa-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6eeaa-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6eeaa-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6eeaa-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6eeaa-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6eeaa-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6eeaa-164">createdDateTime</span></span>|<span data-ttu-id="6eeaa-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6eeaa-165">DateTimeOffset</span></span>|<span data-ttu-id="6eeaa-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-166">DateTime the object was created.</span></span> <span data-ttu-id="6eeaa-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6eeaa-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6eeaa-168">说明</span><span class="sxs-lookup"><span data-stu-id="6eeaa-168">description</span></span>|<span data-ttu-id="6eeaa-169">String</span><span class="sxs-lookup"><span data-stu-id="6eeaa-169">String</span></span>|<span data-ttu-id="6eeaa-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6eeaa-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6eeaa-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6eeaa-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6eeaa-172">displayName</span></span>|<span data-ttu-id="6eeaa-173">String</span><span class="sxs-lookup"><span data-stu-id="6eeaa-173">String</span></span>|<span data-ttu-id="6eeaa-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6eeaa-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6eeaa-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6eeaa-176">version</span><span class="sxs-lookup"><span data-stu-id="6eeaa-176">version</span></span>|<span data-ttu-id="6eeaa-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6eeaa-177">Int32</span></span>|<span data-ttu-id="6eeaa-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-178">Version of the device configuration.</span></span> <span data-ttu-id="6eeaa-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6eeaa-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6eeaa-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="6eeaa-180">usernameSource</span></span>|[<span data-ttu-id="6eeaa-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="6eeaa-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="6eeaa-182">在设备上安装之前从 AAD 中选取并注入到此配置文件中的用户名属性。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6eeaa-183">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="6eeaa-184">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6eeaa-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="6eeaa-185">usernameAADSource</span></span>|[<span data-ttu-id="6eeaa-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="6eeaa-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="6eeaa-187">AAD 字段的名称，该字段将用于检索电子邮件配置文件的 UserName。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="6eeaa-188">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="6eeaa-189">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="6eeaa-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="6eeaa-190">userDomainNameSource</span></span>|[<span data-ttu-id="6eeaa-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="6eeaa-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="6eeaa-192">UserDomainname 属性，在设备上安装之前从 AAD 中选取并注入到此配置文件中。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6eeaa-193">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="6eeaa-194">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="6eeaa-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="6eeaa-195">customDomainName</span></span>|<span data-ttu-id="6eeaa-196">String</span><span class="sxs-lookup"><span data-stu-id="6eeaa-196">String</span></span>|<span data-ttu-id="6eeaa-197">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="6eeaa-198">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="6eeaa-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="6eeaa-199">accountName</span><span class="sxs-lookup"><span data-stu-id="6eeaa-199">accountName</span></span>|<span data-ttu-id="6eeaa-200">String</span><span class="sxs-lookup"><span data-stu-id="6eeaa-200">String</span></span>|<span data-ttu-id="6eeaa-201">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-201">Account name.</span></span>|
|<span data-ttu-id="6eeaa-202">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="6eeaa-202">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="6eeaa-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="6eeaa-203">Boolean</span></span>|<span data-ttu-id="6eeaa-204">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-204">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="6eeaa-205">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-205">This property is read-only.</span></span>|
|<span data-ttu-id="6eeaa-206">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="6eeaa-206">syncCalendar</span></span>|<span data-ttu-id="6eeaa-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="6eeaa-207">Boolean</span></span>|<span data-ttu-id="6eeaa-208">是否同步日历。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-208">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="6eeaa-209">syncContacts</span><span class="sxs-lookup"><span data-stu-id="6eeaa-209">syncContacts</span></span>|<span data-ttu-id="6eeaa-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="6eeaa-210">Boolean</span></span>|<span data-ttu-id="6eeaa-211">是否同步联系人。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-211">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="6eeaa-212">syncTasks</span><span class="sxs-lookup"><span data-stu-id="6eeaa-212">syncTasks</span></span>|<span data-ttu-id="6eeaa-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="6eeaa-213">Boolean</span></span>|<span data-ttu-id="6eeaa-214">是否同步任务。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-214">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="6eeaa-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="6eeaa-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="6eeaa-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="6eeaa-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="6eeaa-217">要同步的电子邮件的持续时间。可能的值是 `userDefined` `oneDay` `threeDays` ：、、、、、、。 `oneWeek` `twoWeeks` `oneMonth` `unlimited`</span><span class="sxs-lookup"><span data-stu-id="6eeaa-217">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="6eeaa-218">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="6eeaa-218">emailAddressSource</span></span>|[<span data-ttu-id="6eeaa-219">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="6eeaa-219">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="6eeaa-220">从 AAD 中选取并注入到此配置文件中的电子邮件属性，在设备上安装之前。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-220">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6eeaa-221">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-221">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6eeaa-222">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="6eeaa-222">emailSyncSchedule</span></span>|[<span data-ttu-id="6eeaa-223">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="6eeaa-223">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="6eeaa-224">电子邮件同步计划。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-224">Email sync schedule.</span></span> <span data-ttu-id="6eeaa-225">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes` 或 `basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-225">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="6eeaa-226">hostName</span><span class="sxs-lookup"><span data-stu-id="6eeaa-226">hostName</span></span>|<span data-ttu-id="6eeaa-227">String</span><span class="sxs-lookup"><span data-stu-id="6eeaa-227">String</span></span>|<span data-ttu-id="6eeaa-228">使用本机 (连接到) URL 的 Exchange 位置。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-228">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="6eeaa-229">requireSsl</span><span class="sxs-lookup"><span data-stu-id="6eeaa-229">requireSsl</span></span>|<span data-ttu-id="6eeaa-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="6eeaa-230">Boolean</span></span>|<span data-ttu-id="6eeaa-231">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-231">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="6eeaa-232">响应</span><span class="sxs-lookup"><span data-stu-id="6eeaa-232">Response</span></span>
<span data-ttu-id="6eeaa-233">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-233">If successful, this method returns a `201 Created` response code and a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6eeaa-234">示例</span><span class="sxs-lookup"><span data-stu-id="6eeaa-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="6eeaa-235">请求</span><span class="sxs-lookup"><span data-stu-id="6eeaa-235">Request</span></span>
<span data-ttu-id="6eeaa-236">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="6eeaa-237">响应</span><span class="sxs-lookup"><span data-stu-id="6eeaa-237">Response</span></span>
<span data-ttu-id="6eeaa-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6eeaa-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




