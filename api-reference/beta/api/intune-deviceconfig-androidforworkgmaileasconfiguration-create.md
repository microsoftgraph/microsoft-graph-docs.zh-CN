---
title: 创建 androidForWorkGmailEasConfiguration
description: 创建新的 androidForWorkGmailEasConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6f20b1437b0e05bec5a99d5047d0f44cd472b89
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36312115"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="a0670-103">创建 androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0670-103">Create androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="a0670-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a0670-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0670-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a0670-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0670-106">创建新的[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a0670-106">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0670-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a0670-107">Prerequisites</span></span>
<span data-ttu-id="a0670-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0670-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0670-110">Permission type</span></span>|<span data-ttu-id="a0670-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a0670-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0670-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0670-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0670-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0670-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0670-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0670-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0670-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0670-115">Not supported.</span></span>|
|<span data-ttu-id="a0670-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0670-116">Application</span></span>|<span data-ttu-id="a0670-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0670-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0670-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0670-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a0670-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0670-119">Request headers</span></span>
|<span data-ttu-id="a0670-120">标头</span><span class="sxs-lookup"><span data-stu-id="a0670-120">Header</span></span>|<span data-ttu-id="a0670-121">值</span><span class="sxs-lookup"><span data-stu-id="a0670-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0670-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0670-122">Authorization</span></span>|<span data-ttu-id="a0670-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a0670-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0670-124">接受</span><span class="sxs-lookup"><span data-stu-id="a0670-124">Accept</span></span>|<span data-ttu-id="a0670-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0670-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0670-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0670-126">Request body</span></span>
<span data-ttu-id="a0670-127">在请求正文中, 提供 androidForWorkGmailEasConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0670-127">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="a0670-128">下表显示创建 androidForWorkGmailEasConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a0670-128">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="a0670-129">属性</span><span class="sxs-lookup"><span data-stu-id="a0670-129">Property</span></span>|<span data-ttu-id="a0670-130">类型</span><span class="sxs-lookup"><span data-stu-id="a0670-130">Type</span></span>|<span data-ttu-id="a0670-131">说明</span><span class="sxs-lookup"><span data-stu-id="a0670-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0670-132">id</span><span class="sxs-lookup"><span data-stu-id="a0670-132">id</span></span>|<span data-ttu-id="a0670-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a0670-133">String</span></span>|<span data-ttu-id="a0670-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a0670-134">Key of the entity.</span></span> <span data-ttu-id="a0670-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0670-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0670-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0670-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a0670-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0670-137">DateTimeOffset</span></span>|<span data-ttu-id="a0670-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a0670-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a0670-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0670-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0670-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0670-140">roleScopeTagIds</span></span>|<span data-ttu-id="a0670-141">String collection</span><span class="sxs-lookup"><span data-stu-id="a0670-141">String collection</span></span>|<span data-ttu-id="a0670-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a0670-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a0670-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0670-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0670-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a0670-144">supportsScopeTags</span></span>|<span data-ttu-id="a0670-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0670-145">Boolean</span></span>|<span data-ttu-id="a0670-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="a0670-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a0670-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="a0670-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a0670-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="a0670-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a0670-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a0670-149">This property is read-only.</span></span> <span data-ttu-id="a0670-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0670-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0670-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a0670-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a0670-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a0670-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a0670-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="a0670-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a0670-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0670-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0670-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a0670-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a0670-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a0670-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a0670-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a0670-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a0670-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0670-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0670-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a0670-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a0670-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a0670-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a0670-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a0670-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a0670-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0670-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0670-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0670-163">createdDateTime</span></span>|<span data-ttu-id="a0670-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0670-164">DateTimeOffset</span></span>|<span data-ttu-id="a0670-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a0670-165">DateTime the object was created.</span></span> <span data-ttu-id="a0670-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0670-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0670-167">说明</span><span class="sxs-lookup"><span data-stu-id="a0670-167">description</span></span>|<span data-ttu-id="a0670-168">String</span><span class="sxs-lookup"><span data-stu-id="a0670-168">String</span></span>|<span data-ttu-id="a0670-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a0670-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a0670-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0670-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0670-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a0670-171">displayName</span></span>|<span data-ttu-id="a0670-172">String</span><span class="sxs-lookup"><span data-stu-id="a0670-172">String</span></span>|<span data-ttu-id="a0670-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a0670-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a0670-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0670-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0670-175">version</span><span class="sxs-lookup"><span data-stu-id="a0670-175">version</span></span>|<span data-ttu-id="a0670-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a0670-176">Int32</span></span>|<span data-ttu-id="a0670-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a0670-177">Version of the device configuration.</span></span> <span data-ttu-id="a0670-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0670-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0670-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a0670-179">authenticationMethod</span></span>|[<span data-ttu-id="a0670-180">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a0670-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="a0670-181">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="a0670-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="a0670-182">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="a0670-182">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="a0670-183">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="a0670-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a0670-184">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="a0670-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="a0670-185">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="a0670-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="a0670-186">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="a0670-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="a0670-187">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="a0670-187">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="a0670-188">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="a0670-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="a0670-189">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="a0670-189">emailAddressSource</span></span>|[<span data-ttu-id="a0670-190">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="a0670-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a0670-191">在设备上安装之前, 从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="a0670-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a0670-192">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="a0670-192">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="a0670-193">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="a0670-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a0670-194">hostName</span><span class="sxs-lookup"><span data-stu-id="a0670-194">hostName</span></span>|<span data-ttu-id="a0670-195">String</span><span class="sxs-lookup"><span data-stu-id="a0670-195">String</span></span>|<span data-ttu-id="a0670-196">邮件应用程序连接到的 Exchange 位置 (URL)。</span><span class="sxs-lookup"><span data-stu-id="a0670-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="a0670-197">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0670-197">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="a0670-198">requireSsl</span><span class="sxs-lookup"><span data-stu-id="a0670-198">requireSsl</span></span>|<span data-ttu-id="a0670-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0670-199">Boolean</span></span>|<span data-ttu-id="a0670-200">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="a0670-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="a0670-201">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0670-201">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="a0670-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a0670-202">usernameSource</span></span>|[<span data-ttu-id="a0670-203">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="a0670-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="a0670-204">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="a0670-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a0670-205">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="a0670-205">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="a0670-206">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="a0670-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="a0670-207">响应</span><span class="sxs-lookup"><span data-stu-id="a0670-207">Response</span></span>
<span data-ttu-id="a0670-208">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a0670-208">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0670-209">示例</span><span class="sxs-lookup"><span data-stu-id="a0670-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0670-210">请求</span><span class="sxs-lookup"><span data-stu-id="a0670-210">Request</span></span>
<span data-ttu-id="a0670-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0670-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="a0670-212">响应</span><span class="sxs-lookup"><span data-stu-id="a0670-212">Response</span></span>
<span data-ttu-id="a0670-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0670-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






