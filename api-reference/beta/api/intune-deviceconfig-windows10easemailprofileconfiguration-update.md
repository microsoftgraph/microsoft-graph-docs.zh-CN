---
title: 更新 windows10EasEmailProfileConfiguration
description: 更新 windows10EasEmailProfileConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62b038837d82f14d52f2697680eff459f3dfe48f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131118"
---
# <a name="update-windows10easemailprofileconfiguration"></a><span data-ttu-id="2651d-103">更新 windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="2651d-103">Update windows10EasEmailProfileConfiguration</span></span>

<span data-ttu-id="2651d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2651d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2651d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2651d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2651d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2651d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2651d-107">更新 [windows10EasEmailProfileConfiguration 对象](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="2651d-107">Update the properties of a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2651d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2651d-108">Prerequisites</span></span>
<span data-ttu-id="2651d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2651d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2651d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2651d-111">Permission type</span></span>|<span data-ttu-id="2651d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2651d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2651d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2651d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2651d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2651d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2651d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2651d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2651d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2651d-116">Not supported.</span></span>|
|<span data-ttu-id="2651d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2651d-117">Application</span></span>|<span data-ttu-id="2651d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2651d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2651d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2651d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2651d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2651d-120">Request headers</span></span>
|<span data-ttu-id="2651d-121">标头</span><span class="sxs-lookup"><span data-stu-id="2651d-121">Header</span></span>|<span data-ttu-id="2651d-122">值</span><span class="sxs-lookup"><span data-stu-id="2651d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2651d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2651d-123">Authorization</span></span>|<span data-ttu-id="2651d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2651d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2651d-125">接受</span><span class="sxs-lookup"><span data-stu-id="2651d-125">Accept</span></span>|<span data-ttu-id="2651d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2651d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2651d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2651d-127">Request body</span></span>
<span data-ttu-id="2651d-128">在请求正文中，提供 [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2651d-128">In the request body, supply a JSON representation for the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="2651d-129">下表显示创建 [windows10EasEmailProfileConfiguration 时所需的属性](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="2651d-129">The following table shows the properties that are required when you create the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="2651d-130">属性</span><span class="sxs-lookup"><span data-stu-id="2651d-130">Property</span></span>|<span data-ttu-id="2651d-131">类型</span><span class="sxs-lookup"><span data-stu-id="2651d-131">Type</span></span>|<span data-ttu-id="2651d-132">说明</span><span class="sxs-lookup"><span data-stu-id="2651d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2651d-133">id</span><span class="sxs-lookup"><span data-stu-id="2651d-133">id</span></span>|<span data-ttu-id="2651d-134">String</span><span class="sxs-lookup"><span data-stu-id="2651d-134">String</span></span>|<span data-ttu-id="2651d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2651d-135">Key of the entity.</span></span> <span data-ttu-id="2651d-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2651d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2651d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2651d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2651d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2651d-138">DateTimeOffset</span></span>|<span data-ttu-id="2651d-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2651d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2651d-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2651d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2651d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2651d-141">roleScopeTagIds</span></span>|<span data-ttu-id="2651d-142">String collection</span><span class="sxs-lookup"><span data-stu-id="2651d-142">String collection</span></span>|<span data-ttu-id="2651d-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2651d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2651d-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2651d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2651d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2651d-145">supportsScopeTags</span></span>|<span data-ttu-id="2651d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2651d-146">Boolean</span></span>|<span data-ttu-id="2651d-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="2651d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2651d-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="2651d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2651d-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="2651d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2651d-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2651d-150">This property is read-only.</span></span> <span data-ttu-id="2651d-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2651d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2651d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2651d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2651d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2651d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2651d-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="2651d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2651d-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2651d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2651d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2651d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2651d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2651d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2651d-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2651d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2651d-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2651d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2651d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2651d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2651d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2651d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2651d-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2651d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2651d-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2651d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2651d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2651d-164">createdDateTime</span></span>|<span data-ttu-id="2651d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2651d-165">DateTimeOffset</span></span>|<span data-ttu-id="2651d-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2651d-166">DateTime the object was created.</span></span> <span data-ttu-id="2651d-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2651d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2651d-168">说明</span><span class="sxs-lookup"><span data-stu-id="2651d-168">description</span></span>|<span data-ttu-id="2651d-169">String</span><span class="sxs-lookup"><span data-stu-id="2651d-169">String</span></span>|<span data-ttu-id="2651d-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2651d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2651d-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2651d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2651d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2651d-172">displayName</span></span>|<span data-ttu-id="2651d-173">String</span><span class="sxs-lookup"><span data-stu-id="2651d-173">String</span></span>|<span data-ttu-id="2651d-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2651d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2651d-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2651d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2651d-176">version</span><span class="sxs-lookup"><span data-stu-id="2651d-176">version</span></span>|<span data-ttu-id="2651d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2651d-177">Int32</span></span>|<span data-ttu-id="2651d-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2651d-178">Version of the device configuration.</span></span> <span data-ttu-id="2651d-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2651d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2651d-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="2651d-180">usernameSource</span></span>|[<span data-ttu-id="2651d-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="2651d-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="2651d-182">在设备上安装之前从 AAD 中选取并注入到此配置文件中的用户名属性。</span><span class="sxs-lookup"><span data-stu-id="2651d-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2651d-183">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="2651d-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="2651d-184">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="2651d-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="2651d-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="2651d-185">usernameAADSource</span></span>|[<span data-ttu-id="2651d-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="2651d-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="2651d-187">AAD 字段的名称，该字段将用于检索电子邮件配置文件的 UserName。</span><span class="sxs-lookup"><span data-stu-id="2651d-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="2651d-188">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="2651d-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="2651d-189">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="2651d-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="2651d-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="2651d-190">userDomainNameSource</span></span>|[<span data-ttu-id="2651d-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="2651d-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="2651d-192">UserDomainname 属性，在设备上安装之前从 AAD 中选取并注入到此配置文件中。</span><span class="sxs-lookup"><span data-stu-id="2651d-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2651d-193">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="2651d-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="2651d-194">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="2651d-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="2651d-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="2651d-195">customDomainName</span></span>|<span data-ttu-id="2651d-196">String</span><span class="sxs-lookup"><span data-stu-id="2651d-196">String</span></span>|<span data-ttu-id="2651d-197">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="2651d-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="2651d-198">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="2651d-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="2651d-199">accountName</span><span class="sxs-lookup"><span data-stu-id="2651d-199">accountName</span></span>|<span data-ttu-id="2651d-200">String</span><span class="sxs-lookup"><span data-stu-id="2651d-200">String</span></span>|<span data-ttu-id="2651d-201">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="2651d-201">Account name.</span></span>|
|<span data-ttu-id="2651d-202">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="2651d-202">syncCalendar</span></span>|<span data-ttu-id="2651d-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="2651d-203">Boolean</span></span>|<span data-ttu-id="2651d-204">是否同步日历。</span><span class="sxs-lookup"><span data-stu-id="2651d-204">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="2651d-205">syncContacts</span><span class="sxs-lookup"><span data-stu-id="2651d-205">syncContacts</span></span>|<span data-ttu-id="2651d-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="2651d-206">Boolean</span></span>|<span data-ttu-id="2651d-207">是否同步联系人。</span><span class="sxs-lookup"><span data-stu-id="2651d-207">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="2651d-208">syncTasks</span><span class="sxs-lookup"><span data-stu-id="2651d-208">syncTasks</span></span>|<span data-ttu-id="2651d-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="2651d-209">Boolean</span></span>|<span data-ttu-id="2651d-210">是否同步任务。</span><span class="sxs-lookup"><span data-stu-id="2651d-210">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="2651d-211">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="2651d-211">durationOfEmailToSync</span></span>|[<span data-ttu-id="2651d-212">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="2651d-212">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="2651d-213">要同步的电子邮件的持续时间。可能的值是 `userDefined` `oneDay` `threeDays` ：、、、、、、。 `oneWeek` `twoWeeks` `oneMonth` `unlimited`</span><span class="sxs-lookup"><span data-stu-id="2651d-213">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="2651d-214">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="2651d-214">emailAddressSource</span></span>|[<span data-ttu-id="2651d-215">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="2651d-215">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="2651d-216">从 AAD 中选取并注入到此配置文件中的电子邮件属性，在设备上安装之前。</span><span class="sxs-lookup"><span data-stu-id="2651d-216">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2651d-217">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="2651d-217">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="2651d-218">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="2651d-218">emailSyncSchedule</span></span>|[<span data-ttu-id="2651d-219">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="2651d-219">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="2651d-220">电子邮件同步计划。</span><span class="sxs-lookup"><span data-stu-id="2651d-220">Email sync schedule.</span></span> <span data-ttu-id="2651d-221">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes` 或 `basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="2651d-221">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="2651d-222">hostName</span><span class="sxs-lookup"><span data-stu-id="2651d-222">hostName</span></span>|<span data-ttu-id="2651d-223">String</span><span class="sxs-lookup"><span data-stu-id="2651d-223">String</span></span>|<span data-ttu-id="2651d-224">使用本机 (连接到) URL 的 Exchange 位置。</span><span class="sxs-lookup"><span data-stu-id="2651d-224">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="2651d-225">requireSsl</span><span class="sxs-lookup"><span data-stu-id="2651d-225">requireSsl</span></span>|<span data-ttu-id="2651d-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="2651d-226">Boolean</span></span>|<span data-ttu-id="2651d-227">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="2651d-227">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="2651d-228">响应</span><span class="sxs-lookup"><span data-stu-id="2651d-228">Response</span></span>
<span data-ttu-id="2651d-229">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2651d-229">If successful, this method returns a `200 OK` response code and an updated [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2651d-230">示例</span><span class="sxs-lookup"><span data-stu-id="2651d-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="2651d-231">请求</span><span class="sxs-lookup"><span data-stu-id="2651d-231">Request</span></span>
<span data-ttu-id="2651d-232">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2651d-232">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1526

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="2651d-233">响应</span><span class="sxs-lookup"><span data-stu-id="2651d-233">Response</span></span>
<span data-ttu-id="2651d-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2651d-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1698

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
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




