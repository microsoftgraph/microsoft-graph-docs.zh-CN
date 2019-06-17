---
title: 创建 windowsPhoneEASEmailProfileConfiguration
description: 创建新的 windowsPhoneEASEmailProfileConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c39dfe88b5e2a4bddc91991f85e7395d7f074d6d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961488"
---
# <a name="create-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="4fdcc-103">创建 windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="4fdcc-103">Create windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="4fdcc-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fdcc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fdcc-106">创建新的[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-106">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fdcc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4fdcc-107">Prerequisites</span></span>
<span data-ttu-id="4fdcc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fdcc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fdcc-110">Permission type</span></span>|<span data-ttu-id="4fdcc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4fdcc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fdcc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fdcc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4fdcc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fdcc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4fdcc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fdcc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fdcc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-115">Not supported.</span></span>|
|<span data-ttu-id="4fdcc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4fdcc-116">Application</span></span>|<span data-ttu-id="4fdcc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fdcc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fdcc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4fdcc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fdcc-119">Request headers</span></span>
|<span data-ttu-id="4fdcc-120">标头</span><span class="sxs-lookup"><span data-stu-id="4fdcc-120">Header</span></span>|<span data-ttu-id="4fdcc-121">值</span><span class="sxs-lookup"><span data-stu-id="4fdcc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fdcc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fdcc-122">Authorization</span></span>|<span data-ttu-id="4fdcc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fdcc-124">接受</span><span class="sxs-lookup"><span data-stu-id="4fdcc-124">Accept</span></span>|<span data-ttu-id="4fdcc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4fdcc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fdcc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fdcc-126">Request body</span></span>
<span data-ttu-id="4fdcc-127">在请求正文中, 提供 windowsPhoneEASEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-127">In the request body, supply a JSON representation for the windowsPhoneEASEmailProfileConfiguration object.</span></span>

<span data-ttu-id="4fdcc-128">下表显示创建 windowsPhoneEASEmailProfileConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-128">The following table shows the properties that are required when you create the windowsPhoneEASEmailProfileConfiguration.</span></span>

|<span data-ttu-id="4fdcc-129">属性</span><span class="sxs-lookup"><span data-stu-id="4fdcc-129">Property</span></span>|<span data-ttu-id="4fdcc-130">类型</span><span class="sxs-lookup"><span data-stu-id="4fdcc-130">Type</span></span>|<span data-ttu-id="4fdcc-131">说明</span><span class="sxs-lookup"><span data-stu-id="4fdcc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fdcc-132">id</span><span class="sxs-lookup"><span data-stu-id="4fdcc-132">id</span></span>|<span data-ttu-id="4fdcc-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4fdcc-133">String</span></span>|<span data-ttu-id="4fdcc-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-134">Key of the entity.</span></span> <span data-ttu-id="4fdcc-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4fdcc-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fdcc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4fdcc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4fdcc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fdcc-137">DateTimeOffset</span></span>|<span data-ttu-id="4fdcc-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4fdcc-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4fdcc-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fdcc-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4fdcc-140">roleScopeTagIds</span></span>|<span data-ttu-id="4fdcc-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4fdcc-141">String collection</span></span>|<span data-ttu-id="4fdcc-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4fdcc-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4fdcc-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fdcc-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4fdcc-144">supportsScopeTags</span></span>|<span data-ttu-id="4fdcc-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fdcc-145">Boolean</span></span>|<span data-ttu-id="4fdcc-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4fdcc-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4fdcc-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4fdcc-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-149">This property is read-only.</span></span> <span data-ttu-id="4fdcc-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4fdcc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fdcc-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4fdcc-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4fdcc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4fdcc-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4fdcc-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4fdcc-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4fdcc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fdcc-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4fdcc-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4fdcc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4fdcc-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4fdcc-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4fdcc-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4fdcc-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fdcc-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4fdcc-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4fdcc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4fdcc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4fdcc-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4fdcc-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4fdcc-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fdcc-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4fdcc-163">createdDateTime</span></span>|<span data-ttu-id="4fdcc-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fdcc-164">DateTimeOffset</span></span>|<span data-ttu-id="4fdcc-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-165">DateTime the object was created.</span></span> <span data-ttu-id="4fdcc-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4fdcc-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fdcc-167">说明</span><span class="sxs-lookup"><span data-stu-id="4fdcc-167">description</span></span>|<span data-ttu-id="4fdcc-168">String</span><span class="sxs-lookup"><span data-stu-id="4fdcc-168">String</span></span>|<span data-ttu-id="4fdcc-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4fdcc-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4fdcc-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fdcc-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4fdcc-171">displayName</span></span>|<span data-ttu-id="4fdcc-172">String</span><span class="sxs-lookup"><span data-stu-id="4fdcc-172">String</span></span>|<span data-ttu-id="4fdcc-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4fdcc-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4fdcc-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fdcc-175">version</span><span class="sxs-lookup"><span data-stu-id="4fdcc-175">version</span></span>|<span data-ttu-id="4fdcc-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4fdcc-176">Int32</span></span>|<span data-ttu-id="4fdcc-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-177">Version of the device configuration.</span></span> <span data-ttu-id="4fdcc-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4fdcc-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fdcc-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4fdcc-179">usernameSource</span></span>|[<span data-ttu-id="4fdcc-180">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="4fdcc-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4fdcc-181">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4fdcc-182">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4fdcc-183">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4fdcc-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="4fdcc-184">usernameAADSource</span></span>|[<span data-ttu-id="4fdcc-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4fdcc-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="4fdcc-186">AAD 字段的名称, 将用于检索电子邮件配置文件的用户名。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="4fdcc-187">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4fdcc-188">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="4fdcc-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="4fdcc-189">userDomainNameSource</span></span>|[<span data-ttu-id="4fdcc-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="4fdcc-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="4fdcc-191">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4fdcc-192">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4fdcc-193">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="4fdcc-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="4fdcc-194">customDomainName</span></span>|<span data-ttu-id="4fdcc-195">String</span><span class="sxs-lookup"><span data-stu-id="4fdcc-195">String</span></span>|<span data-ttu-id="4fdcc-196">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="4fdcc-197">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="4fdcc-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="4fdcc-198">帐户</span><span class="sxs-lookup"><span data-stu-id="4fdcc-198">accountName</span></span>|<span data-ttu-id="4fdcc-199">String</span><span class="sxs-lookup"><span data-stu-id="4fdcc-199">String</span></span>|<span data-ttu-id="4fdcc-200">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-200">Account name.</span></span>|
|<span data-ttu-id="4fdcc-201">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="4fdcc-201">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="4fdcc-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fdcc-202">Boolean</span></span>|<span data-ttu-id="4fdcc-203">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-203">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="4fdcc-204">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-204">This property is read-only.</span></span>|
|<span data-ttu-id="4fdcc-205">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="4fdcc-205">syncCalendar</span></span>|<span data-ttu-id="4fdcc-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fdcc-206">Boolean</span></span>|<span data-ttu-id="4fdcc-207">是否同步日历。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-207">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="4fdcc-208">syncContacts</span><span class="sxs-lookup"><span data-stu-id="4fdcc-208">syncContacts</span></span>|<span data-ttu-id="4fdcc-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fdcc-209">Boolean</span></span>|<span data-ttu-id="4fdcc-210">是否同步联系人。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-210">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="4fdcc-211">syncTasks</span><span class="sxs-lookup"><span data-stu-id="4fdcc-211">syncTasks</span></span>|<span data-ttu-id="4fdcc-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fdcc-212">Boolean</span></span>|<span data-ttu-id="4fdcc-213">是否同步任务。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-213">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="4fdcc-214">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="4fdcc-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="4fdcc-215">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="4fdcc-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="4fdcc-216">要同步的电子邮件的持续时间。可能的值为`userDefined`: `oneDay`、 `threeDays`、 `oneWeek` `twoWeeks`、、 `oneMonth`、 `unlimited`、。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-216">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="4fdcc-217">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="4fdcc-217">emailAddressSource</span></span>|[<span data-ttu-id="4fdcc-218">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="4fdcc-218">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4fdcc-219">在设备上安装之前, 从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-219">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4fdcc-220">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-220">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4fdcc-221">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="4fdcc-221">emailSyncSchedule</span></span>|[<span data-ttu-id="4fdcc-222">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="4fdcc-222">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="4fdcc-223">电子邮件同步计划。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-223">Email sync schedule.</span></span> <span data-ttu-id="4fdcc-224">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes` 或 `basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-224">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="4fdcc-225">hostName</span><span class="sxs-lookup"><span data-stu-id="4fdcc-225">hostName</span></span>|<span data-ttu-id="4fdcc-226">String</span><span class="sxs-lookup"><span data-stu-id="4fdcc-226">String</span></span>|<span data-ttu-id="4fdcc-227">本机邮件应用程序连接到的 Exchange 位置 (URL)。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-227">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="4fdcc-228">requireSsl</span><span class="sxs-lookup"><span data-stu-id="4fdcc-228">requireSsl</span></span>|<span data-ttu-id="4fdcc-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fdcc-229">Boolean</span></span>|<span data-ttu-id="4fdcc-230">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-230">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="4fdcc-231">响应</span><span class="sxs-lookup"><span data-stu-id="4fdcc-231">Response</span></span>
<span data-ttu-id="4fdcc-232">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-232">If successful, this method returns a `201 Created` response code and a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fdcc-233">示例</span><span class="sxs-lookup"><span data-stu-id="4fdcc-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fdcc-234">请求</span><span class="sxs-lookup"><span data-stu-id="4fdcc-234">Request</span></span>
<span data-ttu-id="4fdcc-235">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4fdcc-236">响应</span><span class="sxs-lookup"><span data-stu-id="4fdcc-236">Response</span></span>
<span data-ttu-id="4fdcc-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4fdcc-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





