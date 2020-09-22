---
title: 创建 windows10TeamGeneralConfiguration
description: 创建新的 windows10TeamGeneralConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca152abe3374cf3cdb355012d623ff35fd34761b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48045675"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="c0742-103">创建 windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0742-103">Create windows10TeamGeneralConfiguration</span></span>

<span data-ttu-id="c0742-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0742-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0742-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0742-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0742-106">创建新的 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0742-106">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0742-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c0742-107">Prerequisites</span></span>
<span data-ttu-id="c0742-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0742-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0742-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0742-110">Permission type</span></span>|<span data-ttu-id="c0742-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c0742-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0742-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0742-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0742-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0742-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0742-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0742-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0742-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0742-115">Not supported.</span></span>|
|<span data-ttu-id="c0742-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0742-116">Application</span></span>|<span data-ttu-id="c0742-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0742-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0742-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0742-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c0742-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0742-119">Request headers</span></span>
|<span data-ttu-id="c0742-120">标头</span><span class="sxs-lookup"><span data-stu-id="c0742-120">Header</span></span>|<span data-ttu-id="c0742-121">值</span><span class="sxs-lookup"><span data-stu-id="c0742-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0742-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0742-122">Authorization</span></span>|<span data-ttu-id="c0742-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c0742-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0742-124">接受</span><span class="sxs-lookup"><span data-stu-id="c0742-124">Accept</span></span>|<span data-ttu-id="c0742-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0742-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0742-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0742-126">Request body</span></span>
<span data-ttu-id="c0742-127">在请求正文中，提供 windows10TeamGeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0742-127">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="c0742-128">下表显示了创建 windows10TeamGeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c0742-128">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="c0742-129">属性</span><span class="sxs-lookup"><span data-stu-id="c0742-129">Property</span></span>|<span data-ttu-id="c0742-130">类型</span><span class="sxs-lookup"><span data-stu-id="c0742-130">Type</span></span>|<span data-ttu-id="c0742-131">说明</span><span class="sxs-lookup"><span data-stu-id="c0742-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0742-132">id</span><span class="sxs-lookup"><span data-stu-id="c0742-132">id</span></span>|<span data-ttu-id="c0742-133">String</span><span class="sxs-lookup"><span data-stu-id="c0742-133">String</span></span>|<span data-ttu-id="c0742-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c0742-134">Key of the entity.</span></span> <span data-ttu-id="c0742-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0742-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0742-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0742-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c0742-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0742-137">DateTimeOffset</span></span>|<span data-ttu-id="c0742-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c0742-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c0742-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0742-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0742-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0742-140">createdDateTime</span></span>|<span data-ttu-id="c0742-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0742-141">DateTimeOffset</span></span>|<span data-ttu-id="c0742-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c0742-142">DateTime the object was created.</span></span> <span data-ttu-id="c0742-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0742-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0742-144">description</span><span class="sxs-lookup"><span data-stu-id="c0742-144">description</span></span>|<span data-ttu-id="c0742-145">String</span><span class="sxs-lookup"><span data-stu-id="c0742-145">String</span></span>|<span data-ttu-id="c0742-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c0742-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c0742-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0742-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0742-148">displayName</span><span class="sxs-lookup"><span data-stu-id="c0742-148">displayName</span></span>|<span data-ttu-id="c0742-149">String</span><span class="sxs-lookup"><span data-stu-id="c0742-149">String</span></span>|<span data-ttu-id="c0742-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c0742-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c0742-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0742-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0742-152">version</span><span class="sxs-lookup"><span data-stu-id="c0742-152">version</span></span>|<span data-ttu-id="c0742-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c0742-153">Int32</span></span>|<span data-ttu-id="c0742-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c0742-154">Version of the device configuration.</span></span> <span data-ttu-id="c0742-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0742-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0742-156">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="c0742-156">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="c0742-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0742-157">Boolean</span></span>|<span data-ttu-id="c0742-158">指示是否阻止 Azure 操作见解。</span><span class="sxs-lookup"><span data-stu-id="c0742-158">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="c0742-159">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="c0742-159">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="c0742-160">String</span><span class="sxs-lookup"><span data-stu-id="c0742-160">String</span></span>|<span data-ttu-id="c0742-161">Azure 操作见解工作区 ID。</span><span class="sxs-lookup"><span data-stu-id="c0742-161">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="c0742-162">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="c0742-162">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="c0742-163">String</span><span class="sxs-lookup"><span data-stu-id="c0742-163">String</span></span>|<span data-ttu-id="c0742-164">Azure 操作见解工作区键。</span><span class="sxs-lookup"><span data-stu-id="c0742-164">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="c0742-165">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="c0742-165">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="c0742-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0742-166">Boolean</span></span>|<span data-ttu-id="c0742-167">指定是否在启动投影时自动启动 Connect 应用。</span><span class="sxs-lookup"><span data-stu-id="c0742-167">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="c0742-168">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="c0742-168">maintenanceWindowBlocked</span></span>|<span data-ttu-id="c0742-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0742-169">Boolean</span></span>|<span data-ttu-id="c0742-170">指示是否阻止设置设备更新的维护时段。</span><span class="sxs-lookup"><span data-stu-id="c0742-170">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="c0742-171">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="c0742-171">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="c0742-172">Int32</span><span class="sxs-lookup"><span data-stu-id="c0742-172">Int32</span></span>|<span data-ttu-id="c0742-173">设备更新的维护时段持续时间。</span><span class="sxs-lookup"><span data-stu-id="c0742-173">Maintenance window duration for device updates.</span></span> <span data-ttu-id="c0742-174">有效值为 0 至 5</span><span class="sxs-lookup"><span data-stu-id="c0742-174">Valid values 0 to 5</span></span>|
|<span data-ttu-id="c0742-175">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="c0742-175">maintenanceWindowStartTime</span></span>|<span data-ttu-id="c0742-176">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c0742-176">TimeOfDay</span></span>|<span data-ttu-id="c0742-177">设备更新的维护时段开始时间。</span><span class="sxs-lookup"><span data-stu-id="c0742-177">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="c0742-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="c0742-178">miracastChannel</span></span>|[<span data-ttu-id="c0742-179">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="c0742-179">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="c0742-180">频道。</span><span class="sxs-lookup"><span data-stu-id="c0742-180">The channel.</span></span> <span data-ttu-id="c0742-181">可取值为：`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive`。</span><span class="sxs-lookup"><span data-stu-id="c0742-181">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="c0742-182">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="c0742-182">miracastBlocked</span></span>|<span data-ttu-id="c0742-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0742-183">Boolean</span></span>|<span data-ttu-id="c0742-184">指示是否阻止无线投影。</span><span class="sxs-lookup"><span data-stu-id="c0742-184">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="c0742-185">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="c0742-185">miracastRequirePin</span></span>|<span data-ttu-id="c0742-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0742-186">Boolean</span></span>|<span data-ttu-id="c0742-187">指示是否需要 PIN 才能进行无线投影。</span><span class="sxs-lookup"><span data-stu-id="c0742-187">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="c0742-188">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="c0742-188">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="c0742-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0742-189">Boolean</span></span>|<span data-ttu-id="c0742-190">指定是否禁用“开始”菜单中的“我的会议和文件”功能，该功能显示来自 Office 365 的已登录用户的会议和文件。</span><span class="sxs-lookup"><span data-stu-id="c0742-190">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="c0742-191">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="c0742-191">settingsBlockSessionResume</span></span>|<span data-ttu-id="c0742-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0742-192">Boolean</span></span>|<span data-ttu-id="c0742-193">指定是否允许在会话超时时恢复会话。</span><span class="sxs-lookup"><span data-stu-id="c0742-193">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="c0742-194">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="c0742-194">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="c0742-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0742-195">Boolean</span></span>|<span data-ttu-id="c0742-196">指定是否禁用计划会议的被邀请者自动填充登录对话框。</span><span class="sxs-lookup"><span data-stu-id="c0742-196">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="c0742-197">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="c0742-197">settingsDefaultVolume</span></span>|<span data-ttu-id="c0742-198">Int32</span><span class="sxs-lookup"><span data-stu-id="c0742-198">Int32</span></span>|<span data-ttu-id="c0742-199">指定新会话的默认音量值。</span><span class="sxs-lookup"><span data-stu-id="c0742-199">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="c0742-200">允许的值为 0-100。</span><span class="sxs-lookup"><span data-stu-id="c0742-200">Permitted values are 0-100.</span></span> <span data-ttu-id="c0742-201">默认值为 45。</span><span class="sxs-lookup"><span data-stu-id="c0742-201">The default is 45.</span></span> <span data-ttu-id="c0742-202">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="c0742-202">Valid values 0 to 100</span></span>|
|<span data-ttu-id="c0742-203">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="c0742-203">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="c0742-204">Int32</span><span class="sxs-lookup"><span data-stu-id="c0742-204">Int32</span></span>|<span data-ttu-id="c0742-205">指定 Hub 屏幕关闭前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c0742-205">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="c0742-206">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="c0742-206">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="c0742-207">Int32</span><span class="sxs-lookup"><span data-stu-id="c0742-207">Int32</span></span>|<span data-ttu-id="c0742-208">指定会话超时前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c0742-208">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="c0742-209">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="c0742-209">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="c0742-210">Int32</span><span class="sxs-lookup"><span data-stu-id="c0742-210">Int32</span></span>|<span data-ttu-id="c0742-211">指定 Hub 进入睡眠模式前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c0742-211">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="c0742-212">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="c0742-212">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="c0742-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0742-213">Boolean</span></span>|<span data-ttu-id="c0742-214">指示当某人进入会议室时是否阻止欢迎屏幕自动唤醒。</span><span class="sxs-lookup"><span data-stu-id="c0742-214">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="c0742-215">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="c0742-215">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="c0742-216">String</span><span class="sxs-lookup"><span data-stu-id="c0742-216">String</span></span>|<span data-ttu-id="c0742-217">欢迎屏幕背景图像 URL。</span><span class="sxs-lookup"><span data-stu-id="c0742-217">The welcome screen background image URL.</span></span> <span data-ttu-id="c0742-218">URL 必须使用 HTTPS 协议并返回 PNG 图像。</span><span class="sxs-lookup"><span data-stu-id="c0742-218">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="c0742-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="c0742-219">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="c0742-220">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="c0742-220">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="c0742-221">显示的欢迎屏幕会议信息。</span><span class="sxs-lookup"><span data-stu-id="c0742-221">The welcome screen meeting information shown.</span></span> <span data-ttu-id="c0742-222">可取值为：`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject`。</span><span class="sxs-lookup"><span data-stu-id="c0742-222">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="c0742-223">响应</span><span class="sxs-lookup"><span data-stu-id="c0742-223">Response</span></span>
<span data-ttu-id="c0742-224">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0742-224">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0742-225">示例</span><span class="sxs-lookup"><span data-stu-id="c0742-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0742-226">请求</span><span class="sxs-lookup"><span data-stu-id="c0742-226">Request</span></span>
<span data-ttu-id="c0742-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0742-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="c0742-228">响应</span><span class="sxs-lookup"><span data-stu-id="c0742-228">Response</span></span>
<span data-ttu-id="c0742-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c0742-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









