---
title: 创建 windows10GeneralConfiguration
description: 创建新的 windows10GeneralConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 59806e9e767985bc1f1a272b5ad6e874abce11ae
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66736858"
---
# <a name="create-windows10generalconfiguration"></a>创建 windows10GeneralConfiguration

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 windows10GeneralConfiguration 对象的 JSON 表示形式。

下表显示了创建 windows10GeneralConfiguration 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|enterpriseCloudPrintDiscoveryEndPoint|String|发现云打印机的终结点。|
|enterpriseCloudPrintOAuthAuthority|String|获取 OAuth 令牌的身份验证终结点。|
|enterpriseCloudPrintOAuthClientIdentifier|String|被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。|
|enterpriseCloudPrintResourceIdentifier|String|在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|应该从发现终结点查询的打印机最大数量。 此设置仅限移动设备。 有效值为 1 至 65535|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|String|在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。|
|searchBlockDiacritics|Boolean|指定搜索是否可以使用音调符号。|
|searchDisableAutoLanguageDetection|Boolean|指定建立内容和属性索引时是否使用自动语言检测。|
|searchDisableIndexingEncryptedItems|Boolean|指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。|
|searchEnableRemoteQueries|Boolean|指示是否阻止此计算机索引的远程查询。|
|searchDisableIndexerBackoff|Boolean|指示是否禁用搜索索引器回退功能。|
|searchDisableIndexingRemovableDrive|Boolean|指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。|
|searchEnableAutomaticIndexSizeManangement|Boolean|在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。|
|diagnosticsDataSubmissionMode|[diagnosticDataSubmissionMode](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。 可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。|
|oneDriveDisableFileSync|Boolean|获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。|
|smartScreenEnableAppInstallControl|Boolean|此属性将于 2019 年 7 月弃用，并将替换为属性 SmartScreenAppInstallControl。 允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。|
|personalizationDesktopImageUrl|String|指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。|
|personalizationLockScreenImageUrl|String|指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。|
|bluetoothAllowedServices|String 集合|以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。|
|bluetoothBlockAdvertising|Boolean|是否阻止用户使用蓝牙广告。|
|bluetoothBlockDiscoverableMode|Boolean|是否阻止用户使用蓝牙可发现模式。|
|bluetoothBlockPrePairing|Boolean|是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。|
|edgeBlockAutofill|Boolean|指示是否阻止自动填充。|
|edgeBlocked|Boolean|指示是否阻止用户使用 Edge 浏览器。|
|edgeCookiePolicy|[edgeCookiePolicy](../resources/intune-deviceconfig-edgecookiepolicy.md)|指示要在 Edge 浏览器中阻止的 Cookie。 可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。|
|edgeBlockDeveloperTools|Boolean|指示是否在 Edge 浏览器中阻止开发人员工具。|
|edgeBlockSendingDoNotTrackHeader|Boolean|指示是否阻止用户发送 Do Not Track 标头。|
|edgeBlockExtensions|Boolean|指示是否在 Edge 浏览器中阻止扩展。|
|edgeBlockInPrivateBrowsing|Boolean|指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。|
|edgeBlockJavaScript|Boolean|指示是否阻止用户使用 JavaScript。|
|edgeBlockPasswordManager|Boolean|指示是否阻止密码管理器。|
|edgeBlockAddressBarDropdown|Boolean|阻止 Microsoft Edge 中的地址栏下拉功能。 禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。|
|edgeBlockCompatibilityList|Boolean|阻止 Microsoft Edge 中的 Microsoft 兼容性列表。 Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。|
|edgeClearBrowsingDataOnExit|Boolean|退出 Microsoft Edge 时清除浏览数据。|
|edgeAllowStartPagesModification|Boolean|允许用户更改 Edge 上的开始页面。 使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。|
|edgeDisableFirstRunPage|Boolean|阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。 此策略允许企业（如那些参与零排放配置的企业）阻止此页面。|
|edgeBlockLiveTileDataCollection|Boolean|当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。|
|edgeSyncFavoritesWithInternetExplorer|Boolean|在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。 在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。|
|cellularBlockDataWhenRoaming|Boolean|是否阻止用户在漫游时通过手机网络使用数据。|
|cellularBlockVpn|Boolean|是否阻止用户通过手机网络使用 VPN。|
|cellularBlockVpnWhenRoaming|Boolean|通过手机网络漫游时是否阻止用户使用 VPN。|
|defenderRequireRealTimeMonitoring|Boolean|指示是否需要实时监控。|
|defenderRequireBehaviorMonitoring|Boolean|指示是否需要行为监控。|
|defenderRequireNetworkInspectionSystem|Boolean|指示是否需要网络检查系统。|
|defenderScanDownloads|Boolean|指示是否扫描下载内容。|
|defenderScanScriptsLoadedInInternetExplorer|Boolean|指示是否扫描在 Internet Explorer 浏览器中加载的脚本。|
|defenderBlockEndUserAccess|Boolean|是否阻止最终用户访问 Defender。|
|defenderSignatureUpdateIntervalInHours|Int32|签名更新间隔（以小时为单位）。 指定 0 不检查。 有效值为 0 至 24|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|监视文件活动的值。 可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|删除隔离的恶意软件之前的天数。 有效值为 0 至 90|
|defenderScanMaxCpu|Int32|扫描期间最大 CPU 使用率。 有效值为 0 至 100|
|defenderScanArchiveFiles|Boolean|指示是否扫描存档文件。|
|defenderScanIncomingMail|Boolean|指示是否扫描传入的邮件。|
|defenderScanRemovableDrivesDuringFullScan|Boolean|指示在全面扫描期间是否扫描可移动驱动器。|
|defenderScanMappedNetworkDrivesDuringFullScan|Boolean|指示在全面扫描期间是否扫描映射的网络驱动器。|
|defenderScanNetworkFiles|Boolean|指示是否扫描从网络文件夹打开的文件。|
|defenderRequireCloudProtection|Boolean|指示是否需要云保护。|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|指定云提供的保护级别。 可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|如何提示用户提交样本的配置。 可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。|
|defenderScheduledQuickScanTime|TimeOfDay|执行每日快速扫描的时间。|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|Defender 系统扫描类型。 可取值为：`userDefined`、`disabled`、`quick`、`full`。|
|defenderSystemScanSchedule|[weeklySchedule](../resources/intune-deviceconfig-weeklyschedule.md)|Defender 进行系统扫描的星期几。 可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。|
|defenderScheduledScanTime|TimeOfDay|系统扫描的 Defender 时间。|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。|
|defenderFileExtensionsToExclude|String 集合|要从扫描和实时保护中排除的文件扩展名。|
|defenderFilesAndFoldersToExclude|String 集合|要从扫描和实时保护中排除的文件和文件夹。|
|defenderProcessesToExclude|String 集合|要从扫描和实时保护中排除的进程。|
|lockScreenAllowTimeoutConfiguration|Boolean|指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。 如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。|
|lockScreenBlockActionCenterNotifications|Boolean|指示在锁定屏幕上是否阻止操作中心通知。|
|lockScreenBlockCortana|Boolean|指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。|
|lockScreenBlockToastNotifications|Boolean|指示是否允许设备锁定屏幕上方的 Toast 通知。|
|lockScreenTimeoutInSeconds|Int32|设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。 支持的值为 11-1800。 有效值为 11 至 1800|
|passwordBlockSimple|Boolean|指定是否允许使用 PIN 或密码，例如“1111”或“1234”。 对于 Windows 10 台式机，它也控制图片密码的使用。|
|passwordExpirationDays|Int32|密码过期天数。 有效值为 0 至 730|
|passwordMinimumLength|Int32|密码最短长度。 有效值为 4 至 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|passwordMinimumCharacterSetCount|Int32|密码中必需的字符集数。|
|passwordPreviousPasswordBlockCount|Int32|防止重复使用的先前密码的数量。 有效值为 0 至 50|
|passwordRequired|Boolean|指示是否要求用户输入密码。|
|passwordRequireWhenResumeFromIdleState|Boolean|指示从空闲状态恢复时是否需要密码。|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|必需的密码类型。 可取值为：`deviceDefault`、`alphanumeric`、`numeric`。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|恢复出厂设置之前登录失败的次数。 有效值为 0 至 999|
|privacyAdvertisingId|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|启用或禁用广告 ID 的使用。 已添加到 Windows 10 版本 1607 中。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|privacyAutoAcceptPairingAndConsentPrompts|Boolean|指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。|
|privacyBlockInputPersonalization|Boolean|指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。|
|startBlockUnpinningAppsFromTaskbar|Boolean|指示是否阻止用户从任务栏取消固定应用。|
|startMenuAppListVisibility|[windowsStartMenuAppListVisibilityType](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。 可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。|
|startMenuHideChangeAccountSettings|Boolean|启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。|
|startMenuHideFrequentlyUsedApps|Boolean|启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。|
|startMenuHideHibernate|Boolean|启用此策略会将休眠从开始菜单的电源按钮中隐藏。|
|startMenuHideLock|Boolean|启用此策略会将锁定从开始菜单的用户磁贴中隐藏。|
|startMenuHidePowerButton|Boolean|启用此策略会将电源按钮从开始菜单中隐藏。|
|startMenuHideRecentJumpLists|Boolean|启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。|
|startMenuHideRecentlyAddedApps|Boolean|启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。|
|startMenuHideRestartOptions|Boolean|启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。|
|startMenuHideShutDown|Boolean|启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。|
|startMenuHideSignOut|Boolean|启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。|
|startMenuHideSleep|Boolean|启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。|
|startMenuHideSwitchAccount|Boolean|启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。|
|startMenuHideUserTile|Boolean|启用此策略会将用户磁贴从开始菜单中隐藏。|
|startMenuLayoutEdgeAssetsXml|Binary|此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。 “开始”菜单布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。 在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。 仅当修改 startMenuLayoutXml 策略时才应用此策略。 该值应该是一个 UTF-8 Base64 编码的字节数组。|
|startMenuLayoutXml|Binary|允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。 通过基于布局修改架构指定 XML 文件来修改布局。 XML 需要采用 UTF8 编码的字节数组格式。|
|startMenuMode|[windowsStartMenuModeType](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|允许管理员决定显示“开始”菜单的方式。 可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。|
|startMenuPinnedFolderDocuments|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。 可取值为：`notConfigured`、`hide`、`show`。|
|startMenuPinnedFolderDownloads|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。 可取值为：`notConfigured`、`hide`、`show`。|
|startMenuPinnedFolderFileExplorer|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。 可取值为：`notConfigured`、`hide`、`show`。|
|startMenuPinnedFolderHomeGroup|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。 可取值为：`notConfigured`、`hide`、`show`。|
|startMenuPinnedFolderMusic|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。 可取值为：`notConfigured`、`hide`、`show`。|
|startMenuPinnedFolderNetwork|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。 可取值为：`notConfigured`、`hide`、`show`。|
|startMenuPinnedFolderPersonalFolder|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。 可取值为：`notConfigured`、`hide`、`show`。|
|startMenuPinnedFolderPictures|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。 可取值为：`notConfigured`、`hide`、`show`。|
|startMenuPinnedFolderSettings|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。 可取值为：`notConfigured`、`hide`、`show`。|
|startMenuPinnedFolderVideos|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。 可取值为：`notConfigured`、`hide`、`show`。|
|settingsBlockSettingsApp|Boolean|指示是否阻止访问“设置”应用。|
|settingsBlockSystemPage|Boolean|指示是否阻止在“设置”应用中访问系统。|
|settingsBlockDevicesPage|Boolean|指示是否阻止在“设置”应用中访问设备。|
|settingsBlockNetworkInternetPage|Boolean|指示是否阻止在“设置”应用中访问“网络和 Internet”。|
|settingsBlockPersonalizationPage|Boolean|指示是否阻止在“设置”应用中访问“个性化”。|
|settingsBlockAccountsPage|Boolean|指示是否阻止在“设置”应用中访问“帐户”。|
|settingsBlockTimeLanguagePage|Boolean|指示是否阻止在“设置”应用中访问“时间和语言”。|
|settingsBlockEaseOfAccessPage|Boolean|指示是否阻止在“设置”应用中访问“轻松使用”。|
|settingsBlockPrivacyPage|Boolean|指示是否阻止在“设置”应用中访问“隐私”。|
|settingsBlockUpdateSecurityPage|Boolean|指示是否阻止在“设置”应用中访问“更新和安全”。|
|settingsBlockAppsPage|Boolean|指示是否阻止在“设置”应用中访问“应用”。|
|settingsBlockGamingPage|Boolean|指示是否阻止在“设置”应用中访问“游戏”。|
|windowsSpotlightBlockConsumerSpecificFeatures|Boolean|允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。|
|windowsSpotlightBlocked|Boolean|允许 IT 管理员关闭所有 Windows 聚焦功能|
|windowsSpotlightBlockOnActionCenter|Boolean|阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能|
|windowsSpotlightBlockTailoredExperiences|Boolean|基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。|
|windowsSpotlightBlockThirdPartyNotifications|Boolean|阻止通过 Windows 聚焦投放的第三方内容|
|windowsSpotlightBlockWelcomeExperience|Boolean|阻止 Windows 聚焦 Windows 欢迎体验|
|windowsSpotlightBlockWindowsTips|Boolean|允许 IT 管理员关闭 Windows 提示的弹出窗口。|
|windowsSpotlightConfigureOnLockScreen|[windowsSpotlightEnablementSettings](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|指定聚焦的类型。 可取值为：`notConfigured`、`disabled`、`enabled`。|
|networkProxyApplySettingsDeviceWide|Boolean|如果设置，代理设置将应用于设备中的所有进程和帐户。 否则，它将应用于注册到 MDM 中的用户帐户。|
|networkProxyDisableAutoDetect|Boolean|禁用自动检测设置。 如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。|
|networkProxyAutomaticConfigurationUrl|String|指向你要使用的代理自动配置 (PAC) 脚本的地址。|
|networkProxyServer|[windows10NetworkProxyServer](../resources/intune-deviceconfig-windows10networkproxyserver.md)|指定手动代理服务器设置。|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolean|指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。|
|antiTheftModeBlocked|Boolean|指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。|
|bluetoothBlocked|Boolean|是否阻止用户使用蓝牙。|
|cameraBlocked|Boolean|是否阻止用户访问设备的照相机。|
|connectedDevicesServiceBlocked|Boolean|是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。|
|certificatesBlockManualRootCertificateInstallation|Boolean|是否阻止用户执行手动根证书安装。|
|copyPasteBlocked|Boolean|是否阻止用户使用复制粘贴。|
|cortanaBlocked|Boolean|是否阻止用户使用 Cortana。|
|deviceManagementBlockFactoryResetOnMobile|Boolean|指示是否阻止用户重置手机。|
|deviceManagementBlockManualUnenroll|Boolean|指示是否阻止用户从设备管理手动取消注册。|
|safeSearchFilter|[safeSearchFilterType](../resources/intune-deviceconfig-safesearchfiltertype.md)|指定需要的安全搜索筛选级别。 可取值为：`userDefined`、`strict`、`moderate`。|
|edgeBlockPopups|Boolean|指示是否阻止弹出窗口。|
|edgeBlockSearchSuggestions|Boolean|指示是否阻止用户在地址栏中使用搜索建议。|
|edgeBlockSendingIntranetTrafficToInternetExplorer|Boolean|指示是否将 Intranet 流量从 Edge 切换到 Internet Explorer。 注意：此属性的名称具有误导性;属性已过时，请改用 EdgeSendIntranetTrafficToInternetExplorer。|
|edgeSendIntranetTrafficToInternetExplorer|Boolean|指示是否将 Intranet 流量从 Edge 切换到 Internet Explorer。|
|edgeRequireSmartScreen|Boolean|指示是否要求用户使用智能屏蔽筛选器。|
|edgeEnterpriseModeSiteListLocation|String|指示企业模式站点列表位置。 可能是本地文件、本地网络或 http 位置。|
|edgeFirstRunUrl|String|第一次打开 Edge 浏览器时的首个运行 URL。|
|edgeSearchEngine|[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)|允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。 如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。|
|edgeHomepageUrls|String 集合|Edge 浏览器上 MDM 注册设备上的主页 URL 列表。|
|edgeBlockAccessToAboutFlags|Boolean|指示是否阻止访问 Edge 浏览器上关于标志的信息。|
|smartScreenBlockPromptOverride|Boolean|指示用户是否可以替代有关潜在恶意网站的 SmartScreen 筛选器警告。|
|smartScreenBlockPromptOverrideForFiles|Boolean|指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告|
|webRtcBlockLocalhostIpAddress|Boolean|指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址|
|internetSharingBlocked|Boolean|指示是否阻止用户使用 Internet 共享。|
|settingsBlockAddProvisioningPackage|Boolean|指示是否阻止用户安装预配程序包。|
|settingsBlockRemoveProvisioningPackage|Boolean|指示是否阻止运行时配置代理删除预配程序包。|
|settingsBlockChangeSystemTime|Boolean|指示是否阻止用户更改日期和时间设置。|
|settingsBlockEditDeviceName|Boolean|指示是否阻止用户编辑设备名称。|
|settingsBlockChangeRegion|Boolean|指示是否阻止用户更改区域设置。|
|settingsBlockChangeLanguage|Boolean|指示是否阻止用户更改语言设置。|
|settingsBlockChangePowerSleep|Boolean|指示是否阻止用户更改电源和睡眠设置。|
|locationServicesBlocked|Boolean|指示是否阻止用户使用位置服务。|
|microsoftAccountBlocked|Boolean|指示是否阻止 Microsoft 帐户。|
|microsoftAccountBlockSettingsSync|Boolean|指示是否阻止 Microsoft 帐户设置同步。|
|nfcBlocked|Boolean|指示是否阻止用户使用近场通信。|
|resetProtectionModeBlocked|Boolean|指示是否阻止用户进入重置保护模式。|
|screenCaptureBlocked|Boolean|指示是否阻止用户进行屏幕截图。|
|storageBlockRemovableStorage|Boolean|指示是否阻止用户使用可移动存储。|
|storageRequireMobileDeviceEncryption|Boolean|指示是否需要在移动设备上进行加密。|
|usbBlocked|Boolean|指示是否阻止用户使用 USB 连接。|
|voiceRecordingBlocked|Boolean|指示是否阻止用户进行语音录制。|
|wiFiBlockAutomaticConnectHotspots|Boolean|指示是否阻止自动连接到 Wi-Fi 热点。 如果 Wi-Fi 被阻止，没有任何影响。|
|wiFiBlocked|Boolean|指示是否阻止用户使用 Wi-Fi。|
|wiFiBlockManualConfiguration|Boolean|指示是否阻止用户使用 Wi-Fi 手动配置。|
|wiFiScanInterval|Int32|指定设备扫描 Wi-Fi 网络的频率。 支持的值是 1-500，其中 100 为默认值，500 为低频率。 有效值为 1 至 500|
|wirelessDisplayBlockProjectionToThisDevice|Boolean|指示是否允许其他设备发现此电脑进行投影。|
|wirelessDisplayBlockUserInputFromReceiver|Boolean|指示是否允许来自无线显示接收器的用户输入。|
|wirelessDisplayRequirePinForPairing|Boolean|指示是否需要新设备的 PIN 才能启动配对。|
|windowsStoreBlocked|Boolean|指示是否阻止用户使用 Windows 应用商店。|
|appsAllowTrustedAppsSideloading|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|windowsStoreBlockAutoUpdate|Boolean|指示是否阻止从 Windows 应用商店自动更新应用。|
|developerUnlockSetting|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|指示是否允许开发人员解锁。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|sharedUserAppDataAllowed|Boolean|指示是否阻止同一应用的多个用户共享数据。|
|appsBlockWindowsStoreOriginatedApps|Boolean|指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。|
|windowsStoreEnablePrivateStoreOnly|Boolean|指示是否启用“仅限专用应用商店”。|
|storageRestrictAppDataToSystemVolume|Boolean|指示应用程序数据是否仅限于系统驱动器。|
|storageRestrictAppInstallToSystemVolume|Boolean|指示应用程序的安装是否仅限于系统驱动器。|
|gameDvrBlocked|Boolean|指示是否阻止 DVR 和广播。|
|experienceBlockDeviceDiscovery|Boolean|指示是否启用设备发现 UX。|
|experienceBlockErrorDialogWhenNoSIM|Boolean|指示是否允许在未检测到 SIM 卡时显示错误对话框。|
|experienceBlockTaskSwitcher|Boolean|指示是否在设备上启用任务切换。|
|logonBlockFastUserSwitching|Boolean|禁用在不注销的情况下在同时登录的用户之间快速切换的功能。|
|tenantLockdownRequireNetworkDuringOutOfBoxExperience|Boolean|设备是否需要连接到网络。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 9822

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderScanDownloads": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderMonitorFileActivity": "disable",
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderScanMaxCpu": 2,
  "defenderScanArchiveFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderRequireCloudProtection": true,
  "defenderCloudBlockLevel": "high",
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderScanType": "disabled",
  "defenderSystemScanSchedule": "everyday",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9994

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderScanDownloads": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderMonitorFileActivity": "disable",
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderScanMaxCpu": 2,
  "defenderScanArchiveFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderRequireCloudProtection": true,
  "defenderCloudBlockLevel": "high",
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderScanType": "disabled",
  "defenderSystemScanSchedule": "everyday",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true
}
```





