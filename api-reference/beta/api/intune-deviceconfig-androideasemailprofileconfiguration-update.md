---
title: 更新 androidEasEmailProfileConfiguration
description: 更新 androidEasEmailProfileConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1bf87238d42b9520544380225f985479e9d05bf5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933058"
---
# <a name="update-androideasemailprofileconfiguration"></a><span data-ttu-id="fb609-103">更新 androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb609-103">Update androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="fb609-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fb609-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb609-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb609-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb609-106">更新[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fb609-106">Update the properties of a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb609-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb609-107">Prerequisites</span></span>
<span data-ttu-id="fb609-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb609-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb609-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb609-110">Permission type</span></span>|<span data-ttu-id="fb609-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fb609-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb609-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb609-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb609-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb609-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb609-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb609-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb609-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb609-115">Not supported.</span></span>|
|<span data-ttu-id="fb609-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb609-116">Application</span></span>|<span data-ttu-id="fb609-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb609-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb609-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb609-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fb609-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb609-119">Request headers</span></span>
|<span data-ttu-id="fb609-120">标头</span><span class="sxs-lookup"><span data-stu-id="fb609-120">Header</span></span>|<span data-ttu-id="fb609-121">值</span><span class="sxs-lookup"><span data-stu-id="fb609-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb609-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb609-122">Authorization</span></span>|<span data-ttu-id="fb609-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fb609-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb609-124">接受</span><span class="sxs-lookup"><span data-stu-id="fb609-124">Accept</span></span>|<span data-ttu-id="fb609-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb609-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb609-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb609-126">Request body</span></span>
<span data-ttu-id="fb609-127">在请求正文中, 提供[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb609-127">In the request body, supply a JSON representation for the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="fb609-128">下表显示创建[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fb609-128">The following table shows the properties that are required when you create the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="fb609-129">属性</span><span class="sxs-lookup"><span data-stu-id="fb609-129">Property</span></span>|<span data-ttu-id="fb609-130">类型</span><span class="sxs-lookup"><span data-stu-id="fb609-130">Type</span></span>|<span data-ttu-id="fb609-131">说明</span><span class="sxs-lookup"><span data-stu-id="fb609-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb609-132">id</span><span class="sxs-lookup"><span data-stu-id="fb609-132">id</span></span>|<span data-ttu-id="fb609-133">字符串</span><span class="sxs-lookup"><span data-stu-id="fb609-133">String</span></span>|<span data-ttu-id="fb609-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fb609-134">Key of the entity.</span></span> <span data-ttu-id="fb609-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb609-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb609-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb609-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fb609-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb609-137">DateTimeOffset</span></span>|<span data-ttu-id="fb609-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fb609-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fb609-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb609-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb609-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fb609-140">roleScopeTagIds</span></span>|<span data-ttu-id="fb609-141">String collection</span><span class="sxs-lookup"><span data-stu-id="fb609-141">String collection</span></span>|<span data-ttu-id="fb609-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="fb609-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fb609-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb609-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb609-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fb609-144">supportsScopeTags</span></span>|<span data-ttu-id="fb609-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb609-145">Boolean</span></span>|<span data-ttu-id="fb609-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="fb609-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fb609-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="fb609-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fb609-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="fb609-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fb609-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="fb609-149">This property is read-only.</span></span> <span data-ttu-id="fb609-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb609-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb609-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb609-151">createdDateTime</span></span>|<span data-ttu-id="fb609-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb609-152">DateTimeOffset</span></span>|<span data-ttu-id="fb609-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fb609-153">DateTime the object was created.</span></span> <span data-ttu-id="fb609-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb609-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb609-155">说明</span><span class="sxs-lookup"><span data-stu-id="fb609-155">description</span></span>|<span data-ttu-id="fb609-156">String</span><span class="sxs-lookup"><span data-stu-id="fb609-156">String</span></span>|<span data-ttu-id="fb609-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="fb609-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fb609-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb609-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb609-159">displayName</span><span class="sxs-lookup"><span data-stu-id="fb609-159">displayName</span></span>|<span data-ttu-id="fb609-160">String</span><span class="sxs-lookup"><span data-stu-id="fb609-160">String</span></span>|<span data-ttu-id="fb609-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="fb609-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fb609-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb609-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb609-163">version</span><span class="sxs-lookup"><span data-stu-id="fb609-163">version</span></span>|<span data-ttu-id="fb609-164">Int32</span><span class="sxs-lookup"><span data-stu-id="fb609-164">Int32</span></span>|<span data-ttu-id="fb609-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="fb609-165">Version of the device configuration.</span></span> <span data-ttu-id="fb609-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb609-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb609-167">帐户</span><span class="sxs-lookup"><span data-stu-id="fb609-167">accountName</span></span>|<span data-ttu-id="fb609-168">String</span><span class="sxs-lookup"><span data-stu-id="fb609-168">String</span></span>|<span data-ttu-id="fb609-169">Exchange ActiveSync 帐户名称, 以 EAS (此) 配置文件的名称的形式显示给用户。</span><span class="sxs-lookup"><span data-stu-id="fb609-169">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="fb609-170">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fb609-170">authenticationMethod</span></span>|[<span data-ttu-id="fb609-171">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fb609-171">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="fb609-172">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="fb609-172">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="fb609-173">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="fb609-173">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="fb609-174">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="fb609-174">syncCalendar</span></span>|<span data-ttu-id="fb609-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb609-175">Boolean</span></span>|<span data-ttu-id="fb609-176">切换同步日历。</span><span class="sxs-lookup"><span data-stu-id="fb609-176">Toggles syncing the calendar.</span></span> <span data-ttu-id="fb609-177">如果设置为 "false 日历" 将在设备上处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="fb609-177">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="fb609-178">syncContacts</span><span class="sxs-lookup"><span data-stu-id="fb609-178">syncContacts</span></span>|<span data-ttu-id="fb609-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb609-179">Boolean</span></span>|<span data-ttu-id="fb609-180">切换同步联系人。</span><span class="sxs-lookup"><span data-stu-id="fb609-180">Toggles syncing contacts.</span></span> <span data-ttu-id="fb609-181">如果设置为 false, 则设备上的联系人处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="fb609-181">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="fb609-182">syncTasks</span><span class="sxs-lookup"><span data-stu-id="fb609-182">syncTasks</span></span>|<span data-ttu-id="fb609-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb609-183">Boolean</span></span>|<span data-ttu-id="fb609-184">切换同步任务。</span><span class="sxs-lookup"><span data-stu-id="fb609-184">Toggles syncing tasks.</span></span> <span data-ttu-id="fb609-185">如果设备上的 "设置为 false 任务" 处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="fb609-185">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="fb609-186">syncNotes</span><span class="sxs-lookup"><span data-stu-id="fb609-186">syncNotes</span></span>|<span data-ttu-id="fb609-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb609-187">Boolean</span></span>|<span data-ttu-id="fb609-188">切换同步注释。</span><span class="sxs-lookup"><span data-stu-id="fb609-188">Toggles syncing notes.</span></span> <span data-ttu-id="fb609-189">如果将设备上的设置为 "false 注释", 则会关闭。</span><span class="sxs-lookup"><span data-stu-id="fb609-189">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="fb609-190">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="fb609-190">durationOfEmailToSync</span></span>|[<span data-ttu-id="fb609-191">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="fb609-191">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="fb609-192">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="fb609-192">Duration of time email should be synced to.</span></span> <span data-ttu-id="fb609-193">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="fb609-193">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="fb609-194">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="fb609-194">emailAddressSource</span></span>|[<span data-ttu-id="fb609-195">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="fb609-195">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="fb609-196">在设备上安装之前, 从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="fb609-196">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="fb609-197">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="fb609-197">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="fb609-198">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="fb609-198">emailSyncSchedule</span></span>|[<span data-ttu-id="fb609-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="fb609-199">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="fb609-200">电子邮件同步计划。</span><span class="sxs-lookup"><span data-stu-id="fb609-200">Email sync schedule.</span></span> <span data-ttu-id="fb609-201">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes` 或 `basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="fb609-201">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="fb609-202">hostName</span><span class="sxs-lookup"><span data-stu-id="fb609-202">hostName</span></span>|<span data-ttu-id="fb609-203">String</span><span class="sxs-lookup"><span data-stu-id="fb609-203">String</span></span>|<span data-ttu-id="fb609-204">本机邮件应用程序连接到的 Exchange 位置 (URL)。</span><span class="sxs-lookup"><span data-stu-id="fb609-204">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="fb609-205">requireSmime</span><span class="sxs-lookup"><span data-stu-id="fb609-205">requireSmime</span></span>|<span data-ttu-id="fb609-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb609-206">Boolean</span></span>|<span data-ttu-id="fb609-207">指示是否使用 S/MIME 证书。</span><span class="sxs-lookup"><span data-stu-id="fb609-207">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="fb609-208">requireSsl</span><span class="sxs-lookup"><span data-stu-id="fb609-208">requireSsl</span></span>|<span data-ttu-id="fb609-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb609-209">Boolean</span></span>|<span data-ttu-id="fb609-210">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="fb609-210">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="fb609-211">usernameSource</span><span class="sxs-lookup"><span data-stu-id="fb609-211">usernameSource</span></span>|[<span data-ttu-id="fb609-212">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="fb609-212">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="fb609-213">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="fb609-213">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="fb609-214">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="fb609-214">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="fb609-215">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="fb609-215">userDomainNameSource</span></span>|[<span data-ttu-id="fb609-216">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="fb609-216">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="fb609-217">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="fb609-217">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="fb609-218">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="fb609-218">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="fb609-219">customDomainName</span><span class="sxs-lookup"><span data-stu-id="fb609-219">customDomainName</span></span>|<span data-ttu-id="fb609-220">String</span><span class="sxs-lookup"><span data-stu-id="fb609-220">String</span></span>|<span data-ttu-id="fb609-221">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="fb609-221">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="fb609-222">响应</span><span class="sxs-lookup"><span data-stu-id="fb609-222">Response</span></span>
<span data-ttu-id="fb609-223">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fb609-223">If successful, this method returns a `200 OK` response code and an updated [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb609-224">示例</span><span class="sxs-lookup"><span data-stu-id="fb609-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb609-225">请求</span><span class="sxs-lookup"><span data-stu-id="fb609-225">Request</span></span>
<span data-ttu-id="fb609-226">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb609-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 793

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```

### <a name="response"></a><span data-ttu-id="fb609-227">响应</span><span class="sxs-lookup"><span data-stu-id="fb609-227">Response</span></span>
<span data-ttu-id="fb609-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb609-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 965

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```




