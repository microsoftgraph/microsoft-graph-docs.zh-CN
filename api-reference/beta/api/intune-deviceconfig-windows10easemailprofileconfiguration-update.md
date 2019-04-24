---
title: 更新 windows10EasEmailProfileConfiguration
description: 更新 windows10EasEmailProfileConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d87cff9e4b7c82b1f75a98cba9b6f0fe43cc692d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32516712"
---
# <a name="update-windows10easemailprofileconfiguration"></a><span data-ttu-id="c9ce8-103">更新 windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="c9ce8-103">Update windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="c9ce8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9ce8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9ce8-106">更新[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-106">Update the properties of a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9ce8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c9ce8-107">Prerequisites</span></span>
<span data-ttu-id="c9ce8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9ce8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9ce8-110">Permission type</span></span>|<span data-ttu-id="c9ce8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c9ce8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9ce8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9ce8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9ce8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9ce8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9ce8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9ce8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9ce8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-115">Not supported.</span></span>|
|<span data-ttu-id="c9ce8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9ce8-116">Application</span></span>|<span data-ttu-id="c9ce8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9ce8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9ce8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c9ce8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9ce8-119">Request headers</span></span>
|<span data-ttu-id="c9ce8-120">标头</span><span class="sxs-lookup"><span data-stu-id="c9ce8-120">Header</span></span>|<span data-ttu-id="c9ce8-121">值</span><span class="sxs-lookup"><span data-stu-id="c9ce8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9ce8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9ce8-122">Authorization</span></span>|<span data-ttu-id="c9ce8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9ce8-124">接受</span><span class="sxs-lookup"><span data-stu-id="c9ce8-124">Accept</span></span>|<span data-ttu-id="c9ce8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9ce8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9ce8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9ce8-126">Request body</span></span>
<span data-ttu-id="c9ce8-127">在请求正文中, 提供[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-127">In the request body, supply a JSON representation for the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="c9ce8-128">下表显示创建[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-128">The following table shows the properties that are required when you create the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="c9ce8-129">属性</span><span class="sxs-lookup"><span data-stu-id="c9ce8-129">Property</span></span>|<span data-ttu-id="c9ce8-130">类型</span><span class="sxs-lookup"><span data-stu-id="c9ce8-130">Type</span></span>|<span data-ttu-id="c9ce8-131">说明</span><span class="sxs-lookup"><span data-stu-id="c9ce8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9ce8-132">id</span><span class="sxs-lookup"><span data-stu-id="c9ce8-132">id</span></span>|<span data-ttu-id="c9ce8-133">String</span><span class="sxs-lookup"><span data-stu-id="c9ce8-133">String</span></span>|<span data-ttu-id="c9ce8-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-134">Key of the entity.</span></span> <span data-ttu-id="c9ce8-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9ce8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ce8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9ce8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c9ce8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9ce8-137">DateTimeOffset</span></span>|<span data-ttu-id="c9ce8-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c9ce8-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9ce8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ce8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c9ce8-140">roleScopeTagIds</span></span>|<span data-ttu-id="c9ce8-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c9ce8-141">String collection</span></span>|<span data-ttu-id="c9ce8-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c9ce8-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9ce8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ce8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c9ce8-144">supportsScopeTags</span></span>|<span data-ttu-id="c9ce8-145">布尔</span><span class="sxs-lookup"><span data-stu-id="c9ce8-145">Boolean</span></span>|<span data-ttu-id="c9ce8-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c9ce8-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c9ce8-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c9ce8-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-149">This property is read-only.</span></span> <span data-ttu-id="c9ce8-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9ce8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ce8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9ce8-151">createdDateTime</span></span>|<span data-ttu-id="c9ce8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9ce8-152">DateTimeOffset</span></span>|<span data-ttu-id="c9ce8-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-153">DateTime the object was created.</span></span> <span data-ttu-id="c9ce8-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9ce8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ce8-155">description</span><span class="sxs-lookup"><span data-stu-id="c9ce8-155">description</span></span>|<span data-ttu-id="c9ce8-156">字符串</span><span class="sxs-lookup"><span data-stu-id="c9ce8-156">String</span></span>|<span data-ttu-id="c9ce8-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c9ce8-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9ce8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ce8-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c9ce8-159">displayName</span></span>|<span data-ttu-id="c9ce8-160">String</span><span class="sxs-lookup"><span data-stu-id="c9ce8-160">String</span></span>|<span data-ttu-id="c9ce8-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c9ce8-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9ce8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ce8-163">version</span><span class="sxs-lookup"><span data-stu-id="c9ce8-163">version</span></span>|<span data-ttu-id="c9ce8-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c9ce8-164">Int32</span></span>|<span data-ttu-id="c9ce8-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-165">Version of the device configuration.</span></span> <span data-ttu-id="c9ce8-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9ce8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ce8-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c9ce8-167">usernameSource</span></span>|[<span data-ttu-id="c9ce8-168">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="c9ce8-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c9ce8-169">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c9ce8-170">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c9ce8-171">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c9ce8-172">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="c9ce8-172">usernameAADSource</span></span>|[<span data-ttu-id="c9ce8-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c9ce8-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="c9ce8-174">AAD 字段的名称, 将用于检索电子邮件配置文件的用户名。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="c9ce8-175">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c9ce8-176">可取值为：`userPrincipalName`、`primarySmtpAddress`、`samAccountName`。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="c9ce8-177">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="c9ce8-177">userDomainNameSource</span></span>|[<span data-ttu-id="c9ce8-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="c9ce8-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="c9ce8-179">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c9ce8-180">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c9ce8-181">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="c9ce8-182">customDomainName</span><span class="sxs-lookup"><span data-stu-id="c9ce8-182">customDomainName</span></span>|<span data-ttu-id="c9ce8-183">字符串</span><span class="sxs-lookup"><span data-stu-id="c9ce8-183">String</span></span>|<span data-ttu-id="c9ce8-184">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="c9ce8-185">继承自[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="c9ce8-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="c9ce8-186">accountName</span><span class="sxs-lookup"><span data-stu-id="c9ce8-186">accountName</span></span>|<span data-ttu-id="c9ce8-187">字符串</span><span class="sxs-lookup"><span data-stu-id="c9ce8-187">String</span></span>|<span data-ttu-id="c9ce8-188">帐户名称。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-188">Account name.</span></span>|
|<span data-ttu-id="c9ce8-189">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="c9ce8-189">syncCalendar</span></span>|<span data-ttu-id="c9ce8-190">布尔</span><span class="sxs-lookup"><span data-stu-id="c9ce8-190">Boolean</span></span>|<span data-ttu-id="c9ce8-191">是否同步日历。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-191">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="c9ce8-192">syncContacts</span><span class="sxs-lookup"><span data-stu-id="c9ce8-192">syncContacts</span></span>|<span data-ttu-id="c9ce8-193">布尔</span><span class="sxs-lookup"><span data-stu-id="c9ce8-193">Boolean</span></span>|<span data-ttu-id="c9ce8-194">是否同步联系人。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-194">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="c9ce8-195">syncTasks</span><span class="sxs-lookup"><span data-stu-id="c9ce8-195">syncTasks</span></span>|<span data-ttu-id="c9ce8-196">布尔</span><span class="sxs-lookup"><span data-stu-id="c9ce8-196">Boolean</span></span>|<span data-ttu-id="c9ce8-197">是否同步任务。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-197">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="c9ce8-198">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="c9ce8-198">durationOfEmailToSync</span></span>|[<span data-ttu-id="c9ce8-199">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="c9ce8-199">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="c9ce8-200">要同步的电子邮件的持续时间。可能的值为`userDefined`: `oneDay`、 `threeDays`、 `oneWeek` `twoWeeks`、、 `oneMonth`、 `unlimited`、。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-200">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="c9ce8-201">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="c9ce8-201">emailAddressSource</span></span>|[<span data-ttu-id="c9ce8-202">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="c9ce8-202">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c9ce8-203">在设备上安装之前, 从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-203">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c9ce8-204">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-204">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c9ce8-205">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="c9ce8-205">emailSyncSchedule</span></span>|[<span data-ttu-id="c9ce8-206">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="c9ce8-206">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="c9ce8-207">电子邮件同步计划。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-207">Email sync schedule.</span></span> <span data-ttu-id="c9ce8-208">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes` 或 `basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-208">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="c9ce8-209">hostName</span><span class="sxs-lookup"><span data-stu-id="c9ce8-209">hostName</span></span>|<span data-ttu-id="c9ce8-210">String</span><span class="sxs-lookup"><span data-stu-id="c9ce8-210">String</span></span>|<span data-ttu-id="c9ce8-211">本机邮件应用程序连接到的 Exchange 位置 (URL)。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-211">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="c9ce8-212">requireSsl</span><span class="sxs-lookup"><span data-stu-id="c9ce8-212">requireSsl</span></span>|<span data-ttu-id="c9ce8-213">布尔</span><span class="sxs-lookup"><span data-stu-id="c9ce8-213">Boolean</span></span>|<span data-ttu-id="c9ce8-214">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-214">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="c9ce8-215">响应</span><span class="sxs-lookup"><span data-stu-id="c9ce8-215">Response</span></span>
<span data-ttu-id="c9ce8-216">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-216">If successful, this method returns a `200 OK` response code and an updated [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9ce8-217">示例</span><span class="sxs-lookup"><span data-stu-id="c9ce8-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9ce8-218">请求</span><span class="sxs-lookup"><span data-stu-id="c9ce8-218">Request</span></span>
<span data-ttu-id="c9ce8-219">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 753

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="c9ce8-220">响应</span><span class="sxs-lookup"><span data-stu-id="c9ce8-220">Response</span></span>
<span data-ttu-id="c9ce8-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c9ce8-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





