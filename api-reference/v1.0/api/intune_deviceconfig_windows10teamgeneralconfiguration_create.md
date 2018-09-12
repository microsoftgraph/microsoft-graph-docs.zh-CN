# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="701f3-101">创建 windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="701f3-101">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="701f3-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="701f3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="701f3-103">创建新的 [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="701f3-103">Create a new [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="701f3-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="701f3-104">Prerequisites</span></span>
<span data-ttu-id="701f3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="701f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="701f3-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="701f3-107">Permission type</span></span>|<span data-ttu-id="701f3-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="701f3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="701f3-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="701f3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="701f3-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="701f3-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="701f3-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="701f3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="701f3-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="701f3-112">Not supported.</span></span>|
|<span data-ttu-id="701f3-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="701f3-113">Application</span></span>|<span data-ttu-id="701f3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="701f3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="701f3-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="701f3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="701f3-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="701f3-116">Request headers</span></span>
|<span data-ttu-id="701f3-117">标头</span><span class="sxs-lookup"><span data-stu-id="701f3-117">Header</span></span>|<span data-ttu-id="701f3-118">值</span><span class="sxs-lookup"><span data-stu-id="701f3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="701f3-119">授权</span><span class="sxs-lookup"><span data-stu-id="701f3-119">Authorization</span></span>|<span data-ttu-id="701f3-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="701f3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="701f3-121">接受</span><span class="sxs-lookup"><span data-stu-id="701f3-121">Accept</span></span>|<span data-ttu-id="701f3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="701f3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="701f3-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="701f3-123">Request body</span></span>
<span data-ttu-id="701f3-124">在请求正文中，提供 windows10TeamGeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="701f3-124">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="701f3-125">下表显示了创建 windows10TeamGeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="701f3-125">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="701f3-126">属性</span><span class="sxs-lookup"><span data-stu-id="701f3-126">Property</span></span>|<span data-ttu-id="701f3-127">类型</span><span class="sxs-lookup"><span data-stu-id="701f3-127">Type</span></span>|<span data-ttu-id="701f3-128">说明</span><span class="sxs-lookup"><span data-stu-id="701f3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="701f3-129">ID</span><span class="sxs-lookup"><span data-stu-id="701f3-129">id</span></span>|<span data-ttu-id="701f3-130">字符串</span><span class="sxs-lookup"><span data-stu-id="701f3-130">String</span></span>|<span data-ttu-id="701f3-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="701f3-131">Key of the entity.</span></span> <span data-ttu-id="701f3-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="701f3-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="701f3-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="701f3-133">lastModifiedDateTime</span></span>|<span data-ttu-id="701f3-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="701f3-134">DateTimeOffset</span></span>|<span data-ttu-id="701f3-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="701f3-135">DateTime the object was last modified.</span></span> <span data-ttu-id="701f3-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="701f3-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="701f3-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="701f3-137">createdDateTime</span></span>|<span data-ttu-id="701f3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="701f3-138">DateTimeOffset</span></span>|<span data-ttu-id="701f3-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="701f3-139">DateTime the object was created.</span></span> <span data-ttu-id="701f3-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="701f3-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="701f3-141">描述</span><span class="sxs-lookup"><span data-stu-id="701f3-141">description</span></span>|<span data-ttu-id="701f3-142">字符串</span><span class="sxs-lookup"><span data-stu-id="701f3-142">String</span></span>|<span data-ttu-id="701f3-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="701f3-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="701f3-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="701f3-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="701f3-145">displayName</span><span class="sxs-lookup"><span data-stu-id="701f3-145">displayName</span></span>|<span data-ttu-id="701f3-146">字符串</span><span class="sxs-lookup"><span data-stu-id="701f3-146">String</span></span>|<span data-ttu-id="701f3-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="701f3-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="701f3-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="701f3-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="701f3-149">版本</span><span class="sxs-lookup"><span data-stu-id="701f3-149">version</span></span>|<span data-ttu-id="701f3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="701f3-150">Int32</span></span>|<span data-ttu-id="701f3-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="701f3-151">Version of the device configuration.</span></span> <span data-ttu-id="701f3-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="701f3-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="701f3-153">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="701f3-153">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="701f3-154">布尔</span><span class="sxs-lookup"><span data-stu-id="701f3-154">Boolean</span></span>|<span data-ttu-id="701f3-155">指示是否阻止 Azure 操作见解。</span><span class="sxs-lookup"><span data-stu-id="701f3-155">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="701f3-156">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="701f3-156">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="701f3-157">字符串</span><span class="sxs-lookup"><span data-stu-id="701f3-157">String</span></span>|<span data-ttu-id="701f3-158">Azure 操作见解工作区 ID。</span><span class="sxs-lookup"><span data-stu-id="701f3-158">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="701f3-159">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="701f3-159">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="701f3-160">字符串</span><span class="sxs-lookup"><span data-stu-id="701f3-160">String</span></span>|<span data-ttu-id="701f3-161">Azure 操作见解工作区键。</span><span class="sxs-lookup"><span data-stu-id="701f3-161">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="701f3-162">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="701f3-162">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="701f3-163">布尔</span><span class="sxs-lookup"><span data-stu-id="701f3-163">Boolean</span></span>|<span data-ttu-id="701f3-164">指定是否在启动投影时自动启动 Connect 应用。</span><span class="sxs-lookup"><span data-stu-id="701f3-164">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="701f3-165">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="701f3-165">maintenanceWindowBlocked</span></span>|<span data-ttu-id="701f3-166">布尔</span><span class="sxs-lookup"><span data-stu-id="701f3-166">Boolean</span></span>|<span data-ttu-id="701f3-167">指示是否阻止设置设备更新的维护时段。</span><span class="sxs-lookup"><span data-stu-id="701f3-167">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="701f3-168">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="701f3-168">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="701f3-169">Int32</span><span class="sxs-lookup"><span data-stu-id="701f3-169">Int32</span></span>|<span data-ttu-id="701f3-170">设备更新的维护时段持续时间。</span><span class="sxs-lookup"><span data-stu-id="701f3-170">Maintenance window duration for device updates.</span></span> <span data-ttu-id="701f3-171">有效值为 0 至 5</span><span class="sxs-lookup"><span data-stu-id="701f3-171">Valid values 0 to 5</span></span>|
|<span data-ttu-id="701f3-172">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="701f3-172">maintenanceWindowStartTime</span></span>|<span data-ttu-id="701f3-173">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="701f3-173">TimeOfDay</span></span>|<span data-ttu-id="701f3-174">设备更新的维护时段开始时间。</span><span class="sxs-lookup"><span data-stu-id="701f3-174">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="701f3-175">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="701f3-175">miracastChannel</span></span>|[<span data-ttu-id="701f3-176">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="701f3-176">miracastChannel</span></span>](../resources/intune_deviceconfig_miracastchannel.md)|<span data-ttu-id="701f3-p109">频道。可能的值是：`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive`。</span><span class="sxs-lookup"><span data-stu-id="701f3-p109">The channel. The possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="701f3-179">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="701f3-179">miracastBlocked</span></span>|<span data-ttu-id="701f3-180">布尔</span><span class="sxs-lookup"><span data-stu-id="701f3-180">Boolean</span></span>|<span data-ttu-id="701f3-181">指示是否阻止无线投影。</span><span class="sxs-lookup"><span data-stu-id="701f3-181">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="701f3-182">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="701f3-182">miracastRequirePin</span></span>|<span data-ttu-id="701f3-183">布尔</span><span class="sxs-lookup"><span data-stu-id="701f3-183">Boolean</span></span>|<span data-ttu-id="701f3-184">指示是否需要 PIN 才能进行无线投影。</span><span class="sxs-lookup"><span data-stu-id="701f3-184">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="701f3-185">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="701f3-185">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="701f3-186">布尔</span><span class="sxs-lookup"><span data-stu-id="701f3-186">Boolean</span></span>|<span data-ttu-id="701f3-187">指定是否禁用“开始”菜单中的“我的会议和文件”功能，该功能显示来自 Office 365 的已登录用户的会议和文件。</span><span class="sxs-lookup"><span data-stu-id="701f3-187">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="701f3-188">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="701f3-188">settingsBlockSessionResume</span></span>|<span data-ttu-id="701f3-189">布尔</span><span class="sxs-lookup"><span data-stu-id="701f3-189">Boolean</span></span>|<span data-ttu-id="701f3-190">指定是否允许在会话超时时恢复会话。</span><span class="sxs-lookup"><span data-stu-id="701f3-190">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="701f3-191">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="701f3-191">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="701f3-192">布尔</span><span class="sxs-lookup"><span data-stu-id="701f3-192">Boolean</span></span>|<span data-ttu-id="701f3-193">指定是否禁用计划会议的被邀请者自动填充登录对话框。</span><span class="sxs-lookup"><span data-stu-id="701f3-193">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="701f3-194">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="701f3-194">settingsDefaultVolume</span></span>|<span data-ttu-id="701f3-195">Int32</span><span class="sxs-lookup"><span data-stu-id="701f3-195">Int32</span></span>|<span data-ttu-id="701f3-196">指定新会话的默认音量值。</span><span class="sxs-lookup"><span data-stu-id="701f3-196">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="701f3-197">允许的值为 0-100。</span><span class="sxs-lookup"><span data-stu-id="701f3-197">Permitted values are 0-100.</span></span> <span data-ttu-id="701f3-198">默认值为 45。</span><span class="sxs-lookup"><span data-stu-id="701f3-198">The default is 45.</span></span> <span data-ttu-id="701f3-199">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="701f3-199">Valid values 0 to 100</span></span>|
|<span data-ttu-id="701f3-200">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="701f3-200">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="701f3-201">Int32</span><span class="sxs-lookup"><span data-stu-id="701f3-201">Int32</span></span>|<span data-ttu-id="701f3-202">指定 Hub 屏幕关闭前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="701f3-202">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="701f3-203">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="701f3-203">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="701f3-204">Int32</span><span class="sxs-lookup"><span data-stu-id="701f3-204">Int32</span></span>|<span data-ttu-id="701f3-205">指定会话超时前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="701f3-205">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="701f3-206">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="701f3-206">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="701f3-207">Int32</span><span class="sxs-lookup"><span data-stu-id="701f3-207">Int32</span></span>|<span data-ttu-id="701f3-208">指定 Hub 进入睡眠模式前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="701f3-208">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="701f3-209">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="701f3-209">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="701f3-210">布尔</span><span class="sxs-lookup"><span data-stu-id="701f3-210">Boolean</span></span>|<span data-ttu-id="701f3-211">指示当某人进入会议室时是否阻止欢迎屏幕自动唤醒。</span><span class="sxs-lookup"><span data-stu-id="701f3-211">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="701f3-212">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="701f3-212">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="701f3-213">字符串</span><span class="sxs-lookup"><span data-stu-id="701f3-213">String</span></span>|<span data-ttu-id="701f3-214">欢迎屏幕背景图像 URL。</span><span class="sxs-lookup"><span data-stu-id="701f3-214">The welcome screen background image URL.</span></span> <span data-ttu-id="701f3-215">URL 必须使用 HTTPS 协议并返回 PNG 图像。</span><span class="sxs-lookup"><span data-stu-id="701f3-215">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="701f3-216">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="701f3-216">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="701f3-217">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="701f3-217">welcomeScreenMeetingInformation</span></span>](../resources/intune_deviceconfig_welcomescreenmeetinginformation.md)|<span data-ttu-id="701f3-p112">显示的欢迎屏幕会议信息。可取值是：`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject`。</span><span class="sxs-lookup"><span data-stu-id="701f3-p112">The welcome screen meeting information shown. The possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="701f3-220">响应</span><span class="sxs-lookup"><span data-stu-id="701f3-220">Response</span></span>
<span data-ttu-id="701f3-221">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="701f3-221">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="701f3-222">示例</span><span class="sxs-lookup"><span data-stu-id="701f3-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="701f3-223">请求</span><span class="sxs-lookup"><span data-stu-id="701f3-223">Request</span></span>
<span data-ttu-id="701f3-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="701f3-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1214

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="701f3-225">响应</span><span class="sxs-lookup"><span data-stu-id="701f3-225">Response</span></span>
<span data-ttu-id="701f3-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="701f3-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








