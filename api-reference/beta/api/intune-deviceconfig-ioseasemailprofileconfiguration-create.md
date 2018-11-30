---
title: 创建 iosEasEmailProfileConfiguration
description: 创建新的 iosEasEmailProfileConfiguration 对象。
ms.openlocfilehash: 78cf37fc63f6cc62d40ffc1ef3deda587b65aaf3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045182"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="6c22a-103">创建 iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c22a-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="6c22a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6c22a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c22a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6c22a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c22a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6c22a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c22a-107">创建新的[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6c22a-107">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6c22a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6c22a-108">Prerequisites</span></span>
<span data-ttu-id="6c22a-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6c22a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c22a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c22a-111">Permission type</span></span>|<span data-ttu-id="6c22a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6c22a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c22a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c22a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c22a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c22a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c22a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c22a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c22a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c22a-116">Not supported.</span></span>|
|<span data-ttu-id="6c22a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c22a-117">Application</span></span>|<span data-ttu-id="6c22a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c22a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c22a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c22a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6c22a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c22a-120">Request headers</span></span>
|<span data-ttu-id="6c22a-121">标头</span><span class="sxs-lookup"><span data-stu-id="6c22a-121">Header</span></span>|<span data-ttu-id="6c22a-122">值</span><span class="sxs-lookup"><span data-stu-id="6c22a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c22a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c22a-123">Authorization</span></span>|<span data-ttu-id="6c22a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6c22a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c22a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6c22a-125">Accept</span></span>|<span data-ttu-id="6c22a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c22a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c22a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c22a-127">Request body</span></span>
<span data-ttu-id="6c22a-128">在请求正文中，提供 iosEasEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c22a-128">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="6c22a-129">下表显示时创建 iosEasEmailProfileConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6c22a-129">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="6c22a-130">属性</span><span class="sxs-lookup"><span data-stu-id="6c22a-130">Property</span></span>|<span data-ttu-id="6c22a-131">类型</span><span class="sxs-lookup"><span data-stu-id="6c22a-131">Type</span></span>|<span data-ttu-id="6c22a-132">说明</span><span class="sxs-lookup"><span data-stu-id="6c22a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c22a-133">id</span><span class="sxs-lookup"><span data-stu-id="6c22a-133">id</span></span>|<span data-ttu-id="6c22a-134">String</span><span class="sxs-lookup"><span data-stu-id="6c22a-134">String</span></span>|<span data-ttu-id="6c22a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6c22a-135">Key of the entity.</span></span> <span data-ttu-id="6c22a-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c22a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c22a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c22a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6c22a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c22a-138">DateTimeOffset</span></span>|<span data-ttu-id="6c22a-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6c22a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6c22a-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c22a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c22a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c22a-141">roleScopeTagIds</span></span>|<span data-ttu-id="6c22a-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="6c22a-142">String collection</span></span>|<span data-ttu-id="6c22a-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="6c22a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6c22a-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c22a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c22a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6c22a-145">supportsScopeTags</span></span>|<span data-ttu-id="6c22a-146">布尔</span><span class="sxs-lookup"><span data-stu-id="6c22a-146">Boolean</span></span>|<span data-ttu-id="6c22a-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="6c22a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6c22a-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="6c22a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6c22a-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="6c22a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6c22a-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6c22a-150">This property is read-only.</span></span> <span data-ttu-id="6c22a-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c22a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c22a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c22a-152">createdDateTime</span></span>|<span data-ttu-id="6c22a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c22a-153">DateTimeOffset</span></span>|<span data-ttu-id="6c22a-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6c22a-154">DateTime the object was created.</span></span> <span data-ttu-id="6c22a-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c22a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c22a-156">description</span><span class="sxs-lookup"><span data-stu-id="6c22a-156">description</span></span>|<span data-ttu-id="6c22a-157">String</span><span class="sxs-lookup"><span data-stu-id="6c22a-157">String</span></span>|<span data-ttu-id="6c22a-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6c22a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6c22a-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c22a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c22a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6c22a-160">displayName</span></span>|<span data-ttu-id="6c22a-161">String</span><span class="sxs-lookup"><span data-stu-id="6c22a-161">String</span></span>|<span data-ttu-id="6c22a-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6c22a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6c22a-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c22a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c22a-164">version</span><span class="sxs-lookup"><span data-stu-id="6c22a-164">version</span></span>|<span data-ttu-id="6c22a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6c22a-165">Int32</span></span>|<span data-ttu-id="6c22a-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6c22a-166">Version of the device configuration.</span></span> <span data-ttu-id="6c22a-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c22a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c22a-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="6c22a-168">usernameSource</span></span>|[<span data-ttu-id="6c22a-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="6c22a-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="6c22a-170">Username 属性是从 AAD 选取并在设备上安装之前将其插入此配置文件。</span><span class="sxs-lookup"><span data-stu-id="6c22a-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6c22a-171">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="6c22a-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="6c22a-172">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="6c22a-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6c22a-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="6c22a-173">usernameAADSource</span></span>|[<span data-ttu-id="6c22a-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="6c22a-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="6c22a-175">AAD 字段，将用于检索用户名电子邮件配置文件的名称。</span><span class="sxs-lookup"><span data-stu-id="6c22a-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="6c22a-176">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="6c22a-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="6c22a-177">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="6c22a-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="6c22a-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="6c22a-178">userDomainNameSource</span></span>|[<span data-ttu-id="6c22a-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="6c22a-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="6c22a-180">是从 AAD 选取并在设备上安装之前将其插入此配置文件的用户域名属性。</span><span class="sxs-lookup"><span data-stu-id="6c22a-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6c22a-181">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="6c22a-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="6c22a-182">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="6c22a-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="6c22a-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="6c22a-183">customDomainName</span></span>|<span data-ttu-id="6c22a-184">字符串</span><span class="sxs-lookup"><span data-stu-id="6c22a-184">String</span></span>|<span data-ttu-id="6c22a-185">在设备上安装之前生成的电子邮件配置文件时使用的自定义域名称值。</span><span class="sxs-lookup"><span data-stu-id="6c22a-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="6c22a-186">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="6c22a-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="6c22a-187">accountName</span><span class="sxs-lookup"><span data-stu-id="6c22a-187">accountName</span></span>|<span data-ttu-id="6c22a-188">字符串</span><span class="sxs-lookup"><span data-stu-id="6c22a-188">String</span></span>|<span data-ttu-id="6c22a-189">帐户名。</span><span class="sxs-lookup"><span data-stu-id="6c22a-189">Account name.</span></span>|
|<span data-ttu-id="6c22a-190">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6c22a-190">authenticationMethod</span></span>|[<span data-ttu-id="6c22a-191">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6c22a-191">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="6c22a-192">此电子邮件配置文件的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="6c22a-192">Authentication method for this Email profile.</span></span> <span data-ttu-id="6c22a-193">可取值为：`usernameAndPassword`、`certificate`。</span><span class="sxs-lookup"><span data-stu-id="6c22a-193">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="6c22a-194">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="6c22a-194">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="6c22a-195">布尔</span><span class="sxs-lookup"><span data-stu-id="6c22a-195">Boolean</span></span>|<span data-ttu-id="6c22a-196">指示阻止移动到其他电子邮件帐户的消息。</span><span class="sxs-lookup"><span data-stu-id="6c22a-196">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="6c22a-197">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="6c22a-197">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="6c22a-198">布尔</span><span class="sxs-lookup"><span data-stu-id="6c22a-198">Boolean</span></span>|<span data-ttu-id="6c22a-199">指示阻止发送电子邮件从第三方应用程序。</span><span class="sxs-lookup"><span data-stu-id="6c22a-199">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="6c22a-200">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="6c22a-200">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="6c22a-201">布尔</span><span class="sxs-lookup"><span data-stu-id="6c22a-201">Boolean</span></span>|<span data-ttu-id="6c22a-202">指示阻止同步最近使用的电子邮件地址，例如-撰写新电子邮件时。</span><span class="sxs-lookup"><span data-stu-id="6c22a-202">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="6c22a-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="6c22a-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="6c22a-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="6c22a-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="6c22a-205">应返回到同步的时间电子邮件持续时间。</span><span class="sxs-lookup"><span data-stu-id="6c22a-205">Duration of time email should be synced back to.</span></span> <span data-ttu-id="6c22a-206">.</span><span class="sxs-lookup"><span data-stu-id="6c22a-206"></span></span> <span data-ttu-id="6c22a-207">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited`。</span><span class="sxs-lookup"><span data-stu-id="6c22a-207">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="6c22a-208">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="6c22a-208">emailAddressSource</span></span>|[<span data-ttu-id="6c22a-209">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="6c22a-209">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="6c22a-210">电子邮件是从 AAD 选取并在设备上安装之前将其插入此配置文件的属性。</span><span class="sxs-lookup"><span data-stu-id="6c22a-210">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6c22a-211">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="6c22a-211">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6c22a-212">hostName</span><span class="sxs-lookup"><span data-stu-id="6c22a-212">hostName</span></span>|<span data-ttu-id="6c22a-213">String</span><span class="sxs-lookup"><span data-stu-id="6c22a-213">String</span></span>|<span data-ttu-id="6c22a-214">Exchange 的 (URL) 的位置的本机邮件应用程序连接到。</span><span class="sxs-lookup"><span data-stu-id="6c22a-214">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="6c22a-215">requireSmime</span><span class="sxs-lookup"><span data-stu-id="6c22a-215">requireSmime</span></span>|<span data-ttu-id="6c22a-216">布尔</span><span class="sxs-lookup"><span data-stu-id="6c22a-216">Boolean</span></span>|<span data-ttu-id="6c22a-217">指示使用 S/MIME 证书。</span><span class="sxs-lookup"><span data-stu-id="6c22a-217">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="6c22a-218">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="6c22a-218">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="6c22a-219">布尔</span><span class="sxs-lookup"><span data-stu-id="6c22a-219">Boolean</span></span>|<span data-ttu-id="6c22a-220">指示允许未加密的邮件。</span><span class="sxs-lookup"><span data-stu-id="6c22a-220">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="6c22a-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="6c22a-221">requireSsl</span></span>|<span data-ttu-id="6c22a-222">布尔</span><span class="sxs-lookup"><span data-stu-id="6c22a-222">Boolean</span></span>|<span data-ttu-id="6c22a-223">指示使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="6c22a-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="6c22a-224">useOAuth</span><span class="sxs-lookup"><span data-stu-id="6c22a-224">useOAuth</span></span>|<span data-ttu-id="6c22a-225">布尔</span><span class="sxs-lookup"><span data-stu-id="6c22a-225">Boolean</span></span>|<span data-ttu-id="6c22a-226">指定连接是否应使用 OAuth 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="6c22a-226">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="6c22a-227">响应</span><span class="sxs-lookup"><span data-stu-id="6c22a-227">Response</span></span>
<span data-ttu-id="6c22a-228">如果成功，此方法返回`201 Created`响应代码和响应正文中的[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6c22a-228">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c22a-229">示例</span><span class="sxs-lookup"><span data-stu-id="6c22a-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="6c22a-230">请求</span><span class="sxs-lookup"><span data-stu-id="6c22a-230">Request</span></span>
<span data-ttu-id="6c22a-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6c22a-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 974

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "requireSsl": true,
  "useOAuth": true
}
```

### <a name="response"></a><span data-ttu-id="6c22a-232">响应</span><span class="sxs-lookup"><span data-stu-id="6c22a-232">Response</span></span>
<span data-ttu-id="6c22a-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6c22a-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1082

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "id": "e03086da-86da-e030-da86-30e0da8630e0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "requireSsl": true,
  "useOAuth": true
}
```





