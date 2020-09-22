---
title: 更新 androidDeviceOwnerGeneralDeviceConfiguration
description: 更新 androidDeviceOwnerGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10b53ccaa538b4a357684d7755c4f37c634d72cb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48005983"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a>更新 androidDeviceOwnerGeneralDeviceConfiguration

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象的 JSON 表示形式。

下表显示创建 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持作用域标记的分配。 如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。 这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|适用于此策略的操作系统版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|accountsBlockModification|Boolean|指示是否禁用添加或删除帐户。|
|appsAllowInstallFromUnknownSources|Boolean|指示是否允许用户启用 "未知源" 设置。|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|指示应用程序自动更新策略的值。 可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|指示对运行时权限请求的权限策略（如果专门没有为应用程序定义）。 可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。|
|appsRecommendSkippingFirstUseHints|Boolean|是否建议所有应用都将跳过他们可能已添加的任何首次使用提示。|
|bluetoothBlockConfiguration|Boolean|指示是否阻止用户配置蓝牙。|
|bluetoothBlockContactSharing|Boolean|指示是否阻止用户通过蓝牙共享联系人。|
|cameraBlocked|Boolean|指示是否禁用相机的使用。|
|cellularBlockWiFiTethering|Boolean|指示是否阻止 Wi-Fi 网络共享。|
|certificateCredentialConfigurationDisabled|Boolean|指示是否阻止来自任何证书凭据配置的用户。|
|microsoftLauncherConfigurationEnabled|Boolean|指示是否要配置 Microsoft 启动器。|
|microsoftLauncherCustomWallpaperEnabled|Boolean|指示是否在目标设备上配置墙纸。|
|microsoftLauncherCustomWallpaperImageUrl|String|指示用作目标设备墙纸的图像文件的 URL。|
|microsoftLauncherCustomWallpaperAllowUserModification|Boolean|指示用户是否可以修改墙纸以个性化设置其设备。|
|microsoftLauncherFeedEnabled|Boolean|指示是否要在设备上启用启动器源。|
|microsoftLauncherFeedAllowUserModification|Boolean|指示用户是否可以修改设备上的启动器源。|
|microsoftLauncherDockPresenceConfiguration|[microsoftLauncherDockPresence](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|指示是否要配置设备停靠。 可取值为：`notConfigured`、`show`、`hide`、`disabled`。|
|microsoftLauncherDockPresenceAllowUserModification|Boolean|指示用户是否可以修改设备上的设备停靠配置。|
|microsoftLauncherSearchBarPlacementConfiguration|[microsoftLauncherSearchBarPlacement](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|指示设备上的搜索栏的布局配置。 可取值为：`notConfigured`、`top`、`bottom`、`hide`。|
|enrollmentProfile|[androidDeviceOwnerEnrollmentProfileType](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|指示要配置的注册配置文件。 可取值为：`notConfigured`、`dedicatedDevice`、`fullyManaged`。|
|dataRoamingBlocked|Boolean|指示是否阻止用户使用数据漫游。|
|dateTimeConfigurationBlocked|Boolean|指示是否阻止用户手动更改设备上的日期或时间|
|factoryResetDeviceAdministratorEmails|String collection|在设备出厂重置之前，将需要进行身份验证的 Google 帐户电子邮件的列表，然后才能对其进行设置。|
|factoryResetBlocked|Boolean|指示是否禁用了 "设置" 中的 "恢复出厂设置" 选项。|
|globalProxy|[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|代理是与主机、端口和已排除的主机直接建立的。|
|googleAccountsBlocked|Boolean|指示是否将阻止 google 帐户。|
|kioskModeScreenSaverConfigurationEnabled|Boolean|是否启用屏幕保护程序模式或不启用展台模式。|
|kioskModeScreenSaverImageUrl|String|将作为展台模式下设备的屏幕保护程序的图像的 URL。|
|kioskModeScreenSaverDisplayTimeInSeconds|Int32|设备将在展台模式下显示屏幕保护程序的秒数。 有效值为0至9999999|
|kioskModeScreenSaverStartDelayInSeconds|Int32|在 Kiosk 模式下显示屏幕保护程序之前设备需要保持非活动状态的秒数。 有效值为1至9999999|
|kioskModeScreenSaverDetectMediaDisabled|Boolean|如果音频/视频在展台模式下播放，则设备屏幕是否应显示屏幕保护程序。|
|kioskModeApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|设备处于展台模式时将显示的托管应用列表。 该集合最多可包含 500 个元素。|
|kioskModeWallpaperUrl|String|在设备处于展台模式时用于墙纸的可公开访问图像的 URL。|
|kioskModeExitCode|String|退出代码，以允许用户在设备处于展台模式时从展台模式中进行转义。|
|kioskModeVirtualHomeButtonEnabled|Boolean|设备处于展台模式时是否显示虚拟 "主页" 按钮。|
|kioskModeVirtualHomeButtonType|[androidDeviceOwnerVirtualHomeButtonType](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|指示虚拟 home 按钮是否为向上轻扫主页按钮或浮动主页按钮。 可取值为：`notConfigured`、`swipeUp`、`floating`。|
|kioskModeBluetoothConfigurationEnabled|Boolean|是否允许用户在展台模式下配置蓝牙设置。|
|kioskModeWiFiConfigurationEnabled|Boolean|是否允许用户在展台模式下配置 Wi-fi 设置。|
|kioskModeFlashlightConfigurationEnabled|Boolean|是否允许用户在展台模式下使用该模式。|
|kioskModeMediaVolumeConfigurationEnabled|Boolean|是否允许用户在展台模式下更改媒体音量。|
|kioskModeShowDeviceInfo|Boolean|是否允许用户访问基本设备信息。|
|kioskModeManagedSettingsEntryDisabled|Boolean|是否在展台模式下在托管的主屏幕上显示托管设置入口点。|
|kioskModeDebugMenuEasyAccessEnabled|Boolean|是否允许用户在展台模式下轻松访问 "调试" 菜单。|
|kioskModeShowAppNotificationBadge|Boolean|是否在展台模式下显示应用程序通知徽章。|
|kioskModeScreenOrientation|[androidDeviceOwnerKioskModeScreenOrientation](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|在展台模式下管理的主屏幕的屏幕方向配置。 可取值为：`notConfigured`、`portrait`、`landscape`、`autoRotate`。|
|kioskModeIconSize|[androidDeviceOwnerKioskModeIconSize](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|在展台模式下，管理的主屏幕的图标大小配置。 可取值为：`notConfigured`、`smallest`、`small`、`regular`、`large`、`largest`。|
|kioskModeFolderIcon|[androidDeviceOwnerKioskModeFolderIcon](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|展台模式下的托管主屏幕的文件夹图标配置。 可取值为：`notConfigured`、`darkSquare`、`darkCircle`、`lightSquare`、`lightCircle`。|
|kioskModeWifiAllowedSsids|String collection|可供用户在展台模式下进行配置的受限制的 WIFI Ssid 集。 该集合最多可包含 500 个元素。|
|microphoneForceMute|Boolean|指示是否阻止观众在设备上的麦克风。|
|networkEscapeHatchAllowed|Boolean|指示在引导时设备是否允许连接到临时网络连接。|
|nfcBlockOutgoingBeam|Boolean|指示是否阻止 NFC 传出横梁。|
|passwordBlockKeyguard|Boolean|指示是否禁用 keyguard。|
|passwordBlockKeyguardFeatures|[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) 集合|要阻止的设备 keyguard 功能的列表。 该集合最多可包含 7 个元素。 可取值为：`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures`。|
|passwordExpirationDays|Int32|指示密码在过期之前可以设置的时间量，并需要新密码。 有效值为 1 至 365。|
|passwordMinimumLength|Int32|指示设备上所需密码的最小长度。 有效值为 4 至 16|
|passwordMinimumLetterCharacters|Int32|指示设备密码所需的字母字符的最小数量。 有效值为1至16|
|passwordMinimumLowerCaseCharacters|Int32|指示设备密码所需的最小小写字符数。 有效值为1至16|
|passwordMinimumNonLetterCharacters|Int32|指示设备密码所需的最小非字母字符数。 有效值为1至16|
|passwordMinimumNumericCharacters|Int32|指示设备密码所需的最小数字字符数。 有效值为1至16|
|passwordMinimumSymbolCharacters|Int32|指示设备密码所需的最小符号字符数。 有效值为1至16|
|passwordMinimumUpperCaseCharacters|Int32|指示设备密码所需的大写字母字符的最小数量。 有效值为1至16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|passwordPreviousPasswordCountToBlock|Int32|指示密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。 有效值为 0 至 24|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|指示设备上所需的最小密码质量。 可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|指示用户在擦除设备之前可以输入不正确密码的次数。 有效值为 4 至 11|
|playStoreMode|[androidDeviceOwnerPlayStoreMode](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|指示设备的播放存储模式。 可取值为：`notConfigured`、`allowList`、`blockList`。|
|safeBootBlocked|Boolean|指示是否禁用重新启动设备到安全启动。|
|screenCaptureBlocked|Boolean|指示是否禁用获取屏幕截图的功能。|
|securityAllowDebuggingFeatures|Boolean|指示是否阻止用户启用设备上的调试功能。|
|securityRequireVerifyApps|Boolean|指示是否需要验证应用。|
|statusBarBlocked|Boolean|指示是否禁用状态栏，包括通知、快速设置和其他屏幕重叠。|
|stayOnModes|[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) 集合|设备的显示将保持开机状态的模式列表。 此集合最多可包含4个元素。 可取值为：`notConfigured`、`ac`、`usb`、`wireless`。|
|storageAllowUsb|Boolean|指示是否允许 USB 大容量存储。|
|storageBlockExternalMedia|Boolean|指示是否阻止外部媒体。|
|storageBlockUsbFileTransfer|Boolean|指示是否阻止 USB 文件传输。|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|指示系统更新窗口午夜后启动的分钟数。 有效值为0至1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|指示系统更新窗口结束后的分钟数。 有效值为0至1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|系统更新配置的类型。 可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。|
|systemWindowsBlocked|Boolean|是否阻止 Android 系统提示符窗口，如 toast、电话活动和系统通知。|
|usersBlockAdd|Boolean|指示是否禁用添加用户和配置文件。|
|usersBlockRemove|Boolean|指示是否禁用从设备中删除其他用户。|
|volumeBlockAdjustment|Boolean|指示是否禁用了调整主音量。|
|vpnAlwaysOnLockdownMode|Boolean|如果指定了 always on VPN 包名称，则在断开 VPN 连接时是否锁定网络流量。|
|vpnAlwaysOnPackageIdentifier|String|将处理永不启用 VPN 连接的应用程序的 Android 应用程序包名称。|
|wifiBlockEditConfigurations|Boolean|指示是否阻止用户编辑 wifi 连接设置。|
|wifiBlockEditPolicyDefinedConfigurations|Boolean|指示是否阻止用户仅编辑策略定义的网络。|
|personalProfileAppsAllowInstallFromUnknownSources|Boolean|指示用户是否可以在个人配置文件上安装来自未知源的应用程序。|
|personalProfileCameraBlocked|Boolean|指示是否禁用个人配置文件上的摄像头的使用。|
|personalProfileScreenCaptureBlocked|Boolean|指示是否禁用在个人配置文件上采用屏幕截图的功能。|
|workProfilePasswordExpirationDays|Int32|指示工作配置文件密码在过期之前可以设置的天数，并将需要新密码。 有效值为 1 至 365。|
|workProfilePasswordMinimumLength|Int32|指示工作配置文件密码的最小长度。 有效值为 4 至 16|
|workProfilePasswordMinimumNumericCharacters|Int32|指示工作配置文件密码所需的最小数字字符数。 有效值为1至16|
|workProfilePasswordMinimumNonLetterCharacters|Int32|指示工作配置文件密码所需的最小非字母字符数。 有效值为1至16|
|workProfilePasswordMinimumLetterCharacters|Int32|指示工作配置文件密码所需的字母字符的最小数量。 有效值为1至16|
|workProfilePasswordMinimumLowerCaseCharacters|Int32|指示工作配置文件密码所需的最小小写字符数。 有效值为1至16|
|workProfilePasswordMinimumUpperCaseCharacters|Int32|指示工作配置文件密码所需的大写字母字符的最小数量。 有效值为1至16|
|workProfilePasswordMinimumSymbolCharacters|Int32|指示工作配置文件密码所需的最小符号字符数。 有效值为1至16|
|workProfilePasswordPreviousPasswordCountToBlock|Int32|指示工作配置文件密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。 有效值为 0 至 24|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|指示用户在擦除设备之前可以输入不正确的工作配置文件密码的次数。 有效值为 4 至 11|
|workProfilePasswordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|指示工作配置文件密码所需的最小密码质量。 可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。|



## <a name="response"></a>响应
如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 6096

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
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
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
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
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
  "workProfilePasswordRequiredType": "required"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 6268

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
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
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
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
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
  "workProfilePasswordRequiredType": "required"
}
```






