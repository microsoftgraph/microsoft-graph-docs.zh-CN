---
title: 创建 androidEasEmailProfileConfiguration
description: 创建新的 androidEasEmailProfileConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f556f04d63092e9ed385b95e93d48e4b905bedc3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43349481"
---
# <a name="create-androideasemailprofileconfiguration"></a><span data-ttu-id="f1d3a-103">创建 androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1d3a-103">Create androidEasEmailProfileConfiguration</span></span>

<span data-ttu-id="f1d3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1d3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1d3a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1d3a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1d3a-107">创建新的[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-107">Create a new [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1d3a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f1d3a-108">Prerequisites</span></span>
<span data-ttu-id="f1d3a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1d3a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1d3a-111">Permission type</span></span>|<span data-ttu-id="f1d3a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f1d3a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1d3a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1d3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1d3a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1d3a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1d3a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1d3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1d3a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-116">Not supported.</span></span>|
|<span data-ttu-id="f1d3a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1d3a-117">Application</span></span>|<span data-ttu-id="f1d3a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1d3a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1d3a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1d3a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f1d3a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1d3a-120">Request headers</span></span>
|<span data-ttu-id="f1d3a-121">标头</span><span class="sxs-lookup"><span data-stu-id="f1d3a-121">Header</span></span>|<span data-ttu-id="f1d3a-122">值</span><span class="sxs-lookup"><span data-stu-id="f1d3a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1d3a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1d3a-123">Authorization</span></span>|<span data-ttu-id="f1d3a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1d3a-125">接受</span><span class="sxs-lookup"><span data-stu-id="f1d3a-125">Accept</span></span>|<span data-ttu-id="f1d3a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1d3a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1d3a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1d3a-127">Request body</span></span>
<span data-ttu-id="f1d3a-128">在请求正文中，提供 androidEasEmailProfileConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-128">In the request body, supply a JSON representation for the androidEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="f1d3a-129">下表显示创建 androidEasEmailProfileConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-129">The following table shows the properties that are required when you create the androidEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="f1d3a-130">属性</span><span class="sxs-lookup"><span data-stu-id="f1d3a-130">Property</span></span>|<span data-ttu-id="f1d3a-131">类型</span><span class="sxs-lookup"><span data-stu-id="f1d3a-131">Type</span></span>|<span data-ttu-id="f1d3a-132">说明</span><span class="sxs-lookup"><span data-stu-id="f1d3a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1d3a-133">id</span><span class="sxs-lookup"><span data-stu-id="f1d3a-133">id</span></span>|<span data-ttu-id="f1d3a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="f1d3a-134">String</span></span>|<span data-ttu-id="f1d3a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-135">Key of the entity.</span></span> <span data-ttu-id="f1d3a-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1d3a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1d3a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1d3a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f1d3a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1d3a-138">DateTimeOffset</span></span>|<span data-ttu-id="f1d3a-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f1d3a-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1d3a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1d3a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1d3a-141">roleScopeTagIds</span></span>|<span data-ttu-id="f1d3a-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="f1d3a-142">String collection</span></span>|<span data-ttu-id="f1d3a-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f1d3a-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1d3a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1d3a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f1d3a-145">supportsScopeTags</span></span>|<span data-ttu-id="f1d3a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1d3a-146">Boolean</span></span>|<span data-ttu-id="f1d3a-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f1d3a-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f1d3a-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f1d3a-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-150">This property is read-only.</span></span> <span data-ttu-id="f1d3a-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1d3a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1d3a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f1d3a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f1d3a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f1d3a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f1d3a-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f1d3a-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1d3a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1d3a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f1d3a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f1d3a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f1d3a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f1d3a-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f1d3a-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1d3a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1d3a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f1d3a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f1d3a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f1d3a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f1d3a-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f1d3a-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1d3a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1d3a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1d3a-164">createdDateTime</span></span>|<span data-ttu-id="f1d3a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1d3a-165">DateTimeOffset</span></span>|<span data-ttu-id="f1d3a-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-166">DateTime the object was created.</span></span> <span data-ttu-id="f1d3a-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1d3a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1d3a-168">description</span><span class="sxs-lookup"><span data-stu-id="f1d3a-168">description</span></span>|<span data-ttu-id="f1d3a-169">String</span><span class="sxs-lookup"><span data-stu-id="f1d3a-169">String</span></span>|<span data-ttu-id="f1d3a-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1d3a-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1d3a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1d3a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f1d3a-172">displayName</span></span>|<span data-ttu-id="f1d3a-173">String</span><span class="sxs-lookup"><span data-stu-id="f1d3a-173">String</span></span>|<span data-ttu-id="f1d3a-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1d3a-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1d3a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1d3a-176">version</span><span class="sxs-lookup"><span data-stu-id="f1d3a-176">version</span></span>|<span data-ttu-id="f1d3a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f1d3a-177">Int32</span></span>|<span data-ttu-id="f1d3a-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-178">Version of the device configuration.</span></span> <span data-ttu-id="f1d3a-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1d3a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1d3a-180">帐户</span><span class="sxs-lookup"><span data-stu-id="f1d3a-180">accountName</span></span>|<span data-ttu-id="f1d3a-181">字符串</span><span class="sxs-lookup"><span data-stu-id="f1d3a-181">String</span></span>|<span data-ttu-id="f1d3a-182">Exchange ActiveSync 帐户名称，以 EAS （此）配置文件的名称的形式显示给用户。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-182">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="f1d3a-183">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f1d3a-183">authenticationMethod</span></span>|[<span data-ttu-id="f1d3a-184">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f1d3a-184">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="f1d3a-185">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-185">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="f1d3a-186">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-186">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="f1d3a-187">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="f1d3a-187">syncCalendar</span></span>|<span data-ttu-id="f1d3a-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1d3a-188">Boolean</span></span>|<span data-ttu-id="f1d3a-189">切换同步日历。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-189">Toggles syncing the calendar.</span></span> <span data-ttu-id="f1d3a-190">如果设置为 "false 日历" 将在设备上处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-190">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="f1d3a-191">syncContacts</span><span class="sxs-lookup"><span data-stu-id="f1d3a-191">syncContacts</span></span>|<span data-ttu-id="f1d3a-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1d3a-192">Boolean</span></span>|<span data-ttu-id="f1d3a-193">切换同步联系人。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-193">Toggles syncing contacts.</span></span> <span data-ttu-id="f1d3a-194">如果设置为 false，则设备上的联系人处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-194">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="f1d3a-195">syncTasks</span><span class="sxs-lookup"><span data-stu-id="f1d3a-195">syncTasks</span></span>|<span data-ttu-id="f1d3a-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1d3a-196">Boolean</span></span>|<span data-ttu-id="f1d3a-197">切换同步任务。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-197">Toggles syncing tasks.</span></span> <span data-ttu-id="f1d3a-198">如果设备上的 "设置为 false 任务" 处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-198">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="f1d3a-199">syncNotes</span><span class="sxs-lookup"><span data-stu-id="f1d3a-199">syncNotes</span></span>|<span data-ttu-id="f1d3a-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1d3a-200">Boolean</span></span>|<span data-ttu-id="f1d3a-201">切换同步注释。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-201">Toggles syncing notes.</span></span> <span data-ttu-id="f1d3a-202">如果将设备上的设置为 "false 注释"，则会关闭。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-202">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="f1d3a-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="f1d3a-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="f1d3a-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="f1d3a-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="f1d3a-205">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-205">Duration of time email should be synced to.</span></span> <span data-ttu-id="f1d3a-206">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-206">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="f1d3a-207">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="f1d3a-207">emailAddressSource</span></span>|[<span data-ttu-id="f1d3a-208">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="f1d3a-208">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="f1d3a-209">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-209">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f1d3a-210">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-210">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="f1d3a-211">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="f1d3a-211">emailSyncSchedule</span></span>|[<span data-ttu-id="f1d3a-212">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="f1d3a-212">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="f1d3a-213">电子邮件同步计划。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-213">Email sync schedule.</span></span> <span data-ttu-id="f1d3a-214">可取值为：`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes` 或 `basedOnMyUsage`。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-214">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="f1d3a-215">hostName</span><span class="sxs-lookup"><span data-stu-id="f1d3a-215">hostName</span></span>|<span data-ttu-id="f1d3a-216">String</span><span class="sxs-lookup"><span data-stu-id="f1d3a-216">String</span></span>|<span data-ttu-id="f1d3a-217">本机邮件应用程序连接到的 Exchange 位置（URL）。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-217">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="f1d3a-218">requireSmime</span><span class="sxs-lookup"><span data-stu-id="f1d3a-218">requireSmime</span></span>|<span data-ttu-id="f1d3a-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1d3a-219">Boolean</span></span>|<span data-ttu-id="f1d3a-220">指示是否使用 S/MIME 证书。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-220">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="f1d3a-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="f1d3a-221">requireSsl</span></span>|<span data-ttu-id="f1d3a-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1d3a-222">Boolean</span></span>|<span data-ttu-id="f1d3a-223">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="f1d3a-224">usernameSource</span><span class="sxs-lookup"><span data-stu-id="f1d3a-224">usernameSource</span></span>|[<span data-ttu-id="f1d3a-225">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="f1d3a-225">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="f1d3a-226">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-226">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f1d3a-227">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-227">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="f1d3a-228">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="f1d3a-228">userDomainNameSource</span></span>|[<span data-ttu-id="f1d3a-229">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="f1d3a-229">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="f1d3a-230">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 UserDomainname 属性。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-230">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f1d3a-231">可取值为：`fullDomainName`、`netBiosDomainName`。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-231">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="f1d3a-232">customDomainName</span><span class="sxs-lookup"><span data-stu-id="f1d3a-232">customDomainName</span></span>|<span data-ttu-id="f1d3a-233">字符串</span><span class="sxs-lookup"><span data-stu-id="f1d3a-233">String</span></span>|<span data-ttu-id="f1d3a-234">在设备上安装之前生成电子邮件配置文件时使用的自定义域名值。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-234">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="f1d3a-235">响应</span><span class="sxs-lookup"><span data-stu-id="f1d3a-235">Response</span></span>
<span data-ttu-id="f1d3a-236">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-236">If successful, this method returns a `201 Created` response code and a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1d3a-237">示例</span><span class="sxs-lookup"><span data-stu-id="f1d3a-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1d3a-238">请求</span><span class="sxs-lookup"><span data-stu-id="f1d3a-238">Request</span></span>
<span data-ttu-id="f1d3a-239">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-239">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f1d3a-240">响应</span><span class="sxs-lookup"><span data-stu-id="f1d3a-240">Response</span></span>
<span data-ttu-id="f1d3a-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f1d3a-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



