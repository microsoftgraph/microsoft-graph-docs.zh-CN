---
title: 更新 androidForWorkGmailEasConfiguration
description: 更新 androidForWorkGmailEasConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d41b37cd5028814d317fcf2c1122e52abbbc1e9d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39928201"
---
# <a name="update-androidforworkgmaileasconfiguration"></a><span data-ttu-id="35df6-103">更新 androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="35df6-103">Update androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="35df6-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35df6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35df6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35df6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35df6-106">更新[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="35df6-106">Update the properties of a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35df6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="35df6-107">Prerequisites</span></span>
<span data-ttu-id="35df6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35df6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35df6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="35df6-110">Permission type</span></span>|<span data-ttu-id="35df6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="35df6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35df6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35df6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35df6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35df6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35df6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35df6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35df6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="35df6-115">Not supported.</span></span>|
|<span data-ttu-id="35df6-116">Application</span><span class="sxs-lookup"><span data-stu-id="35df6-116">Application</span></span>|<span data-ttu-id="35df6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35df6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35df6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35df6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="35df6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="35df6-119">Request headers</span></span>
|<span data-ttu-id="35df6-120">标头</span><span class="sxs-lookup"><span data-stu-id="35df6-120">Header</span></span>|<span data-ttu-id="35df6-121">值</span><span class="sxs-lookup"><span data-stu-id="35df6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35df6-122">授权</span><span class="sxs-lookup"><span data-stu-id="35df6-122">Authorization</span></span>|<span data-ttu-id="35df6-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="35df6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35df6-124">接受</span><span class="sxs-lookup"><span data-stu-id="35df6-124">Accept</span></span>|<span data-ttu-id="35df6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35df6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35df6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="35df6-126">Request body</span></span>
<span data-ttu-id="35df6-127">在请求正文中，提供[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35df6-127">In the request body, supply a JSON representation for the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="35df6-128">下表显示创建[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="35df6-128">The following table shows the properties that are required when you create the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span></span>

|<span data-ttu-id="35df6-129">属性</span><span class="sxs-lookup"><span data-stu-id="35df6-129">Property</span></span>|<span data-ttu-id="35df6-130">类型</span><span class="sxs-lookup"><span data-stu-id="35df6-130">Type</span></span>|<span data-ttu-id="35df6-131">说明</span><span class="sxs-lookup"><span data-stu-id="35df6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35df6-132">id</span><span class="sxs-lookup"><span data-stu-id="35df6-132">id</span></span>|<span data-ttu-id="35df6-133">字符串</span><span class="sxs-lookup"><span data-stu-id="35df6-133">String</span></span>|<span data-ttu-id="35df6-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="35df6-134">Key of the entity.</span></span> <span data-ttu-id="35df6-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35df6-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35df6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35df6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="35df6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35df6-137">DateTimeOffset</span></span>|<span data-ttu-id="35df6-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="35df6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="35df6-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35df6-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35df6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="35df6-140">roleScopeTagIds</span></span>|<span data-ttu-id="35df6-141">String collection</span><span class="sxs-lookup"><span data-stu-id="35df6-141">String collection</span></span>|<span data-ttu-id="35df6-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="35df6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="35df6-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35df6-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35df6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="35df6-144">supportsScopeTags</span></span>|<span data-ttu-id="35df6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="35df6-145">Boolean</span></span>|<span data-ttu-id="35df6-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="35df6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="35df6-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="35df6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="35df6-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="35df6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="35df6-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="35df6-149">This property is read-only.</span></span> <span data-ttu-id="35df6-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35df6-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35df6-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="35df6-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="35df6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="35df6-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="35df6-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="35df6-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="35df6-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35df6-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35df6-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="35df6-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="35df6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="35df6-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="35df6-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="35df6-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="35df6-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35df6-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35df6-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="35df6-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="35df6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="35df6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="35df6-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="35df6-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="35df6-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35df6-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35df6-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35df6-163">createdDateTime</span></span>|<span data-ttu-id="35df6-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35df6-164">DateTimeOffset</span></span>|<span data-ttu-id="35df6-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="35df6-165">DateTime the object was created.</span></span> <span data-ttu-id="35df6-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35df6-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35df6-167">说明</span><span class="sxs-lookup"><span data-stu-id="35df6-167">description</span></span>|<span data-ttu-id="35df6-168">String</span><span class="sxs-lookup"><span data-stu-id="35df6-168">String</span></span>|<span data-ttu-id="35df6-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="35df6-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="35df6-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35df6-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35df6-171">displayName</span><span class="sxs-lookup"><span data-stu-id="35df6-171">displayName</span></span>|<span data-ttu-id="35df6-172">String</span><span class="sxs-lookup"><span data-stu-id="35df6-172">String</span></span>|<span data-ttu-id="35df6-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="35df6-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="35df6-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35df6-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35df6-175">version</span><span class="sxs-lookup"><span data-stu-id="35df6-175">version</span></span>|<span data-ttu-id="35df6-176">Int32</span><span class="sxs-lookup"><span data-stu-id="35df6-176">Int32</span></span>|<span data-ttu-id="35df6-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="35df6-177">Version of the device configuration.</span></span> <span data-ttu-id="35df6-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35df6-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35df6-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="35df6-179">authenticationMethod</span></span>|[<span data-ttu-id="35df6-180">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="35df6-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="35df6-181">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="35df6-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="35df6-182">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="35df6-182">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="35df6-183">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="35df6-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="35df6-184">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="35df6-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="35df6-185">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="35df6-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="35df6-186">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="35df6-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="35df6-187">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="35df6-187">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="35df6-188">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="35df6-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="35df6-189">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="35df6-189">emailAddressSource</span></span>|[<span data-ttu-id="35df6-190">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="35df6-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="35df6-191">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="35df6-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="35df6-192">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="35df6-192">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="35df6-193">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="35df6-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="35df6-194">hostName</span><span class="sxs-lookup"><span data-stu-id="35df6-194">hostName</span></span>|<span data-ttu-id="35df6-195">String</span><span class="sxs-lookup"><span data-stu-id="35df6-195">String</span></span>|<span data-ttu-id="35df6-196">邮件应用程序连接到的 Exchange 位置（URL）。</span><span class="sxs-lookup"><span data-stu-id="35df6-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="35df6-197">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="35df6-197">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="35df6-198">requireSsl</span><span class="sxs-lookup"><span data-stu-id="35df6-198">requireSsl</span></span>|<span data-ttu-id="35df6-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="35df6-199">Boolean</span></span>|<span data-ttu-id="35df6-200">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="35df6-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="35df6-201">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="35df6-201">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="35df6-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="35df6-202">usernameSource</span></span>|[<span data-ttu-id="35df6-203">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="35df6-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="35df6-204">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="35df6-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="35df6-205">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="35df6-205">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="35df6-206">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="35df6-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="35df6-207">响应</span><span class="sxs-lookup"><span data-stu-id="35df6-207">Response</span></span>
<span data-ttu-id="35df6-208">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="35df6-208">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35df6-209">示例</span><span class="sxs-lookup"><span data-stu-id="35df6-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="35df6-210">请求</span><span class="sxs-lookup"><span data-stu-id="35df6-210">Request</span></span>
<span data-ttu-id="35df6-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="35df6-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1264

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="35df6-212">响应</span><span class="sxs-lookup"><span data-stu-id="35df6-212">Response</span></span>
<span data-ttu-id="35df6-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="35df6-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1436

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
  "id": "2bafc891-c891-2baf-91c8-af2b91c8af2b",
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





