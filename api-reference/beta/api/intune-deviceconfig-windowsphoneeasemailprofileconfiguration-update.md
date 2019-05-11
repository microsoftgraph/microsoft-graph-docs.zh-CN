---
title: 更新 windowsPhoneEASEmailProfileConfiguration
description: 更新 windowsPhoneEASEmailProfileConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3caaf15680c1faed48a2e477b5cee5a81e54f5c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917511"
---
# <a name="update-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="9b3d0-103">更新 windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b3d0-103">Update windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="9b3d0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b3d0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b3d0-106">更新[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-106">Update the properties of a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b3d0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9b3d0-107">Prerequisites</span></span>
<span data-ttu-id="9b3d0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b3d0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b3d0-110">Permission type</span></span>|<span data-ttu-id="9b3d0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9b3d0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b3d0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b3d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b3d0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b3d0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b3d0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b3d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b3d0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-115">Not supported.</span></span>|
|<span data-ttu-id="9b3d0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b3d0-116">Application</span></span>|<span data-ttu-id="9b3d0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b3d0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b3d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9b3d0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b3d0-119">Request headers</span></span>
|<span data-ttu-id="9b3d0-120">标头</span><span class="sxs-lookup"><span data-stu-id="9b3d0-120">Header</span></span>|<span data-ttu-id="9b3d0-121">值</span><span class="sxs-lookup"><span data-stu-id="9b3d0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b3d0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b3d0-122">Authorization</span></span>|<span data-ttu-id="9b3d0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b3d0-124">接受</span><span class="sxs-lookup"><span data-stu-id="9b3d0-124">Accept</span></span>|<span data-ttu-id="9b3d0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b3d0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b3d0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b3d0-126">Request body</span></span>
<span data-ttu-id="9b3d0-127">在请求正文中, 提供[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-127">In the request body, supply a JSON representation for the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="9b3d0-128">下表显示创建[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-128">The following table shows the properties that are required when you create the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="9b3d0-129">属性</span><span class="sxs-lookup"><span data-stu-id="9b3d0-129">Property</span></span>|<span data-ttu-id="9b3d0-130">类型</span><span class="sxs-lookup"><span data-stu-id="9b3d0-130">Type</span></span>|<span data-ttu-id="9b3d0-131">说明</span><span class="sxs-lookup"><span data-stu-id="9b3d0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b3d0-132">id</span><span class="sxs-lookup"><span data-stu-id="9b3d0-132">id</span></span>|<span data-ttu-id="9b3d0-133">字符串</span><span class="sxs-lookup"><span data-stu-id="9b3d0-133">String</span></span>|<span data-ttu-id="9b3d0-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-134">Key of the entity.</span></span> <span data-ttu-id="9b3d0-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b3d0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b3d0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b3d0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9b3d0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b3d0-137">DateTimeOffset</span></span>|<span data-ttu-id="9b3d0-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9b3d0-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b3d0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b3d0-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9b3d0-140">roleScopeTagIds</span></span>|<span data-ttu-id="9b3d0-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9b3d0-141">String collection</span></span>|<span data-ttu-id="9b3d0-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9b3d0-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b3d0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b3d0-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9b3d0-144">supportsScopeTags</span></span>|<span data-ttu-id="9b3d0-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b3d0-145">Boolean</span></span>|<span data-ttu-id="9b3d0-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9b3d0-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9b3d0-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9b3d0-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-149">This property is read-only.</span></span> <span data-ttu-id="9b3d0-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b3d0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b3d0-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b3d0-151">createdDateTime</span></span>|<span data-ttu-id="9b3d0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b3d0-152">DateTimeOffset</span></span>|<span data-ttu-id="9b3d0-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-153">DateTime the object was created.</span></span> <span data-ttu-id="9b3d0-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b3d0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b3d0-155">说明</span><span class="sxs-lookup"><span data-stu-id="9b3d0-155">description</span></span>|<span data-ttu-id="9b3d0-156">String</span><span class="sxs-lookup"><span data-stu-id="9b3d0-156">String</span></span>|<span data-ttu-id="9b3d0-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9b3d0-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b3d0-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b3d0-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9b3d0-159">displayName</span></span>|<span data-ttu-id="9b3d0-160">String</span><span class="sxs-lookup"><span data-stu-id="9b3d0-160">String</span></span>|<span data-ttu-id="9b3d0-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9b3d0-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b3d0-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b3d0-163">version</span><span class="sxs-lookup"><span data-stu-id="9b3d0-163">version</span></span>|<span data-ttu-id="9b3d0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9b3d0-164">Int32</span></span>|<span data-ttu-id="9b3d0-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-165">Version of the device configuration.</span></span> <span data-ttu-id="9b3d0-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b3d0-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b3d0-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="9b3d0-167">usernameSource</span></span>|[<span data-ttu-id="9b3d0-168">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="9b3d0-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="9b3d0-169">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9b3d0-170">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9b3d0-171">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9b3d0-172">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="9b3d0-172">usernameAADSource</span></span>|[<span data-ttu-id="9b3d0-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="9b3d0-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="9b3d0-174">AAD 字段的名称, 将用于检索电子邮件配置文件的用户名。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="9b3d0-175">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9b3d0-176">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="9b3d0-177">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="9b3d0-177">userDomainNameSource</span></span>|[<span data-ttu-id="9b3d0-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="9b3d0-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="9b3d0-179">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9b3d0-180">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9b3d0-181">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="9b3d0-182">customDomainName</span><span class="sxs-lookup"><span data-stu-id="9b3d0-182">customDomainName</span></span>|<span data-ttu-id="9b3d0-183">String</span><span class="sxs-lookup"><span data-stu-id="9b3d0-183">String</span></span>|<span data-ttu-id="9b3d0-184">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="9b3d0-185">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="9b3d0-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="9b3d0-186">帐户</span><span class="sxs-lookup"><span data-stu-id="9b3d0-186">accountName</span></span>|<span data-ttu-id="9b3d0-187">String</span><span class="sxs-lookup"><span data-stu-id="9b3d0-187">String</span></span>|<span data-ttu-id="9b3d0-188">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-188">Account name.</span></span>|
|<span data-ttu-id="9b3d0-189">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="9b3d0-189">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="9b3d0-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b3d0-190">Boolean</span></span>|<span data-ttu-id="9b3d0-191">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-191">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="9b3d0-192">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-192">This property is read-only.</span></span>|
|<span data-ttu-id="9b3d0-193">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="9b3d0-193">syncCalendar</span></span>|<span data-ttu-id="9b3d0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b3d0-194">Boolean</span></span>|<span data-ttu-id="9b3d0-195">是否同步日历。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-195">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="9b3d0-196">syncContacts</span><span class="sxs-lookup"><span data-stu-id="9b3d0-196">syncContacts</span></span>|<span data-ttu-id="9b3d0-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b3d0-197">Boolean</span></span>|<span data-ttu-id="9b3d0-198">是否同步联系人。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-198">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="9b3d0-199">syncTasks</span><span class="sxs-lookup"><span data-stu-id="9b3d0-199">syncTasks</span></span>|<span data-ttu-id="9b3d0-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b3d0-200">Boolean</span></span>|<span data-ttu-id="9b3d0-201">是否同步任务。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-201">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="9b3d0-202">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="9b3d0-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="9b3d0-203">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="9b3d0-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="9b3d0-204">要同步的电子邮件的持续时间。可能的值为`userDefined`: `oneDay`、 `threeDays`、 `oneWeek` `twoWeeks`、、 `oneMonth`、 `unlimited`、。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-204">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="9b3d0-205">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="9b3d0-205">emailAddressSource</span></span>|[<span data-ttu-id="9b3d0-206">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="9b3d0-206">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="9b3d0-207">在设备上安装之前, 从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-207">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9b3d0-208">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-208">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9b3d0-209">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="9b3d0-209">emailSyncSchedule</span></span>|[<span data-ttu-id="9b3d0-210">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="9b3d0-210">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="9b3d0-211">电子邮件同步计划。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-211">Email sync schedule.</span></span> <span data-ttu-id="9b3d0-212">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes` 或 `basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-212">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="9b3d0-213">hostName</span><span class="sxs-lookup"><span data-stu-id="9b3d0-213">hostName</span></span>|<span data-ttu-id="9b3d0-214">String</span><span class="sxs-lookup"><span data-stu-id="9b3d0-214">String</span></span>|<span data-ttu-id="9b3d0-215">本机邮件应用程序连接到的 Exchange 位置 (URL)。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-215">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="9b3d0-216">requireSsl</span><span class="sxs-lookup"><span data-stu-id="9b3d0-216">requireSsl</span></span>|<span data-ttu-id="9b3d0-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b3d0-217">Boolean</span></span>|<span data-ttu-id="9b3d0-218">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-218">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="9b3d0-219">响应</span><span class="sxs-lookup"><span data-stu-id="9b3d0-219">Response</span></span>
<span data-ttu-id="9b3d0-220">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-220">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b3d0-221">示例</span><span class="sxs-lookup"><span data-stu-id="9b3d0-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b3d0-222">请求</span><span class="sxs-lookup"><span data-stu-id="9b3d0-222">Request</span></span>
<span data-ttu-id="9b3d0-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="9b3d0-224">响应</span><span class="sxs-lookup"><span data-stu-id="9b3d0-224">Response</span></span>
<span data-ttu-id="9b3d0-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9b3d0-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




