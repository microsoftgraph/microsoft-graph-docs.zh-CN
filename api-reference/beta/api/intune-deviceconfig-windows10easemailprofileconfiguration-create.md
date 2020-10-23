---
title: 创建 windows10EasEmailProfileConfiguration
description: 创建新的 windows10EasEmailProfileConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0bc103de91c4c03a9ecef77f8f0fd72ade66045f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734887"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="9ce61-103">创建 windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="9ce61-103">Create windows10EasEmailProfileConfiguration</span></span>

<span data-ttu-id="9ce61-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ce61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ce61-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9ce61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ce61-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ce61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ce61-107">创建新的 [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ce61-107">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ce61-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9ce61-108">Prerequisites</span></span>
<span data-ttu-id="9ce61-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ce61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ce61-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ce61-111">Permission type</span></span>|<span data-ttu-id="9ce61-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9ce61-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ce61-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ce61-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ce61-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ce61-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ce61-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ce61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ce61-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ce61-116">Not supported.</span></span>|
|<span data-ttu-id="9ce61-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ce61-117">Application</span></span>|<span data-ttu-id="9ce61-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ce61-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ce61-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ce61-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9ce61-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ce61-120">Request headers</span></span>
|<span data-ttu-id="9ce61-121">标头</span><span class="sxs-lookup"><span data-stu-id="9ce61-121">Header</span></span>|<span data-ttu-id="9ce61-122">值</span><span class="sxs-lookup"><span data-stu-id="9ce61-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ce61-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ce61-123">Authorization</span></span>|<span data-ttu-id="9ce61-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9ce61-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ce61-125">接受</span><span class="sxs-lookup"><span data-stu-id="9ce61-125">Accept</span></span>|<span data-ttu-id="9ce61-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ce61-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ce61-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ce61-127">Request body</span></span>
<span data-ttu-id="9ce61-128">在请求正文中，提供 windows10EasEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ce61-128">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="9ce61-129">下表显示创建 windows10EasEmailProfileConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9ce61-129">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="9ce61-130">属性</span><span class="sxs-lookup"><span data-stu-id="9ce61-130">Property</span></span>|<span data-ttu-id="9ce61-131">类型</span><span class="sxs-lookup"><span data-stu-id="9ce61-131">Type</span></span>|<span data-ttu-id="9ce61-132">说明</span><span class="sxs-lookup"><span data-stu-id="9ce61-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ce61-133">id</span><span class="sxs-lookup"><span data-stu-id="9ce61-133">id</span></span>|<span data-ttu-id="9ce61-134">String</span><span class="sxs-lookup"><span data-stu-id="9ce61-134">String</span></span>|<span data-ttu-id="9ce61-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9ce61-135">Key of the entity.</span></span> <span data-ttu-id="9ce61-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ce61-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ce61-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ce61-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9ce61-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ce61-138">DateTimeOffset</span></span>|<span data-ttu-id="9ce61-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9ce61-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9ce61-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ce61-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ce61-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ce61-141">roleScopeTagIds</span></span>|<span data-ttu-id="9ce61-142">String collection</span><span class="sxs-lookup"><span data-stu-id="9ce61-142">String collection</span></span>|<span data-ttu-id="9ce61-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9ce61-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ce61-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ce61-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ce61-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9ce61-145">supportsScopeTags</span></span>|<span data-ttu-id="9ce61-146">布尔</span><span class="sxs-lookup"><span data-stu-id="9ce61-146">Boolean</span></span>|<span data-ttu-id="9ce61-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="9ce61-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9ce61-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="9ce61-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9ce61-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="9ce61-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9ce61-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9ce61-150">This property is read-only.</span></span> <span data-ttu-id="9ce61-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ce61-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ce61-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9ce61-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9ce61-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9ce61-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9ce61-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9ce61-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9ce61-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ce61-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ce61-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9ce61-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9ce61-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9ce61-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9ce61-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9ce61-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9ce61-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ce61-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ce61-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9ce61-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9ce61-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9ce61-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9ce61-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9ce61-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9ce61-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ce61-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ce61-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ce61-164">createdDateTime</span></span>|<span data-ttu-id="9ce61-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ce61-165">DateTimeOffset</span></span>|<span data-ttu-id="9ce61-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9ce61-166">DateTime the object was created.</span></span> <span data-ttu-id="9ce61-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ce61-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ce61-168">说明</span><span class="sxs-lookup"><span data-stu-id="9ce61-168">description</span></span>|<span data-ttu-id="9ce61-169">String</span><span class="sxs-lookup"><span data-stu-id="9ce61-169">String</span></span>|<span data-ttu-id="9ce61-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9ce61-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ce61-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ce61-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ce61-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9ce61-172">displayName</span></span>|<span data-ttu-id="9ce61-173">String</span><span class="sxs-lookup"><span data-stu-id="9ce61-173">String</span></span>|<span data-ttu-id="9ce61-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9ce61-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ce61-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ce61-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ce61-176">version</span><span class="sxs-lookup"><span data-stu-id="9ce61-176">version</span></span>|<span data-ttu-id="9ce61-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9ce61-177">Int32</span></span>|<span data-ttu-id="9ce61-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9ce61-178">Version of the device configuration.</span></span> <span data-ttu-id="9ce61-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ce61-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ce61-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="9ce61-180">usernameSource</span></span>|[<span data-ttu-id="9ce61-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="9ce61-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="9ce61-182">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="9ce61-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9ce61-183">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="9ce61-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9ce61-184">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="9ce61-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9ce61-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="9ce61-185">usernameAADSource</span></span>|[<span data-ttu-id="9ce61-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="9ce61-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="9ce61-187">AAD 字段的名称，将用于检索电子邮件配置文件的用户名。</span><span class="sxs-lookup"><span data-stu-id="9ce61-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="9ce61-188">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="9ce61-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9ce61-189">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="9ce61-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="9ce61-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="9ce61-190">userDomainNameSource</span></span>|[<span data-ttu-id="9ce61-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="9ce61-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="9ce61-192">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="9ce61-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9ce61-193">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="9ce61-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9ce61-194">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="9ce61-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="9ce61-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="9ce61-195">customDomainName</span></span>|<span data-ttu-id="9ce61-196">String</span><span class="sxs-lookup"><span data-stu-id="9ce61-196">String</span></span>|<span data-ttu-id="9ce61-197">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="9ce61-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="9ce61-198">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="9ce61-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="9ce61-199">帐户</span><span class="sxs-lookup"><span data-stu-id="9ce61-199">accountName</span></span>|<span data-ttu-id="9ce61-200">String</span><span class="sxs-lookup"><span data-stu-id="9ce61-200">String</span></span>|<span data-ttu-id="9ce61-201">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="9ce61-201">Account name.</span></span>|
|<span data-ttu-id="9ce61-202">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="9ce61-202">syncCalendar</span></span>|<span data-ttu-id="9ce61-203">布尔</span><span class="sxs-lookup"><span data-stu-id="9ce61-203">Boolean</span></span>|<span data-ttu-id="9ce61-204">是否同步日历。</span><span class="sxs-lookup"><span data-stu-id="9ce61-204">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="9ce61-205">syncContacts</span><span class="sxs-lookup"><span data-stu-id="9ce61-205">syncContacts</span></span>|<span data-ttu-id="9ce61-206">布尔</span><span class="sxs-lookup"><span data-stu-id="9ce61-206">Boolean</span></span>|<span data-ttu-id="9ce61-207">是否同步联系人。</span><span class="sxs-lookup"><span data-stu-id="9ce61-207">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="9ce61-208">syncTasks</span><span class="sxs-lookup"><span data-stu-id="9ce61-208">syncTasks</span></span>|<span data-ttu-id="9ce61-209">布尔</span><span class="sxs-lookup"><span data-stu-id="9ce61-209">Boolean</span></span>|<span data-ttu-id="9ce61-210">是否同步任务。</span><span class="sxs-lookup"><span data-stu-id="9ce61-210">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="9ce61-211">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="9ce61-211">durationOfEmailToSync</span></span>|[<span data-ttu-id="9ce61-212">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="9ce61-212">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="9ce61-213">要同步的电子邮件的持续时间。可能的值为：、、、、、 `userDefined` `oneDay` `threeDays` `oneWeek` `twoWeeks` `oneMonth` 、 `unlimited` 。</span><span class="sxs-lookup"><span data-stu-id="9ce61-213">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="9ce61-214">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="9ce61-214">emailAddressSource</span></span>|[<span data-ttu-id="9ce61-215">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="9ce61-215">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="9ce61-216">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="9ce61-216">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9ce61-217">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="9ce61-217">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9ce61-218">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="9ce61-218">emailSyncSchedule</span></span>|[<span data-ttu-id="9ce61-219">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="9ce61-219">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="9ce61-220">电子邮件同步计划。</span><span class="sxs-lookup"><span data-stu-id="9ce61-220">Email sync schedule.</span></span> <span data-ttu-id="9ce61-221">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes` 或 `basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="9ce61-221">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="9ce61-222">hostName</span><span class="sxs-lookup"><span data-stu-id="9ce61-222">hostName</span></span>|<span data-ttu-id="9ce61-223">String</span><span class="sxs-lookup"><span data-stu-id="9ce61-223">String</span></span>|<span data-ttu-id="9ce61-224">本地邮件应用程序连接到 (URL) 的 Exchange 位置。</span><span class="sxs-lookup"><span data-stu-id="9ce61-224">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="9ce61-225">requireSsl</span><span class="sxs-lookup"><span data-stu-id="9ce61-225">requireSsl</span></span>|<span data-ttu-id="9ce61-226">布尔</span><span class="sxs-lookup"><span data-stu-id="9ce61-226">Boolean</span></span>|<span data-ttu-id="9ce61-227">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="9ce61-227">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="9ce61-228">响应</span><span class="sxs-lookup"><span data-stu-id="9ce61-228">Response</span></span>
<span data-ttu-id="9ce61-229">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ce61-229">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ce61-230">示例</span><span class="sxs-lookup"><span data-stu-id="9ce61-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ce61-231">请求</span><span class="sxs-lookup"><span data-stu-id="9ce61-231">Request</span></span>
<span data-ttu-id="9ce61-232">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ce61-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ce61-233">响应</span><span class="sxs-lookup"><span data-stu-id="9ce61-233">Response</span></span>
<span data-ttu-id="9ce61-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9ce61-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





