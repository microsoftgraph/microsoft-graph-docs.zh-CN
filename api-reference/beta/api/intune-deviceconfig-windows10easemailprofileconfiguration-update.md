---
title: 更新 windows10EasEmailProfileConfiguration
description: 更新 windows10EasEmailProfileConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8db1a25f4211794e95b177f63ae7f2b3d9f4c0eb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986803"
---
# <a name="update-windows10easemailprofileconfiguration"></a><span data-ttu-id="0e4ba-103">更新 windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e4ba-103">Update windows10EasEmailProfileConfiguration</span></span>

<span data-ttu-id="0e4ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e4ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e4ba-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e4ba-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e4ba-107">更新 [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-107">Update the properties of a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e4ba-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0e4ba-108">Prerequisites</span></span>
<span data-ttu-id="0e4ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e4ba-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e4ba-111">Permission type</span></span>|<span data-ttu-id="0e4ba-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0e4ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e4ba-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e4ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e4ba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e4ba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e4ba-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e4ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e4ba-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-116">Not supported.</span></span>|
|<span data-ttu-id="0e4ba-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e4ba-117">Application</span></span>|<span data-ttu-id="0e4ba-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e4ba-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e4ba-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e4ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0e4ba-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e4ba-120">Request headers</span></span>
|<span data-ttu-id="0e4ba-121">标头</span><span class="sxs-lookup"><span data-stu-id="0e4ba-121">Header</span></span>|<span data-ttu-id="0e4ba-122">值</span><span class="sxs-lookup"><span data-stu-id="0e4ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e4ba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e4ba-123">Authorization</span></span>|<span data-ttu-id="0e4ba-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e4ba-125">接受</span><span class="sxs-lookup"><span data-stu-id="0e4ba-125">Accept</span></span>|<span data-ttu-id="0e4ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e4ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e4ba-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e4ba-127">Request body</span></span>
<span data-ttu-id="0e4ba-128">在请求正文中，提供 [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-128">In the request body, supply a JSON representation for the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="0e4ba-129">下表显示创建 [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-129">The following table shows the properties that are required when you create the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="0e4ba-130">属性</span><span class="sxs-lookup"><span data-stu-id="0e4ba-130">Property</span></span>|<span data-ttu-id="0e4ba-131">类型</span><span class="sxs-lookup"><span data-stu-id="0e4ba-131">Type</span></span>|<span data-ttu-id="0e4ba-132">说明</span><span class="sxs-lookup"><span data-stu-id="0e4ba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e4ba-133">id</span><span class="sxs-lookup"><span data-stu-id="0e4ba-133">id</span></span>|<span data-ttu-id="0e4ba-134">String</span><span class="sxs-lookup"><span data-stu-id="0e4ba-134">String</span></span>|<span data-ttu-id="0e4ba-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-135">Key of the entity.</span></span> <span data-ttu-id="0e4ba-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4ba-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4ba-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e4ba-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0e4ba-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e4ba-138">DateTimeOffset</span></span>|<span data-ttu-id="0e4ba-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0e4ba-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4ba-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4ba-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e4ba-141">roleScopeTagIds</span></span>|<span data-ttu-id="0e4ba-142">String collection</span><span class="sxs-lookup"><span data-stu-id="0e4ba-142">String collection</span></span>|<span data-ttu-id="0e4ba-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0e4ba-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4ba-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4ba-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0e4ba-145">supportsScopeTags</span></span>|<span data-ttu-id="0e4ba-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e4ba-146">Boolean</span></span>|<span data-ttu-id="0e4ba-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0e4ba-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0e4ba-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0e4ba-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-150">This property is read-only.</span></span> <span data-ttu-id="0e4ba-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4ba-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4ba-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0e4ba-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0e4ba-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0e4ba-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0e4ba-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0e4ba-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4ba-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4ba-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0e4ba-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0e4ba-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0e4ba-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0e4ba-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0e4ba-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4ba-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4ba-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0e4ba-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0e4ba-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0e4ba-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0e4ba-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0e4ba-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4ba-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4ba-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e4ba-164">createdDateTime</span></span>|<span data-ttu-id="0e4ba-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e4ba-165">DateTimeOffset</span></span>|<span data-ttu-id="0e4ba-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-166">DateTime the object was created.</span></span> <span data-ttu-id="0e4ba-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4ba-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4ba-168">description</span><span class="sxs-lookup"><span data-stu-id="0e4ba-168">description</span></span>|<span data-ttu-id="0e4ba-169">String</span><span class="sxs-lookup"><span data-stu-id="0e4ba-169">String</span></span>|<span data-ttu-id="0e4ba-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0e4ba-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4ba-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4ba-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0e4ba-172">displayName</span></span>|<span data-ttu-id="0e4ba-173">String</span><span class="sxs-lookup"><span data-stu-id="0e4ba-173">String</span></span>|<span data-ttu-id="0e4ba-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0e4ba-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4ba-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4ba-176">version</span><span class="sxs-lookup"><span data-stu-id="0e4ba-176">version</span></span>|<span data-ttu-id="0e4ba-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0e4ba-177">Int32</span></span>|<span data-ttu-id="0e4ba-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-178">Version of the device configuration.</span></span> <span data-ttu-id="0e4ba-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4ba-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4ba-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="0e4ba-180">usernameSource</span></span>|[<span data-ttu-id="0e4ba-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="0e4ba-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="0e4ba-182">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0e4ba-183">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="0e4ba-184">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0e4ba-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="0e4ba-185">usernameAADSource</span></span>|[<span data-ttu-id="0e4ba-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="0e4ba-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="0e4ba-187">AAD 字段的名称，将用于检索电子邮件配置文件的用户名。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="0e4ba-188">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="0e4ba-189">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="0e4ba-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="0e4ba-190">userDomainNameSource</span></span>|[<span data-ttu-id="0e4ba-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="0e4ba-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="0e4ba-192">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0e4ba-193">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="0e4ba-194">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="0e4ba-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="0e4ba-195">customDomainName</span></span>|<span data-ttu-id="0e4ba-196">String</span><span class="sxs-lookup"><span data-stu-id="0e4ba-196">String</span></span>|<span data-ttu-id="0e4ba-197">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="0e4ba-198">继承自 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="0e4ba-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="0e4ba-199">帐户</span><span class="sxs-lookup"><span data-stu-id="0e4ba-199">accountName</span></span>|<span data-ttu-id="0e4ba-200">String</span><span class="sxs-lookup"><span data-stu-id="0e4ba-200">String</span></span>|<span data-ttu-id="0e4ba-201">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-201">Account name.</span></span>|
|<span data-ttu-id="0e4ba-202">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="0e4ba-202">syncCalendar</span></span>|<span data-ttu-id="0e4ba-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e4ba-203">Boolean</span></span>|<span data-ttu-id="0e4ba-204">是否同步日历。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-204">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="0e4ba-205">syncContacts</span><span class="sxs-lookup"><span data-stu-id="0e4ba-205">syncContacts</span></span>|<span data-ttu-id="0e4ba-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e4ba-206">Boolean</span></span>|<span data-ttu-id="0e4ba-207">是否同步联系人。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-207">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="0e4ba-208">syncTasks</span><span class="sxs-lookup"><span data-stu-id="0e4ba-208">syncTasks</span></span>|<span data-ttu-id="0e4ba-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e4ba-209">Boolean</span></span>|<span data-ttu-id="0e4ba-210">是否同步任务。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-210">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="0e4ba-211">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="0e4ba-211">durationOfEmailToSync</span></span>|[<span data-ttu-id="0e4ba-212">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="0e4ba-212">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="0e4ba-213">要同步的电子邮件的持续时间。可能的值为：、、、、、 `userDefined` `oneDay` `threeDays` `oneWeek` `twoWeeks` `oneMonth` 、 `unlimited` 。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-213">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="0e4ba-214">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="0e4ba-214">emailAddressSource</span></span>|[<span data-ttu-id="0e4ba-215">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="0e4ba-215">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="0e4ba-216">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-216">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0e4ba-217">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-217">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0e4ba-218">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="0e4ba-218">emailSyncSchedule</span></span>|[<span data-ttu-id="0e4ba-219">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="0e4ba-219">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="0e4ba-220">电子邮件同步计划。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-220">Email sync schedule.</span></span> <span data-ttu-id="0e4ba-221">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes` 或 `basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-221">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="0e4ba-222">hostName</span><span class="sxs-lookup"><span data-stu-id="0e4ba-222">hostName</span></span>|<span data-ttu-id="0e4ba-223">String</span><span class="sxs-lookup"><span data-stu-id="0e4ba-223">String</span></span>|<span data-ttu-id="0e4ba-224">本地邮件应用程序连接到 (URL) 的 Exchange 位置。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-224">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="0e4ba-225">requireSsl</span><span class="sxs-lookup"><span data-stu-id="0e4ba-225">requireSsl</span></span>|<span data-ttu-id="0e4ba-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e4ba-226">Boolean</span></span>|<span data-ttu-id="0e4ba-227">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-227">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="0e4ba-228">响应</span><span class="sxs-lookup"><span data-stu-id="0e4ba-228">Response</span></span>
<span data-ttu-id="0e4ba-229">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-229">If successful, this method returns a `200 OK` response code and an updated [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e4ba-230">示例</span><span class="sxs-lookup"><span data-stu-id="0e4ba-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e4ba-231">请求</span><span class="sxs-lookup"><span data-stu-id="0e4ba-231">Request</span></span>
<span data-ttu-id="0e4ba-232">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0e4ba-233">响应</span><span class="sxs-lookup"><span data-stu-id="0e4ba-233">Response</span></span>
<span data-ttu-id="0e4ba-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e4ba-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






