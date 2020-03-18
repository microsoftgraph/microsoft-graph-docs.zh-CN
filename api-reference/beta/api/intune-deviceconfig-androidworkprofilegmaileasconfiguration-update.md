---
title: 更新 androidWorkProfileGmailEasConfiguration
description: 更新 androidWorkProfileGmailEasConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b206f1bede41859781e58726d7b397c3fdd2b83d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42758423"
---
# <a name="update-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="13c70-103">更新 androidWorkProfileGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="13c70-103">Update androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="13c70-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13c70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13c70-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13c70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13c70-106">更新[androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="13c70-106">Update the properties of a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13c70-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="13c70-107">Prerequisites</span></span>
<span data-ttu-id="13c70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13c70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13c70-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="13c70-110">Permission type</span></span>|<span data-ttu-id="13c70-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="13c70-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13c70-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13c70-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13c70-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c70-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13c70-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13c70-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13c70-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="13c70-115">Not supported.</span></span>|
|<span data-ttu-id="13c70-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="13c70-116">Application</span></span>|<span data-ttu-id="13c70-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c70-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13c70-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13c70-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="13c70-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="13c70-119">Request headers</span></span>
|<span data-ttu-id="13c70-120">标头</span><span class="sxs-lookup"><span data-stu-id="13c70-120">Header</span></span>|<span data-ttu-id="13c70-121">值</span><span class="sxs-lookup"><span data-stu-id="13c70-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13c70-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="13c70-122">Authorization</span></span>|<span data-ttu-id="13c70-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="13c70-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13c70-124">接受</span><span class="sxs-lookup"><span data-stu-id="13c70-124">Accept</span></span>|<span data-ttu-id="13c70-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13c70-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13c70-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="13c70-126">Request body</span></span>
<span data-ttu-id="13c70-127">在请求正文中，提供[androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13c70-127">In the request body, supply a JSON representation for the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="13c70-128">下表显示创建[androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="13c70-128">The following table shows the properties that are required when you create the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span></span>

|<span data-ttu-id="13c70-129">属性</span><span class="sxs-lookup"><span data-stu-id="13c70-129">Property</span></span>|<span data-ttu-id="13c70-130">类型</span><span class="sxs-lookup"><span data-stu-id="13c70-130">Type</span></span>|<span data-ttu-id="13c70-131">说明</span><span class="sxs-lookup"><span data-stu-id="13c70-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13c70-132">id</span><span class="sxs-lookup"><span data-stu-id="13c70-132">id</span></span>|<span data-ttu-id="13c70-133">字符串</span><span class="sxs-lookup"><span data-stu-id="13c70-133">String</span></span>|<span data-ttu-id="13c70-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="13c70-134">Key of the entity.</span></span> <span data-ttu-id="13c70-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13c70-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13c70-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13c70-136">lastModifiedDateTime</span></span>|<span data-ttu-id="13c70-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13c70-137">DateTimeOffset</span></span>|<span data-ttu-id="13c70-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="13c70-138">DateTime the object was last modified.</span></span> <span data-ttu-id="13c70-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13c70-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13c70-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="13c70-140">roleScopeTagIds</span></span>|<span data-ttu-id="13c70-141">String collection</span><span class="sxs-lookup"><span data-stu-id="13c70-141">String collection</span></span>|<span data-ttu-id="13c70-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="13c70-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="13c70-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13c70-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13c70-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="13c70-144">supportsScopeTags</span></span>|<span data-ttu-id="13c70-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="13c70-145">Boolean</span></span>|<span data-ttu-id="13c70-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="13c70-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="13c70-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="13c70-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="13c70-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="13c70-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="13c70-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="13c70-149">This property is read-only.</span></span> <span data-ttu-id="13c70-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13c70-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13c70-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="13c70-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="13c70-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="13c70-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="13c70-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="13c70-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="13c70-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13c70-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13c70-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="13c70-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="13c70-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="13c70-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="13c70-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="13c70-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="13c70-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13c70-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13c70-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="13c70-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="13c70-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="13c70-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="13c70-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="13c70-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="13c70-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13c70-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13c70-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13c70-163">createdDateTime</span></span>|<span data-ttu-id="13c70-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13c70-164">DateTimeOffset</span></span>|<span data-ttu-id="13c70-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="13c70-165">DateTime the object was created.</span></span> <span data-ttu-id="13c70-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13c70-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13c70-167">说明</span><span class="sxs-lookup"><span data-stu-id="13c70-167">description</span></span>|<span data-ttu-id="13c70-168">String</span><span class="sxs-lookup"><span data-stu-id="13c70-168">String</span></span>|<span data-ttu-id="13c70-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="13c70-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="13c70-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13c70-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13c70-171">displayName</span><span class="sxs-lookup"><span data-stu-id="13c70-171">displayName</span></span>|<span data-ttu-id="13c70-172">String</span><span class="sxs-lookup"><span data-stu-id="13c70-172">String</span></span>|<span data-ttu-id="13c70-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="13c70-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="13c70-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13c70-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13c70-175">version</span><span class="sxs-lookup"><span data-stu-id="13c70-175">version</span></span>|<span data-ttu-id="13c70-176">Int32</span><span class="sxs-lookup"><span data-stu-id="13c70-176">Int32</span></span>|<span data-ttu-id="13c70-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="13c70-177">Version of the device configuration.</span></span> <span data-ttu-id="13c70-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13c70-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13c70-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="13c70-179">authenticationMethod</span></span>|[<span data-ttu-id="13c70-180">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="13c70-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="13c70-181">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="13c70-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="13c70-182">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="13c70-182">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="13c70-183">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="13c70-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="13c70-184">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="13c70-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="13c70-185">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="13c70-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="13c70-186">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="13c70-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="13c70-187">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="13c70-187">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="13c70-188">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="13c70-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="13c70-189">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="13c70-189">emailAddressSource</span></span>|[<span data-ttu-id="13c70-190">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="13c70-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="13c70-191">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="13c70-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="13c70-192">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="13c70-192">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="13c70-193">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="13c70-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="13c70-194">hostName</span><span class="sxs-lookup"><span data-stu-id="13c70-194">hostName</span></span>|<span data-ttu-id="13c70-195">String</span><span class="sxs-lookup"><span data-stu-id="13c70-195">String</span></span>|<span data-ttu-id="13c70-196">邮件应用程序连接到的 Exchange 位置（URL）。</span><span class="sxs-lookup"><span data-stu-id="13c70-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="13c70-197">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="13c70-197">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="13c70-198">requireSsl</span><span class="sxs-lookup"><span data-stu-id="13c70-198">requireSsl</span></span>|<span data-ttu-id="13c70-199">布尔值</span><span class="sxs-lookup"><span data-stu-id="13c70-199">Boolean</span></span>|<span data-ttu-id="13c70-200">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="13c70-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="13c70-201">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="13c70-201">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="13c70-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="13c70-202">usernameSource</span></span>|[<span data-ttu-id="13c70-203">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="13c70-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="13c70-204">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="13c70-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="13c70-205">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="13c70-205">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="13c70-206">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="13c70-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="13c70-207">响应</span><span class="sxs-lookup"><span data-stu-id="13c70-207">Response</span></span>
<span data-ttu-id="13c70-208">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="13c70-208">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13c70-209">示例</span><span class="sxs-lookup"><span data-stu-id="13c70-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="13c70-210">请求</span><span class="sxs-lookup"><span data-stu-id="13c70-210">Request</span></span>
<span data-ttu-id="13c70-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="13c70-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1268

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
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
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName"
}
```

### <a name="response"></a><span data-ttu-id="13c70-212">响应</span><span class="sxs-lookup"><span data-stu-id="13c70-212">Response</span></span>
<span data-ttu-id="13c70-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13c70-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1440

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
  "id": "a4a44bb5-4bb5-a4a4-b54b-a4a4b54ba4a4",
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
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName"
}
```




