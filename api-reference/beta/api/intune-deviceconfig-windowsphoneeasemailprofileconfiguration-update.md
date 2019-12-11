---
title: 更新 windowsPhoneEASEmailProfileConfiguration
description: 更新 windowsPhoneEASEmailProfileConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26200701b50460af342158587eeb7176e0c04c8b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946425"
---
# <a name="update-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="2c97d-103">更新 windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c97d-103">Update windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="2c97d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2c97d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c97d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c97d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c97d-106">更新[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2c97d-106">Update the properties of a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c97d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2c97d-107">Prerequisites</span></span>
<span data-ttu-id="2c97d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c97d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c97d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c97d-110">Permission type</span></span>|<span data-ttu-id="2c97d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2c97d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c97d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c97d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c97d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c97d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c97d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c97d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c97d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c97d-115">Not supported.</span></span>|
|<span data-ttu-id="2c97d-116">Application</span><span class="sxs-lookup"><span data-stu-id="2c97d-116">Application</span></span>|<span data-ttu-id="2c97d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c97d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c97d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c97d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2c97d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c97d-119">Request headers</span></span>
|<span data-ttu-id="2c97d-120">标头</span><span class="sxs-lookup"><span data-stu-id="2c97d-120">Header</span></span>|<span data-ttu-id="2c97d-121">值</span><span class="sxs-lookup"><span data-stu-id="2c97d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c97d-122">授权</span><span class="sxs-lookup"><span data-stu-id="2c97d-122">Authorization</span></span>|<span data-ttu-id="2c97d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2c97d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c97d-124">接受</span><span class="sxs-lookup"><span data-stu-id="2c97d-124">Accept</span></span>|<span data-ttu-id="2c97d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c97d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c97d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c97d-126">Request body</span></span>
<span data-ttu-id="2c97d-127">在请求正文中，提供[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c97d-127">In the request body, supply a JSON representation for the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="2c97d-128">下表显示创建[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2c97d-128">The following table shows the properties that are required when you create the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="2c97d-129">属性</span><span class="sxs-lookup"><span data-stu-id="2c97d-129">Property</span></span>|<span data-ttu-id="2c97d-130">类型</span><span class="sxs-lookup"><span data-stu-id="2c97d-130">Type</span></span>|<span data-ttu-id="2c97d-131">说明</span><span class="sxs-lookup"><span data-stu-id="2c97d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c97d-132">id</span><span class="sxs-lookup"><span data-stu-id="2c97d-132">id</span></span>|<span data-ttu-id="2c97d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2c97d-133">String</span></span>|<span data-ttu-id="2c97d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2c97d-134">Key of the entity.</span></span> <span data-ttu-id="2c97d-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c97d-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c97d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c97d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2c97d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c97d-137">DateTimeOffset</span></span>|<span data-ttu-id="2c97d-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2c97d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2c97d-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c97d-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c97d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2c97d-140">roleScopeTagIds</span></span>|<span data-ttu-id="2c97d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="2c97d-141">String collection</span></span>|<span data-ttu-id="2c97d-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2c97d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2c97d-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c97d-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c97d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2c97d-144">supportsScopeTags</span></span>|<span data-ttu-id="2c97d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c97d-145">Boolean</span></span>|<span data-ttu-id="2c97d-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="2c97d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2c97d-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="2c97d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2c97d-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="2c97d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2c97d-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2c97d-149">This property is read-only.</span></span> <span data-ttu-id="2c97d-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c97d-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c97d-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2c97d-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2c97d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2c97d-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2c97d-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="2c97d-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2c97d-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c97d-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c97d-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2c97d-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2c97d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2c97d-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2c97d-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2c97d-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2c97d-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c97d-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c97d-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2c97d-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2c97d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2c97d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2c97d-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2c97d-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2c97d-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c97d-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c97d-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c97d-163">createdDateTime</span></span>|<span data-ttu-id="2c97d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c97d-164">DateTimeOffset</span></span>|<span data-ttu-id="2c97d-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2c97d-165">DateTime the object was created.</span></span> <span data-ttu-id="2c97d-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c97d-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c97d-167">说明</span><span class="sxs-lookup"><span data-stu-id="2c97d-167">description</span></span>|<span data-ttu-id="2c97d-168">String</span><span class="sxs-lookup"><span data-stu-id="2c97d-168">String</span></span>|<span data-ttu-id="2c97d-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2c97d-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2c97d-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c97d-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c97d-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2c97d-171">displayName</span></span>|<span data-ttu-id="2c97d-172">String</span><span class="sxs-lookup"><span data-stu-id="2c97d-172">String</span></span>|<span data-ttu-id="2c97d-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2c97d-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2c97d-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c97d-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c97d-175">version</span><span class="sxs-lookup"><span data-stu-id="2c97d-175">version</span></span>|<span data-ttu-id="2c97d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2c97d-176">Int32</span></span>|<span data-ttu-id="2c97d-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2c97d-177">Version of the device configuration.</span></span> <span data-ttu-id="2c97d-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c97d-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c97d-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="2c97d-179">usernameSource</span></span>|[<span data-ttu-id="2c97d-180">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="2c97d-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="2c97d-181">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="2c97d-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2c97d-182">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="2c97d-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="2c97d-183">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="2c97d-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="2c97d-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="2c97d-184">usernameAADSource</span></span>|[<span data-ttu-id="2c97d-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="2c97d-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="2c97d-186">AAD 字段的名称，将用于检索电子邮件配置文件的用户名。</span><span class="sxs-lookup"><span data-stu-id="2c97d-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="2c97d-187">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="2c97d-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="2c97d-188">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="2c97d-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="2c97d-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="2c97d-189">userDomainNameSource</span></span>|[<span data-ttu-id="2c97d-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="2c97d-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="2c97d-191">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="2c97d-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2c97d-192">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="2c97d-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="2c97d-193">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="2c97d-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="2c97d-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="2c97d-194">customDomainName</span></span>|<span data-ttu-id="2c97d-195">字符串</span><span class="sxs-lookup"><span data-stu-id="2c97d-195">String</span></span>|<span data-ttu-id="2c97d-196">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="2c97d-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="2c97d-197">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="2c97d-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="2c97d-198">帐户</span><span class="sxs-lookup"><span data-stu-id="2c97d-198">accountName</span></span>|<span data-ttu-id="2c97d-199">字符串</span><span class="sxs-lookup"><span data-stu-id="2c97d-199">String</span></span>|<span data-ttu-id="2c97d-200">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="2c97d-200">Account name.</span></span>|
|<span data-ttu-id="2c97d-201">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="2c97d-201">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="2c97d-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c97d-202">Boolean</span></span>|<span data-ttu-id="2c97d-203">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="2c97d-203">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="2c97d-204">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2c97d-204">This property is read-only.</span></span>|
|<span data-ttu-id="2c97d-205">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="2c97d-205">syncCalendar</span></span>|<span data-ttu-id="2c97d-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c97d-206">Boolean</span></span>|<span data-ttu-id="2c97d-207">是否同步日历。</span><span class="sxs-lookup"><span data-stu-id="2c97d-207">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="2c97d-208">syncContacts</span><span class="sxs-lookup"><span data-stu-id="2c97d-208">syncContacts</span></span>|<span data-ttu-id="2c97d-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c97d-209">Boolean</span></span>|<span data-ttu-id="2c97d-210">是否同步联系人。</span><span class="sxs-lookup"><span data-stu-id="2c97d-210">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="2c97d-211">syncTasks</span><span class="sxs-lookup"><span data-stu-id="2c97d-211">syncTasks</span></span>|<span data-ttu-id="2c97d-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c97d-212">Boolean</span></span>|<span data-ttu-id="2c97d-213">是否同步任务。</span><span class="sxs-lookup"><span data-stu-id="2c97d-213">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="2c97d-214">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="2c97d-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="2c97d-215">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="2c97d-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="2c97d-216">要同步的电子邮件的持续时间。可能的值为`userDefined`： `oneDay`、 `threeDays`、 `oneWeek` `twoWeeks`、、 `oneMonth`、 `unlimited`、。</span><span class="sxs-lookup"><span data-stu-id="2c97d-216">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="2c97d-217">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="2c97d-217">emailAddressSource</span></span>|[<span data-ttu-id="2c97d-218">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="2c97d-218">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="2c97d-219">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="2c97d-219">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2c97d-220">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="2c97d-220">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="2c97d-221">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="2c97d-221">emailSyncSchedule</span></span>|[<span data-ttu-id="2c97d-222">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="2c97d-222">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="2c97d-223">电子邮件同步计划。</span><span class="sxs-lookup"><span data-stu-id="2c97d-223">Email sync schedule.</span></span> <span data-ttu-id="2c97d-224">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes` 或 `basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="2c97d-224">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="2c97d-225">hostName</span><span class="sxs-lookup"><span data-stu-id="2c97d-225">hostName</span></span>|<span data-ttu-id="2c97d-226">String</span><span class="sxs-lookup"><span data-stu-id="2c97d-226">String</span></span>|<span data-ttu-id="2c97d-227">本机邮件应用程序连接到的 Exchange 位置（URL）。</span><span class="sxs-lookup"><span data-stu-id="2c97d-227">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="2c97d-228">requireSsl</span><span class="sxs-lookup"><span data-stu-id="2c97d-228">requireSsl</span></span>|<span data-ttu-id="2c97d-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c97d-229">Boolean</span></span>|<span data-ttu-id="2c97d-230">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="2c97d-230">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="2c97d-231">响应</span><span class="sxs-lookup"><span data-stu-id="2c97d-231">Response</span></span>
<span data-ttu-id="2c97d-232">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2c97d-232">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c97d-233">示例</span><span class="sxs-lookup"><span data-stu-id="2c97d-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c97d-234">请求</span><span class="sxs-lookup"><span data-stu-id="2c97d-234">Request</span></span>
<span data-ttu-id="2c97d-235">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c97d-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2c97d-236">响应</span><span class="sxs-lookup"><span data-stu-id="2c97d-236">Response</span></span>
<span data-ttu-id="2c97d-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c97d-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





