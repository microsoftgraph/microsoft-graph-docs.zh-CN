---
title: 更新 androidWorkProfileNineWorkEasConfiguration
description: 更新 androidWorkProfileNineWorkEasConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc90da5918cbf08f561f9864ab9253d7e41fc7d3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340630"
---
# <a name="update-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="2a22c-103">更新 androidWorkProfileNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="2a22c-103">Update androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="2a22c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a22c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a22c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a22c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a22c-106">更新[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2a22c-106">Update the properties of a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a22c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a22c-107">Prerequisites</span></span>
<span data-ttu-id="2a22c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a22c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a22c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a22c-110">Permission type</span></span>|<span data-ttu-id="2a22c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a22c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a22c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a22c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a22c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a22c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2a22c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a22c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a22c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a22c-115">Not supported.</span></span>|
|<span data-ttu-id="2a22c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a22c-116">Application</span></span>|<span data-ttu-id="2a22c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a22c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a22c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a22c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2a22c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a22c-119">Request headers</span></span>
|<span data-ttu-id="2a22c-120">标头</span><span class="sxs-lookup"><span data-stu-id="2a22c-120">Header</span></span>|<span data-ttu-id="2a22c-121">值</span><span class="sxs-lookup"><span data-stu-id="2a22c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a22c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a22c-122">Authorization</span></span>|<span data-ttu-id="2a22c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a22c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a22c-124">接受</span><span class="sxs-lookup"><span data-stu-id="2a22c-124">Accept</span></span>|<span data-ttu-id="2a22c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a22c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a22c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a22c-126">Request body</span></span>
<span data-ttu-id="2a22c-127">在请求正文中, 提供[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a22c-127">In the request body, supply a JSON representation for the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="2a22c-128">下表显示创建[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2a22c-128">The following table shows the properties that are required when you create the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="2a22c-129">属性</span><span class="sxs-lookup"><span data-stu-id="2a22c-129">Property</span></span>|<span data-ttu-id="2a22c-130">类型</span><span class="sxs-lookup"><span data-stu-id="2a22c-130">Type</span></span>|<span data-ttu-id="2a22c-131">说明</span><span class="sxs-lookup"><span data-stu-id="2a22c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a22c-132">id</span><span class="sxs-lookup"><span data-stu-id="2a22c-132">id</span></span>|<span data-ttu-id="2a22c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2a22c-133">String</span></span>|<span data-ttu-id="2a22c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2a22c-134">Key of the entity.</span></span> <span data-ttu-id="2a22c-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a22c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a22c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a22c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2a22c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a22c-137">DateTimeOffset</span></span>|<span data-ttu-id="2a22c-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2a22c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2a22c-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a22c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a22c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2a22c-140">roleScopeTagIds</span></span>|<span data-ttu-id="2a22c-141">String collection</span><span class="sxs-lookup"><span data-stu-id="2a22c-141">String collection</span></span>|<span data-ttu-id="2a22c-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2a22c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2a22c-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a22c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a22c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2a22c-144">supportsScopeTags</span></span>|<span data-ttu-id="2a22c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a22c-145">Boolean</span></span>|<span data-ttu-id="2a22c-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="2a22c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2a22c-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="2a22c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2a22c-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="2a22c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2a22c-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2a22c-149">This property is read-only.</span></span> <span data-ttu-id="2a22c-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a22c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a22c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2a22c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2a22c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2a22c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2a22c-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="2a22c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2a22c-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a22c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a22c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2a22c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2a22c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2a22c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2a22c-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2a22c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2a22c-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a22c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a22c-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2a22c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2a22c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2a22c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2a22c-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2a22c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2a22c-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a22c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a22c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a22c-163">createdDateTime</span></span>|<span data-ttu-id="2a22c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a22c-164">DateTimeOffset</span></span>|<span data-ttu-id="2a22c-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2a22c-165">DateTime the object was created.</span></span> <span data-ttu-id="2a22c-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a22c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a22c-167">说明</span><span class="sxs-lookup"><span data-stu-id="2a22c-167">description</span></span>|<span data-ttu-id="2a22c-168">String</span><span class="sxs-lookup"><span data-stu-id="2a22c-168">String</span></span>|<span data-ttu-id="2a22c-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2a22c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2a22c-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a22c-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a22c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2a22c-171">displayName</span></span>|<span data-ttu-id="2a22c-172">String</span><span class="sxs-lookup"><span data-stu-id="2a22c-172">String</span></span>|<span data-ttu-id="2a22c-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2a22c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2a22c-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a22c-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a22c-175">version</span><span class="sxs-lookup"><span data-stu-id="2a22c-175">version</span></span>|<span data-ttu-id="2a22c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2a22c-176">Int32</span></span>|<span data-ttu-id="2a22c-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2a22c-177">Version of the device configuration.</span></span> <span data-ttu-id="2a22c-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a22c-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a22c-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2a22c-179">authenticationMethod</span></span>|[<span data-ttu-id="2a22c-180">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2a22c-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="2a22c-181">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="2a22c-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="2a22c-182">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2a22c-182">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="2a22c-183">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="2a22c-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="2a22c-184">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="2a22c-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="2a22c-185">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="2a22c-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="2a22c-186">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="2a22c-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="2a22c-187">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2a22c-187">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="2a22c-188">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="2a22c-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="2a22c-189">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="2a22c-189">emailAddressSource</span></span>|[<span data-ttu-id="2a22c-190">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="2a22c-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="2a22c-191">在设备上安装之前, 从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="2a22c-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2a22c-192">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2a22c-192">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="2a22c-193">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="2a22c-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="2a22c-194">hostName</span><span class="sxs-lookup"><span data-stu-id="2a22c-194">hostName</span></span>|<span data-ttu-id="2a22c-195">String</span><span class="sxs-lookup"><span data-stu-id="2a22c-195">String</span></span>|<span data-ttu-id="2a22c-196">邮件应用程序连接到的 Exchange 位置 (URL)。</span><span class="sxs-lookup"><span data-stu-id="2a22c-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="2a22c-197">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2a22c-197">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="2a22c-198">requireSsl</span><span class="sxs-lookup"><span data-stu-id="2a22c-198">requireSsl</span></span>|<span data-ttu-id="2a22c-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a22c-199">Boolean</span></span>|<span data-ttu-id="2a22c-200">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="2a22c-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="2a22c-201">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2a22c-201">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="2a22c-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="2a22c-202">usernameSource</span></span>|[<span data-ttu-id="2a22c-203">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="2a22c-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="2a22c-204">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="2a22c-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2a22c-205">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2a22c-205">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="2a22c-206">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="2a22c-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="2a22c-207">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="2a22c-207">syncCalendar</span></span>|<span data-ttu-id="2a22c-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a22c-208">Boolean</span></span>|<span data-ttu-id="2a22c-209">切换同步日历。</span><span class="sxs-lookup"><span data-stu-id="2a22c-209">Toggles syncing the calendar.</span></span> <span data-ttu-id="2a22c-210">如果设置为 false, 则表示设备上的日历处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="2a22c-210">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="2a22c-211">syncContacts</span><span class="sxs-lookup"><span data-stu-id="2a22c-211">syncContacts</span></span>|<span data-ttu-id="2a22c-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a22c-212">Boolean</span></span>|<span data-ttu-id="2a22c-213">切换同步联系人。</span><span class="sxs-lookup"><span data-stu-id="2a22c-213">Toggles syncing contacts.</span></span> <span data-ttu-id="2a22c-214">如果设置为 false, 则设备上的联系人处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="2a22c-214">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="2a22c-215">syncTasks</span><span class="sxs-lookup"><span data-stu-id="2a22c-215">syncTasks</span></span>|<span data-ttu-id="2a22c-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a22c-216">Boolean</span></span>|<span data-ttu-id="2a22c-217">切换同步任务。</span><span class="sxs-lookup"><span data-stu-id="2a22c-217">Toggles syncing tasks.</span></span> <span data-ttu-id="2a22c-218">如果设备上的 "设置为 false 任务" 处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="2a22c-218">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="2a22c-219">响应</span><span class="sxs-lookup"><span data-stu-id="2a22c-219">Response</span></span>
<span data-ttu-id="2a22c-220">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2a22c-220">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a22c-221">示例</span><span class="sxs-lookup"><span data-stu-id="2a22c-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a22c-222">请求</span><span class="sxs-lookup"><span data-stu-id="2a22c-222">Request</span></span>
<span data-ttu-id="2a22c-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a22c-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1343

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="2a22c-224">响应</span><span class="sxs-lookup"><span data-stu-id="2a22c-224">Response</span></span>
<span data-ttu-id="2a22c-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a22c-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1515

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "id": "3d9e3a30-3a30-3d9e-303a-9e3d303a9e3d",
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






