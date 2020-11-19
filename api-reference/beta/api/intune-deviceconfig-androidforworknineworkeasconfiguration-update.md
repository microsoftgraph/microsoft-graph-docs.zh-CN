---
title: 更新 androidForWorkNineWorkEasConfiguration
description: 更新 androidForWorkNineWorkEasConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b88740be5e3e31149e0dfe1cb191adcca91d09b6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49238575"
---
# <a name="update-androidforworknineworkeasconfiguration"></a><span data-ttu-id="611d9-103">更新 androidForWorkNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="611d9-103">Update androidForWorkNineWorkEasConfiguration</span></span>

<span data-ttu-id="611d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="611d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="611d9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="611d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="611d9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="611d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="611d9-107">更新 [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="611d9-107">Update the properties of a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="611d9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="611d9-108">Prerequisites</span></span>
<span data-ttu-id="611d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="611d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="611d9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="611d9-111">Permission type</span></span>|<span data-ttu-id="611d9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="611d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="611d9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="611d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="611d9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="611d9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="611d9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="611d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="611d9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="611d9-116">Not supported.</span></span>|
|<span data-ttu-id="611d9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="611d9-117">Application</span></span>|<span data-ttu-id="611d9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="611d9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="611d9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="611d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="611d9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="611d9-120">Request headers</span></span>
|<span data-ttu-id="611d9-121">标头</span><span class="sxs-lookup"><span data-stu-id="611d9-121">Header</span></span>|<span data-ttu-id="611d9-122">值</span><span class="sxs-lookup"><span data-stu-id="611d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="611d9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="611d9-123">Authorization</span></span>|<span data-ttu-id="611d9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="611d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="611d9-125">接受</span><span class="sxs-lookup"><span data-stu-id="611d9-125">Accept</span></span>|<span data-ttu-id="611d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="611d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="611d9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="611d9-127">Request body</span></span>
<span data-ttu-id="611d9-128">在请求正文中，提供 [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="611d9-128">In the request body, supply a JSON representation for the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="611d9-129">下表显示创建 [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="611d9-129">The following table shows the properties that are required when you create the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="611d9-130">属性</span><span class="sxs-lookup"><span data-stu-id="611d9-130">Property</span></span>|<span data-ttu-id="611d9-131">类型</span><span class="sxs-lookup"><span data-stu-id="611d9-131">Type</span></span>|<span data-ttu-id="611d9-132">说明</span><span class="sxs-lookup"><span data-stu-id="611d9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="611d9-133">id</span><span class="sxs-lookup"><span data-stu-id="611d9-133">id</span></span>|<span data-ttu-id="611d9-134">String</span><span class="sxs-lookup"><span data-stu-id="611d9-134">String</span></span>|<span data-ttu-id="611d9-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="611d9-135">Key of the entity.</span></span> <span data-ttu-id="611d9-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="611d9-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="611d9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="611d9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="611d9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="611d9-138">DateTimeOffset</span></span>|<span data-ttu-id="611d9-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="611d9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="611d9-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="611d9-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="611d9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="611d9-141">roleScopeTagIds</span></span>|<span data-ttu-id="611d9-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="611d9-142">String collection</span></span>|<span data-ttu-id="611d9-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="611d9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="611d9-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="611d9-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="611d9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="611d9-145">supportsScopeTags</span></span>|<span data-ttu-id="611d9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="611d9-146">Boolean</span></span>|<span data-ttu-id="611d9-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="611d9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="611d9-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="611d9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="611d9-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="611d9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="611d9-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="611d9-150">This property is read-only.</span></span> <span data-ttu-id="611d9-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="611d9-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="611d9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="611d9-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="611d9-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="611d9-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="611d9-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="611d9-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="611d9-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="611d9-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="611d9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="611d9-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="611d9-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="611d9-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="611d9-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="611d9-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="611d9-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="611d9-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="611d9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="611d9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="611d9-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="611d9-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="611d9-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="611d9-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="611d9-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="611d9-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="611d9-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="611d9-164">createdDateTime</span></span>|<span data-ttu-id="611d9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="611d9-165">DateTimeOffset</span></span>|<span data-ttu-id="611d9-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="611d9-166">DateTime the object was created.</span></span> <span data-ttu-id="611d9-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="611d9-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="611d9-168">description</span><span class="sxs-lookup"><span data-stu-id="611d9-168">description</span></span>|<span data-ttu-id="611d9-169">String</span><span class="sxs-lookup"><span data-stu-id="611d9-169">String</span></span>|<span data-ttu-id="611d9-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="611d9-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="611d9-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="611d9-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="611d9-172">displayName</span><span class="sxs-lookup"><span data-stu-id="611d9-172">displayName</span></span>|<span data-ttu-id="611d9-173">String</span><span class="sxs-lookup"><span data-stu-id="611d9-173">String</span></span>|<span data-ttu-id="611d9-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="611d9-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="611d9-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="611d9-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="611d9-176">version</span><span class="sxs-lookup"><span data-stu-id="611d9-176">version</span></span>|<span data-ttu-id="611d9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="611d9-177">Int32</span></span>|<span data-ttu-id="611d9-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="611d9-178">Version of the device configuration.</span></span> <span data-ttu-id="611d9-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="611d9-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="611d9-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="611d9-180">authenticationMethod</span></span>|[<span data-ttu-id="611d9-181">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="611d9-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="611d9-182">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="611d9-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="611d9-183">继承自 [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="611d9-183">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="611d9-184">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="611d9-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="611d9-185">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="611d9-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="611d9-186">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="611d9-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="611d9-187">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="611d9-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="611d9-188">继承自 [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="611d9-188">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="611d9-189">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="611d9-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="611d9-190">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="611d9-190">emailAddressSource</span></span>|[<span data-ttu-id="611d9-191">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="611d9-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="611d9-192">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="611d9-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="611d9-193">继承自 [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="611d9-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="611d9-194">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="611d9-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="611d9-195">hostName</span><span class="sxs-lookup"><span data-stu-id="611d9-195">hostName</span></span>|<span data-ttu-id="611d9-196">String</span><span class="sxs-lookup"><span data-stu-id="611d9-196">String</span></span>|<span data-ttu-id="611d9-197">邮件应用程序连接到的 Exchange 位置 (URL) 。</span><span class="sxs-lookup"><span data-stu-id="611d9-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="611d9-198">继承自 [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="611d9-198">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="611d9-199">requireSsl</span><span class="sxs-lookup"><span data-stu-id="611d9-199">requireSsl</span></span>|<span data-ttu-id="611d9-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="611d9-200">Boolean</span></span>|<span data-ttu-id="611d9-201">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="611d9-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="611d9-202">继承自 [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="611d9-202">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="611d9-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="611d9-203">usernameSource</span></span>|[<span data-ttu-id="611d9-204">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="611d9-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="611d9-205">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="611d9-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="611d9-206">继承自 [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="611d9-206">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="611d9-207">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="611d9-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="611d9-208">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="611d9-208">syncCalendar</span></span>|<span data-ttu-id="611d9-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="611d9-209">Boolean</span></span>|<span data-ttu-id="611d9-210">切换同步日历。</span><span class="sxs-lookup"><span data-stu-id="611d9-210">Toggles syncing the calendar.</span></span> <span data-ttu-id="611d9-211">如果设置为 false，则表示设备上的日历处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="611d9-211">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="611d9-212">syncContacts</span><span class="sxs-lookup"><span data-stu-id="611d9-212">syncContacts</span></span>|<span data-ttu-id="611d9-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="611d9-213">Boolean</span></span>|<span data-ttu-id="611d9-214">切换同步联系人。</span><span class="sxs-lookup"><span data-stu-id="611d9-214">Toggles syncing contacts.</span></span> <span data-ttu-id="611d9-215">如果设置为 false，则设备上的联系人处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="611d9-215">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="611d9-216">syncTasks</span><span class="sxs-lookup"><span data-stu-id="611d9-216">syncTasks</span></span>|<span data-ttu-id="611d9-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="611d9-217">Boolean</span></span>|<span data-ttu-id="611d9-218">切换同步任务。</span><span class="sxs-lookup"><span data-stu-id="611d9-218">Toggles syncing tasks.</span></span> <span data-ttu-id="611d9-219">如果设备上的 "设置为 false 任务" 处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="611d9-219">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="611d9-220">响应</span><span class="sxs-lookup"><span data-stu-id="611d9-220">Response</span></span>
<span data-ttu-id="611d9-221">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="611d9-221">If successful, this method returns a `200 OK` response code and an updated [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="611d9-222">示例</span><span class="sxs-lookup"><span data-stu-id="611d9-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="611d9-223">请求</span><span class="sxs-lookup"><span data-stu-id="611d9-223">Request</span></span>
<span data-ttu-id="611d9-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="611d9-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1339

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
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
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```

### <a name="response"></a><span data-ttu-id="611d9-225">响应</span><span class="sxs-lookup"><span data-stu-id="611d9-225">Response</span></span>
<span data-ttu-id="611d9-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="611d9-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1511

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
  "id": "f8ef19e0-19e0-f8ef-e019-eff8e019eff8",
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
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```




