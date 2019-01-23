---
title: 创建 windowsPhoneEASEmailProfileConfiguration
description: 创建新的 windowsPhoneEASEmailProfileConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b304c7b45ef487845a66ee6df74e74195aa46ad3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408556"
---
# <a name="create-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="37c89-103">创建 windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="37c89-103">Create windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="37c89-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="37c89-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="37c89-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="37c89-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37c89-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="37c89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37c89-107">创建新的[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="37c89-107">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37c89-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="37c89-108">Prerequisites</span></span>
<span data-ttu-id="37c89-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="37c89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="37c89-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="37c89-111">Permission type</span></span>|<span data-ttu-id="37c89-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="37c89-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37c89-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37c89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37c89-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37c89-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37c89-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37c89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37c89-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="37c89-116">Not supported.</span></span>|
|<span data-ttu-id="37c89-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="37c89-117">Application</span></span>|<span data-ttu-id="37c89-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="37c89-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37c89-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37c89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="37c89-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="37c89-120">Request headers</span></span>
|<span data-ttu-id="37c89-121">标头</span><span class="sxs-lookup"><span data-stu-id="37c89-121">Header</span></span>|<span data-ttu-id="37c89-122">值</span><span class="sxs-lookup"><span data-stu-id="37c89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37c89-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37c89-123">Authorization</span></span>|<span data-ttu-id="37c89-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="37c89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37c89-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37c89-125">Accept</span></span>|<span data-ttu-id="37c89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37c89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37c89-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="37c89-127">Request body</span></span>
<span data-ttu-id="37c89-128">在请求正文中，提供 windowsPhoneEASEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37c89-128">In the request body, supply a JSON representation for the windowsPhoneEASEmailProfileConfiguration object.</span></span>

<span data-ttu-id="37c89-129">下表显示时创建 windowsPhoneEASEmailProfileConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="37c89-129">The following table shows the properties that are required when you create the windowsPhoneEASEmailProfileConfiguration.</span></span>

|<span data-ttu-id="37c89-130">属性</span><span class="sxs-lookup"><span data-stu-id="37c89-130">Property</span></span>|<span data-ttu-id="37c89-131">类型</span><span class="sxs-lookup"><span data-stu-id="37c89-131">Type</span></span>|<span data-ttu-id="37c89-132">说明</span><span class="sxs-lookup"><span data-stu-id="37c89-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37c89-133">id</span><span class="sxs-lookup"><span data-stu-id="37c89-133">id</span></span>|<span data-ttu-id="37c89-134">String</span><span class="sxs-lookup"><span data-stu-id="37c89-134">String</span></span>|<span data-ttu-id="37c89-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="37c89-135">Key of the entity.</span></span> <span data-ttu-id="37c89-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c89-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c89-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37c89-137">lastModifiedDateTime</span></span>|<span data-ttu-id="37c89-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37c89-138">DateTimeOffset</span></span>|<span data-ttu-id="37c89-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="37c89-139">DateTime the object was last modified.</span></span> <span data-ttu-id="37c89-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c89-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c89-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="37c89-141">roleScopeTagIds</span></span>|<span data-ttu-id="37c89-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="37c89-142">String collection</span></span>|<span data-ttu-id="37c89-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="37c89-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="37c89-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c89-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c89-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="37c89-145">supportsScopeTags</span></span>|<span data-ttu-id="37c89-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="37c89-146">Boolean</span></span>|<span data-ttu-id="37c89-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="37c89-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="37c89-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="37c89-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="37c89-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="37c89-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="37c89-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="37c89-150">This property is read-only.</span></span> <span data-ttu-id="37c89-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c89-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c89-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37c89-152">createdDateTime</span></span>|<span data-ttu-id="37c89-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37c89-153">DateTimeOffset</span></span>|<span data-ttu-id="37c89-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="37c89-154">DateTime the object was created.</span></span> <span data-ttu-id="37c89-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c89-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c89-156">description</span><span class="sxs-lookup"><span data-stu-id="37c89-156">description</span></span>|<span data-ttu-id="37c89-157">String</span><span class="sxs-lookup"><span data-stu-id="37c89-157">String</span></span>|<span data-ttu-id="37c89-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="37c89-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="37c89-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c89-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c89-160">displayName</span><span class="sxs-lookup"><span data-stu-id="37c89-160">displayName</span></span>|<span data-ttu-id="37c89-161">String</span><span class="sxs-lookup"><span data-stu-id="37c89-161">String</span></span>|<span data-ttu-id="37c89-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="37c89-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="37c89-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c89-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c89-164">version</span><span class="sxs-lookup"><span data-stu-id="37c89-164">version</span></span>|<span data-ttu-id="37c89-165">Int32</span><span class="sxs-lookup"><span data-stu-id="37c89-165">Int32</span></span>|<span data-ttu-id="37c89-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="37c89-166">Version of the device configuration.</span></span> <span data-ttu-id="37c89-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37c89-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37c89-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="37c89-168">usernameSource</span></span>|[<span data-ttu-id="37c89-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="37c89-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="37c89-170">Username 属性是从 AAD 选取并在设备上安装之前将其插入此配置文件。</span><span class="sxs-lookup"><span data-stu-id="37c89-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="37c89-171">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="37c89-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="37c89-172">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="37c89-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="37c89-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="37c89-173">usernameAADSource</span></span>|[<span data-ttu-id="37c89-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="37c89-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="37c89-175">AAD 字段，将用于检索用户名电子邮件配置文件的名称。</span><span class="sxs-lookup"><span data-stu-id="37c89-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="37c89-176">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="37c89-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="37c89-177">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="37c89-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="37c89-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="37c89-178">userDomainNameSource</span></span>|[<span data-ttu-id="37c89-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="37c89-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="37c89-180">是从 AAD 选取并在设备上安装之前将其插入此配置文件的用户域名属性。</span><span class="sxs-lookup"><span data-stu-id="37c89-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="37c89-181">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="37c89-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="37c89-182">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="37c89-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="37c89-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="37c89-183">customDomainName</span></span>|<span data-ttu-id="37c89-184">String</span><span class="sxs-lookup"><span data-stu-id="37c89-184">String</span></span>|<span data-ttu-id="37c89-185">在设备上安装之前生成的电子邮件配置文件时使用的自定义域名称值。</span><span class="sxs-lookup"><span data-stu-id="37c89-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="37c89-186">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="37c89-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="37c89-187">accountName</span><span class="sxs-lookup"><span data-stu-id="37c89-187">accountName</span></span>|<span data-ttu-id="37c89-188">String</span><span class="sxs-lookup"><span data-stu-id="37c89-188">String</span></span>|<span data-ttu-id="37c89-189">帐户名。</span><span class="sxs-lookup"><span data-stu-id="37c89-189">Account name.</span></span>|
|<span data-ttu-id="37c89-190">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="37c89-190">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="37c89-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="37c89-191">Boolean</span></span>|<span data-ttu-id="37c89-192">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="37c89-192">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="37c89-193">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="37c89-193">This property is read-only.</span></span>|
|<span data-ttu-id="37c89-194">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="37c89-194">syncCalendar</span></span>|<span data-ttu-id="37c89-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="37c89-195">Boolean</span></span>|<span data-ttu-id="37c89-196">是否同步日历。</span><span class="sxs-lookup"><span data-stu-id="37c89-196">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="37c89-197">syncContacts</span><span class="sxs-lookup"><span data-stu-id="37c89-197">syncContacts</span></span>|<span data-ttu-id="37c89-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="37c89-198">Boolean</span></span>|<span data-ttu-id="37c89-199">是否同步联系人。</span><span class="sxs-lookup"><span data-stu-id="37c89-199">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="37c89-200">syncTasks</span><span class="sxs-lookup"><span data-stu-id="37c89-200">syncTasks</span></span>|<span data-ttu-id="37c89-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="37c89-201">Boolean</span></span>|<span data-ttu-id="37c89-202">是否同步任务。</span><span class="sxs-lookup"><span data-stu-id="37c89-202">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="37c89-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="37c89-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="37c89-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="37c89-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="37c89-205">若要同步的电子邮件的持续时间。可能的值为： `userDefined`， `oneDay`， `threeDays`， `oneWeek`， `twoWeeks`， `oneMonth`， `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="37c89-205">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="37c89-206">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="37c89-206">emailAddressSource</span></span>|[<span data-ttu-id="37c89-207">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="37c89-207">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="37c89-208">电子邮件是从 AAD 选取并在设备上安装之前将其插入此配置文件的属性。</span><span class="sxs-lookup"><span data-stu-id="37c89-208">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="37c89-209">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="37c89-209">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="37c89-210">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="37c89-210">emailSyncSchedule</span></span>|[<span data-ttu-id="37c89-211">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="37c89-211">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="37c89-212">电子邮件的同步计划。</span><span class="sxs-lookup"><span data-stu-id="37c89-212">Email sync schedule.</span></span> <span data-ttu-id="37c89-213">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="37c89-213">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="37c89-214">hostName</span><span class="sxs-lookup"><span data-stu-id="37c89-214">hostName</span></span>|<span data-ttu-id="37c89-215">String</span><span class="sxs-lookup"><span data-stu-id="37c89-215">String</span></span>|<span data-ttu-id="37c89-216">Exchange 的 (URL) 的位置的本机邮件应用程序连接到。</span><span class="sxs-lookup"><span data-stu-id="37c89-216">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="37c89-217">requireSsl</span><span class="sxs-lookup"><span data-stu-id="37c89-217">requireSsl</span></span>|<span data-ttu-id="37c89-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="37c89-218">Boolean</span></span>|<span data-ttu-id="37c89-219">指示使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="37c89-219">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="37c89-220">响应</span><span class="sxs-lookup"><span data-stu-id="37c89-220">Response</span></span>
<span data-ttu-id="37c89-221">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="37c89-221">If successful, this method returns a `201 Created` response code and a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37c89-222">示例</span><span class="sxs-lookup"><span data-stu-id="37c89-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="37c89-223">请求</span><span class="sxs-lookup"><span data-stu-id="37c89-223">Request</span></span>
<span data-ttu-id="37c89-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="37c89-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 794

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="37c89-225">响应</span><span class="sxs-lookup"><span data-stu-id="37c89-225">Response</span></span>
<span data-ttu-id="37c89-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="37c89-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




