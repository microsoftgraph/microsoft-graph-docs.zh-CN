---
title: 创建 androidDeviceOwnerGeneralDeviceConfiguration
description: 创建新的 androidDeviceOwnerGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 959cbb063fe8d61383a1d804eb2a49a858b88911
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668235"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a>创建 androidDeviceOwnerGeneralDeviceConfiguration

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象。

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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，为 androidDeviceOwnerGeneralDeviceConfiguration 对象提供 JSON 表示形式。

下表显示了创建 androidDeviceOwnerGeneralDeviceConfiguration 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|字符串集合|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持分配范围标记。 如果此值为 false，并且作用域内用户不可见，则不允许分配到 ScopeTags 属性。 对于在 Silverlight 中创建的旧策略，可以通过在 Azure 门户中删除和重新创建策略来解决此问题。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的 OS 版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的 OS 版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|说明|字符串|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|azureAdSharedDeviceDataClearApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|托管应用的列表，这些应用将在 AAD 共享设备模式下的全局注销期间清除其数据。 该集合最多可包含 500 个元素。|
|accountsBlockModification|Boolean|指示是否禁用添加或删除帐户。|
|appsAllowInstallFromUnknownSources|布尔|指示是否允许用户启用未知源设置。|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|指示应用自动更新策略的值。 可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|指示针对运行时权限的请求的权限策略（如果未专门为应用定义权限）。 可能的值是：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。|
|appsRecommendSkippingFirstUseHints|布尔|是否建议所有应用跳过他们可能添加的任何首次使用提示。|
|bluetoothBlockConfiguration|布尔|指示是否阻止用户配置蓝牙。|
|bluetoothBlockContactSharing|Boolean|指示是否阻止用户通过蓝牙共享联系人。|
|cameraBlocked|Boolean|指示是否禁用相机。|
|cellularBlockWiFiTethering|Boolean|指示是否阻止 Wi-Fi 网络共享。|
|certificateCredentialConfigurationDisabled|Boolean|指示是否阻止用户进行任何证书凭据配置。|
|crossProfilePoliciesAllowCopyPaste|Boolean|指示从一个配置文件复制的文本 (个人或工作) 是否可以粘贴到另一个配置文件中。|
|crossProfilePoliciesAllowDataSharing|[androidDeviceOwnerCrossProfileDataSharing](../resources/intune-deviceconfig-androiddeviceownercrossprofiledatasharing.md)|指示从一个配置文件 (个人或工作) 的数据是否可以与其他配置文件中的应用共享。 可取值为：`notConfigured`、`crossProfileDataSharingBlocked`、`dataSharingFromWorkToPersonalBlocked`、`crossProfileDataSharingAllowed`、`unkownFutureValue`。|
|crossProfilePoliciesShowWorkContactsInPersonalProfile|Boolean|指示是否在个人配置文件联系人搜索/传入呼叫中显示存储在工作配置文件中的联系人。|
|microsoftLauncherConfigurationEnabled|Boolean|指示是否要配置 Microsoft Launcher。|
|microsoftLauncherCustomWallpaperEnabled|布尔|指示是否在目标设备上配置壁纸。|
|microsoftLauncherCustomWallpaperImageUrl|String|指示要用作目标设备上的壁纸的图像文件的 URL。|
|microsoftLauncherCustomWallpaperAllowUserModification|Boolean|指示用户是否可以修改壁纸以个性化其设备。|
|microsoftLauncherFeedEnabled|布尔|指示是否要在设备上启用启动器源。|
|microsoftLauncherFeedAllowUserModification|Boolean|指示用户是否可以修改设备上的启动器源。|
|microsoftLauncherDockPresenceConfiguration|[microsoftLauncherDockPresence](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|指示是否要配置设备停靠。 可能的值是：`notConfigured`、`show`、`hide`、`disabled`。|
|microsoftLauncherDockPresenceAllowUserModification|Boolean|指示用户是否可以修改设备上的设备停靠配置。|
|microsoftLauncherSearchBarPlacementConfiguration|[microsoftLauncherSearchBarPlacement](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|指示设备上的搜索栏放置配置。 可能的值是：`notConfigured`、`top`、`bottom`、`hide`。|
|enrollmentProfile|[androidDeviceOwnerEnrollmentProfileType](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|指示要配置的注册配置文件。 可取值为：`notConfigured`、`dedicatedDevice`、`fullyManaged`。|
|dataRoamingBlocked|Boolean|指示是否阻止用户进行数据漫游。|
|dateTimeConfigurationBlocked|布尔|指示是否阻止用户手动更改设备上的日期或时间|
|detailedHelpText|[androidDeviceOwnerUserFacingMessage](../resources/intune-deviceconfig-androiddeviceowneruserfacingmessage.md)|表示用户尝试修改其设备上的托管设置时提供的自定义详细帮助文本。|
|deviceOwnerLockScreenMessage|[androidDeviceOwnerUserFacingMessage](../resources/intune-deviceconfig-androiddeviceowneruserfacingmessage.md)|表示用户尝试修改其设备上的托管设置时提供的自定义锁屏消息。|
|securityCommonCriteriaModeEnabled|Boolean|表示在用户尝试修改其设备上的托管设置时为其提供的安全通用条件模式。|
|factoryResetDeviceAdministratorEmails|String collection|在设备在设置出厂重置后需要进行身份验证的 Google 帐户电子邮件列表。|
|factoryResetBlocked|Boolean|指示是否禁用设置中的出厂重置选项。|
|globalProxy|[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|代理直接使用主机、端口和排除的主机进行设置。|
|googleAccountsBlocked|Boolean|指示是否阻止 Google 帐户。|
|kioskCustomizationDeviceSettingsBlocked|Boolean|指示用户是否可以在展台模式下访问设备的“设置”应用。|
|kioskCustomizationPowerButtonActionsBlocked|Boolean|当用户长时间按展台模式下设备的 Power 按钮时，是否显示电源菜单。|
|kioskCustomizationStatusBar|[androidDeviceOwnerKioskCustomizationStatusBar](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|指示是否在展台模式下禁用系统信息和通知。 可取值为：`notConfigured`、`notificationsAndSystemInfoEnabled`、`systemInfoOnly`。|
|kioskCustomizationSystemErrorWarnings|Boolean|指示是否在展台模式下显示崩溃或无响应应用的系统错误对话框。|
|kioskCustomizationSystemNavigation|[androidDeviceOwnerKioskCustomizationSystemNavigation](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|指示在展台模式下启用了哪些导航功能。 可取值为：`notConfigured`、`navigationEnabled`、`homeButtonOnly`。|
|kioskModeScreenSaverConfigurationEnabled|Boolean|是否在展台模式下启用屏幕保护模式。|
|kioskModeScreenSaverImageUrl|String|映像的 URL，该图像将成为展台模式下设备的屏幕保护程序。|
|kioskModeScreenSaverDisplayTimeInSeconds|Int32|设备在展台模式下显示屏幕保护程序的秒数。 有效值 0 到9999999|
|kioskModeScreenSaverStartDelayInSeconds|Int32|在展台模式下显示屏幕保护程序之前，设备需要处于非活动状态的秒数。 有效值 1 到9999999|
|kioskModeScreenSaverDetectMediaDisabled|Boolean|如果音频/视频在展台模式下播放，设备屏幕是否应显示屏幕保护程序。|
|kioskModeApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|当设备处于展台模式时将显示的托管应用列表。 该集合最多可包含 500 个元素。|
|kioskModeWallpaperUrl|字符串|当设备处于展台模式时，用于壁纸的可公开访问的映像的 URL。|
|kioskModeExitCode|String|退出代码以允许用户在设备处于展台模式时从展台模式中转义。|
|kioskModeVirtualHomeButtonEnabled|Boolean|设备处于展台模式时是否显示虚拟主页按钮。|
|kioskModeVirtualHomeButtonType|[androidDeviceOwnerVirtualHomeButtonType](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|指示虚拟主页按钮是向上轻扫主页按钮还是浮动主页按钮。 可取值为：`notConfigured`、`swipeUp`、`floating`。|
|kioskModeBluetoothConfigurationEnabled|Boolean|是否允许用户在展台模式下配置蓝牙设置。|
|kioskModeWiFiConfigurationEnabled|Boolean|是否允许用户在展台模式下配置Wi-Fi设置。|
|kioskModeFlashlightConfigurationEnabled|布尔|是否允许用户在展台模式下使用手电筒。|
|kioskModeMediaVolumeConfigurationEnabled|Boolean|是否允许用户在展台模式下更改媒体卷。|
|kioskModeShowDeviceInfo|Boolean|是否允许用户访问基本设备信息。|
|kioskModeManagedSettingsEntryDisabled|Boolean|是否在展台模式下的托管主屏幕上显示托管设置入口点。|
|kioskModeDebugMenuEasyAccessEnabled|Boolean|是否允许用户轻松访问展台模式下的调试菜单。|
|kioskModeShowAppNotificationBadge|布尔|是否在展台模式下显示应用程序通知徽章。|
|kioskModeScreenOrientation|[androidDeviceOwnerKioskModeScreenOrientation](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|展台模式下托管主屏幕的屏幕方向配置。 可取值为：`notConfigured`、`portrait`、`landscape`、`autoRotate`。|
|kioskModeIconSize|[androidDeviceOwnerKioskModeIconSize](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|展台模式下托管主屏幕的图标大小配置。 可取值为：`notConfigured`、`smallest`、`small`、`regular`、`large`、`largest`。|
|kioskModeFolderIcon|[androidDeviceOwnerKioskModeFolderIcon](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|展台模式下托管主屏幕的文件夹图标配置。 可取值为：`notConfigured`、`darkSquare`、`darkCircle`、`lightSquare`、`lightCircle`。|
|kioskModeWifiAllowedSsids|字符串集合|用户可在展台模式下配置的受限 WIFI SSID 集。 该集合最多可包含 500 个元素。|
|kioskModeAppOrderEnabled|Boolean|是否在展台模式下启用应用排序。|
|kioskModeAppsInFolderOrderedByName|Boolean|是否在展台模式下对文件夹中的应用程序进行字母表单。|
|kioskModeGridHeight|Int32|在展台模式下启用了应用排序的托管主屏幕网格的行数。 有效值 1 到9999999|
|kioskModeGridWidth|Int32|在展台模式下启用了应用排序的托管主屏幕网格的列数。 有效值 1 到9999999|
|kioskModeLockHomeScreen|Boolean|是否在展台模式下将主屏幕锁定到最终用户。|
|kioskModeManagedFolders|[androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md) 集合|展台模式下设备的托管文件夹列表。 该集合最多可包含 500 个元素。|
|kioskModeAppPositions|[androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md) 集合|展台模式上的项排序托管主屏幕。 该集合最多可包含 500 个元素。|
|kioskModeManagedHomeScreenAutoSignout|Boolean|是否在非活动状态后自动注销 MHS 和共享设备模式应用程序以进行托管主屏幕。|
|kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds|Int32|在自动注销用户以进行托管主屏幕之前通知用户的秒数。 有效值 0 到9999999|
|kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds|Int32|在自动将用户注销托管主屏幕之前，设备处于非活动状态的秒数。 有效值 0 到9999999|
|kioskModeManagedHomeScreenPinComplexity|[kioskModeManagedHomeScreenPinComplexity](../resources/intune-deviceconfig-kioskmodemanagedhomescreenpincomplexity.md)|托管主屏幕登录会话的 PIN 复杂性。 可取值为：`notConfigured`、`simple`、`complex`。|
|kioskModeManagedHomeScreenPinRequired|Boolean|是否要求用户为托管主屏幕的登录会话设置 PIN。|
|kioskModeManagedHomeScreenPinRequiredToResume|Boolean|是否需要用户输入会话 PIN（如果屏幕保护程序已显示为托管主屏幕）。|
|kioskModeManagedHomeScreenSignInBackground|String|托管主屏幕登录屏幕的自定义 URL 背景。|
|kioskModeManagedHomeScreenSignInBrandingLogo|String|用于登录屏幕的自定义 URL 品牌徽标和用于托管主屏幕的会话固定页。|
|kioskModeManagedHomeScreenSignInEnabled|布尔|是否显示托管主屏幕的登录屏幕。|
|kioskModeUseManagedHomeScreenApp|[kioskModeType](../resources/intune-deviceconfig-kioskmodetype.md)|是否使用单个应用展台模式或多应用展台模式。 可取值为：`notConfigured`、`singleAppMode`、`multiAppMode`。|
|microphoneForceMute|布尔|指示是否阻止在设备上取消麦克风。|
|networkEscapeHatchAllowed|布尔|指示设备是否允许在启动时连接到临时网络连接。|
|nfcBlockOutgoingBeam|Boolean|指示是否阻止 NFC 传出光束。|
|passwordBlockKeyguard|Boolean|指示是否禁用了密钥防护。|
|passwordBlockKeyguardFeatures|[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) 集合|要阻止的设备密钥防护功能列表。 该集合最多可包含 7 个元素。 可取值为：`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures`、`face`、`iris`、`biometrics`。|
|passwordExpirationDays|Int32|指示在密码过期之前可以设置密码的时间，并且需要新密码。 有效值为 1 至 365。|
|passwordMinimumLength|Int32|指示设备上所需的密码的最小长度。 有效值为 4 至 16|
|passwordMinimumLetterCharacters|Int32|指示设备密码所需的最小字母字符数。 有效值 1 到 16|
|passwordMinimumLowerCaseCharacters|Int32|指示设备密码所需的最小大小写字符数。 有效值 1 到 16|
|passwordMinimumNonLetterCharacters|Int32|指示设备密码所需的最小非字母字符数。 有效值 1 到 16|
|passwordMinimumNumericCharacters|Int32|指示设备密码所需的最小数值字符数。 有效值 1 到 16|
|passwordMinimumSymbolCharacters|Int32|指示设备密码所需的最小符号字符数。 有效值 1 到 16|
|passwordMinimumUpperCaseCharacters|Int32|指示设备密码所需的最小大写字母字符数。 有效值 1 到 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|passwordPreviousPasswordCountToBlock|Int32|指示密码历史记录的长度，其中用户将无法输入与历史记录中任何密码相同的新密码。 有效值为 0 至 24|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|指示设备上所需的最低密码质量。 可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。|
|passwordRequireUnlock|[androidDeviceOwnerRequiredPasswordUnlock](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordunlock.md)|指示必须使用强身份验证的形式解锁设备的超时时间段。 可取值为：`deviceDefault`、`daily`、`unkownFutureValue`。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|指示用户在擦除设备之前输入错误密码的次数。 有效值为 4 至 11|
|playStoreMode|[androidDeviceOwnerPlayStoreMode](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|指示设备的 Play 应用商店模式。 可取值为：`notConfigured`、`allowList`、`blockList`。|
|screenCaptureBlocked|Boolean|指示是否禁用拍摄屏幕截图的功能。|
|securityDeveloperSettingsEnabled|Boolean|指示是否允许用户访问开发人员设置，例如开发人员选项和设备上的安全启动。|
|securityRequireVerifyApps|Boolean|指示是否验证是否需要应用。|
|shortHelpText|[androidDeviceOwnerUserFacingMessage](../resources/intune-deviceconfig-androiddeviceowneruserfacingmessage.md)|表示用户尝试修改其设备上的托管设置时提供的自定义的简短帮助文本。|
|statusBarBlocked|布尔|指示是否禁用状态栏，包括通知、快速设置和其他屏幕覆盖。|
|stayOnModes|[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) 集合|设备显示将保持启用状态的模式列表。 此集合最多可以包含 4 个元素。 可能的值是：`notConfigured`、`ac`、`usb`、`wireless`。|
|storageAllowUsb|Boolean|指示是否允许 USB 大容量存储。|
|storageBlockExternalMedia|Boolean|指示是否阻止外部媒体。|
|storageBlockUsbFileTransfer|Boolean|指示是否阻止 USB 文件传输。|
|systemUpdateFreezePeriods|[androidDeviceOwnerSystemUpdateFreezePeriod](../resources/intune-deviceconfig-androiddeviceownersystemupdatefreezeperiod.md) 集合|指示系统更新延迟的每年重复时间段。 该集合最多可包含 500 个元素。|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|指示系统更新窗口在午夜后启动的分钟数。 有效值 0 到 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|指示系统更新窗口在午夜后结束的分钟数。 有效值 0 到 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|系统更新配置的类型。 可能的值是：`deviceDefault`、`postpone`、`windowed`、`automatic`。|
|systemWindowsBlocked|Boolean|是否阻止 Android 系统提示窗口，例如 Toast、电话活动和系统警报。|
|usersBlockAdd|Boolean|指示是否禁用添加用户和配置文件。|
|usersBlockRemove|Boolean|指示是否禁用从设备中删除其他用户。|
|volumeBlockAdjustment|Boolean|指示是否禁用了调整主卷。|
|vpnAlwaysOnLockdownMode|布尔|如果指定了 Always on VPN 包名称，则在该 VPN 断开连接时是否锁定网络流量。|
|vpnAlwaysOnPackageIdentifier|String|用于处理始终开启 VPN 连接的应用的 Android 应用包名称。|
|wifiBlockEditConfigurations|Boolean|指示是否阻止用户编辑 wifi 连接设置。|
|wifiBlockEditPolicyDefinedConfigurations|布尔|指示是否仅阻止用户编辑策略定义的网络。|
|personalProfileAppsAllowInstallFromUnknownSources|Boolean|指示用户是否可以在个人配置文件上安装来自未知源的应用。|
|personalProfileCameraBlocked|Boolean|指示是否在个人配置文件上禁用相机。|
|personalProfileScreenCaptureBlocked|Boolean|指示是否禁用在个人配置文件上拍摄屏幕截图的功能。|
|personalProfilePlayStoreMode|[personalProfilePersonalPlayStoreMode](../resources/intune-deviceconfig-personalprofilepersonalplaystoremode.md)|与 PersonalProfilePersonalApplications 一起使用，用于控制允许或阻止个人配置文件中的应用的方式。 可取值为：`notConfigured`、`blockedApps`、`allowedApps`。|
|personalProfilePersonalApplications|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|应用于个人配置文件中的应用程序的策略。 该集合最多可包含 500 个元素。|
|workProfilePasswordExpirationDays|Int32|指示工作配置文件密码过期前可以设置的工作配置文件密码的天数，并且需要新密码。 有效值为 1 至 365。|
|workProfilePasswordMinimumLength|Int32|指示工作配置文件密码的最小长度。 有效值为 4 至 16|
|workProfilePasswordMinimumNumericCharacters|Int32|指示工作配置文件密码所需的最小数值字符数。 有效值 1 到 16|
|workProfilePasswordMinimumNonLetterCharacters|Int32|指示工作配置文件密码所需的最小非字母字符数。 有效值 1 到 16|
|workProfilePasswordMinimumLetterCharacters|Int32|指示工作配置文件密码所需的最小字母字符数。 有效值 1 到 16|
|workProfilePasswordMinimumLowerCaseCharacters|Int32|指示工作配置文件密码所需的最小大小写字符数。 有效值 1 到 16|
|workProfilePasswordMinimumUpperCaseCharacters|Int32|指示工作配置文件密码所需的最小大写字母字符数。 有效值 1 到 16|
|workProfilePasswordMinimumSymbolCharacters|Int32|指示工作配置文件密码所需的最小符号字符数。 有效值 1 到 16|
|workProfilePasswordPreviousPasswordCountToBlock|Int32|指示工作配置文件密码历史记录的长度，其中用户将无法输入与历史记录中的任何密码相同的新密码。 有效值为 0 至 24|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|指示用户在擦除设备之前输入不正确的工作配置文件密码的次数。 有效值为 4 至 11|
|workProfilePasswordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|指示工作配置文件密码所需的最低密码质量。 可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。|
|workProfilePasswordRequireUnlock|[androidDeviceOwnerRequiredPasswordUnlock](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordunlock.md)|指示必须使用强身份验证的形式解锁工作配置文件之后的超时时间段。 可取值为：`deviceDefault`、`daily`、`unkownFutureValue`。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 10090

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
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
  "azureAdSharedDeviceDataClearApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "crossProfilePoliciesAllowCopyPaste": true,
  "crossProfilePoliciesAllowDataSharing": "crossProfileDataSharingBlocked",
  "crossProfilePoliciesShowWorkContactsInPersonalProfile": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "detailedHelpText": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "defaultMessage": "Default Message value"
  },
  "deviceOwnerLockScreenMessage": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "defaultMessage": "Default Message value"
  },
  "securityCommonCriteriaModeEnabled": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "navigationEnabled",
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 3,
  "kioskModeGridWidth": 2,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "Folder Name value",
      "folderIdentifier": "Folder Identifier value",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "Label value",
          "link": "Link value"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 8,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "Label value",
        "link": "Link value"
      }
    }
  ],
  "kioskModeManagedHomeScreenAutoSignout": true,
  "kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds": 7,
  "kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds": 8,
  "kioskModeManagedHomeScreenPinComplexity": "simple",
  "kioskModeManagedHomeScreenPinRequired": true,
  "kioskModeManagedHomeScreenPinRequiredToResume": true,
  "kioskModeManagedHomeScreenSignInBackground": "Kiosk Mode Managed Home Screen Sign In Background value",
  "kioskModeManagedHomeScreenSignInBrandingLogo": "Kiosk Mode Managed Home Screen Sign In Branding Logo value",
  "kioskModeManagedHomeScreenSignInEnabled": true,
  "kioskModeUseManagedHomeScreenApp": "singleAppMode",
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordRequireUnlock": "daily",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "screenCaptureBlocked": true,
  "securityDeveloperSettingsEnabled": true,
  "securityRequireVerifyApps": true,
  "shortHelpText": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "defaultMessage": "Default Message value"
  },
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateFreezePeriods": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerSystemUpdateFreezePeriod",
      "startMonth": 10,
      "startDay": 8,
      "endMonth": 8,
      "endDay": 6
    }
  ],
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "personalProfilePlayStoreMode": "blockedApps",
  "personalProfilePersonalApplications": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required",
  "workProfilePasswordRequireUnlock": "daily"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10262

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
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
  "azureAdSharedDeviceDataClearApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "crossProfilePoliciesAllowCopyPaste": true,
  "crossProfilePoliciesAllowDataSharing": "crossProfileDataSharingBlocked",
  "crossProfilePoliciesShowWorkContactsInPersonalProfile": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "detailedHelpText": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "defaultMessage": "Default Message value"
  },
  "deviceOwnerLockScreenMessage": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "defaultMessage": "Default Message value"
  },
  "securityCommonCriteriaModeEnabled": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "navigationEnabled",
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 3,
  "kioskModeGridWidth": 2,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "Folder Name value",
      "folderIdentifier": "Folder Identifier value",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "Label value",
          "link": "Link value"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 8,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "Label value",
        "link": "Link value"
      }
    }
  ],
  "kioskModeManagedHomeScreenAutoSignout": true,
  "kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds": 7,
  "kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds": 8,
  "kioskModeManagedHomeScreenPinComplexity": "simple",
  "kioskModeManagedHomeScreenPinRequired": true,
  "kioskModeManagedHomeScreenPinRequiredToResume": true,
  "kioskModeManagedHomeScreenSignInBackground": "Kiosk Mode Managed Home Screen Sign In Background value",
  "kioskModeManagedHomeScreenSignInBrandingLogo": "Kiosk Mode Managed Home Screen Sign In Branding Logo value",
  "kioskModeManagedHomeScreenSignInEnabled": true,
  "kioskModeUseManagedHomeScreenApp": "singleAppMode",
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordRequireUnlock": "daily",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "screenCaptureBlocked": true,
  "securityDeveloperSettingsEnabled": true,
  "securityRequireVerifyApps": true,
  "shortHelpText": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "defaultMessage": "Default Message value"
  },
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateFreezePeriods": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerSystemUpdateFreezePeriod",
      "startMonth": 10,
      "startDay": 8,
      "endMonth": 8,
      "endDay": 6
    }
  ],
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "personalProfilePlayStoreMode": "blockedApps",
  "personalProfilePersonalApplications": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required",
  "workProfilePasswordRequireUnlock": "daily"
}
```




