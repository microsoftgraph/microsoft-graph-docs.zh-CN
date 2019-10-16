---
title: 创建 windows10EasEmailProfileConfiguration
description: 创建新的 windows10EasEmailProfileConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 933f95ac8adbf46932b2c17892349fb8535f0eb3
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533241"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="c715c-103">创建 windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="c715c-103">Create windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="c715c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c715c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c715c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c715c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c715c-106">创建新的[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c715c-106">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c715c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c715c-107">Prerequisites</span></span>
<span data-ttu-id="c715c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c715c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c715c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c715c-110">Permission type</span></span>|<span data-ttu-id="c715c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c715c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c715c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c715c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c715c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c715c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c715c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c715c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c715c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c715c-115">Not supported.</span></span>|
|<span data-ttu-id="c715c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c715c-116">Application</span></span>|<span data-ttu-id="c715c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c715c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c715c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c715c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c715c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c715c-119">Request headers</span></span>
|<span data-ttu-id="c715c-120">标头</span><span class="sxs-lookup"><span data-stu-id="c715c-120">Header</span></span>|<span data-ttu-id="c715c-121">值</span><span class="sxs-lookup"><span data-stu-id="c715c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c715c-122">授权</span><span class="sxs-lookup"><span data-stu-id="c715c-122">Authorization</span></span>|<span data-ttu-id="c715c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c715c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c715c-124">接受</span><span class="sxs-lookup"><span data-stu-id="c715c-124">Accept</span></span>|<span data-ttu-id="c715c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c715c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c715c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c715c-126">Request body</span></span>
<span data-ttu-id="c715c-127">在请求正文中，提供 windows10EasEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c715c-127">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="c715c-128">下表显示创建 windows10EasEmailProfileConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c715c-128">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="c715c-129">属性</span><span class="sxs-lookup"><span data-stu-id="c715c-129">Property</span></span>|<span data-ttu-id="c715c-130">类型</span><span class="sxs-lookup"><span data-stu-id="c715c-130">Type</span></span>|<span data-ttu-id="c715c-131">说明</span><span class="sxs-lookup"><span data-stu-id="c715c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c715c-132">id</span><span class="sxs-lookup"><span data-stu-id="c715c-132">id</span></span>|<span data-ttu-id="c715c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c715c-133">String</span></span>|<span data-ttu-id="c715c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c715c-134">Key of the entity.</span></span> <span data-ttu-id="c715c-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c715c-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c715c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c715c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c715c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c715c-137">DateTimeOffset</span></span>|<span data-ttu-id="c715c-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c715c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c715c-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c715c-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c715c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c715c-140">roleScopeTagIds</span></span>|<span data-ttu-id="c715c-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="c715c-141">String collection</span></span>|<span data-ttu-id="c715c-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c715c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c715c-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c715c-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c715c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c715c-144">supportsScopeTags</span></span>|<span data-ttu-id="c715c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c715c-145">Boolean</span></span>|<span data-ttu-id="c715c-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c715c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c715c-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c715c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c715c-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c715c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c715c-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c715c-149">This property is read-only.</span></span> <span data-ttu-id="c715c-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c715c-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c715c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c715c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c715c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c715c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c715c-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c715c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c715c-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c715c-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c715c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c715c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c715c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c715c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c715c-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c715c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c715c-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c715c-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c715c-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c715c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c715c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c715c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c715c-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c715c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c715c-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c715c-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c715c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c715c-163">createdDateTime</span></span>|<span data-ttu-id="c715c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c715c-164">DateTimeOffset</span></span>|<span data-ttu-id="c715c-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c715c-165">DateTime the object was created.</span></span> <span data-ttu-id="c715c-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c715c-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c715c-167">说明</span><span class="sxs-lookup"><span data-stu-id="c715c-167">description</span></span>|<span data-ttu-id="c715c-168">String</span><span class="sxs-lookup"><span data-stu-id="c715c-168">String</span></span>|<span data-ttu-id="c715c-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c715c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c715c-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c715c-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c715c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c715c-171">displayName</span></span>|<span data-ttu-id="c715c-172">String</span><span class="sxs-lookup"><span data-stu-id="c715c-172">String</span></span>|<span data-ttu-id="c715c-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c715c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c715c-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c715c-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c715c-175">version</span><span class="sxs-lookup"><span data-stu-id="c715c-175">version</span></span>|<span data-ttu-id="c715c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c715c-176">Int32</span></span>|<span data-ttu-id="c715c-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c715c-177">Version of the device configuration.</span></span> <span data-ttu-id="c715c-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c715c-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c715c-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c715c-179">usernameSource</span></span>|[<span data-ttu-id="c715c-180">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="c715c-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c715c-181">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="c715c-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c715c-182">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="c715c-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c715c-183">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="c715c-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c715c-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="c715c-184">usernameAADSource</span></span>|[<span data-ttu-id="c715c-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c715c-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="c715c-186">AAD 字段的名称，将用于检索电子邮件配置文件的用户名。</span><span class="sxs-lookup"><span data-stu-id="c715c-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="c715c-187">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="c715c-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c715c-188">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="c715c-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="c715c-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="c715c-189">userDomainNameSource</span></span>|[<span data-ttu-id="c715c-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="c715c-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="c715c-191">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="c715c-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c715c-192">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="c715c-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c715c-193">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="c715c-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="c715c-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="c715c-194">customDomainName</span></span>|<span data-ttu-id="c715c-195">字符串</span><span class="sxs-lookup"><span data-stu-id="c715c-195">String</span></span>|<span data-ttu-id="c715c-196">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="c715c-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="c715c-197">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="c715c-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="c715c-198">帐户</span><span class="sxs-lookup"><span data-stu-id="c715c-198">accountName</span></span>|<span data-ttu-id="c715c-199">字符串</span><span class="sxs-lookup"><span data-stu-id="c715c-199">String</span></span>|<span data-ttu-id="c715c-200">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="c715c-200">Account name.</span></span>|
|<span data-ttu-id="c715c-201">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="c715c-201">syncCalendar</span></span>|<span data-ttu-id="c715c-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="c715c-202">Boolean</span></span>|<span data-ttu-id="c715c-203">是否同步日历。</span><span class="sxs-lookup"><span data-stu-id="c715c-203">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="c715c-204">syncContacts</span><span class="sxs-lookup"><span data-stu-id="c715c-204">syncContacts</span></span>|<span data-ttu-id="c715c-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="c715c-205">Boolean</span></span>|<span data-ttu-id="c715c-206">是否同步联系人。</span><span class="sxs-lookup"><span data-stu-id="c715c-206">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="c715c-207">syncTasks</span><span class="sxs-lookup"><span data-stu-id="c715c-207">syncTasks</span></span>|<span data-ttu-id="c715c-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="c715c-208">Boolean</span></span>|<span data-ttu-id="c715c-209">是否同步任务。</span><span class="sxs-lookup"><span data-stu-id="c715c-209">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="c715c-210">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="c715c-210">durationOfEmailToSync</span></span>|[<span data-ttu-id="c715c-211">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="c715c-211">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="c715c-212">要同步的电子邮件的持续时间。可能的值为`userDefined`： `oneDay`、 `threeDays`、 `oneWeek` `twoWeeks`、、 `oneMonth`、 `unlimited`、。</span><span class="sxs-lookup"><span data-stu-id="c715c-212">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="c715c-213">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="c715c-213">emailAddressSource</span></span>|[<span data-ttu-id="c715c-214">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="c715c-214">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c715c-215">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="c715c-215">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c715c-216">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="c715c-216">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c715c-217">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="c715c-217">emailSyncSchedule</span></span>|[<span data-ttu-id="c715c-218">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="c715c-218">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="c715c-219">电子邮件同步计划。</span><span class="sxs-lookup"><span data-stu-id="c715c-219">Email sync schedule.</span></span> <span data-ttu-id="c715c-220">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes` 或 `basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="c715c-220">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="c715c-221">hostName</span><span class="sxs-lookup"><span data-stu-id="c715c-221">hostName</span></span>|<span data-ttu-id="c715c-222">String</span><span class="sxs-lookup"><span data-stu-id="c715c-222">String</span></span>|<span data-ttu-id="c715c-223">本机邮件应用程序连接到的 Exchange 位置（URL）。</span><span class="sxs-lookup"><span data-stu-id="c715c-223">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="c715c-224">requireSsl</span><span class="sxs-lookup"><span data-stu-id="c715c-224">requireSsl</span></span>|<span data-ttu-id="c715c-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c715c-225">Boolean</span></span>|<span data-ttu-id="c715c-226">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="c715c-226">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="c715c-227">响应</span><span class="sxs-lookup"><span data-stu-id="c715c-227">Response</span></span>
<span data-ttu-id="c715c-228">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c715c-228">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c715c-229">示例</span><span class="sxs-lookup"><span data-stu-id="c715c-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="c715c-230">请求</span><span class="sxs-lookup"><span data-stu-id="c715c-230">Request</span></span>
<span data-ttu-id="c715c-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c715c-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="c715c-232">响应</span><span class="sxs-lookup"><span data-stu-id="c715c-232">Response</span></span>
<span data-ttu-id="c715c-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c715c-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






