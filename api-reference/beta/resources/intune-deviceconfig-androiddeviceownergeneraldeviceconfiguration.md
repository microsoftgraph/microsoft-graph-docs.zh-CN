---
title: androidDeviceOwnerGeneralDeviceConfiguration 资源类型
description: 本主题提供由 androidDeviceOwnerGeneralDeviceConfiguration 资源公开的已声明方法、属性和关系的说明。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da46dd2a062ee12b1dfc12272711489212ad843c
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630875"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>androidDeviceOwnerGeneralDeviceConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

本主题提供由 androidDeviceOwnerGeneralDeviceConfiguration 资源公开的已声明方法、属性和关系的说明。


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 androidDeviceOwnerGeneralDeviceConfigurations](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 集合|列出 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象的属性和关系。|
|[获取 androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|读取 [androidDeviceOwnerGeneralDeviceConfiguration 对象的属性和](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 关系。|
|[创建 androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|创建新的 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象。|
|[删除 androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|无|删除 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)。|
|[更新 androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|更新 [androidDeviceOwnerGeneralDeviceConfiguration 对象](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持分配范围标记。 当此值为 false 且实体对范围用户不可见时，不允许分配给 ScopeTags 属性。 这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的操作系统版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|azureAdSharedDeviceDataClearApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|在 AAD 共享设备模式下全局注销期间将清除其数据的托管应用列表。 该集合最多可包含 500 个元素。|
|accountsBlockModification|Boolean|指示是否禁用添加或删除帐户。|
|appsAllowInstallFromUnknownSources|Boolean|指示是否允许用户启用未知源设置。|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|指示应用自动更新策略的值。 可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|指示运行时权限请求的权限策略（如果没有为应用专门定义权限）。 可能的值是：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。|
|appsRecommendSkippingFirstUseHints|Boolean|是否推荐所有应用跳过他们可能会添加的任何首次使用提示。|
|bluetoothBlockConfiguration|Boolean|指示是否阻止用户配置蓝牙。|
|bluetoothBlockContactSharing|Boolean|指示是否阻止用户通过蓝牙共享联系人。|
|cameraBlocked|Boolean|指示是否禁用相机的使用。|
|cellularBlockWiFiTethering|Boolean|指示是否阻止 Wi-Fi 网络共享。|
|certificateCredentialConfigurationDisabled|Boolean|指示是否阻止用户进行任何证书凭据配置。|
|crossProfilePoliciesAllowCopyPaste|Boolean|指示从一个配置文件复制的文本是否 (个人) 复制的文本是否可以粘贴到另一个配置文件中。|
|crossProfilePoliciesAllowDataSharing|[androidDeviceOwnerCrossProfileDataSharing](../resources/intune-deviceconfig-androiddeviceownercrossprofiledatasharing.md)|指示一个配置文件的数据 (配置文件或工作) 配置文件中的应用共享。 可取值为：`notConfigured`、`crossProfileDataSharingBlocked`、`dataSharingFromWorkToPersonalBlocked`、`crossProfileDataSharingAllowed`、`unkownFutureValue`。|
|crossProfilePoliciesShowWorkContactsInPersonalProfile|Boolean|指示存储在工作配置文件中的联系人是否显示在个人配置文件联系人搜索/传入呼叫中。|
|microsoftLauncherConfigurationEnabled|Boolean|指示是否要配置 Microsoft 启动器。|
|microsoftLauncherCustomWallpaperEnabled|Boolean|指示是否在目标设备上配置墙纸。|
|microsoftLauncherCustomWallpaperImageUrl|String|指示要用作目标设备上墙纸的图像文件的 URL。|
|microsoftLauncherCustomWallpaperAllowUserModification|Boolean|指示用户是否可以修改墙纸以个性化设置其设备。|
|microsoftLauncherFeedEnabled|Boolean|指示是否要在设备上启用启动器源。|
|microsoftLauncherFeedAllowUserModification|Boolean|指示用户是否可以在设备上修改启动器源。|
|microsoftLauncherDockPresenceConfiguration|[microsoftLauncherDockPresence](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|指示是否要配置设备扩展坞。 可能的值是：`notConfigured`、`show`、`hide`、`disabled`。|
|microsoftLauncherDockPresenceAllowUserModification|Boolean|指示用户是否可以在设备上修改设备扩展坞配置。|
|microsoftLauncherSearchBarPlacementConfiguration|[microsoftLauncherSearchBarPlacement](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|指示设备上搜索栏放置的配置。 可取值为：`notConfigured`、`top`、`bottom`、`hide`。|
|enrollmentProfile|[androidDeviceOwnerEnrollmentProfileType](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|指示要配置的注册配置文件。 可取值为：`notConfigured`、`dedicatedDevice`、`fullyManaged`。|
|dataRoamingBlocked|Boolean|指示是否阻止用户进行数据漫游。|
|dateTimeConfigurationBlocked|Boolean|指示是否阻止用户手动更改设备上的日期或时间|
|factoryResetDeviceAdministratorEmails|字符串集合|在设备恢复出厂设置后进行身份验证所需的 Google 帐户电子邮件列表，才能进行设置。|
|factoryResetBlocked|Boolean|指示设置中的恢复出厂设置选项是否已禁用。|
|globalProxy|[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|直接使用主机、端口和排除的主机设置代理。|
|googleAccountsBlocked|Boolean|指示是否将阻止 Google 帐户。|
|kioskCustomizationDeviceSettingsBlocked|Boolean|指示用户是否可以在展台模式下访问设备的"设置"应用。|
|kioskCustomizationPowerButtonActionsBlocked|Boolean|当用户长按展台模式下设备的电源按钮时是否显示电源菜单。|
|kioskCustomizationStatusBar|[androidDeviceOwnerKioskCustomizationStatusBar](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|指示在展台模式下是否禁用系统信息和通知。 可取值为：`notConfigured`、`notificationsAndSystemInfoEnabled`、`systemInfoOnly`。|
|kioskCustomizationSystemErrorWarnings|Boolean|指示崩溃或无响应应用的系统错误对话框是否在展台模式下显示。|
|kioskCustomizationSystemNavigation|[androidDeviceOwnerKioskCustomizationSystemNavigation](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|指示在展台模式下启用的导航功能。 可取值为：`notConfigured`、`navigationEnabled`、`homeButtonOnly`。|
|kioskModeScreenSaverConfigurationEnabled|Boolean|是否在展台模式下启用屏幕保护程序模式。|
|kioskModeScreenSaverImageUrl|String|将在展台模式下作为设备的屏幕保护程序的图像的 URL。|
|kioskModeScreenSaverDisplayTimeInSeconds|Int32|设备在展台模式下显示屏幕保护程序所等待的秒数。 有效值为 0 到 9999999|
|kioskModeScreenSaverStartDelayInSeconds|Int32|在展台模式下显示屏幕保护程序之前，设备需要处于非活动状态的秒数。 有效值为 1 到 9999999|
|kioskModeScreenSaverDetectMediaDisabled|Boolean|如果在展台模式下播放音频/视频，设备屏幕是否应该显示屏幕保护程序。|
|kioskModeApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|设备在展台模式下时将显示的托管应用列表。 该集合最多可包含 500 个元素。|
|kioskModeWallpaperUrl|String|设备在展台模式下时用于墙纸的可公开访问图像的 URL。|
|kioskModeExitCode|String|退出代码，以允许用户在设备进入展台模式时从展台模式下进行转义。|
|kioskModeVirtualHomeButtonEnabled|Boolean|设备在展台模式下时是否显示虚拟主页按钮。|
|kioskModeVirtualHomeButtonType|[androidDeviceOwnerVirtualHomeButtonType](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|指示虚拟主页按钮是向上轻扫"开始"按钮还是浮动"主页"按钮。 可取值为：`notConfigured`、`swipeUp`、`floating`。|
|kioskModeBluetoothConfigurationEnabled|Boolean|是否允许用户在展台模式下配置Bluetooth设置。|
|kioskModeWiFiConfigurationEnabled|Boolean|是否允许用户在展台模式下Wi-Fi自定义设置。|
|kioskModeFlashlightConfigurationEnabled|Boolean|是否允许用户在展台模式下使用网亭。|
|kioskModeMediaVolumeConfigurationEnabled|Boolean|是否允许用户在展台模式下更改媒体卷。|
|kioskModeShowDeviceInfo|Boolean|是否允许用户访问基本设备信息。|
|kioskModeManagedSettingsEntryDisabled|Boolean|是否在展台模式下在托管主屏幕上显示托管设置入口点。|
|kioskModeDebugMenuEasyAccessEnabled|Boolean|是否允许用户在展台模式下轻松访问调试菜单。|
|kioskModeShowAppNotificationBadge|Boolean|是否在展台模式下显示应用程序通知锁屏提醒。|
|kioskModeScreenOrientation|[androidDeviceOwnerKioskModeScreenOrientation](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|展台模式下托管主屏幕的屏幕方向配置。 可能的值是：`notConfigured`、`portrait`、`landscape`、`autoRotate`。|
|kioskModeIconSize|[androidDeviceOwnerKioskModeIconSize](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|展台模式下托管主屏幕的图标大小配置。 可取值为：`notConfigured`、`smallest`、`small`、`regular`、`large`、`largest`。|
|kioskModeFolderIcon|[androidDeviceOwnerKioskModeFolderIcon](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|展台模式下托管主屏幕的文件夹图标配置。 可取值为：`notConfigured`、`darkSquare`、`darkCircle`、`lightSquare`、`lightCircle`。|
|kioskModeWifiAllowedSsids|String collection|用户可以在展台模式下配置的受限 WIFI SS ID 集。 该集合最多可包含 500 个元素。|
|kioskModeAppOrderEnabled|Boolean|是否在展台模式下启用应用排序。|
|kioskModeAppsInFolderOrderedByName|Boolean|是否在展台模式下对文件夹中的应用程序进行字母顺序排序。|
|kioskModeGridHeight|Int32|在展台模式下启用应用排序的托管主屏幕网格的行数。 有效值为 1 到 9999999|
|kioskModeGridWidth|Int32|在展台模式下启用应用排序的托管主屏幕网格的列数。 有效值为 1 到 9999999|
|kioskModeLockHomeScreen|Boolean|是否在展台模式下向最终用户锁定主屏幕。|
|kioskModeManagedFolders|[androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md) 集合|展台模式下设备的托管文件夹列表。 该集合最多可包含 500 个元素。|
|kioskModeAppPositions|[androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md) 集合|展台模式托管主屏幕上的项目排序。 该集合最多可包含 500 个元素。|
|kioskModeManagedHomeScreenAutoSignout|Boolean|托管主屏幕处于非活动状态后是否自动注销 M分屏和共享设备模式应用程序。|
|kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds|Int32|在用户自动将其从托管主屏幕中退出之前向用户发出通知的秒数。 有效值为 0 到 9999999|
|kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds|Int32|在自动将用户从托管主屏幕中退出之前，设备处于非活动状态的秒数。 有效值为 0 到 9999999|
|kioskModeManagedHomeScreenPinComplexity|[kioskModeManagedHomeScreenPinComplexity](../resources/intune-deviceconfig-kioskmodemanagedhomescreenpincomplexity.md)|托管主屏幕登录会话的 PIN 的复杂性。 可取值为：`notConfigured`、`simple`、`complex`。|
|kioskModeManagedHomeScreenPinRequired|Boolean|是否要求用户为托管主屏幕的登录会话设置 PIN。|
|kioskModeManagedHomeScreenPinRequiredToResume|Boolean|如果屏幕保护程序已出现托管主屏幕，是否要求用户输入会话 PIN。|
|kioskModeManagedHomeScreenSignInBackground|String|托管主屏幕的登录屏幕的自定义 URL 背景。|
|kioskModeManagedHomeScreenSignInBrandingLogo|String|托管主屏幕的登录屏幕和会话固定页的自定义 URL 品牌徽标。|
|kioskModeManagedHomeScreenSignInEnabled|Boolean|是否显示托管主屏幕的登录屏幕。|
|kioskModeUseManagedHomeScreenApp|[kioskModeType](../resources/intune-deviceconfig-kioskmodetype.md)|是使用单个应用展台模式还是多应用展台模式。 可取值为：`notConfigured`、`singleAppMode`、`multiAppMode`。|
|microphoneForceMute|Boolean|指示是否阻止取消设备上麦克风的静音。|
|networkEscapeHatchAllowed|Boolean|指示设备是否允许在启动时连接到临时网络连接。|
|nfcBlockOutgoingBeam|Boolean|指示是否阻止 NFC 传出光线。|
|passwordBlockKeyguard|Boolean|指示是否禁用了键保护。|
|passwordBlockKeyguardFeatures|[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) 集合|要阻止的设备键保护功能列表。 该集合最多可包含 7 个元素。|
|passwordExpirationDays|Int32|指示密码过期前可以设置密码的时间，并且需要新密码。 有效值为 1 至 365。|
|passwordMinimumLength|Int32|指示设备上所需的密码的最小长度。 有效值为 4 至 16|
|passwordMinimumLetterCharacters|Int32|指示设备密码所需的最小字母字符数。 有效值为 1 到 16|
|passwordMinimumLowerCaseCharacters|Int32|指示设备密码所需的最小小写字符数。 有效值为 1 到 16|
|passwordMinimumNonLetterCharacters|Int32|指示设备密码所需的最少非字母字符数。 有效值为 1 到 16|
|passwordMinimumNumericCharacters|Int32|指示设备密码所需的最少数字字符数。 有效值为 1 到 16|
|passwordMinimumSymbolCharacters|Int32|指示设备密码所需的最少符号字符数。 有效值为 1 到 16|
|passwordMinimumUpperCaseCharacters|Int32|指示设备密码所需的最小大写字母字符数。 有效值为 1 到 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|passwordPreviousPasswordCountToBlock|Int32|指示密码历史记录的长度，用户将无法输入与历史记录中任何密码相同的新密码。 有效值为 0 至 24|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|指示设备上所需的最低密码质量。 可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|指示擦除设备之前用户可以输入错误密码次数。 有效值为 4 至 11|
|playStoreMode|[androidDeviceOwnerPlayStoreMode](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|指示设备的 Play Store 模式。 可取值为：`notConfigured`、`allowList`、`blockList`。|
|screenCaptureBlocked|Boolean|指示是否禁用屏幕截图功能。|
|securityDeveloperSettingsEnabled|Boolean|指示是否允许用户访问开发人员设置，如开发人员选项和设备上的安全启动。|
|securityRequireVerifyApps|Boolean|指示是否需要验证应用。|
|statusBarBlocked|Boolean|指示是否禁用状态栏，包括通知、快速设置和其他屏幕覆盖。|
|stayOnModes|[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) 集合|设备屏幕将保持打开状态的模式列表。 此集合最多可包含 4 个元素。|
|storageAllowUsb|Boolean|指示是否允许 USB 大容量存储。|
|storageBlockExternalMedia|Boolean|指示是否阻止外部媒体。|
|storageBlockUsbFileTransfer|Boolean|指示是否阻止 USB 文件传输。|
|systemUpdateFreezePeriods|[androidDeviceOwnerSystemUpdateFreezePeriod](../resources/intune-deviceconfig-androiddeviceownersystemupdatefreezeperiod.md) 集合|指示延迟系统更新的每年重复时间段。 该集合最多可包含 500 个元素。|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|指示系统更新窗口在午夜后启动的分钟数。 有效值为 0 到 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|指示系统更新窗口在午夜后结束的分钟数。 有效值为 0 到 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|系统更新配置的类型。 可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。|
|systemWindowsBlocked|Boolean|是否阻止 Android 系统提示窗口，如 Toast、手机活动和系统警报。|
|usersBlockAdd|Boolean|指示是否禁用添加用户和配置文件。|
|usersBlockRemove|Boolean|指示是否禁用从设备中删除其他用户。|
|volumeBlockAdjustment|Boolean|指示是否禁用调整主卷。|
|vpnAlwaysOnLockdownMode|Boolean|如果指定了始终启用 VPN 包的名称，是否在断开 VPN 连接时锁定网络流量。|
|vpnAlwaysOnPackageIdentifier|String|将处理始终打开 VPN 连接的应用的 Android 应用包名称。|
|wifiBlockEditConfigurations|Boolean|指示是否阻止用户编辑 wifi 连接设置。|
|wifiBlockEditPolicyDefinedConfigurations|Boolean|指示是否阻止用户仅编辑策略定义的网络。|
|personalProfileAppsAllowInstallFromUnknownSources|Boolean|指示用户是否可以在个人配置文件上安装来自未知源的应用。|
|personalProfileCameraBlocked|Boolean|指示是否禁止在个人配置文件上使用相机。|
|personalProfileScreenCaptureBlocked|Boolean|指示是否禁用在个人配置文件上拍摄屏幕截图的功能。|
|personalProfilePlayStoreMode|[personalProfilePersonalPlayStoreMode](../resources/intune-deviceconfig-personalprofilepersonalplaystoremode.md)|与 PersonalProfilePersonalApplications 一起用于控制如何允许或阻止个人配置文件中的应用程序。 可取值为：`notConfigured`、`blockedApps`、`allowedApps`。|
|personalProfilePersonalApplications|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|应用于个人配置文件中的应用程序的策略。 该集合最多可包含 500 个元素。|
|workProfilePasswordExpirationDays|Int32|指示工作配置文件密码在过期之前可以设置的天数，并且需要新密码。 有效值为 1 至 365。|
|workProfilePasswordMinimumLength|Int32|指示工作配置文件密码的最小长度。 有效值为 4 至 16|
|workProfilePasswordMinimumNumericCharacters|Int32|指示工作配置文件密码所需的最少数字字符数。 有效值为 1 到 16|
|workProfilePasswordMinimumNonLetterCharacters|Int32|指示工作配置文件密码所需的最少非字母字符数。 有效值为 1 到 16|
|workProfilePasswordMinimumLetterCharacters|Int32|指示工作配置文件密码所需的最小字母字符数。 有效值为 1 到 16|
|workProfilePasswordMinimumLowerCaseCharacters|Int32|指示工作配置文件密码所需的最小小写字符数。 有效值为 1 到 16|
|workProfilePasswordMinimumUpperCaseCharacters|Int32|指示工作配置文件密码所需的最小大写字母字符数。 有效值为 1 到 16|
|workProfilePasswordMinimumSymbolCharacters|Int32|指示工作配置文件密码所需的最少符号字符数。 有效值为 1 到 16|
|workProfilePasswordPreviousPasswordCountToBlock|Int32|指示工作配置文件密码历史记录的长度，用户将无法输入与历史记录中任何密码相同的新密码。 有效值为 0 至 24|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|指示擦除设备之前，用户可以输入不正确的工作配置文件密码次数。 有效值为 4 至 11|
|workProfilePasswordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|指示工作配置文件密码所需的最低密码质量。 可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "azureAdSharedDeviceDataClearApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "String",
  "appsDefaultPermissionPolicy": "String",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "crossProfilePoliciesAllowCopyPaste": true,
  "crossProfilePoliciesAllowDataSharing": "String",
  "crossProfilePoliciesShowWorkContactsInPersonalProfile": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "String",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "String",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "String",
  "enrollmentProfile": "String",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "String"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "String"
  },
  "googleAccountsBlocked": true,
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "String",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "String",
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "String",
  "kioskModeScreenSaverDisplayTimeInSeconds": 1024,
  "kioskModeScreenSaverStartDelayInSeconds": 1024,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "kioskModeWallpaperUrl": "String",
  "kioskModeExitCode": "String",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "String",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "String",
  "kioskModeIconSize": "String",
  "kioskModeFolderIcon": "String",
  "kioskModeWifiAllowedSsids": [
    "String"
  ],
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 1024,
  "kioskModeGridWidth": 1024,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "String",
      "folderIdentifier": "String",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "String",
          "link": "String"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 1024,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "String",
        "link": "String"
      }
    }
  ],
  "kioskModeManagedHomeScreenAutoSignout": true,
  "kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds": 1024,
  "kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds": 1024,
  "kioskModeManagedHomeScreenPinComplexity": "String",
  "kioskModeManagedHomeScreenPinRequired": true,
  "kioskModeManagedHomeScreenPinRequiredToResume": true,
  "kioskModeManagedHomeScreenSignInBackground": "String",
  "kioskModeManagedHomeScreenSignInBrandingLogo": "String",
  "kioskModeManagedHomeScreenSignInEnabled": true,
  "kioskModeUseManagedHomeScreenApp": "String",
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "String"
  ],
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumLetterCharacters": 1024,
  "passwordMinimumLowerCaseCharacters": 1024,
  "passwordMinimumNonLetterCharacters": 1024,
  "passwordMinimumNumericCharacters": 1024,
  "passwordMinimumSymbolCharacters": 1024,
  "passwordMinimumUpperCaseCharacters": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordCountToBlock": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "playStoreMode": "String",
  "screenCaptureBlocked": true,
  "securityDeveloperSettingsEnabled": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "String"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateFreezePeriods": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerSystemUpdateFreezePeriod",
      "startMonth": 1024,
      "startDay": 1024,
      "endMonth": 1024,
      "endDay": 1024
    }
  ],
  "systemUpdateWindowStartMinutesAfterMidnight": 1024,
  "systemUpdateWindowEndMinutesAfterMidnight": 1024,
  "systemUpdateInstallType": "String",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "String",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "personalProfilePlayStoreMode": "String",
  "personalProfilePersonalApplications": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "workProfilePasswordExpirationDays": 1024,
  "workProfilePasswordMinimumLength": 1024,
  "workProfilePasswordMinimumNumericCharacters": 1024,
  "workProfilePasswordMinimumNonLetterCharacters": 1024,
  "workProfilePasswordMinimumLetterCharacters": 1024,
  "workProfilePasswordMinimumLowerCaseCharacters": 1024,
  "workProfilePasswordMinimumUpperCaseCharacters": 1024,
  "workProfilePasswordMinimumSymbolCharacters": 1024,
  "workProfilePasswordPreviousPasswordCountToBlock": 1024,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 1024,
  "workProfilePasswordRequiredType": "String"
}
```




