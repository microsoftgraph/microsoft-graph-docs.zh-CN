---
title: 创建 windowsPhoneEASEmailProfileConfiguration
description: 创建新的 windowsPhoneEASEmailProfileConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5ae12e9cd535e38305c9f41b50f7a2a073858f28
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836174"
---
# <a name="create-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="74d36-103">创建 windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="74d36-103">Create windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="74d36-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="74d36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74d36-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="74d36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74d36-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="74d36-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74d36-107">创建新的[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="74d36-107">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74d36-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="74d36-108">Prerequisites</span></span>
<span data-ttu-id="74d36-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="74d36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74d36-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="74d36-111">Permission type</span></span>|<span data-ttu-id="74d36-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="74d36-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74d36-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74d36-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74d36-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74d36-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74d36-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74d36-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74d36-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="74d36-116">Not supported.</span></span>|
|<span data-ttu-id="74d36-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="74d36-117">Application</span></span>|<span data-ttu-id="74d36-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="74d36-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74d36-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74d36-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="74d36-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="74d36-120">Request headers</span></span>
|<span data-ttu-id="74d36-121">标头</span><span class="sxs-lookup"><span data-stu-id="74d36-121">Header</span></span>|<span data-ttu-id="74d36-122">值</span><span class="sxs-lookup"><span data-stu-id="74d36-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74d36-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74d36-123">Authorization</span></span>|<span data-ttu-id="74d36-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="74d36-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74d36-125">Accept</span><span class="sxs-lookup"><span data-stu-id="74d36-125">Accept</span></span>|<span data-ttu-id="74d36-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74d36-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74d36-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="74d36-127">Request body</span></span>
<span data-ttu-id="74d36-128">在请求正文中，提供 windowsPhoneEASEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74d36-128">In the request body, supply a JSON representation for the windowsPhoneEASEmailProfileConfiguration object.</span></span>

<span data-ttu-id="74d36-129">下表显示时创建 windowsPhoneEASEmailProfileConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="74d36-129">The following table shows the properties that are required when you create the windowsPhoneEASEmailProfileConfiguration.</span></span>

|<span data-ttu-id="74d36-130">属性</span><span class="sxs-lookup"><span data-stu-id="74d36-130">Property</span></span>|<span data-ttu-id="74d36-131">类型</span><span class="sxs-lookup"><span data-stu-id="74d36-131">Type</span></span>|<span data-ttu-id="74d36-132">说明</span><span class="sxs-lookup"><span data-stu-id="74d36-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74d36-133">id</span><span class="sxs-lookup"><span data-stu-id="74d36-133">id</span></span>|<span data-ttu-id="74d36-134">String</span><span class="sxs-lookup"><span data-stu-id="74d36-134">String</span></span>|<span data-ttu-id="74d36-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="74d36-135">Key of the entity.</span></span> <span data-ttu-id="74d36-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74d36-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74d36-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74d36-137">lastModifiedDateTime</span></span>|<span data-ttu-id="74d36-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74d36-138">DateTimeOffset</span></span>|<span data-ttu-id="74d36-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="74d36-139">DateTime the object was last modified.</span></span> <span data-ttu-id="74d36-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74d36-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74d36-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="74d36-141">roleScopeTagIds</span></span>|<span data-ttu-id="74d36-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="74d36-142">String collection</span></span>|<span data-ttu-id="74d36-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="74d36-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="74d36-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74d36-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74d36-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="74d36-145">supportsScopeTags</span></span>|<span data-ttu-id="74d36-146">布尔</span><span class="sxs-lookup"><span data-stu-id="74d36-146">Boolean</span></span>|<span data-ttu-id="74d36-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="74d36-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="74d36-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="74d36-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="74d36-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="74d36-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="74d36-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="74d36-150">This property is read-only.</span></span> <span data-ttu-id="74d36-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74d36-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74d36-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74d36-152">createdDateTime</span></span>|<span data-ttu-id="74d36-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74d36-153">DateTimeOffset</span></span>|<span data-ttu-id="74d36-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="74d36-154">DateTime the object was created.</span></span> <span data-ttu-id="74d36-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74d36-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74d36-156">description</span><span class="sxs-lookup"><span data-stu-id="74d36-156">description</span></span>|<span data-ttu-id="74d36-157">String</span><span class="sxs-lookup"><span data-stu-id="74d36-157">String</span></span>|<span data-ttu-id="74d36-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="74d36-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="74d36-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74d36-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74d36-160">displayName</span><span class="sxs-lookup"><span data-stu-id="74d36-160">displayName</span></span>|<span data-ttu-id="74d36-161">String</span><span class="sxs-lookup"><span data-stu-id="74d36-161">String</span></span>|<span data-ttu-id="74d36-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="74d36-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="74d36-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74d36-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74d36-164">version</span><span class="sxs-lookup"><span data-stu-id="74d36-164">version</span></span>|<span data-ttu-id="74d36-165">Int32</span><span class="sxs-lookup"><span data-stu-id="74d36-165">Int32</span></span>|<span data-ttu-id="74d36-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="74d36-166">Version of the device configuration.</span></span> <span data-ttu-id="74d36-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74d36-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74d36-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="74d36-168">usernameSource</span></span>|[<span data-ttu-id="74d36-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="74d36-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="74d36-170">Username 属性是从 AAD 选取并在设备上安装之前将其插入此配置文件。</span><span class="sxs-lookup"><span data-stu-id="74d36-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="74d36-171">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="74d36-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="74d36-172">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="74d36-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="74d36-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="74d36-173">usernameAADSource</span></span>|[<span data-ttu-id="74d36-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="74d36-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="74d36-175">AAD 字段，将用于检索用户名电子邮件配置文件的名称。</span><span class="sxs-lookup"><span data-stu-id="74d36-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="74d36-176">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="74d36-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="74d36-177">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="74d36-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="74d36-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="74d36-178">userDomainNameSource</span></span>|[<span data-ttu-id="74d36-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="74d36-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="74d36-180">是从 AAD 选取并在设备上安装之前将其插入此配置文件的用户域名属性。</span><span class="sxs-lookup"><span data-stu-id="74d36-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="74d36-181">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="74d36-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="74d36-182">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="74d36-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="74d36-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="74d36-183">customDomainName</span></span>|<span data-ttu-id="74d36-184">字符串</span><span class="sxs-lookup"><span data-stu-id="74d36-184">String</span></span>|<span data-ttu-id="74d36-185">在设备上安装之前生成的电子邮件配置文件时使用的自定义域名称值。</span><span class="sxs-lookup"><span data-stu-id="74d36-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="74d36-186">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="74d36-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="74d36-187">accountName</span><span class="sxs-lookup"><span data-stu-id="74d36-187">accountName</span></span>|<span data-ttu-id="74d36-188">字符串</span><span class="sxs-lookup"><span data-stu-id="74d36-188">String</span></span>|<span data-ttu-id="74d36-189">帐户名。</span><span class="sxs-lookup"><span data-stu-id="74d36-189">Account name.</span></span>|
|<span data-ttu-id="74d36-190">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="74d36-190">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="74d36-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="74d36-191">Boolean</span></span>|<span data-ttu-id="74d36-192">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="74d36-192">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="74d36-193">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="74d36-193">This property is read-only.</span></span>|
|<span data-ttu-id="74d36-194">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="74d36-194">syncCalendar</span></span>|<span data-ttu-id="74d36-195">布尔</span><span class="sxs-lookup"><span data-stu-id="74d36-195">Boolean</span></span>|<span data-ttu-id="74d36-196">是否同步日历。</span><span class="sxs-lookup"><span data-stu-id="74d36-196">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="74d36-197">syncContacts</span><span class="sxs-lookup"><span data-stu-id="74d36-197">syncContacts</span></span>|<span data-ttu-id="74d36-198">布尔</span><span class="sxs-lookup"><span data-stu-id="74d36-198">Boolean</span></span>|<span data-ttu-id="74d36-199">是否同步联系人。</span><span class="sxs-lookup"><span data-stu-id="74d36-199">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="74d36-200">syncTasks</span><span class="sxs-lookup"><span data-stu-id="74d36-200">syncTasks</span></span>|<span data-ttu-id="74d36-201">布尔</span><span class="sxs-lookup"><span data-stu-id="74d36-201">Boolean</span></span>|<span data-ttu-id="74d36-202">是否同步任务。</span><span class="sxs-lookup"><span data-stu-id="74d36-202">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="74d36-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="74d36-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="74d36-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="74d36-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="74d36-205">若要同步的电子邮件的持续时间。可能的值为： `userDefined`， `oneDay`， `threeDays`， `oneWeek`， `twoWeeks`， `oneMonth`， `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="74d36-205">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="74d36-206">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="74d36-206">emailAddressSource</span></span>|[<span data-ttu-id="74d36-207">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="74d36-207">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="74d36-208">电子邮件是从 AAD 选取并在设备上安装之前将其插入此配置文件的属性。</span><span class="sxs-lookup"><span data-stu-id="74d36-208">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="74d36-209">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="74d36-209">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="74d36-210">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="74d36-210">emailSyncSchedule</span></span>|[<span data-ttu-id="74d36-211">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="74d36-211">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="74d36-212">电子邮件的同步计划。</span><span class="sxs-lookup"><span data-stu-id="74d36-212">Email sync schedule.</span></span> <span data-ttu-id="74d36-213">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="74d36-213">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="74d36-214">hostName</span><span class="sxs-lookup"><span data-stu-id="74d36-214">hostName</span></span>|<span data-ttu-id="74d36-215">String</span><span class="sxs-lookup"><span data-stu-id="74d36-215">String</span></span>|<span data-ttu-id="74d36-216">Exchange 的 (URL) 的位置的本机邮件应用程序连接到。</span><span class="sxs-lookup"><span data-stu-id="74d36-216">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="74d36-217">requireSsl</span><span class="sxs-lookup"><span data-stu-id="74d36-217">requireSsl</span></span>|<span data-ttu-id="74d36-218">布尔</span><span class="sxs-lookup"><span data-stu-id="74d36-218">Boolean</span></span>|<span data-ttu-id="74d36-219">指示使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="74d36-219">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="74d36-220">响应</span><span class="sxs-lookup"><span data-stu-id="74d36-220">Response</span></span>
<span data-ttu-id="74d36-221">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="74d36-221">If successful, this method returns a `201 Created` response code and a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74d36-222">示例</span><span class="sxs-lookup"><span data-stu-id="74d36-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="74d36-223">请求</span><span class="sxs-lookup"><span data-stu-id="74d36-223">Request</span></span>
<span data-ttu-id="74d36-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74d36-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 858

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
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
  "applyOnlyToWindowsPhone81": true,
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

### <a name="response"></a><span data-ttu-id="74d36-225">响应</span><span class="sxs-lookup"><span data-stu-id="74d36-225">Response</span></span>
<span data-ttu-id="74d36-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="74d36-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 966

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
  "id": "554f402a-402a-554f-2a40-4f552a404f55",
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
  "applyOnlyToWindowsPhone81": true,
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





