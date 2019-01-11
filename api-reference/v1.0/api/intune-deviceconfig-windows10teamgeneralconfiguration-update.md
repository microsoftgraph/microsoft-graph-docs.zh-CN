---
title: 更新 windows10TeamGeneralConfiguration
description: 更新 windows10TeamGeneralConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 44ea0c4f76bd95d84ecd5126bec32e988b40a6f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858364"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="bb6a3-103">更新 windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb6a3-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="bb6a3-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb6a3-105">更新 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-105">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bb6a3-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="bb6a3-106">Prerequisites</span></span>
<span data-ttu-id="bb6a3-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bb6a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb6a3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb6a3-109">Permission type</span></span>|<span data-ttu-id="bb6a3-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bb6a3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb6a3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb6a3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb6a3-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb6a3-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb6a3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb6a3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb6a3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-114">Not supported.</span></span>|
|<span data-ttu-id="bb6a3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb6a3-115">Application</span></span>|<span data-ttu-id="bb6a3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb6a3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb6a3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bb6a3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb6a3-118">Request headers</span></span>
|<span data-ttu-id="bb6a3-119">标头</span><span class="sxs-lookup"><span data-stu-id="bb6a3-119">Header</span></span>|<span data-ttu-id="bb6a3-120">值</span><span class="sxs-lookup"><span data-stu-id="bb6a3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb6a3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb6a3-121">Authorization</span></span>|<span data-ttu-id="bb6a3-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb6a3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bb6a3-123">Accept</span></span>|<span data-ttu-id="bb6a3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bb6a3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb6a3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb6a3-125">Request body</span></span>
<span data-ttu-id="bb6a3-126">在请求正文中，提供 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-126">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="bb6a3-127">下表显示了创建 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-127">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="bb6a3-128">属性</span><span class="sxs-lookup"><span data-stu-id="bb6a3-128">Property</span></span>|<span data-ttu-id="bb6a3-129">类型</span><span class="sxs-lookup"><span data-stu-id="bb6a3-129">Type</span></span>|<span data-ttu-id="bb6a3-130">说明</span><span class="sxs-lookup"><span data-stu-id="bb6a3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb6a3-131">id</span><span class="sxs-lookup"><span data-stu-id="bb6a3-131">id</span></span>|<span data-ttu-id="bb6a3-132">String</span><span class="sxs-lookup"><span data-stu-id="bb6a3-132">String</span></span>|<span data-ttu-id="bb6a3-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-133">Key of the entity.</span></span> <span data-ttu-id="bb6a3-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb6a3-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb6a3-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb6a3-135">lastModifiedDateTime</span></span>|<span data-ttu-id="bb6a3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb6a3-136">DateTimeOffset</span></span>|<span data-ttu-id="bb6a3-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-137">DateTime the object was last modified.</span></span> <span data-ttu-id="bb6a3-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb6a3-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb6a3-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb6a3-139">createdDateTime</span></span>|<span data-ttu-id="bb6a3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb6a3-140">DateTimeOffset</span></span>|<span data-ttu-id="bb6a3-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-141">DateTime the object was created.</span></span> <span data-ttu-id="bb6a3-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb6a3-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb6a3-143">description</span><span class="sxs-lookup"><span data-stu-id="bb6a3-143">description</span></span>|<span data-ttu-id="bb6a3-144">String</span><span class="sxs-lookup"><span data-stu-id="bb6a3-144">String</span></span>|<span data-ttu-id="bb6a3-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bb6a3-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb6a3-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb6a3-147">displayName</span><span class="sxs-lookup"><span data-stu-id="bb6a3-147">displayName</span></span>|<span data-ttu-id="bb6a3-148">String</span><span class="sxs-lookup"><span data-stu-id="bb6a3-148">String</span></span>|<span data-ttu-id="bb6a3-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bb6a3-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb6a3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb6a3-151">version</span><span class="sxs-lookup"><span data-stu-id="bb6a3-151">version</span></span>|<span data-ttu-id="bb6a3-152">Int32</span><span class="sxs-lookup"><span data-stu-id="bb6a3-152">Int32</span></span>|<span data-ttu-id="bb6a3-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-153">Version of the device configuration.</span></span> <span data-ttu-id="bb6a3-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb6a3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb6a3-155">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="bb6a3-155">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="bb6a3-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb6a3-156">Boolean</span></span>|<span data-ttu-id="bb6a3-157">指示是否阻止 Azure 操作见解。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-157">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="bb6a3-158">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="bb6a3-158">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="bb6a3-159">String</span><span class="sxs-lookup"><span data-stu-id="bb6a3-159">String</span></span>|<span data-ttu-id="bb6a3-160">Azure 操作见解工作区 ID。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-160">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="bb6a3-161">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="bb6a3-161">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="bb6a3-162">String</span><span class="sxs-lookup"><span data-stu-id="bb6a3-162">String</span></span>|<span data-ttu-id="bb6a3-163">Azure 操作见解工作区键。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-163">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="bb6a3-164">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="bb6a3-164">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="bb6a3-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb6a3-165">Boolean</span></span>|<span data-ttu-id="bb6a3-166">指定是否在启动投影时自动启动 Connect 应用。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-166">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="bb6a3-167">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="bb6a3-167">maintenanceWindowBlocked</span></span>|<span data-ttu-id="bb6a3-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb6a3-168">Boolean</span></span>|<span data-ttu-id="bb6a3-169">指示是否阻止设置设备更新的维护时段。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-169">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="bb6a3-170">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="bb6a3-170">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="bb6a3-171">Int32</span><span class="sxs-lookup"><span data-stu-id="bb6a3-171">Int32</span></span>|<span data-ttu-id="bb6a3-172">设备更新的维护时段持续时间。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-172">Maintenance window duration for device updates.</span></span> <span data-ttu-id="bb6a3-173">有效值为 0 至 5</span><span class="sxs-lookup"><span data-stu-id="bb6a3-173">Valid values 0 to 5</span></span>|
|<span data-ttu-id="bb6a3-174">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="bb6a3-174">maintenanceWindowStartTime</span></span>|<span data-ttu-id="bb6a3-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="bb6a3-175">TimeOfDay</span></span>|<span data-ttu-id="bb6a3-176">设备更新的维护时段开始时间。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-176">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="bb6a3-177">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="bb6a3-177">miracastChannel</span></span>|[<span data-ttu-id="bb6a3-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="bb6a3-178">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="bb6a3-179">频道。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-179">The channel.</span></span> <span data-ttu-id="bb6a3-180">可取值为：`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive`。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-180">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="bb6a3-181">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="bb6a3-181">miracastBlocked</span></span>|<span data-ttu-id="bb6a3-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb6a3-182">Boolean</span></span>|<span data-ttu-id="bb6a3-183">指示是否阻止无线投影。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-183">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="bb6a3-184">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="bb6a3-184">miracastRequirePin</span></span>|<span data-ttu-id="bb6a3-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb6a3-185">Boolean</span></span>|<span data-ttu-id="bb6a3-186">指示是否需要 PIN 才能进行无线投影。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-186">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="bb6a3-187">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="bb6a3-187">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="bb6a3-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb6a3-188">Boolean</span></span>|<span data-ttu-id="bb6a3-189">指定是否禁用“开始”菜单中的“我的会议和文件”功能，该功能显示来自 Office 365 的已登录用户的会议和文件。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-189">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="bb6a3-190">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="bb6a3-190">settingsBlockSessionResume</span></span>|<span data-ttu-id="bb6a3-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb6a3-191">Boolean</span></span>|<span data-ttu-id="bb6a3-192">指定是否允许在会话超时时恢复会话。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-192">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="bb6a3-193">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="bb6a3-193">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="bb6a3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb6a3-194">Boolean</span></span>|<span data-ttu-id="bb6a3-195">指定是否禁用计划会议的被邀请者自动填充登录对话框。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-195">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="bb6a3-196">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="bb6a3-196">settingsDefaultVolume</span></span>|<span data-ttu-id="bb6a3-197">Int32</span><span class="sxs-lookup"><span data-stu-id="bb6a3-197">Int32</span></span>|<span data-ttu-id="bb6a3-198">指定新会话的默认音量值。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-198">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="bb6a3-199">允许的值为 0-100。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-199">Permitted values are 0-100.</span></span> <span data-ttu-id="bb6a3-200">默认值为 45。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-200">The default is 45.</span></span> <span data-ttu-id="bb6a3-201">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="bb6a3-201">Valid values 0 to 100</span></span>|
|<span data-ttu-id="bb6a3-202">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="bb6a3-202">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="bb6a3-203">Int32</span><span class="sxs-lookup"><span data-stu-id="bb6a3-203">Int32</span></span>|<span data-ttu-id="bb6a3-204">指定 Hub 屏幕关闭前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-204">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="bb6a3-205">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="bb6a3-205">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="bb6a3-206">Int32</span><span class="sxs-lookup"><span data-stu-id="bb6a3-206">Int32</span></span>|<span data-ttu-id="bb6a3-207">指定会话超时前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-207">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="bb6a3-208">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="bb6a3-208">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="bb6a3-209">Int32</span><span class="sxs-lookup"><span data-stu-id="bb6a3-209">Int32</span></span>|<span data-ttu-id="bb6a3-210">指定 Hub 进入睡眠模式前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-210">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="bb6a3-211">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="bb6a3-211">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="bb6a3-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb6a3-212">Boolean</span></span>|<span data-ttu-id="bb6a3-213">指示当某人进入会议室时是否阻止欢迎屏幕自动唤醒。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-213">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="bb6a3-214">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="bb6a3-214">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="bb6a3-215">String</span><span class="sxs-lookup"><span data-stu-id="bb6a3-215">String</span></span>|<span data-ttu-id="bb6a3-216">欢迎屏幕背景图像 URL。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-216">The welcome screen background image URL.</span></span> <span data-ttu-id="bb6a3-217">URL 必须使用 HTTPS 协议并返回 PNG 图像。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-217">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="bb6a3-218">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="bb6a3-218">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="bb6a3-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="bb6a3-219">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="bb6a3-220">显示的欢迎屏幕会议信息。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-220">The welcome screen meeting information shown.</span></span> <span data-ttu-id="bb6a3-221">可取值为：`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject`。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-221">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="bb6a3-222">响应</span><span class="sxs-lookup"><span data-stu-id="bb6a3-222">Response</span></span>
<span data-ttu-id="bb6a3-223">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-223">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb6a3-224">示例</span><span class="sxs-lookup"><span data-stu-id="bb6a3-224">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb6a3-225">请求</span><span class="sxs-lookup"><span data-stu-id="bb6a3-225">Request</span></span>
<span data-ttu-id="bb6a3-226">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1150

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="bb6a3-227">响应</span><span class="sxs-lookup"><span data-stu-id="bb6a3-227">Response</span></span>
<span data-ttu-id="bb6a3-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1322

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



