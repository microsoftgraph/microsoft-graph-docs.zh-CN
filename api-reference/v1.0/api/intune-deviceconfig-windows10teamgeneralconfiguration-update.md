---
title: 更新 windows10TeamGeneralConfiguration
description: 更新 windows10TeamGeneralConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 15c91a32a6aca192938b1af53195dbc91044f68b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063350"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="b91be-103">更新 windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="b91be-103">Update windows10TeamGeneralConfiguration</span></span>

<span data-ttu-id="b91be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b91be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b91be-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b91be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b91be-106">更新 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b91be-106">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b91be-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b91be-107">Prerequisites</span></span>
<span data-ttu-id="b91be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b91be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b91be-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b91be-110">Permission type</span></span>|<span data-ttu-id="b91be-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b91be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b91be-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b91be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b91be-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b91be-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b91be-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b91be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b91be-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b91be-115">Not supported.</span></span>|
|<span data-ttu-id="b91be-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b91be-116">Application</span></span>|<span data-ttu-id="b91be-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b91be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b91be-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b91be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b91be-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b91be-119">Request headers</span></span>
|<span data-ttu-id="b91be-120">标头</span><span class="sxs-lookup"><span data-stu-id="b91be-120">Header</span></span>|<span data-ttu-id="b91be-121">值</span><span class="sxs-lookup"><span data-stu-id="b91be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b91be-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b91be-122">Authorization</span></span>|<span data-ttu-id="b91be-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b91be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b91be-124">接受</span><span class="sxs-lookup"><span data-stu-id="b91be-124">Accept</span></span>|<span data-ttu-id="b91be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b91be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b91be-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b91be-126">Request body</span></span>
<span data-ttu-id="b91be-127">在请求正文中，提供 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b91be-127">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="b91be-128">下表显示了创建 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b91be-128">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="b91be-129">属性</span><span class="sxs-lookup"><span data-stu-id="b91be-129">Property</span></span>|<span data-ttu-id="b91be-130">类型</span><span class="sxs-lookup"><span data-stu-id="b91be-130">Type</span></span>|<span data-ttu-id="b91be-131">说明</span><span class="sxs-lookup"><span data-stu-id="b91be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b91be-132">id</span><span class="sxs-lookup"><span data-stu-id="b91be-132">id</span></span>|<span data-ttu-id="b91be-133">String</span><span class="sxs-lookup"><span data-stu-id="b91be-133">String</span></span>|<span data-ttu-id="b91be-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b91be-134">Key of the entity.</span></span> <span data-ttu-id="b91be-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b91be-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b91be-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b91be-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b91be-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b91be-137">DateTimeOffset</span></span>|<span data-ttu-id="b91be-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b91be-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b91be-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b91be-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b91be-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b91be-140">createdDateTime</span></span>|<span data-ttu-id="b91be-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b91be-141">DateTimeOffset</span></span>|<span data-ttu-id="b91be-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b91be-142">DateTime the object was created.</span></span> <span data-ttu-id="b91be-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b91be-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b91be-144">description</span><span class="sxs-lookup"><span data-stu-id="b91be-144">description</span></span>|<span data-ttu-id="b91be-145">String</span><span class="sxs-lookup"><span data-stu-id="b91be-145">String</span></span>|<span data-ttu-id="b91be-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b91be-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b91be-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b91be-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b91be-148">displayName</span><span class="sxs-lookup"><span data-stu-id="b91be-148">displayName</span></span>|<span data-ttu-id="b91be-149">String</span><span class="sxs-lookup"><span data-stu-id="b91be-149">String</span></span>|<span data-ttu-id="b91be-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b91be-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b91be-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b91be-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b91be-152">version</span><span class="sxs-lookup"><span data-stu-id="b91be-152">version</span></span>|<span data-ttu-id="b91be-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b91be-153">Int32</span></span>|<span data-ttu-id="b91be-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b91be-154">Version of the device configuration.</span></span> <span data-ttu-id="b91be-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b91be-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b91be-156">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="b91be-156">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="b91be-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="b91be-157">Boolean</span></span>|<span data-ttu-id="b91be-158">指示是否阻止 Azure 操作见解。</span><span class="sxs-lookup"><span data-stu-id="b91be-158">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="b91be-159">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="b91be-159">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="b91be-160">String</span><span class="sxs-lookup"><span data-stu-id="b91be-160">String</span></span>|<span data-ttu-id="b91be-161">Azure 操作见解工作区 ID。</span><span class="sxs-lookup"><span data-stu-id="b91be-161">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="b91be-162">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="b91be-162">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="b91be-163">String</span><span class="sxs-lookup"><span data-stu-id="b91be-163">String</span></span>|<span data-ttu-id="b91be-164">Azure 操作见解工作区键。</span><span class="sxs-lookup"><span data-stu-id="b91be-164">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="b91be-165">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="b91be-165">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="b91be-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="b91be-166">Boolean</span></span>|<span data-ttu-id="b91be-167">指定是否在启动投影时自动启动 Connect 应用。</span><span class="sxs-lookup"><span data-stu-id="b91be-167">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="b91be-168">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="b91be-168">maintenanceWindowBlocked</span></span>|<span data-ttu-id="b91be-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="b91be-169">Boolean</span></span>|<span data-ttu-id="b91be-170">指示是否阻止设置设备更新的维护时段。</span><span class="sxs-lookup"><span data-stu-id="b91be-170">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="b91be-171">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="b91be-171">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="b91be-172">Int32</span><span class="sxs-lookup"><span data-stu-id="b91be-172">Int32</span></span>|<span data-ttu-id="b91be-173">设备更新的维护时段持续时间。</span><span class="sxs-lookup"><span data-stu-id="b91be-173">Maintenance window duration for device updates.</span></span> <span data-ttu-id="b91be-174">有效值为 0 至 5</span><span class="sxs-lookup"><span data-stu-id="b91be-174">Valid values 0 to 5</span></span>|
|<span data-ttu-id="b91be-175">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="b91be-175">maintenanceWindowStartTime</span></span>|<span data-ttu-id="b91be-176">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b91be-176">TimeOfDay</span></span>|<span data-ttu-id="b91be-177">设备更新的维护时段开始时间。</span><span class="sxs-lookup"><span data-stu-id="b91be-177">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="b91be-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="b91be-178">miracastChannel</span></span>|[<span data-ttu-id="b91be-179">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="b91be-179">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="b91be-180">频道。</span><span class="sxs-lookup"><span data-stu-id="b91be-180">The channel.</span></span> <span data-ttu-id="b91be-181">可取值为：`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive`。</span><span class="sxs-lookup"><span data-stu-id="b91be-181">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="b91be-182">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="b91be-182">miracastBlocked</span></span>|<span data-ttu-id="b91be-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="b91be-183">Boolean</span></span>|<span data-ttu-id="b91be-184">指示是否阻止无线投影。</span><span class="sxs-lookup"><span data-stu-id="b91be-184">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="b91be-185">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="b91be-185">miracastRequirePin</span></span>|<span data-ttu-id="b91be-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="b91be-186">Boolean</span></span>|<span data-ttu-id="b91be-187">指示是否需要 PIN 才能进行无线投影。</span><span class="sxs-lookup"><span data-stu-id="b91be-187">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="b91be-188">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="b91be-188">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="b91be-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="b91be-189">Boolean</span></span>|<span data-ttu-id="b91be-190">指定是否禁用“开始”菜单中的“我的会议和文件”功能，该功能显示来自 Office 365 的已登录用户的会议和文件。</span><span class="sxs-lookup"><span data-stu-id="b91be-190">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="b91be-191">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="b91be-191">settingsBlockSessionResume</span></span>|<span data-ttu-id="b91be-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="b91be-192">Boolean</span></span>|<span data-ttu-id="b91be-193">指定是否允许在会话超时时恢复会话。</span><span class="sxs-lookup"><span data-stu-id="b91be-193">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="b91be-194">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="b91be-194">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="b91be-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b91be-195">Boolean</span></span>|<span data-ttu-id="b91be-196">指定是否禁用计划会议的被邀请者自动填充登录对话框。</span><span class="sxs-lookup"><span data-stu-id="b91be-196">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="b91be-197">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="b91be-197">settingsDefaultVolume</span></span>|<span data-ttu-id="b91be-198">Int32</span><span class="sxs-lookup"><span data-stu-id="b91be-198">Int32</span></span>|<span data-ttu-id="b91be-199">指定新会话的默认音量值。</span><span class="sxs-lookup"><span data-stu-id="b91be-199">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="b91be-200">允许的值为 0-100。</span><span class="sxs-lookup"><span data-stu-id="b91be-200">Permitted values are 0-100.</span></span> <span data-ttu-id="b91be-201">默认值为 45。</span><span class="sxs-lookup"><span data-stu-id="b91be-201">The default is 45.</span></span> <span data-ttu-id="b91be-202">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="b91be-202">Valid values 0 to 100</span></span>|
|<span data-ttu-id="b91be-203">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="b91be-203">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="b91be-204">Int32</span><span class="sxs-lookup"><span data-stu-id="b91be-204">Int32</span></span>|<span data-ttu-id="b91be-205">指定 Hub 屏幕关闭前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b91be-205">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="b91be-206">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="b91be-206">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="b91be-207">Int32</span><span class="sxs-lookup"><span data-stu-id="b91be-207">Int32</span></span>|<span data-ttu-id="b91be-208">指定会话超时前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b91be-208">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="b91be-209">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="b91be-209">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="b91be-210">Int32</span><span class="sxs-lookup"><span data-stu-id="b91be-210">Int32</span></span>|<span data-ttu-id="b91be-211">指定 Hub 进入睡眠模式前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b91be-211">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="b91be-212">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="b91be-212">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="b91be-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="b91be-213">Boolean</span></span>|<span data-ttu-id="b91be-214">指示当某人进入会议室时是否阻止欢迎屏幕自动唤醒。</span><span class="sxs-lookup"><span data-stu-id="b91be-214">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="b91be-215">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="b91be-215">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="b91be-216">String</span><span class="sxs-lookup"><span data-stu-id="b91be-216">String</span></span>|<span data-ttu-id="b91be-217">欢迎屏幕背景图像 URL。</span><span class="sxs-lookup"><span data-stu-id="b91be-217">The welcome screen background image URL.</span></span> <span data-ttu-id="b91be-218">URL 必须使用 HTTPS 协议并返回 PNG 图像。</span><span class="sxs-lookup"><span data-stu-id="b91be-218">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="b91be-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="b91be-219">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="b91be-220">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="b91be-220">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="b91be-221">显示的欢迎屏幕会议信息。</span><span class="sxs-lookup"><span data-stu-id="b91be-221">The welcome screen meeting information shown.</span></span> <span data-ttu-id="b91be-222">可取值为：`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject`。</span><span class="sxs-lookup"><span data-stu-id="b91be-222">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="b91be-223">响应</span><span class="sxs-lookup"><span data-stu-id="b91be-223">Response</span></span>
<span data-ttu-id="b91be-224">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b91be-224">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b91be-225">示例</span><span class="sxs-lookup"><span data-stu-id="b91be-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="b91be-226">请求</span><span class="sxs-lookup"><span data-stu-id="b91be-226">Request</span></span>
<span data-ttu-id="b91be-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b91be-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b91be-228">响应</span><span class="sxs-lookup"><span data-stu-id="b91be-228">Response</span></span>
<span data-ttu-id="b91be-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b91be-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









