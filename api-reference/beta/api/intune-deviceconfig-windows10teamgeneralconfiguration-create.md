---
title: 创建 windows10TeamGeneralConfiguration
description: 创建新的 windows10TeamGeneralConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b1b1061e1aba8f1f3aaccc8cdc2d85565a52dadf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836615"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="1dc27-103">创建 windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="1dc27-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="1dc27-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1dc27-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1dc27-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1dc27-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1dc27-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1dc27-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1dc27-107">创建新的 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1dc27-107">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1dc27-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1dc27-108">Prerequisites</span></span>
<span data-ttu-id="1dc27-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1dc27-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dc27-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1dc27-111">Permission type</span></span>|<span data-ttu-id="1dc27-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1dc27-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dc27-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1dc27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1dc27-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dc27-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1dc27-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1dc27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dc27-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1dc27-116">Not supported.</span></span>|
|<span data-ttu-id="1dc27-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1dc27-117">Application</span></span>|<span data-ttu-id="1dc27-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1dc27-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dc27-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1dc27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1dc27-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1dc27-120">Request headers</span></span>
|<span data-ttu-id="1dc27-121">标头</span><span class="sxs-lookup"><span data-stu-id="1dc27-121">Header</span></span>|<span data-ttu-id="1dc27-122">值</span><span class="sxs-lookup"><span data-stu-id="1dc27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dc27-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dc27-123">Authorization</span></span>|<span data-ttu-id="1dc27-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1dc27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dc27-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1dc27-125">Accept</span></span>|<span data-ttu-id="1dc27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1dc27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dc27-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1dc27-127">Request body</span></span>
<span data-ttu-id="1dc27-128">在请求正文中，提供 windows10TeamGeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1dc27-128">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="1dc27-129">下表显示了创建 windows10TeamGeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1dc27-129">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="1dc27-130">属性</span><span class="sxs-lookup"><span data-stu-id="1dc27-130">Property</span></span>|<span data-ttu-id="1dc27-131">类型</span><span class="sxs-lookup"><span data-stu-id="1dc27-131">Type</span></span>|<span data-ttu-id="1dc27-132">说明</span><span class="sxs-lookup"><span data-stu-id="1dc27-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dc27-133">id</span><span class="sxs-lookup"><span data-stu-id="1dc27-133">id</span></span>|<span data-ttu-id="1dc27-134">String</span><span class="sxs-lookup"><span data-stu-id="1dc27-134">String</span></span>|<span data-ttu-id="1dc27-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1dc27-135">Key of the entity.</span></span> <span data-ttu-id="1dc27-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dc27-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dc27-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dc27-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1dc27-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dc27-138">DateTimeOffset</span></span>|<span data-ttu-id="1dc27-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1dc27-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1dc27-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dc27-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dc27-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1dc27-141">roleScopeTagIds</span></span>|<span data-ttu-id="1dc27-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="1dc27-142">String collection</span></span>|<span data-ttu-id="1dc27-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="1dc27-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1dc27-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dc27-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dc27-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1dc27-145">supportsScopeTags</span></span>|<span data-ttu-id="1dc27-146">布尔</span><span class="sxs-lookup"><span data-stu-id="1dc27-146">Boolean</span></span>|<span data-ttu-id="1dc27-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="1dc27-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1dc27-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="1dc27-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1dc27-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="1dc27-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1dc27-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1dc27-150">This property is read-only.</span></span> <span data-ttu-id="1dc27-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dc27-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dc27-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1dc27-152">createdDateTime</span></span>|<span data-ttu-id="1dc27-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dc27-153">DateTimeOffset</span></span>|<span data-ttu-id="1dc27-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1dc27-154">DateTime the object was created.</span></span> <span data-ttu-id="1dc27-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dc27-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dc27-156">description</span><span class="sxs-lookup"><span data-stu-id="1dc27-156">description</span></span>|<span data-ttu-id="1dc27-157">String</span><span class="sxs-lookup"><span data-stu-id="1dc27-157">String</span></span>|<span data-ttu-id="1dc27-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1dc27-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1dc27-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dc27-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dc27-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1dc27-160">displayName</span></span>|<span data-ttu-id="1dc27-161">String</span><span class="sxs-lookup"><span data-stu-id="1dc27-161">String</span></span>|<span data-ttu-id="1dc27-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1dc27-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1dc27-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dc27-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dc27-164">version</span><span class="sxs-lookup"><span data-stu-id="1dc27-164">version</span></span>|<span data-ttu-id="1dc27-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1dc27-165">Int32</span></span>|<span data-ttu-id="1dc27-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1dc27-166">Version of the device configuration.</span></span> <span data-ttu-id="1dc27-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dc27-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dc27-168">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="1dc27-168">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="1dc27-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc27-169">Boolean</span></span>|<span data-ttu-id="1dc27-170">指示是否阻止 Azure 操作见解。</span><span class="sxs-lookup"><span data-stu-id="1dc27-170">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="1dc27-171">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="1dc27-171">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="1dc27-172">String</span><span class="sxs-lookup"><span data-stu-id="1dc27-172">String</span></span>|<span data-ttu-id="1dc27-173">Azure 操作见解工作区 ID。</span><span class="sxs-lookup"><span data-stu-id="1dc27-173">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="1dc27-174">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="1dc27-174">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="1dc27-175">String</span><span class="sxs-lookup"><span data-stu-id="1dc27-175">String</span></span>|<span data-ttu-id="1dc27-176">Azure 操作见解工作区键。</span><span class="sxs-lookup"><span data-stu-id="1dc27-176">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="1dc27-177">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="1dc27-177">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="1dc27-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc27-178">Boolean</span></span>|<span data-ttu-id="1dc27-179">指定是否在启动投影时自动启动 Connect 应用。</span><span class="sxs-lookup"><span data-stu-id="1dc27-179">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="1dc27-180">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="1dc27-180">maintenanceWindowBlocked</span></span>|<span data-ttu-id="1dc27-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc27-181">Boolean</span></span>|<span data-ttu-id="1dc27-182">指示是否阻止设置设备更新的维护时段。</span><span class="sxs-lookup"><span data-stu-id="1dc27-182">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="1dc27-183">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="1dc27-183">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="1dc27-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1dc27-184">Int32</span></span>|<span data-ttu-id="1dc27-185">设备更新的维护时段持续时间。</span><span class="sxs-lookup"><span data-stu-id="1dc27-185">Maintenance window duration for device updates.</span></span> <span data-ttu-id="1dc27-186">有效值为 0 至 5</span><span class="sxs-lookup"><span data-stu-id="1dc27-186">Valid values 0 to 5</span></span>|
|<span data-ttu-id="1dc27-187">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="1dc27-187">maintenanceWindowStartTime</span></span>|<span data-ttu-id="1dc27-188">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1dc27-188">TimeOfDay</span></span>|<span data-ttu-id="1dc27-189">设备更新的维护时段开始时间。</span><span class="sxs-lookup"><span data-stu-id="1dc27-189">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="1dc27-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="1dc27-190">miracastChannel</span></span>|[<span data-ttu-id="1dc27-191">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="1dc27-191">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="1dc27-192">频道。</span><span class="sxs-lookup"><span data-stu-id="1dc27-192">The channel.</span></span> <span data-ttu-id="1dc27-193">可取值为：`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive`。</span><span class="sxs-lookup"><span data-stu-id="1dc27-193">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="1dc27-194">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="1dc27-194">miracastBlocked</span></span>|<span data-ttu-id="1dc27-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc27-195">Boolean</span></span>|<span data-ttu-id="1dc27-196">指示是否阻止无线投影。</span><span class="sxs-lookup"><span data-stu-id="1dc27-196">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="1dc27-197">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="1dc27-197">miracastRequirePin</span></span>|<span data-ttu-id="1dc27-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc27-198">Boolean</span></span>|<span data-ttu-id="1dc27-199">指示是否需要 PIN 才能进行无线投影。</span><span class="sxs-lookup"><span data-stu-id="1dc27-199">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="1dc27-200">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="1dc27-200">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="1dc27-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc27-201">Boolean</span></span>|<span data-ttu-id="1dc27-202">指定是否禁用“开始”菜单中的“我的会议和文件”功能，该功能显示来自 Office 365 的已登录用户的会议和文件。</span><span class="sxs-lookup"><span data-stu-id="1dc27-202">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="1dc27-203">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="1dc27-203">settingsBlockSessionResume</span></span>|<span data-ttu-id="1dc27-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc27-204">Boolean</span></span>|<span data-ttu-id="1dc27-205">指定是否允许在会话超时时恢复会话。</span><span class="sxs-lookup"><span data-stu-id="1dc27-205">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="1dc27-206">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="1dc27-206">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="1dc27-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc27-207">Boolean</span></span>|<span data-ttu-id="1dc27-208">指定是否禁用计划会议的被邀请者自动填充登录对话框。</span><span class="sxs-lookup"><span data-stu-id="1dc27-208">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="1dc27-209">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="1dc27-209">settingsDefaultVolume</span></span>|<span data-ttu-id="1dc27-210">Int32</span><span class="sxs-lookup"><span data-stu-id="1dc27-210">Int32</span></span>|<span data-ttu-id="1dc27-211">指定新会话的默认音量值。</span><span class="sxs-lookup"><span data-stu-id="1dc27-211">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="1dc27-212">允许的值为 0-100。</span><span class="sxs-lookup"><span data-stu-id="1dc27-212">Permitted values are 0-100.</span></span> <span data-ttu-id="1dc27-213">默认值为 45。</span><span class="sxs-lookup"><span data-stu-id="1dc27-213">The default is 45.</span></span> <span data-ttu-id="1dc27-214">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="1dc27-214">Valid values 0 to 100</span></span>|
|<span data-ttu-id="1dc27-215">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="1dc27-215">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="1dc27-216">Int32</span><span class="sxs-lookup"><span data-stu-id="1dc27-216">Int32</span></span>|<span data-ttu-id="1dc27-217">指定 Hub 屏幕关闭前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="1dc27-217">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="1dc27-218">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="1dc27-218">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="1dc27-219">Int32</span><span class="sxs-lookup"><span data-stu-id="1dc27-219">Int32</span></span>|<span data-ttu-id="1dc27-220">指定会话超时前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="1dc27-220">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="1dc27-221">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="1dc27-221">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="1dc27-222">Int32</span><span class="sxs-lookup"><span data-stu-id="1dc27-222">Int32</span></span>|<span data-ttu-id="1dc27-223">指定 Hub 进入睡眠模式前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="1dc27-223">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="1dc27-224">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="1dc27-224">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="1dc27-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc27-225">Boolean</span></span>|<span data-ttu-id="1dc27-226">指示当某人进入会议室时是否阻止欢迎屏幕自动唤醒。</span><span class="sxs-lookup"><span data-stu-id="1dc27-226">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="1dc27-227">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="1dc27-227">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="1dc27-228">String</span><span class="sxs-lookup"><span data-stu-id="1dc27-228">String</span></span>|<span data-ttu-id="1dc27-229">欢迎屏幕背景图像 URL。</span><span class="sxs-lookup"><span data-stu-id="1dc27-229">The welcome screen background image URL.</span></span> <span data-ttu-id="1dc27-230">URL 必须使用 HTTPS 协议并返回 PNG 图像。</span><span class="sxs-lookup"><span data-stu-id="1dc27-230">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="1dc27-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="1dc27-231">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="1dc27-232">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="1dc27-232">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="1dc27-233">显示的欢迎屏幕会议信息。</span><span class="sxs-lookup"><span data-stu-id="1dc27-233">The welcome screen meeting information shown.</span></span> <span data-ttu-id="1dc27-234">可取值为：`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject`。</span><span class="sxs-lookup"><span data-stu-id="1dc27-234">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="1dc27-235">响应</span><span class="sxs-lookup"><span data-stu-id="1dc27-235">Response</span></span>
<span data-ttu-id="1dc27-236">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1dc27-236">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dc27-237">示例</span><span class="sxs-lookup"><span data-stu-id="1dc27-237">Example</span></span>
### <a name="request"></a><span data-ttu-id="1dc27-238">请求</span><span class="sxs-lookup"><span data-stu-id="1dc27-238">Request</span></span>
<span data-ttu-id="1dc27-239">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1dc27-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1306

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```

### <a name="response"></a><span data-ttu-id="1dc27-240">响应</span><span class="sxs-lookup"><span data-stu-id="1dc27-240">Response</span></span>
<span data-ttu-id="1dc27-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1dc27-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1414

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```





