---
title: 创建 androidEasEmailProfileConfiguration
description: 创建新的 androidEasEmailProfileConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e91b5d7442f9e76a27ad34057d8d2b494b10d6ad
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148459"
---
# <a name="create-androideasemailprofileconfiguration"></a><span data-ttu-id="b866b-103">创建 androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="b866b-103">Create androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="b866b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b866b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b866b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b866b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b866b-106">创建新的[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b866b-106">Create a new [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b866b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b866b-107">Prerequisites</span></span>
<span data-ttu-id="b866b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b866b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b866b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b866b-110">Permission type</span></span>|<span data-ttu-id="b866b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b866b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b866b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b866b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b866b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b866b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b866b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b866b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b866b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b866b-115">Not supported.</span></span>|
|<span data-ttu-id="b866b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b866b-116">Application</span></span>|<span data-ttu-id="b866b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b866b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b866b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b866b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b866b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b866b-119">Request headers</span></span>
|<span data-ttu-id="b866b-120">标头</span><span class="sxs-lookup"><span data-stu-id="b866b-120">Header</span></span>|<span data-ttu-id="b866b-121">值</span><span class="sxs-lookup"><span data-stu-id="b866b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b866b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b866b-122">Authorization</span></span>|<span data-ttu-id="b866b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b866b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b866b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b866b-124">Accept</span></span>|<span data-ttu-id="b866b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b866b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b866b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b866b-126">Request body</span></span>
<span data-ttu-id="b866b-127">在请求正文中, 提供 androidEasEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b866b-127">In the request body, supply a JSON representation for the androidEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="b866b-128">下表显示创建 androidEasEmailProfileConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b866b-128">The following table shows the properties that are required when you create the androidEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="b866b-129">属性</span><span class="sxs-lookup"><span data-stu-id="b866b-129">Property</span></span>|<span data-ttu-id="b866b-130">类型</span><span class="sxs-lookup"><span data-stu-id="b866b-130">Type</span></span>|<span data-ttu-id="b866b-131">说明</span><span class="sxs-lookup"><span data-stu-id="b866b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b866b-132">id</span><span class="sxs-lookup"><span data-stu-id="b866b-132">id</span></span>|<span data-ttu-id="b866b-133">String</span><span class="sxs-lookup"><span data-stu-id="b866b-133">String</span></span>|<span data-ttu-id="b866b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b866b-134">Key of the entity.</span></span> <span data-ttu-id="b866b-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b866b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b866b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b866b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b866b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b866b-137">DateTimeOffset</span></span>|<span data-ttu-id="b866b-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b866b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b866b-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b866b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b866b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b866b-140">roleScopeTagIds</span></span>|<span data-ttu-id="b866b-141">String collection</span><span class="sxs-lookup"><span data-stu-id="b866b-141">String collection</span></span>|<span data-ttu-id="b866b-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b866b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b866b-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b866b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b866b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b866b-144">supportsScopeTags</span></span>|<span data-ttu-id="b866b-145">布尔</span><span class="sxs-lookup"><span data-stu-id="b866b-145">Boolean</span></span>|<span data-ttu-id="b866b-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b866b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b866b-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b866b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b866b-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b866b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b866b-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b866b-149">This property is read-only.</span></span> <span data-ttu-id="b866b-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b866b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b866b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b866b-151">createdDateTime</span></span>|<span data-ttu-id="b866b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b866b-152">DateTimeOffset</span></span>|<span data-ttu-id="b866b-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b866b-153">DateTime the object was created.</span></span> <span data-ttu-id="b866b-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b866b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b866b-155">description</span><span class="sxs-lookup"><span data-stu-id="b866b-155">description</span></span>|<span data-ttu-id="b866b-156">String</span><span class="sxs-lookup"><span data-stu-id="b866b-156">String</span></span>|<span data-ttu-id="b866b-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b866b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b866b-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b866b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b866b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b866b-159">displayName</span></span>|<span data-ttu-id="b866b-160">String</span><span class="sxs-lookup"><span data-stu-id="b866b-160">String</span></span>|<span data-ttu-id="b866b-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b866b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b866b-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b866b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b866b-163">version</span><span class="sxs-lookup"><span data-stu-id="b866b-163">version</span></span>|<span data-ttu-id="b866b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b866b-164">Int32</span></span>|<span data-ttu-id="b866b-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b866b-165">Version of the device configuration.</span></span> <span data-ttu-id="b866b-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b866b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b866b-167">accountName</span><span class="sxs-lookup"><span data-stu-id="b866b-167">accountName</span></span>|<span data-ttu-id="b866b-168">字符串</span><span class="sxs-lookup"><span data-stu-id="b866b-168">String</span></span>|<span data-ttu-id="b866b-169">Exchange ActiveSync 帐户名称, 以 EAS (此) 配置文件的名称的形式显示给用户。</span><span class="sxs-lookup"><span data-stu-id="b866b-169">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="b866b-170">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b866b-170">authenticationMethod</span></span>|[<span data-ttu-id="b866b-171">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b866b-171">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="b866b-172">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="b866b-172">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="b866b-173">可取值为：`usernameAndPassword`、`certificate`。</span><span class="sxs-lookup"><span data-stu-id="b866b-173">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="b866b-174">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="b866b-174">syncCalendar</span></span>|<span data-ttu-id="b866b-175">布尔</span><span class="sxs-lookup"><span data-stu-id="b866b-175">Boolean</span></span>|<span data-ttu-id="b866b-176">切换同步日历。</span><span class="sxs-lookup"><span data-stu-id="b866b-176">Toggles syncing the calendar.</span></span> <span data-ttu-id="b866b-177">如果设置为 "false 日历" 将在设备上处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="b866b-177">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="b866b-178">syncContacts</span><span class="sxs-lookup"><span data-stu-id="b866b-178">syncContacts</span></span>|<span data-ttu-id="b866b-179">布尔</span><span class="sxs-lookup"><span data-stu-id="b866b-179">Boolean</span></span>|<span data-ttu-id="b866b-180">切换同步联系人。</span><span class="sxs-lookup"><span data-stu-id="b866b-180">Toggles syncing contacts.</span></span> <span data-ttu-id="b866b-181">如果设置为 false, 则设备上的联系人处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="b866b-181">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="b866b-182">syncTasks</span><span class="sxs-lookup"><span data-stu-id="b866b-182">syncTasks</span></span>|<span data-ttu-id="b866b-183">布尔</span><span class="sxs-lookup"><span data-stu-id="b866b-183">Boolean</span></span>|<span data-ttu-id="b866b-184">切换同步任务。</span><span class="sxs-lookup"><span data-stu-id="b866b-184">Toggles syncing tasks.</span></span> <span data-ttu-id="b866b-185">如果设备上的 "设置为 false 任务" 处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="b866b-185">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="b866b-186">syncNotes</span><span class="sxs-lookup"><span data-stu-id="b866b-186">syncNotes</span></span>|<span data-ttu-id="b866b-187">布尔</span><span class="sxs-lookup"><span data-stu-id="b866b-187">Boolean</span></span>|<span data-ttu-id="b866b-188">切换同步注释。</span><span class="sxs-lookup"><span data-stu-id="b866b-188">Toggles syncing notes.</span></span> <span data-ttu-id="b866b-189">如果将设备上的设置为 "false 注释", 则会关闭。</span><span class="sxs-lookup"><span data-stu-id="b866b-189">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="b866b-190">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="b866b-190">durationOfEmailToSync</span></span>|[<span data-ttu-id="b866b-191">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="b866b-191">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="b866b-192">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="b866b-192">Duration of time email should be synced to.</span></span> <span data-ttu-id="b866b-193">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited`。</span><span class="sxs-lookup"><span data-stu-id="b866b-193">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="b866b-194">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="b866b-194">emailAddressSource</span></span>|[<span data-ttu-id="b866b-195">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="b866b-195">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="b866b-196">在设备上安装之前, 从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="b866b-196">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b866b-197">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="b866b-197">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b866b-198">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="b866b-198">emailSyncSchedule</span></span>|[<span data-ttu-id="b866b-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="b866b-199">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="b866b-200">电子邮件同步计划。</span><span class="sxs-lookup"><span data-stu-id="b866b-200">Email sync schedule.</span></span> <span data-ttu-id="b866b-201">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="b866b-201">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="b866b-202">hostName</span><span class="sxs-lookup"><span data-stu-id="b866b-202">hostName</span></span>|<span data-ttu-id="b866b-203">String</span><span class="sxs-lookup"><span data-stu-id="b866b-203">String</span></span>|<span data-ttu-id="b866b-204">本机邮件应用程序连接到的 Exchange 位置 (URL)。</span><span class="sxs-lookup"><span data-stu-id="b866b-204">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="b866b-205">requireSmime</span><span class="sxs-lookup"><span data-stu-id="b866b-205">requireSmime</span></span>|<span data-ttu-id="b866b-206">布尔</span><span class="sxs-lookup"><span data-stu-id="b866b-206">Boolean</span></span>|<span data-ttu-id="b866b-207">指示是否使用 S/MIME 证书。</span><span class="sxs-lookup"><span data-stu-id="b866b-207">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="b866b-208">requireSsl</span><span class="sxs-lookup"><span data-stu-id="b866b-208">requireSsl</span></span>|<span data-ttu-id="b866b-209">布尔</span><span class="sxs-lookup"><span data-stu-id="b866b-209">Boolean</span></span>|<span data-ttu-id="b866b-210">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="b866b-210">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="b866b-211">usernameSource</span><span class="sxs-lookup"><span data-stu-id="b866b-211">usernameSource</span></span>|[<span data-ttu-id="b866b-212">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="b866b-212">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="b866b-213">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="b866b-213">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b866b-214">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="b866b-214">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b866b-215">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="b866b-215">userDomainNameSource</span></span>|[<span data-ttu-id="b866b-216">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="b866b-216">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="b866b-217">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="b866b-217">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b866b-218">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="b866b-218">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="b866b-219">customDomainName</span><span class="sxs-lookup"><span data-stu-id="b866b-219">customDomainName</span></span>|<span data-ttu-id="b866b-220">字符串</span><span class="sxs-lookup"><span data-stu-id="b866b-220">String</span></span>|<span data-ttu-id="b866b-221">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="b866b-221">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="b866b-222">响应</span><span class="sxs-lookup"><span data-stu-id="b866b-222">Response</span></span>
<span data-ttu-id="b866b-223">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b866b-223">If successful, this method returns a `201 Created` response code and a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b866b-224">示例</span><span class="sxs-lookup"><span data-stu-id="b866b-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="b866b-225">请求</span><span class="sxs-lookup"><span data-stu-id="b866b-225">Request</span></span>
<span data-ttu-id="b866b-226">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b866b-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="b866b-227">响应</span><span class="sxs-lookup"><span data-stu-id="b866b-227">Response</span></span>
<span data-ttu-id="b866b-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b866b-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




