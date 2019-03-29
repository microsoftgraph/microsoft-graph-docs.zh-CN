---
title: 创建 windows10TeamGeneralConfiguration
description: 创建新的 windows10TeamGeneralConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cabccd8f44f26b4ab8c848866e25f30302dc0198
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958758"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="a4d23-103">创建 windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4d23-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="a4d23-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4d23-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4d23-105">创建新的 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4d23-105">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4d23-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4d23-106">Prerequisites</span></span>
<span data-ttu-id="a4d23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4d23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4d23-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4d23-109">Permission type</span></span>|<span data-ttu-id="a4d23-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a4d23-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4d23-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4d23-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4d23-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4d23-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4d23-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4d23-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4d23-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4d23-114">Not supported.</span></span>|
|<span data-ttu-id="a4d23-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4d23-115">Application</span></span>|<span data-ttu-id="a4d23-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4d23-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4d23-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4d23-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a4d23-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4d23-118">Request headers</span></span>
|<span data-ttu-id="a4d23-119">标头</span><span class="sxs-lookup"><span data-stu-id="a4d23-119">Header</span></span>|<span data-ttu-id="a4d23-120">值</span><span class="sxs-lookup"><span data-stu-id="a4d23-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4d23-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4d23-121">Authorization</span></span>|<span data-ttu-id="a4d23-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4d23-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4d23-123">接受</span><span class="sxs-lookup"><span data-stu-id="a4d23-123">Accept</span></span>|<span data-ttu-id="a4d23-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a4d23-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4d23-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4d23-125">Request body</span></span>
<span data-ttu-id="a4d23-126">在请求正文中，提供 windows10TeamGeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4d23-126">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="a4d23-127">下表显示了创建 windows10TeamGeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a4d23-127">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="a4d23-128">属性</span><span class="sxs-lookup"><span data-stu-id="a4d23-128">Property</span></span>|<span data-ttu-id="a4d23-129">类型</span><span class="sxs-lookup"><span data-stu-id="a4d23-129">Type</span></span>|<span data-ttu-id="a4d23-130">说明</span><span class="sxs-lookup"><span data-stu-id="a4d23-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4d23-131">id</span><span class="sxs-lookup"><span data-stu-id="a4d23-131">id</span></span>|<span data-ttu-id="a4d23-132">String</span><span class="sxs-lookup"><span data-stu-id="a4d23-132">String</span></span>|<span data-ttu-id="a4d23-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a4d23-133">Key of the entity.</span></span> <span data-ttu-id="a4d23-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a4d23-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4d23-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4d23-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a4d23-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4d23-136">DateTimeOffset</span></span>|<span data-ttu-id="a4d23-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a4d23-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a4d23-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a4d23-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4d23-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4d23-139">createdDateTime</span></span>|<span data-ttu-id="a4d23-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4d23-140">DateTimeOffset</span></span>|<span data-ttu-id="a4d23-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a4d23-141">DateTime the object was created.</span></span> <span data-ttu-id="a4d23-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a4d23-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4d23-143">description</span><span class="sxs-lookup"><span data-stu-id="a4d23-143">description</span></span>|<span data-ttu-id="a4d23-144">String</span><span class="sxs-lookup"><span data-stu-id="a4d23-144">String</span></span>|<span data-ttu-id="a4d23-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a4d23-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a4d23-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a4d23-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4d23-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a4d23-147">displayName</span></span>|<span data-ttu-id="a4d23-148">String</span><span class="sxs-lookup"><span data-stu-id="a4d23-148">String</span></span>|<span data-ttu-id="a4d23-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a4d23-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a4d23-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a4d23-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4d23-151">version</span><span class="sxs-lookup"><span data-stu-id="a4d23-151">version</span></span>|<span data-ttu-id="a4d23-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a4d23-152">Int32</span></span>|<span data-ttu-id="a4d23-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a4d23-153">Version of the device configuration.</span></span> <span data-ttu-id="a4d23-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a4d23-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4d23-155">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="a4d23-155">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="a4d23-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4d23-156">Boolean</span></span>|<span data-ttu-id="a4d23-157">指示是否阻止 Azure 操作见解。</span><span class="sxs-lookup"><span data-stu-id="a4d23-157">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="a4d23-158">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="a4d23-158">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="a4d23-159">String</span><span class="sxs-lookup"><span data-stu-id="a4d23-159">String</span></span>|<span data-ttu-id="a4d23-160">Azure 操作见解工作区 ID。</span><span class="sxs-lookup"><span data-stu-id="a4d23-160">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="a4d23-161">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="a4d23-161">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="a4d23-162">String</span><span class="sxs-lookup"><span data-stu-id="a4d23-162">String</span></span>|<span data-ttu-id="a4d23-163">Azure 操作见解工作区键。</span><span class="sxs-lookup"><span data-stu-id="a4d23-163">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="a4d23-164">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="a4d23-164">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="a4d23-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4d23-165">Boolean</span></span>|<span data-ttu-id="a4d23-166">指定是否在启动投影时自动启动 Connect 应用。</span><span class="sxs-lookup"><span data-stu-id="a4d23-166">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="a4d23-167">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="a4d23-167">maintenanceWindowBlocked</span></span>|<span data-ttu-id="a4d23-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4d23-168">Boolean</span></span>|<span data-ttu-id="a4d23-169">指示是否阻止设置设备更新的维护时段。</span><span class="sxs-lookup"><span data-stu-id="a4d23-169">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="a4d23-170">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="a4d23-170">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="a4d23-171">Int32</span><span class="sxs-lookup"><span data-stu-id="a4d23-171">Int32</span></span>|<span data-ttu-id="a4d23-172">设备更新的维护时段持续时间。</span><span class="sxs-lookup"><span data-stu-id="a4d23-172">Maintenance window duration for device updates.</span></span> <span data-ttu-id="a4d23-173">有效值为 0 至 5</span><span class="sxs-lookup"><span data-stu-id="a4d23-173">Valid values 0 to 5</span></span>|
|<span data-ttu-id="a4d23-174">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="a4d23-174">maintenanceWindowStartTime</span></span>|<span data-ttu-id="a4d23-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a4d23-175">TimeOfDay</span></span>|<span data-ttu-id="a4d23-176">设备更新的维护时段开始时间。</span><span class="sxs-lookup"><span data-stu-id="a4d23-176">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="a4d23-177">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="a4d23-177">miracastChannel</span></span>|[<span data-ttu-id="a4d23-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="a4d23-178">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="a4d23-179">频道。</span><span class="sxs-lookup"><span data-stu-id="a4d23-179">The channel.</span></span> <span data-ttu-id="a4d23-180">可取值为：`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive`。</span><span class="sxs-lookup"><span data-stu-id="a4d23-180">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="a4d23-181">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="a4d23-181">miracastBlocked</span></span>|<span data-ttu-id="a4d23-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4d23-182">Boolean</span></span>|<span data-ttu-id="a4d23-183">指示是否阻止无线投影。</span><span class="sxs-lookup"><span data-stu-id="a4d23-183">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="a4d23-184">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="a4d23-184">miracastRequirePin</span></span>|<span data-ttu-id="a4d23-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4d23-185">Boolean</span></span>|<span data-ttu-id="a4d23-186">指示是否需要 PIN 才能进行无线投影。</span><span class="sxs-lookup"><span data-stu-id="a4d23-186">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="a4d23-187">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="a4d23-187">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="a4d23-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4d23-188">Boolean</span></span>|<span data-ttu-id="a4d23-189">指定是否禁用“开始”菜单中的“我的会议和文件”功能，该功能显示来自 Office 365 的已登录用户的会议和文件。</span><span class="sxs-lookup"><span data-stu-id="a4d23-189">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="a4d23-190">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="a4d23-190">settingsBlockSessionResume</span></span>|<span data-ttu-id="a4d23-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4d23-191">Boolean</span></span>|<span data-ttu-id="a4d23-192">指定是否允许在会话超时时恢复会话。</span><span class="sxs-lookup"><span data-stu-id="a4d23-192">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="a4d23-193">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="a4d23-193">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="a4d23-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4d23-194">Boolean</span></span>|<span data-ttu-id="a4d23-195">指定是否禁用计划会议的被邀请者自动填充登录对话框。</span><span class="sxs-lookup"><span data-stu-id="a4d23-195">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="a4d23-196">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="a4d23-196">settingsDefaultVolume</span></span>|<span data-ttu-id="a4d23-197">Int32</span><span class="sxs-lookup"><span data-stu-id="a4d23-197">Int32</span></span>|<span data-ttu-id="a4d23-198">指定新会话的默认音量值。</span><span class="sxs-lookup"><span data-stu-id="a4d23-198">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="a4d23-199">允许的值为 0-100。</span><span class="sxs-lookup"><span data-stu-id="a4d23-199">Permitted values are 0-100.</span></span> <span data-ttu-id="a4d23-200">默认值为 45。</span><span class="sxs-lookup"><span data-stu-id="a4d23-200">The default is 45.</span></span> <span data-ttu-id="a4d23-201">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="a4d23-201">Valid values 0 to 100</span></span>|
|<span data-ttu-id="a4d23-202">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="a4d23-202">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="a4d23-203">Int32</span><span class="sxs-lookup"><span data-stu-id="a4d23-203">Int32</span></span>|<span data-ttu-id="a4d23-204">指定 Hub 屏幕关闭前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="a4d23-204">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="a4d23-205">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="a4d23-205">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="a4d23-206">Int32</span><span class="sxs-lookup"><span data-stu-id="a4d23-206">Int32</span></span>|<span data-ttu-id="a4d23-207">指定会话超时前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="a4d23-207">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="a4d23-208">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="a4d23-208">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="a4d23-209">Int32</span><span class="sxs-lookup"><span data-stu-id="a4d23-209">Int32</span></span>|<span data-ttu-id="a4d23-210">指定 Hub 进入睡眠模式前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="a4d23-210">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="a4d23-211">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="a4d23-211">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="a4d23-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4d23-212">Boolean</span></span>|<span data-ttu-id="a4d23-213">指示当某人进入会议室时是否阻止欢迎屏幕自动唤醒。</span><span class="sxs-lookup"><span data-stu-id="a4d23-213">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="a4d23-214">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="a4d23-214">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="a4d23-215">String</span><span class="sxs-lookup"><span data-stu-id="a4d23-215">String</span></span>|<span data-ttu-id="a4d23-216">欢迎屏幕背景图像 URL。</span><span class="sxs-lookup"><span data-stu-id="a4d23-216">The welcome screen background image URL.</span></span> <span data-ttu-id="a4d23-217">URL 必须使用 HTTPS 协议并返回 PNG 图像。</span><span class="sxs-lookup"><span data-stu-id="a4d23-217">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="a4d23-218">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="a4d23-218">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="a4d23-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="a4d23-219">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="a4d23-220">显示的欢迎屏幕会议信息。</span><span class="sxs-lookup"><span data-stu-id="a4d23-220">The welcome screen meeting information shown.</span></span> <span data-ttu-id="a4d23-221">可取值为：`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject`。</span><span class="sxs-lookup"><span data-stu-id="a4d23-221">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="a4d23-222">响应</span><span class="sxs-lookup"><span data-stu-id="a4d23-222">Response</span></span>
<span data-ttu-id="a4d23-223">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4d23-223">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4d23-224">示例</span><span class="sxs-lookup"><span data-stu-id="a4d23-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4d23-225">请求</span><span class="sxs-lookup"><span data-stu-id="a4d23-225">Request</span></span>
<span data-ttu-id="a4d23-226">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4d23-226">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a4d23-227">响应</span><span class="sxs-lookup"><span data-stu-id="a4d23-227">Response</span></span>
<span data-ttu-id="a4d23-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4d23-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



