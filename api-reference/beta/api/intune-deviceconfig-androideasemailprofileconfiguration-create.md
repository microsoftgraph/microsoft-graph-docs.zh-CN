---
title: 创建 androidEasEmailProfileConfiguration
description: 创建新的 androidEasEmailProfileConfiguration 对象。
ms.openlocfilehash: e989bdec5ab9a02065e3bf9faa13bf4b16e448c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045611"
---
# <a name="create-androideasemailprofileconfiguration"></a><span data-ttu-id="39c77-103">创建 androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="39c77-103">Create androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="39c77-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="39c77-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39c77-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="39c77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39c77-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="39c77-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39c77-107">创建新的[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="39c77-107">Create a new [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39c77-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="39c77-108">Prerequisites</span></span>
<span data-ttu-id="39c77-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="39c77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39c77-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="39c77-111">Permission type</span></span>|<span data-ttu-id="39c77-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="39c77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39c77-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39c77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39c77-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39c77-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39c77-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39c77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39c77-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="39c77-116">Not supported.</span></span>|
|<span data-ttu-id="39c77-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="39c77-117">Application</span></span>|<span data-ttu-id="39c77-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="39c77-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39c77-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39c77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="39c77-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="39c77-120">Request headers</span></span>
|<span data-ttu-id="39c77-121">标头</span><span class="sxs-lookup"><span data-stu-id="39c77-121">Header</span></span>|<span data-ttu-id="39c77-122">值</span><span class="sxs-lookup"><span data-stu-id="39c77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39c77-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="39c77-123">Authorization</span></span>|<span data-ttu-id="39c77-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="39c77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39c77-125">Accept</span><span class="sxs-lookup"><span data-stu-id="39c77-125">Accept</span></span>|<span data-ttu-id="39c77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39c77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39c77-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="39c77-127">Request body</span></span>
<span data-ttu-id="39c77-128">在请求正文中，提供 androidEasEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39c77-128">In the request body, supply a JSON representation for the androidEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="39c77-129">下表显示时创建 androidEasEmailProfileConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="39c77-129">The following table shows the properties that are required when you create the androidEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="39c77-130">属性</span><span class="sxs-lookup"><span data-stu-id="39c77-130">Property</span></span>|<span data-ttu-id="39c77-131">类型</span><span class="sxs-lookup"><span data-stu-id="39c77-131">Type</span></span>|<span data-ttu-id="39c77-132">说明</span><span class="sxs-lookup"><span data-stu-id="39c77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39c77-133">id</span><span class="sxs-lookup"><span data-stu-id="39c77-133">id</span></span>|<span data-ttu-id="39c77-134">String</span><span class="sxs-lookup"><span data-stu-id="39c77-134">String</span></span>|<span data-ttu-id="39c77-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="39c77-135">Key of the entity.</span></span> <span data-ttu-id="39c77-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39c77-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39c77-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39c77-137">lastModifiedDateTime</span></span>|<span data-ttu-id="39c77-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39c77-138">DateTimeOffset</span></span>|<span data-ttu-id="39c77-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="39c77-139">DateTime the object was last modified.</span></span> <span data-ttu-id="39c77-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39c77-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39c77-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="39c77-141">roleScopeTagIds</span></span>|<span data-ttu-id="39c77-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="39c77-142">String collection</span></span>|<span data-ttu-id="39c77-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="39c77-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="39c77-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39c77-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39c77-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="39c77-145">supportsScopeTags</span></span>|<span data-ttu-id="39c77-146">布尔</span><span class="sxs-lookup"><span data-stu-id="39c77-146">Boolean</span></span>|<span data-ttu-id="39c77-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="39c77-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="39c77-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="39c77-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="39c77-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="39c77-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="39c77-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="39c77-150">This property is read-only.</span></span> <span data-ttu-id="39c77-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39c77-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39c77-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39c77-152">createdDateTime</span></span>|<span data-ttu-id="39c77-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39c77-153">DateTimeOffset</span></span>|<span data-ttu-id="39c77-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="39c77-154">DateTime the object was created.</span></span> <span data-ttu-id="39c77-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39c77-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39c77-156">description</span><span class="sxs-lookup"><span data-stu-id="39c77-156">description</span></span>|<span data-ttu-id="39c77-157">String</span><span class="sxs-lookup"><span data-stu-id="39c77-157">String</span></span>|<span data-ttu-id="39c77-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="39c77-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="39c77-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39c77-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39c77-160">displayName</span><span class="sxs-lookup"><span data-stu-id="39c77-160">displayName</span></span>|<span data-ttu-id="39c77-161">String</span><span class="sxs-lookup"><span data-stu-id="39c77-161">String</span></span>|<span data-ttu-id="39c77-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="39c77-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="39c77-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39c77-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39c77-164">version</span><span class="sxs-lookup"><span data-stu-id="39c77-164">version</span></span>|<span data-ttu-id="39c77-165">Int32</span><span class="sxs-lookup"><span data-stu-id="39c77-165">Int32</span></span>|<span data-ttu-id="39c77-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="39c77-166">Version of the device configuration.</span></span> <span data-ttu-id="39c77-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39c77-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39c77-168">accountName</span><span class="sxs-lookup"><span data-stu-id="39c77-168">accountName</span></span>|<span data-ttu-id="39c77-169">字符串</span><span class="sxs-lookup"><span data-stu-id="39c77-169">String</span></span>|<span data-ttu-id="39c77-170">Exchange ActiveSync 帐户名，向用户显示为 EAS (this) 配置文件的名称。</span><span class="sxs-lookup"><span data-stu-id="39c77-170">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="39c77-171">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="39c77-171">authenticationMethod</span></span>|[<span data-ttu-id="39c77-172">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="39c77-172">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="39c77-173">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="39c77-173">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="39c77-174">可取值为：`usernameAndPassword`、`certificate`。</span><span class="sxs-lookup"><span data-stu-id="39c77-174">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="39c77-175">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="39c77-175">syncCalendar</span></span>|<span data-ttu-id="39c77-176">布尔</span><span class="sxs-lookup"><span data-stu-id="39c77-176">Boolean</span></span>|<span data-ttu-id="39c77-177">同步日历的切换。</span><span class="sxs-lookup"><span data-stu-id="39c77-177">Toggles syncing the calendar.</span></span> <span data-ttu-id="39c77-178">如果设置为 false 的日历已在设备上关闭。</span><span class="sxs-lookup"><span data-stu-id="39c77-178">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="39c77-179">syncContacts</span><span class="sxs-lookup"><span data-stu-id="39c77-179">syncContacts</span></span>|<span data-ttu-id="39c77-180">布尔</span><span class="sxs-lookup"><span data-stu-id="39c77-180">Boolean</span></span>|<span data-ttu-id="39c77-181">切换同步联系人。</span><span class="sxs-lookup"><span data-stu-id="39c77-181">Toggles syncing contacts.</span></span> <span data-ttu-id="39c77-182">如果设置为 false 的联系人设备上关闭。</span><span class="sxs-lookup"><span data-stu-id="39c77-182">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="39c77-183">syncTasks</span><span class="sxs-lookup"><span data-stu-id="39c77-183">syncTasks</span></span>|<span data-ttu-id="39c77-184">布尔</span><span class="sxs-lookup"><span data-stu-id="39c77-184">Boolean</span></span>|<span data-ttu-id="39c77-185">同步任务的切换。</span><span class="sxs-lookup"><span data-stu-id="39c77-185">Toggles syncing tasks.</span></span> <span data-ttu-id="39c77-186">如果设置为 false 的任务在设备上关闭。</span><span class="sxs-lookup"><span data-stu-id="39c77-186">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="39c77-187">syncNotes</span><span class="sxs-lookup"><span data-stu-id="39c77-187">syncNotes</span></span>|<span data-ttu-id="39c77-188">布尔</span><span class="sxs-lookup"><span data-stu-id="39c77-188">Boolean</span></span>|<span data-ttu-id="39c77-189">同步注释的切换。</span><span class="sxs-lookup"><span data-stu-id="39c77-189">Toggles syncing notes.</span></span> <span data-ttu-id="39c77-190">如果设置为 false 的说明在设备上关闭。</span><span class="sxs-lookup"><span data-stu-id="39c77-190">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="39c77-191">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="39c77-191">durationOfEmailToSync</span></span>|[<span data-ttu-id="39c77-192">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="39c77-192">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="39c77-193">应为同步的时间电子邮件持续时间。</span><span class="sxs-lookup"><span data-stu-id="39c77-193">Duration of time email should be synced to.</span></span> <span data-ttu-id="39c77-194">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited`。</span><span class="sxs-lookup"><span data-stu-id="39c77-194">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="39c77-195">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="39c77-195">emailAddressSource</span></span>|[<span data-ttu-id="39c77-196">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="39c77-196">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="39c77-197">电子邮件是从 AAD 选取并在设备上安装之前将其插入此配置文件的属性。</span><span class="sxs-lookup"><span data-stu-id="39c77-197">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="39c77-198">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="39c77-198">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="39c77-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="39c77-199">emailSyncSchedule</span></span>|[<span data-ttu-id="39c77-200">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="39c77-200">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="39c77-201">电子邮件的同步计划。</span><span class="sxs-lookup"><span data-stu-id="39c77-201">Email sync schedule.</span></span> <span data-ttu-id="39c77-202">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="39c77-202">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="39c77-203">hostName</span><span class="sxs-lookup"><span data-stu-id="39c77-203">hostName</span></span>|<span data-ttu-id="39c77-204">String</span><span class="sxs-lookup"><span data-stu-id="39c77-204">String</span></span>|<span data-ttu-id="39c77-205">Exchange 位置 (URL) 的本机邮件应用程序连接到。</span><span class="sxs-lookup"><span data-stu-id="39c77-205">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="39c77-206">requireSmime</span><span class="sxs-lookup"><span data-stu-id="39c77-206">requireSmime</span></span>|<span data-ttu-id="39c77-207">布尔</span><span class="sxs-lookup"><span data-stu-id="39c77-207">Boolean</span></span>|<span data-ttu-id="39c77-208">指示使用 S/MIME 证书。</span><span class="sxs-lookup"><span data-stu-id="39c77-208">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="39c77-209">requireSsl</span><span class="sxs-lookup"><span data-stu-id="39c77-209">requireSsl</span></span>|<span data-ttu-id="39c77-210">布尔</span><span class="sxs-lookup"><span data-stu-id="39c77-210">Boolean</span></span>|<span data-ttu-id="39c77-211">指示使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="39c77-211">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="39c77-212">usernameSource</span><span class="sxs-lookup"><span data-stu-id="39c77-212">usernameSource</span></span>|[<span data-ttu-id="39c77-213">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="39c77-213">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="39c77-214">Username 属性是从 AAD 选取并在设备上安装之前将其插入此配置文件。</span><span class="sxs-lookup"><span data-stu-id="39c77-214">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="39c77-215">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="39c77-215">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="39c77-216">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="39c77-216">userDomainNameSource</span></span>|[<span data-ttu-id="39c77-217">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="39c77-217">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="39c77-218">是从 AAD 选取并在设备上安装之前将其插入此配置文件的用户域名属性。</span><span class="sxs-lookup"><span data-stu-id="39c77-218">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="39c77-219">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="39c77-219">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="39c77-220">customDomainName</span><span class="sxs-lookup"><span data-stu-id="39c77-220">customDomainName</span></span>|<span data-ttu-id="39c77-221">字符串</span><span class="sxs-lookup"><span data-stu-id="39c77-221">String</span></span>|<span data-ttu-id="39c77-222">在设备上安装之前生成的电子邮件配置文件时使用的自定义域名称值。</span><span class="sxs-lookup"><span data-stu-id="39c77-222">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="39c77-223">响应</span><span class="sxs-lookup"><span data-stu-id="39c77-223">Response</span></span>
<span data-ttu-id="39c77-224">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="39c77-224">If successful, this method returns a `201 Created` response code and a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39c77-225">示例</span><span class="sxs-lookup"><span data-stu-id="39c77-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="39c77-226">请求</span><span class="sxs-lookup"><span data-stu-id="39c77-226">Request</span></span>
<span data-ttu-id="39c77-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39c77-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 857

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="39c77-228">响应</span><span class="sxs-lookup"><span data-stu-id="39c77-228">Response</span></span>
<span data-ttu-id="39c77-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="39c77-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





