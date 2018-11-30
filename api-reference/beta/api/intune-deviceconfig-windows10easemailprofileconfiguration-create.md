---
title: 创建 windows10EasEmailProfileConfiguration
description: 创建新的 windows10EasEmailProfileConfiguration 对象。
ms.openlocfilehash: 8c3eed8547de75538cfce2a7260deaa0a67fa407
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044437"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="d579a-103">创建 windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="d579a-103">Create windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="d579a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d579a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d579a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d579a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d579a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d579a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d579a-107">创建新的[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d579a-107">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d579a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d579a-108">Prerequisites</span></span>
<span data-ttu-id="d579a-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d579a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d579a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d579a-111">Permission type</span></span>|<span data-ttu-id="d579a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d579a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d579a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d579a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d579a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d579a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d579a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d579a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d579a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d579a-116">Not supported.</span></span>|
|<span data-ttu-id="d579a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d579a-117">Application</span></span>|<span data-ttu-id="d579a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d579a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d579a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d579a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d579a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d579a-120">Request headers</span></span>
|<span data-ttu-id="d579a-121">标头</span><span class="sxs-lookup"><span data-stu-id="d579a-121">Header</span></span>|<span data-ttu-id="d579a-122">值</span><span class="sxs-lookup"><span data-stu-id="d579a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d579a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d579a-123">Authorization</span></span>|<span data-ttu-id="d579a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d579a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d579a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d579a-125">Accept</span></span>|<span data-ttu-id="d579a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d579a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d579a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d579a-127">Request body</span></span>
<span data-ttu-id="d579a-128">在请求正文中，提供 windows10EasEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d579a-128">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="d579a-129">下表显示时创建 windows10EasEmailProfileConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d579a-129">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="d579a-130">属性</span><span class="sxs-lookup"><span data-stu-id="d579a-130">Property</span></span>|<span data-ttu-id="d579a-131">类型</span><span class="sxs-lookup"><span data-stu-id="d579a-131">Type</span></span>|<span data-ttu-id="d579a-132">说明</span><span class="sxs-lookup"><span data-stu-id="d579a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d579a-133">id</span><span class="sxs-lookup"><span data-stu-id="d579a-133">id</span></span>|<span data-ttu-id="d579a-134">String</span><span class="sxs-lookup"><span data-stu-id="d579a-134">String</span></span>|<span data-ttu-id="d579a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d579a-135">Key of the entity.</span></span> <span data-ttu-id="d579a-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d579a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d579a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d579a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d579a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d579a-138">DateTimeOffset</span></span>|<span data-ttu-id="d579a-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d579a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d579a-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d579a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d579a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d579a-141">roleScopeTagIds</span></span>|<span data-ttu-id="d579a-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="d579a-142">String collection</span></span>|<span data-ttu-id="d579a-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="d579a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d579a-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d579a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d579a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d579a-145">supportsScopeTags</span></span>|<span data-ttu-id="d579a-146">布尔</span><span class="sxs-lookup"><span data-stu-id="d579a-146">Boolean</span></span>|<span data-ttu-id="d579a-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="d579a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d579a-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="d579a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d579a-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="d579a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d579a-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d579a-150">This property is read-only.</span></span> <span data-ttu-id="d579a-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d579a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d579a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d579a-152">createdDateTime</span></span>|<span data-ttu-id="d579a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d579a-153">DateTimeOffset</span></span>|<span data-ttu-id="d579a-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d579a-154">DateTime the object was created.</span></span> <span data-ttu-id="d579a-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d579a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d579a-156">description</span><span class="sxs-lookup"><span data-stu-id="d579a-156">description</span></span>|<span data-ttu-id="d579a-157">String</span><span class="sxs-lookup"><span data-stu-id="d579a-157">String</span></span>|<span data-ttu-id="d579a-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d579a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d579a-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d579a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d579a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d579a-160">displayName</span></span>|<span data-ttu-id="d579a-161">String</span><span class="sxs-lookup"><span data-stu-id="d579a-161">String</span></span>|<span data-ttu-id="d579a-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d579a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d579a-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d579a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d579a-164">version</span><span class="sxs-lookup"><span data-stu-id="d579a-164">version</span></span>|<span data-ttu-id="d579a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d579a-165">Int32</span></span>|<span data-ttu-id="d579a-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d579a-166">Version of the device configuration.</span></span> <span data-ttu-id="d579a-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d579a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d579a-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d579a-168">usernameSource</span></span>|[<span data-ttu-id="d579a-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="d579a-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d579a-170">Username 属性是从 AAD 选取并在设备上安装之前将其插入此配置文件。</span><span class="sxs-lookup"><span data-stu-id="d579a-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d579a-171">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="d579a-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d579a-172">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="d579a-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d579a-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="d579a-173">usernameAADSource</span></span>|[<span data-ttu-id="d579a-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d579a-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="d579a-175">AAD 字段，将用于检索用户名电子邮件配置文件的名称。</span><span class="sxs-lookup"><span data-stu-id="d579a-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="d579a-176">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="d579a-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d579a-177">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="d579a-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="d579a-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="d579a-178">userDomainNameSource</span></span>|[<span data-ttu-id="d579a-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="d579a-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="d579a-180">是从 AAD 选取并在设备上安装之前将其插入此配置文件的用户域名属性。</span><span class="sxs-lookup"><span data-stu-id="d579a-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d579a-181">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="d579a-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d579a-182">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="d579a-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="d579a-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="d579a-183">customDomainName</span></span>|<span data-ttu-id="d579a-184">字符串</span><span class="sxs-lookup"><span data-stu-id="d579a-184">String</span></span>|<span data-ttu-id="d579a-185">在设备上安装之前生成的电子邮件配置文件时使用的自定义域名称值。</span><span class="sxs-lookup"><span data-stu-id="d579a-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="d579a-186">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="d579a-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="d579a-187">accountName</span><span class="sxs-lookup"><span data-stu-id="d579a-187">accountName</span></span>|<span data-ttu-id="d579a-188">字符串</span><span class="sxs-lookup"><span data-stu-id="d579a-188">String</span></span>|<span data-ttu-id="d579a-189">帐户名。</span><span class="sxs-lookup"><span data-stu-id="d579a-189">Account name.</span></span>|
|<span data-ttu-id="d579a-190">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="d579a-190">syncCalendar</span></span>|<span data-ttu-id="d579a-191">布尔</span><span class="sxs-lookup"><span data-stu-id="d579a-191">Boolean</span></span>|<span data-ttu-id="d579a-192">是否同步日历。</span><span class="sxs-lookup"><span data-stu-id="d579a-192">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="d579a-193">syncContacts</span><span class="sxs-lookup"><span data-stu-id="d579a-193">syncContacts</span></span>|<span data-ttu-id="d579a-194">布尔</span><span class="sxs-lookup"><span data-stu-id="d579a-194">Boolean</span></span>|<span data-ttu-id="d579a-195">是否同步联系人。</span><span class="sxs-lookup"><span data-stu-id="d579a-195">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="d579a-196">syncTasks</span><span class="sxs-lookup"><span data-stu-id="d579a-196">syncTasks</span></span>|<span data-ttu-id="d579a-197">布尔</span><span class="sxs-lookup"><span data-stu-id="d579a-197">Boolean</span></span>|<span data-ttu-id="d579a-198">是否同步任务。</span><span class="sxs-lookup"><span data-stu-id="d579a-198">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="d579a-199">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="d579a-199">durationOfEmailToSync</span></span>|[<span data-ttu-id="d579a-200">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="d579a-200">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="d579a-201">若要同步的电子邮件的持续时间。可能的值为： `userDefined`， `oneDay`， `threeDays`， `oneWeek`， `twoWeeks`， `oneMonth`， `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="d579a-201">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="d579a-202">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="d579a-202">emailAddressSource</span></span>|[<span data-ttu-id="d579a-203">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="d579a-203">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d579a-204">电子邮件是从 AAD 选取并在设备上安装之前将其插入此配置文件的属性。</span><span class="sxs-lookup"><span data-stu-id="d579a-204">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d579a-205">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="d579a-205">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d579a-206">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="d579a-206">emailSyncSchedule</span></span>|[<span data-ttu-id="d579a-207">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="d579a-207">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="d579a-208">电子邮件的同步计划。</span><span class="sxs-lookup"><span data-stu-id="d579a-208">Email sync schedule.</span></span> <span data-ttu-id="d579a-209">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="d579a-209">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="d579a-210">hostName</span><span class="sxs-lookup"><span data-stu-id="d579a-210">hostName</span></span>|<span data-ttu-id="d579a-211">String</span><span class="sxs-lookup"><span data-stu-id="d579a-211">String</span></span>|<span data-ttu-id="d579a-212">Exchange 的 (URL) 的位置的本机邮件应用程序连接到。</span><span class="sxs-lookup"><span data-stu-id="d579a-212">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="d579a-213">requireSsl</span><span class="sxs-lookup"><span data-stu-id="d579a-213">requireSsl</span></span>|<span data-ttu-id="d579a-214">布尔</span><span class="sxs-lookup"><span data-stu-id="d579a-214">Boolean</span></span>|<span data-ttu-id="d579a-215">指示使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="d579a-215">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="d579a-216">响应</span><span class="sxs-lookup"><span data-stu-id="d579a-216">Response</span></span>
<span data-ttu-id="d579a-217">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d579a-217">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d579a-218">示例</span><span class="sxs-lookup"><span data-stu-id="d579a-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="d579a-219">请求</span><span class="sxs-lookup"><span data-stu-id="d579a-219">Request</span></span>
<span data-ttu-id="d579a-220">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d579a-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 817

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="d579a-221">响应</span><span class="sxs-lookup"><span data-stu-id="d579a-221">Response</span></span>
<span data-ttu-id="d579a-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d579a-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 925

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
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





