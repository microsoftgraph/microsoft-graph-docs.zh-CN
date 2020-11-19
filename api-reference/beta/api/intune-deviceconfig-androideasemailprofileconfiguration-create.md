---
title: 创建 androidEasEmailProfileConfiguration
description: 创建新的 androidEasEmailProfileConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 43f47908bea42e2e29e06ad126ee3bcf553ffe1c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49239982"
---
# <a name="create-androideasemailprofileconfiguration"></a><span data-ttu-id="472a2-103">创建 androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="472a2-103">Create androidEasEmailProfileConfiguration</span></span>

<span data-ttu-id="472a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="472a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="472a2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="472a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="472a2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="472a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="472a2-107">创建新的 [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="472a2-107">Create a new [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="472a2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="472a2-108">Prerequisites</span></span>
<span data-ttu-id="472a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="472a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="472a2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="472a2-111">Permission type</span></span>|<span data-ttu-id="472a2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="472a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="472a2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="472a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="472a2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="472a2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="472a2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="472a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="472a2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="472a2-116">Not supported.</span></span>|
|<span data-ttu-id="472a2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="472a2-117">Application</span></span>|<span data-ttu-id="472a2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="472a2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="472a2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="472a2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="472a2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="472a2-120">Request headers</span></span>
|<span data-ttu-id="472a2-121">标头</span><span class="sxs-lookup"><span data-stu-id="472a2-121">Header</span></span>|<span data-ttu-id="472a2-122">值</span><span class="sxs-lookup"><span data-stu-id="472a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="472a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="472a2-123">Authorization</span></span>|<span data-ttu-id="472a2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="472a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="472a2-125">接受</span><span class="sxs-lookup"><span data-stu-id="472a2-125">Accept</span></span>|<span data-ttu-id="472a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="472a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="472a2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="472a2-127">Request body</span></span>
<span data-ttu-id="472a2-128">在请求正文中，提供 androidEasEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="472a2-128">In the request body, supply a JSON representation for the androidEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="472a2-129">下表显示创建 androidEasEmailProfileConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="472a2-129">The following table shows the properties that are required when you create the androidEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="472a2-130">属性</span><span class="sxs-lookup"><span data-stu-id="472a2-130">Property</span></span>|<span data-ttu-id="472a2-131">类型</span><span class="sxs-lookup"><span data-stu-id="472a2-131">Type</span></span>|<span data-ttu-id="472a2-132">说明</span><span class="sxs-lookup"><span data-stu-id="472a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="472a2-133">id</span><span class="sxs-lookup"><span data-stu-id="472a2-133">id</span></span>|<span data-ttu-id="472a2-134">String</span><span class="sxs-lookup"><span data-stu-id="472a2-134">String</span></span>|<span data-ttu-id="472a2-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="472a2-135">Key of the entity.</span></span> <span data-ttu-id="472a2-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472a2-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472a2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="472a2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="472a2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="472a2-138">DateTimeOffset</span></span>|<span data-ttu-id="472a2-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="472a2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="472a2-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472a2-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472a2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="472a2-141">roleScopeTagIds</span></span>|<span data-ttu-id="472a2-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="472a2-142">String collection</span></span>|<span data-ttu-id="472a2-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="472a2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="472a2-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472a2-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472a2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="472a2-145">supportsScopeTags</span></span>|<span data-ttu-id="472a2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="472a2-146">Boolean</span></span>|<span data-ttu-id="472a2-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="472a2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="472a2-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="472a2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="472a2-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="472a2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="472a2-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="472a2-150">This property is read-only.</span></span> <span data-ttu-id="472a2-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472a2-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472a2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="472a2-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="472a2-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="472a2-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="472a2-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="472a2-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="472a2-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472a2-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472a2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="472a2-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="472a2-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="472a2-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="472a2-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="472a2-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="472a2-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472a2-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472a2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="472a2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="472a2-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="472a2-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="472a2-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="472a2-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="472a2-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472a2-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472a2-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="472a2-164">createdDateTime</span></span>|<span data-ttu-id="472a2-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="472a2-165">DateTimeOffset</span></span>|<span data-ttu-id="472a2-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="472a2-166">DateTime the object was created.</span></span> <span data-ttu-id="472a2-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472a2-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472a2-168">description</span><span class="sxs-lookup"><span data-stu-id="472a2-168">description</span></span>|<span data-ttu-id="472a2-169">String</span><span class="sxs-lookup"><span data-stu-id="472a2-169">String</span></span>|<span data-ttu-id="472a2-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="472a2-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="472a2-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472a2-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472a2-172">displayName</span><span class="sxs-lookup"><span data-stu-id="472a2-172">displayName</span></span>|<span data-ttu-id="472a2-173">String</span><span class="sxs-lookup"><span data-stu-id="472a2-173">String</span></span>|<span data-ttu-id="472a2-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="472a2-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="472a2-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472a2-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472a2-176">version</span><span class="sxs-lookup"><span data-stu-id="472a2-176">version</span></span>|<span data-ttu-id="472a2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="472a2-177">Int32</span></span>|<span data-ttu-id="472a2-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="472a2-178">Version of the device configuration.</span></span> <span data-ttu-id="472a2-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472a2-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472a2-180">帐户</span><span class="sxs-lookup"><span data-stu-id="472a2-180">accountName</span></span>|<span data-ttu-id="472a2-181">String</span><span class="sxs-lookup"><span data-stu-id="472a2-181">String</span></span>|<span data-ttu-id="472a2-182">Exchange ActiveSync 帐户名称，向用户显示为 "EAS (此) 配置文件" 的名称。</span><span class="sxs-lookup"><span data-stu-id="472a2-182">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="472a2-183">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="472a2-183">authenticationMethod</span></span>|[<span data-ttu-id="472a2-184">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="472a2-184">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="472a2-185">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="472a2-185">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="472a2-186">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="472a2-186">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="472a2-187">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="472a2-187">syncCalendar</span></span>|<span data-ttu-id="472a2-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="472a2-188">Boolean</span></span>|<span data-ttu-id="472a2-189">切换同步日历。</span><span class="sxs-lookup"><span data-stu-id="472a2-189">Toggles syncing the calendar.</span></span> <span data-ttu-id="472a2-190">如果设置为 "false 日历" 将在设备上处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="472a2-190">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="472a2-191">syncContacts</span><span class="sxs-lookup"><span data-stu-id="472a2-191">syncContacts</span></span>|<span data-ttu-id="472a2-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="472a2-192">Boolean</span></span>|<span data-ttu-id="472a2-193">切换同步联系人。</span><span class="sxs-lookup"><span data-stu-id="472a2-193">Toggles syncing contacts.</span></span> <span data-ttu-id="472a2-194">如果设置为 false，则设备上的联系人处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="472a2-194">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="472a2-195">syncTasks</span><span class="sxs-lookup"><span data-stu-id="472a2-195">syncTasks</span></span>|<span data-ttu-id="472a2-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="472a2-196">Boolean</span></span>|<span data-ttu-id="472a2-197">切换同步任务。</span><span class="sxs-lookup"><span data-stu-id="472a2-197">Toggles syncing tasks.</span></span> <span data-ttu-id="472a2-198">如果设备上的 "设置为 false 任务" 处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="472a2-198">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="472a2-199">syncNotes</span><span class="sxs-lookup"><span data-stu-id="472a2-199">syncNotes</span></span>|<span data-ttu-id="472a2-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="472a2-200">Boolean</span></span>|<span data-ttu-id="472a2-201">切换同步注释。</span><span class="sxs-lookup"><span data-stu-id="472a2-201">Toggles syncing notes.</span></span> <span data-ttu-id="472a2-202">如果将设备上的设置为 "false 注释"，则会关闭。</span><span class="sxs-lookup"><span data-stu-id="472a2-202">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="472a2-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="472a2-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="472a2-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="472a2-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="472a2-205">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="472a2-205">Duration of time email should be synced to.</span></span> <span data-ttu-id="472a2-206">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="472a2-206">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="472a2-207">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="472a2-207">emailAddressSource</span></span>|[<span data-ttu-id="472a2-208">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="472a2-208">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="472a2-209">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="472a2-209">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="472a2-210">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="472a2-210">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="472a2-211">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="472a2-211">emailSyncSchedule</span></span>|[<span data-ttu-id="472a2-212">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="472a2-212">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="472a2-213">电子邮件同步计划。</span><span class="sxs-lookup"><span data-stu-id="472a2-213">Email sync schedule.</span></span> <span data-ttu-id="472a2-214">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes` 或 `basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="472a2-214">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="472a2-215">hostName</span><span class="sxs-lookup"><span data-stu-id="472a2-215">hostName</span></span>|<span data-ttu-id="472a2-216">String</span><span class="sxs-lookup"><span data-stu-id="472a2-216">String</span></span>|<span data-ttu-id="472a2-217">本机邮件应用程序连接到的 Exchange 位置 (URL) 。</span><span class="sxs-lookup"><span data-stu-id="472a2-217">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="472a2-218">requireSmime</span><span class="sxs-lookup"><span data-stu-id="472a2-218">requireSmime</span></span>|<span data-ttu-id="472a2-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="472a2-219">Boolean</span></span>|<span data-ttu-id="472a2-220">指示是否使用 S/MIME 证书。</span><span class="sxs-lookup"><span data-stu-id="472a2-220">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="472a2-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="472a2-221">requireSsl</span></span>|<span data-ttu-id="472a2-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="472a2-222">Boolean</span></span>|<span data-ttu-id="472a2-223">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="472a2-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="472a2-224">usernameSource</span><span class="sxs-lookup"><span data-stu-id="472a2-224">usernameSource</span></span>|[<span data-ttu-id="472a2-225">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="472a2-225">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="472a2-226">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="472a2-226">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="472a2-227">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="472a2-227">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="472a2-228">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="472a2-228">userDomainNameSource</span></span>|[<span data-ttu-id="472a2-229">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="472a2-229">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="472a2-230">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="472a2-230">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="472a2-231">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="472a2-231">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="472a2-232">customDomainName</span><span class="sxs-lookup"><span data-stu-id="472a2-232">customDomainName</span></span>|<span data-ttu-id="472a2-233">String</span><span class="sxs-lookup"><span data-stu-id="472a2-233">String</span></span>|<span data-ttu-id="472a2-234">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="472a2-234">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="472a2-235">响应</span><span class="sxs-lookup"><span data-stu-id="472a2-235">Response</span></span>
<span data-ttu-id="472a2-236">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="472a2-236">If successful, this method returns a `201 Created` response code and a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="472a2-237">示例</span><span class="sxs-lookup"><span data-stu-id="472a2-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="472a2-238">请求</span><span class="sxs-lookup"><span data-stu-id="472a2-238">Request</span></span>
<span data-ttu-id="472a2-239">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="472a2-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1566

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="472a2-240">响应</span><span class="sxs-lookup"><span data-stu-id="472a2-240">Response</span></span>
<span data-ttu-id="472a2-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="472a2-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1738

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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




