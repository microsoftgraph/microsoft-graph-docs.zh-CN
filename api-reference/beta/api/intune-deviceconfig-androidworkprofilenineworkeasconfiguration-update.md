---
title: 更新 androidWorkProfileNineWorkEasConfiguration
description: 更新 androidWorkProfileNineWorkEasConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ebc3946ed7269d6c697dc4b99f04a6ef5801be51
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928391"
---
# <a name="update-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="8eea1-103">更新 androidWorkProfileNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="8eea1-103">Update androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="8eea1-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8eea1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8eea1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8eea1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eea1-106">更新[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8eea1-106">Update the properties of a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8eea1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8eea1-107">Prerequisites</span></span>
<span data-ttu-id="8eea1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8eea1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eea1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8eea1-110">Permission type</span></span>|<span data-ttu-id="8eea1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8eea1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8eea1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8eea1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8eea1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eea1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8eea1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8eea1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8eea1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8eea1-115">Not supported.</span></span>|
|<span data-ttu-id="8eea1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8eea1-116">Application</span></span>|<span data-ttu-id="8eea1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8eea1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8eea1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8eea1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8eea1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8eea1-119">Request headers</span></span>
|<span data-ttu-id="8eea1-120">标头</span><span class="sxs-lookup"><span data-stu-id="8eea1-120">Header</span></span>|<span data-ttu-id="8eea1-121">值</span><span class="sxs-lookup"><span data-stu-id="8eea1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8eea1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eea1-122">Authorization</span></span>|<span data-ttu-id="8eea1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8eea1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8eea1-124">接受</span><span class="sxs-lookup"><span data-stu-id="8eea1-124">Accept</span></span>|<span data-ttu-id="8eea1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8eea1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8eea1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8eea1-126">Request body</span></span>
<span data-ttu-id="8eea1-127">在请求正文中, 提供[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8eea1-127">In the request body, supply a JSON representation for the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="8eea1-128">下表显示创建[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8eea1-128">The following table shows the properties that are required when you create the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="8eea1-129">属性</span><span class="sxs-lookup"><span data-stu-id="8eea1-129">Property</span></span>|<span data-ttu-id="8eea1-130">类型</span><span class="sxs-lookup"><span data-stu-id="8eea1-130">Type</span></span>|<span data-ttu-id="8eea1-131">说明</span><span class="sxs-lookup"><span data-stu-id="8eea1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eea1-132">id</span><span class="sxs-lookup"><span data-stu-id="8eea1-132">id</span></span>|<span data-ttu-id="8eea1-133">字符串</span><span class="sxs-lookup"><span data-stu-id="8eea1-133">String</span></span>|<span data-ttu-id="8eea1-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8eea1-134">Key of the entity.</span></span> <span data-ttu-id="8eea1-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8eea1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eea1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8eea1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8eea1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8eea1-137">DateTimeOffset</span></span>|<span data-ttu-id="8eea1-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8eea1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8eea1-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8eea1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eea1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8eea1-140">roleScopeTagIds</span></span>|<span data-ttu-id="8eea1-141">String collection</span><span class="sxs-lookup"><span data-stu-id="8eea1-141">String collection</span></span>|<span data-ttu-id="8eea1-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="8eea1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8eea1-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8eea1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eea1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8eea1-144">supportsScopeTags</span></span>|<span data-ttu-id="8eea1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8eea1-145">Boolean</span></span>|<span data-ttu-id="8eea1-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="8eea1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8eea1-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="8eea1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8eea1-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="8eea1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8eea1-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8eea1-149">This property is read-only.</span></span> <span data-ttu-id="8eea1-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8eea1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eea1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8eea1-151">createdDateTime</span></span>|<span data-ttu-id="8eea1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8eea1-152">DateTimeOffset</span></span>|<span data-ttu-id="8eea1-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8eea1-153">DateTime the object was created.</span></span> <span data-ttu-id="8eea1-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8eea1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eea1-155">说明</span><span class="sxs-lookup"><span data-stu-id="8eea1-155">description</span></span>|<span data-ttu-id="8eea1-156">String</span><span class="sxs-lookup"><span data-stu-id="8eea1-156">String</span></span>|<span data-ttu-id="8eea1-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8eea1-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8eea1-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8eea1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eea1-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8eea1-159">displayName</span></span>|<span data-ttu-id="8eea1-160">String</span><span class="sxs-lookup"><span data-stu-id="8eea1-160">String</span></span>|<span data-ttu-id="8eea1-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8eea1-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8eea1-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8eea1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eea1-163">version</span><span class="sxs-lookup"><span data-stu-id="8eea1-163">version</span></span>|<span data-ttu-id="8eea1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8eea1-164">Int32</span></span>|<span data-ttu-id="8eea1-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8eea1-165">Version of the device configuration.</span></span> <span data-ttu-id="8eea1-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8eea1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eea1-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8eea1-167">authenticationMethod</span></span>|[<span data-ttu-id="8eea1-168">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8eea1-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="8eea1-169">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="8eea1-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="8eea1-170">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="8eea1-170">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="8eea1-171">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="8eea1-171">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="8eea1-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="8eea1-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="8eea1-173">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="8eea1-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="8eea1-174">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="8eea1-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="8eea1-175">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="8eea1-175">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="8eea1-176">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="8eea1-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="8eea1-177">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="8eea1-177">emailAddressSource</span></span>|[<span data-ttu-id="8eea1-178">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="8eea1-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="8eea1-179">在设备上安装之前, 从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="8eea1-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="8eea1-180">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="8eea1-180">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="8eea1-181">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="8eea1-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="8eea1-182">hostName</span><span class="sxs-lookup"><span data-stu-id="8eea1-182">hostName</span></span>|<span data-ttu-id="8eea1-183">String</span><span class="sxs-lookup"><span data-stu-id="8eea1-183">String</span></span>|<span data-ttu-id="8eea1-184">邮件应用程序连接到的 Exchange 位置 (URL)。</span><span class="sxs-lookup"><span data-stu-id="8eea1-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="8eea1-185">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8eea1-185">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="8eea1-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="8eea1-186">requireSsl</span></span>|<span data-ttu-id="8eea1-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="8eea1-187">Boolean</span></span>|<span data-ttu-id="8eea1-188">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="8eea1-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="8eea1-189">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8eea1-189">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="8eea1-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="8eea1-190">usernameSource</span></span>|[<span data-ttu-id="8eea1-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="8eea1-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="8eea1-192">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="8eea1-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="8eea1-193">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="8eea1-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="8eea1-194">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="8eea1-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="8eea1-195">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="8eea1-195">syncCalendar</span></span>|<span data-ttu-id="8eea1-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="8eea1-196">Boolean</span></span>|<span data-ttu-id="8eea1-197">切换同步日历。</span><span class="sxs-lookup"><span data-stu-id="8eea1-197">Toggles syncing the calendar.</span></span> <span data-ttu-id="8eea1-198">如果设置为 false, 则表示设备上的日历处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="8eea1-198">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="8eea1-199">syncContacts</span><span class="sxs-lookup"><span data-stu-id="8eea1-199">syncContacts</span></span>|<span data-ttu-id="8eea1-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="8eea1-200">Boolean</span></span>|<span data-ttu-id="8eea1-201">切换同步联系人。</span><span class="sxs-lookup"><span data-stu-id="8eea1-201">Toggles syncing contacts.</span></span> <span data-ttu-id="8eea1-202">如果设置为 false, 则设备上的联系人处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="8eea1-202">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="8eea1-203">syncTasks</span><span class="sxs-lookup"><span data-stu-id="8eea1-203">syncTasks</span></span>|<span data-ttu-id="8eea1-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="8eea1-204">Boolean</span></span>|<span data-ttu-id="8eea1-205">切换同步任务。</span><span class="sxs-lookup"><span data-stu-id="8eea1-205">Toggles syncing tasks.</span></span> <span data-ttu-id="8eea1-206">如果设备上的 "设置为 false 任务" 处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="8eea1-206">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="8eea1-207">响应</span><span class="sxs-lookup"><span data-stu-id="8eea1-207">Response</span></span>
<span data-ttu-id="8eea1-208">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8eea1-208">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eea1-209">示例</span><span class="sxs-lookup"><span data-stu-id="8eea1-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="8eea1-210">请求</span><span class="sxs-lookup"><span data-stu-id="8eea1-210">Request</span></span>
<span data-ttu-id="8eea1-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8eea1-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 570

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="8eea1-212">响应</span><span class="sxs-lookup"><span data-stu-id="8eea1-212">Response</span></span>
<span data-ttu-id="8eea1-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8eea1-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 742

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "id": "3d9e3a30-3a30-3d9e-303a-9e3d303a9e3d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




