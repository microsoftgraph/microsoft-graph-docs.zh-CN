# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="7e035-101">更新 windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e035-101">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="7e035-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7e035-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e035-103">更新 [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7e035-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e035-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="7e035-104">Prerequisites</span></span>
<span data-ttu-id="7e035-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7e035-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7e035-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e035-107">Permission type</span></span>|<span data-ttu-id="7e035-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7e035-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e035-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e035-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7e035-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e035-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7e035-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e035-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e035-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e035-112">Not supported.</span></span>|
|<span data-ttu-id="7e035-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e035-113">Application</span></span>|<span data-ttu-id="7e035-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e035-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e035-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e035-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7e035-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e035-116">Request headers</span></span>
|<span data-ttu-id="7e035-117">标头</span><span class="sxs-lookup"><span data-stu-id="7e035-117">Header</span></span>|<span data-ttu-id="7e035-118">值</span><span class="sxs-lookup"><span data-stu-id="7e035-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e035-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e035-119">Authorization</span></span>|<span data-ttu-id="7e035-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7e035-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7e035-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7e035-121">Accept</span></span>|<span data-ttu-id="7e035-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7e035-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e035-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e035-123">Request body</span></span>
<span data-ttu-id="7e035-124">在请求正文中，提供 [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e035-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="7e035-125">下表显示了创建 [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7e035-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="7e035-126">属性</span><span class="sxs-lookup"><span data-stu-id="7e035-126">Property</span></span>|<span data-ttu-id="7e035-127">类型</span><span class="sxs-lookup"><span data-stu-id="7e035-127">Type</span></span>|<span data-ttu-id="7e035-128">说明</span><span class="sxs-lookup"><span data-stu-id="7e035-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e035-129">id</span><span class="sxs-lookup"><span data-stu-id="7e035-129">id</span></span>|<span data-ttu-id="7e035-130">String</span><span class="sxs-lookup"><span data-stu-id="7e035-130">String</span></span>|<span data-ttu-id="7e035-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7e035-131">Key of the setting.</span></span> <span data-ttu-id="7e035-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e035-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e035-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e035-133">lastModifiedDateTime</span></span>|<span data-ttu-id="7e035-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e035-134">DateTimeOffset</span></span>|<span data-ttu-id="7e035-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7e035-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="7e035-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e035-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e035-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e035-137">createdDateTime</span></span>|<span data-ttu-id="7e035-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e035-138">DateTimeOffset</span></span>|<span data-ttu-id="7e035-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7e035-139">DateTime the object was created.</span></span> <span data-ttu-id="7e035-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e035-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e035-141">description</span><span class="sxs-lookup"><span data-stu-id="7e035-141">description</span></span>|<span data-ttu-id="7e035-142">String</span><span class="sxs-lookup"><span data-stu-id="7e035-142">String</span></span>|<span data-ttu-id="7e035-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7e035-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7e035-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e035-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e035-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7e035-145">displayName</span></span>|<span data-ttu-id="7e035-146">String</span><span class="sxs-lookup"><span data-stu-id="7e035-146">String</span></span>|<span data-ttu-id="7e035-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7e035-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7e035-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e035-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e035-149">version</span><span class="sxs-lookup"><span data-stu-id="7e035-149">version</span></span>|<span data-ttu-id="7e035-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7e035-150">Int32</span></span>|<span data-ttu-id="7e035-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7e035-151">Version of the device configuration.</span></span> <span data-ttu-id="7e035-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e035-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e035-153">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="7e035-153">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="7e035-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e035-154">Boolean</span></span>|<span data-ttu-id="7e035-155">指示是否阻止 Azure 操作见解。</span><span class="sxs-lookup"><span data-stu-id="7e035-155">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="7e035-156">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="7e035-156">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="7e035-157">String</span><span class="sxs-lookup"><span data-stu-id="7e035-157">String</span></span>|<span data-ttu-id="7e035-158">Azure 操作见解工作区 ID。</span><span class="sxs-lookup"><span data-stu-id="7e035-158">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="7e035-159">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="7e035-159">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="7e035-160">String</span><span class="sxs-lookup"><span data-stu-id="7e035-160">String</span></span>|<span data-ttu-id="7e035-161">Azure 操作见解工作区键。</span><span class="sxs-lookup"><span data-stu-id="7e035-161">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="7e035-162">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="7e035-162">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="7e035-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e035-163">Boolean</span></span>|<span data-ttu-id="7e035-164">指定是否在启动投影时自动启动 Connect 应用。</span><span class="sxs-lookup"><span data-stu-id="7e035-164">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="7e035-165">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="7e035-165">maintenanceWindowBlocked</span></span>|<span data-ttu-id="7e035-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e035-166">Boolean</span></span>|<span data-ttu-id="7e035-167">指示是否阻止设置设备更新的维护时段。</span><span class="sxs-lookup"><span data-stu-id="7e035-167">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="7e035-168">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="7e035-168">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="7e035-169">Int32</span><span class="sxs-lookup"><span data-stu-id="7e035-169">Int32</span></span>|<span data-ttu-id="7e035-170">设备更新的维护时段持续时间。</span><span class="sxs-lookup"><span data-stu-id="7e035-170">Maintenance window duration for device updates.</span></span> <span data-ttu-id="7e035-171">有效值为 1 至 5</span><span class="sxs-lookup"><span data-stu-id="7e035-171">Valid values 1 to 5</span></span>|
|<span data-ttu-id="7e035-172">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="7e035-172">maintenanceWindowStartTime</span></span>|<span data-ttu-id="7e035-173">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7e035-173">TimeOfDay</span></span>|<span data-ttu-id="7e035-174">设备更新的维护时段开始时间。</span><span class="sxs-lookup"><span data-stu-id="7e035-174">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="7e035-175">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="7e035-175">miracastChannel</span></span>|<span data-ttu-id="7e035-176">String</span><span class="sxs-lookup"><span data-stu-id="7e035-176">String</span></span>|<span data-ttu-id="7e035-177">频道。</span><span class="sxs-lookup"><span data-stu-id="7e035-177">The channel.</span></span> <span data-ttu-id="7e035-178">可取值为：`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive`。</span><span class="sxs-lookup"><span data-stu-id="7e035-178">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="7e035-179">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="7e035-179">miracastBlocked</span></span>|<span data-ttu-id="7e035-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e035-180">Boolean</span></span>|<span data-ttu-id="7e035-181">指示是否阻止无线投影。</span><span class="sxs-lookup"><span data-stu-id="7e035-181">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="7e035-182">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="7e035-182">miracastRequirePin</span></span>|<span data-ttu-id="7e035-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e035-183">Boolean</span></span>|<span data-ttu-id="7e035-184">指示是否需要 PIN 才能进行无线投影。</span><span class="sxs-lookup"><span data-stu-id="7e035-184">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="7e035-185">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="7e035-185">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="7e035-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e035-186">Boolean</span></span>|<span data-ttu-id="7e035-187">指定是否禁用“开始”菜单中的“我的会议和文件”功能，该功能显示来自 Office 365 的已登录用户的会议和文件。</span><span class="sxs-lookup"><span data-stu-id="7e035-187">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="7e035-188">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="7e035-188">settingsBlockSessionResume</span></span>|<span data-ttu-id="7e035-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e035-189">Boolean</span></span>|<span data-ttu-id="7e035-190">指定是否允许在会话超时时恢复会话。</span><span class="sxs-lookup"><span data-stu-id="7e035-190">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="7e035-191">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="7e035-191">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="7e035-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e035-192">Boolean</span></span>|<span data-ttu-id="7e035-193">指定是否禁用计划会议的被邀请者自动填充登录对话框。</span><span class="sxs-lookup"><span data-stu-id="7e035-193">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="7e035-194">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="7e035-194">settingsDefaultVolume</span></span>|<span data-ttu-id="7e035-195">Int32</span><span class="sxs-lookup"><span data-stu-id="7e035-195">Int32</span></span>|<span data-ttu-id="7e035-196">指定新会话的默认音量值。</span><span class="sxs-lookup"><span data-stu-id="7e035-196">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="7e035-197">允许的值为 0-100。</span><span class="sxs-lookup"><span data-stu-id="7e035-197">Permitted values are 0-100.</span></span> <span data-ttu-id="7e035-198">默认值为 45。</span><span class="sxs-lookup"><span data-stu-id="7e035-198">The default is zero.</span></span> <span data-ttu-id="7e035-199">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="7e035-199">Valid values 0 to 100</span></span>|
|<span data-ttu-id="7e035-200">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="7e035-200">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="7e035-201">Int32</span><span class="sxs-lookup"><span data-stu-id="7e035-201">Int32</span></span>|<span data-ttu-id="7e035-202">指定 Hub 屏幕关闭前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="7e035-202">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="7e035-203">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="7e035-203">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="7e035-204">Int32</span><span class="sxs-lookup"><span data-stu-id="7e035-204">Int32</span></span>|<span data-ttu-id="7e035-205">指定会话超时前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="7e035-205">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="7e035-206">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="7e035-206">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="7e035-207">Int32</span><span class="sxs-lookup"><span data-stu-id="7e035-207">Int32</span></span>|<span data-ttu-id="7e035-208">指定 Hub 进入睡眠模式前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="7e035-208">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="7e035-209">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="7e035-209">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="7e035-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e035-210">Boolean</span></span>|<span data-ttu-id="7e035-211">指示当某人进入会议室时是否阻止欢迎屏幕自动唤醒。</span><span class="sxs-lookup"><span data-stu-id="7e035-211">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="7e035-212">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="7e035-212">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="7e035-213">String</span><span class="sxs-lookup"><span data-stu-id="7e035-213">String</span></span>|<span data-ttu-id="7e035-214">欢迎屏幕背景图像 URL。</span><span class="sxs-lookup"><span data-stu-id="7e035-214">The welcome screen background image URL.</span></span> <span data-ttu-id="7e035-215">URL 必须使用 HTTPS 协议并返回 PNG 图像。</span><span class="sxs-lookup"><span data-stu-id="7e035-215">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="7e035-216">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="7e035-216">welcomeScreenMeetingInformation</span></span>|<span data-ttu-id="7e035-217">String</span><span class="sxs-lookup"><span data-stu-id="7e035-217">String</span></span>|<span data-ttu-id="7e035-218">显示的欢迎屏幕会议信息。</span><span class="sxs-lookup"><span data-stu-id="7e035-218">The welcome screen meeting information shown.</span></span> <span data-ttu-id="7e035-219">可取值为：`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject`。</span><span class="sxs-lookup"><span data-stu-id="7e035-219">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="7e035-220">响应</span><span class="sxs-lookup"><span data-stu-id="7e035-220">Response</span></span>
<span data-ttu-id="7e035-221">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7e035-221">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e035-222">示例</span><span class="sxs-lookup"><span data-stu-id="7e035-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="7e035-223">请求</span><span class="sxs-lookup"><span data-stu-id="7e035-223">Request</span></span>
<span data-ttu-id="7e035-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7e035-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1142

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="7e035-225">响应</span><span class="sxs-lookup"><span data-stu-id="7e035-225">Response</span></span>
<span data-ttu-id="7e035-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7e035-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



