---
title: 更新 iosEasEmailProfileConfiguration
description: 更新 iosEasEmailProfileConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a3d31e88c248d57dcba1eb5531751a2d1e213bf3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858483"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="151d1-103">更新 iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="151d1-103">Update iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="151d1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="151d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="151d1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="151d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="151d1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="151d1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="151d1-107">更新[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="151d1-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="151d1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="151d1-108">Prerequisites</span></span>
<span data-ttu-id="151d1-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="151d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="151d1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="151d1-111">Permission type</span></span>|<span data-ttu-id="151d1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="151d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="151d1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="151d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="151d1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="151d1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="151d1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="151d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="151d1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="151d1-116">Not supported.</span></span>|
|<span data-ttu-id="151d1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="151d1-117">Application</span></span>|<span data-ttu-id="151d1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="151d1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="151d1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="151d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="151d1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="151d1-120">Request headers</span></span>
|<span data-ttu-id="151d1-121">标头</span><span class="sxs-lookup"><span data-stu-id="151d1-121">Header</span></span>|<span data-ttu-id="151d1-122">值</span><span class="sxs-lookup"><span data-stu-id="151d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="151d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="151d1-123">Authorization</span></span>|<span data-ttu-id="151d1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="151d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="151d1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="151d1-125">Accept</span></span>|<span data-ttu-id="151d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="151d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="151d1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="151d1-127">Request body</span></span>
<span data-ttu-id="151d1-128">在请求正文中，提供[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="151d1-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="151d1-129">下表显示时创建[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="151d1-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="151d1-130">属性</span><span class="sxs-lookup"><span data-stu-id="151d1-130">Property</span></span>|<span data-ttu-id="151d1-131">类型</span><span class="sxs-lookup"><span data-stu-id="151d1-131">Type</span></span>|<span data-ttu-id="151d1-132">说明</span><span class="sxs-lookup"><span data-stu-id="151d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="151d1-133">id</span><span class="sxs-lookup"><span data-stu-id="151d1-133">id</span></span>|<span data-ttu-id="151d1-134">String</span><span class="sxs-lookup"><span data-stu-id="151d1-134">String</span></span>|<span data-ttu-id="151d1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="151d1-135">Key of the entity.</span></span> <span data-ttu-id="151d1-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="151d1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="151d1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="151d1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="151d1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="151d1-138">DateTimeOffset</span></span>|<span data-ttu-id="151d1-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="151d1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="151d1-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="151d1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="151d1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="151d1-141">roleScopeTagIds</span></span>|<span data-ttu-id="151d1-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="151d1-142">String collection</span></span>|<span data-ttu-id="151d1-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="151d1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="151d1-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="151d1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="151d1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="151d1-145">supportsScopeTags</span></span>|<span data-ttu-id="151d1-146">布尔</span><span class="sxs-lookup"><span data-stu-id="151d1-146">Boolean</span></span>|<span data-ttu-id="151d1-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="151d1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="151d1-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="151d1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="151d1-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="151d1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="151d1-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="151d1-150">This property is read-only.</span></span> <span data-ttu-id="151d1-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="151d1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="151d1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="151d1-152">createdDateTime</span></span>|<span data-ttu-id="151d1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="151d1-153">DateTimeOffset</span></span>|<span data-ttu-id="151d1-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="151d1-154">DateTime the object was created.</span></span> <span data-ttu-id="151d1-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="151d1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="151d1-156">description</span><span class="sxs-lookup"><span data-stu-id="151d1-156">description</span></span>|<span data-ttu-id="151d1-157">String</span><span class="sxs-lookup"><span data-stu-id="151d1-157">String</span></span>|<span data-ttu-id="151d1-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="151d1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="151d1-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="151d1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="151d1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="151d1-160">displayName</span></span>|<span data-ttu-id="151d1-161">String</span><span class="sxs-lookup"><span data-stu-id="151d1-161">String</span></span>|<span data-ttu-id="151d1-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="151d1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="151d1-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="151d1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="151d1-164">version</span><span class="sxs-lookup"><span data-stu-id="151d1-164">version</span></span>|<span data-ttu-id="151d1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="151d1-165">Int32</span></span>|<span data-ttu-id="151d1-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="151d1-166">Version of the device configuration.</span></span> <span data-ttu-id="151d1-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="151d1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="151d1-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="151d1-168">usernameSource</span></span>|[<span data-ttu-id="151d1-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="151d1-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="151d1-170">Username 属性是从 AAD 选取并在设备上安装之前将其插入此配置文件。</span><span class="sxs-lookup"><span data-stu-id="151d1-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="151d1-171">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="151d1-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="151d1-172">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="151d1-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="151d1-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="151d1-173">usernameAADSource</span></span>|[<span data-ttu-id="151d1-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="151d1-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="151d1-175">AAD 字段，将用于检索用户名电子邮件配置文件的名称。</span><span class="sxs-lookup"><span data-stu-id="151d1-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="151d1-176">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="151d1-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="151d1-177">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="151d1-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="151d1-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="151d1-178">userDomainNameSource</span></span>|[<span data-ttu-id="151d1-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="151d1-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="151d1-180">是从 AAD 选取并在设备上安装之前将其插入此配置文件的用户域名属性。</span><span class="sxs-lookup"><span data-stu-id="151d1-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="151d1-181">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="151d1-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="151d1-182">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="151d1-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="151d1-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="151d1-183">customDomainName</span></span>|<span data-ttu-id="151d1-184">字符串</span><span class="sxs-lookup"><span data-stu-id="151d1-184">String</span></span>|<span data-ttu-id="151d1-185">在设备上安装之前生成的电子邮件配置文件时使用的自定义域名称值。</span><span class="sxs-lookup"><span data-stu-id="151d1-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="151d1-186">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="151d1-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="151d1-187">accountName</span><span class="sxs-lookup"><span data-stu-id="151d1-187">accountName</span></span>|<span data-ttu-id="151d1-188">字符串</span><span class="sxs-lookup"><span data-stu-id="151d1-188">String</span></span>|<span data-ttu-id="151d1-189">帐户名。</span><span class="sxs-lookup"><span data-stu-id="151d1-189">Account name.</span></span>|
|<span data-ttu-id="151d1-190">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="151d1-190">authenticationMethod</span></span>|[<span data-ttu-id="151d1-191">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="151d1-191">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="151d1-192">此电子邮件配置文件的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="151d1-192">Authentication method for this Email profile.</span></span> <span data-ttu-id="151d1-193">可取值为：`usernameAndPassword`、`certificate`。</span><span class="sxs-lookup"><span data-stu-id="151d1-193">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="151d1-194">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="151d1-194">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="151d1-195">布尔</span><span class="sxs-lookup"><span data-stu-id="151d1-195">Boolean</span></span>|<span data-ttu-id="151d1-196">指示阻止移动到其他电子邮件帐户的消息。</span><span class="sxs-lookup"><span data-stu-id="151d1-196">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="151d1-197">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="151d1-197">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="151d1-198">布尔</span><span class="sxs-lookup"><span data-stu-id="151d1-198">Boolean</span></span>|<span data-ttu-id="151d1-199">指示阻止发送电子邮件从第三方应用程序。</span><span class="sxs-lookup"><span data-stu-id="151d1-199">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="151d1-200">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="151d1-200">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="151d1-201">布尔</span><span class="sxs-lookup"><span data-stu-id="151d1-201">Boolean</span></span>|<span data-ttu-id="151d1-202">指示阻止同步最近使用的电子邮件地址，例如-撰写新电子邮件时。</span><span class="sxs-lookup"><span data-stu-id="151d1-202">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="151d1-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="151d1-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="151d1-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="151d1-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="151d1-205">应返回到同步的时间电子邮件持续时间。</span><span class="sxs-lookup"><span data-stu-id="151d1-205">Duration of time email should be synced back to.</span></span> <span data-ttu-id="151d1-206">.</span><span class="sxs-lookup"><span data-stu-id="151d1-206"></span></span> <span data-ttu-id="151d1-207">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited`。</span><span class="sxs-lookup"><span data-stu-id="151d1-207">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="151d1-208">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="151d1-208">emailAddressSource</span></span>|[<span data-ttu-id="151d1-209">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="151d1-209">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="151d1-210">电子邮件是从 AAD 选取并在设备上安装之前将其插入此配置文件的属性。</span><span class="sxs-lookup"><span data-stu-id="151d1-210">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="151d1-211">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="151d1-211">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="151d1-212">hostName</span><span class="sxs-lookup"><span data-stu-id="151d1-212">hostName</span></span>|<span data-ttu-id="151d1-213">String</span><span class="sxs-lookup"><span data-stu-id="151d1-213">String</span></span>|<span data-ttu-id="151d1-214">Exchange 的 (URL) 的位置的本机邮件应用程序连接到。</span><span class="sxs-lookup"><span data-stu-id="151d1-214">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="151d1-215">requireSmime</span><span class="sxs-lookup"><span data-stu-id="151d1-215">requireSmime</span></span>|<span data-ttu-id="151d1-216">布尔</span><span class="sxs-lookup"><span data-stu-id="151d1-216">Boolean</span></span>|<span data-ttu-id="151d1-217">指示使用 S/MIME 证书。</span><span class="sxs-lookup"><span data-stu-id="151d1-217">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="151d1-218">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="151d1-218">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="151d1-219">布尔</span><span class="sxs-lookup"><span data-stu-id="151d1-219">Boolean</span></span>|<span data-ttu-id="151d1-220">指示允许未加密的邮件。</span><span class="sxs-lookup"><span data-stu-id="151d1-220">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="151d1-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="151d1-221">requireSsl</span></span>|<span data-ttu-id="151d1-222">布尔</span><span class="sxs-lookup"><span data-stu-id="151d1-222">Boolean</span></span>|<span data-ttu-id="151d1-223">指示使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="151d1-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="151d1-224">useOAuth</span><span class="sxs-lookup"><span data-stu-id="151d1-224">useOAuth</span></span>|<span data-ttu-id="151d1-225">布尔</span><span class="sxs-lookup"><span data-stu-id="151d1-225">Boolean</span></span>|<span data-ttu-id="151d1-226">指定连接是否应使用 OAuth 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="151d1-226">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="151d1-227">响应</span><span class="sxs-lookup"><span data-stu-id="151d1-227">Response</span></span>
<span data-ttu-id="151d1-228">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="151d1-228">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="151d1-229">示例</span><span class="sxs-lookup"><span data-stu-id="151d1-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="151d1-230">请求</span><span class="sxs-lookup"><span data-stu-id="151d1-230">Request</span></span>
<span data-ttu-id="151d1-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="151d1-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 904

{
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

### <a name="response"></a><span data-ttu-id="151d1-232">响应</span><span class="sxs-lookup"><span data-stu-id="151d1-232">Response</span></span>
<span data-ttu-id="151d1-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="151d1-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





