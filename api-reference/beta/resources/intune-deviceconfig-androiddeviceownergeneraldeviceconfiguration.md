---
title: androidDeviceOwnerGeneralDeviceConfiguration 资源类型
description: 本主题提供由 androidDeviceOwnerGeneralDeviceConfiguration 资源公开的已声明方法、属性和关系的说明。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2360d840fd8e2fbb4577ee67839c3557c9aef93d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955713"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>androidDeviceOwnerGeneralDeviceConfiguration 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

本主题提供由 androidDeviceOwnerGeneralDeviceConfiguration 资源公开的已声明方法、属性和关系的说明。


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 androidDeviceOwnerGeneralDeviceConfigurations](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)集合|列出[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的属性和关系。|
|[获取 androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|读取[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的属性和关系。|
|[创建 androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|创建新的[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。|
|[删除 androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|None|删除[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)。|
|[更新 androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|更新[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持作用域标记的分配。 如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。 这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|适用于此策略的操作系统版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
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
|dataRoamingBlocked|Boolean|指示是否阻止用户使用数据漫游。|
|dateTimeConfigurationBlocked|Boolean|指示是否阻止用户手动更改设备上的日期或时间|
|factoryResetDeviceAdministratorEmails|String collection|在设备出厂重置之前，将需要进行身份验证的 Google 帐户电子邮件的列表，然后才能对其进行设置。|
|factoryResetBlocked|Boolean|指示是否禁用了 "设置" 中的 "恢复出厂设置" 选项。|
|globalProxy|[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|代理是与主机、端口和已排除的主机直接建立的。|
|googleAccountsBlocked|Boolean|指示是否将阻止 google 帐户。|
|kioskModeScreenSaverConfigurationEnabled|Boolean|是否启用屏幕保护程序模式或不启用展台模式。|
|kioskModeScreenSaverImageUrl|字符串|将作为展台模式下设备的屏幕保护程序的图像的 URL。|
|kioskModeScreenSaverDisplayTimeInSeconds|Int32|设备将在展台模式下显示屏幕保护程序的秒数。 有效值为0至9999999|
|kioskModeScreenSaverStartDelayInSeconds|Int32|在 Kiosk 模式下显示屏幕保护程序之前设备需要保持非活动状态的秒数。 有效值为1至9999999|
|kioskModeScreenSaverDetectMediaDisabled|Boolean|如果音频/视频在展台模式下播放，则设备屏幕是否应显示屏幕保护程序。|
|kioskModeApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|设备处于展台模式时将显示的托管应用列表。 该集合最多可包含 500 个元素。|
|kioskModeWallpaperUrl|字符串|在设备处于展台模式时用于墙纸的可公开访问图像的 URL。|
|kioskModeExitCode|字符串|退出代码，以允许用户在设备处于展台模式时从展台模式中进行转义。|
|kioskModeVirtualHomeButtonEnabled|Boolean|设备处于展台模式时是否显示虚拟 "主页" 按钮。|
|kioskModeVirtualHomeButtonType|[androidDeviceOwnerVirtualHomeButtonType](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|指示虚拟 home 按钮是否为向上轻扫主页按钮或浮动主页按钮。 可取值为：`notConfigured`、`swipeUp`、`floating`。|
|kioskModeBluetoothConfigurationEnabled|Boolean|是否允许用户在展台模式下配置蓝牙设置。|
|kioskModeWiFiConfigurationEnabled|Boolean|是否允许用户在展台模式下配置 Wi-fi 设置。|
|kioskModeFlashlightConfigurationEnabled|Boolean|是否允许用户在展台模式下使用该模式。|
|kioskModeMediaVolumeConfigurationEnabled|Boolean|是否允许用户在展台模式下更改媒体音量。|
|microphoneForceMute|Boolean|指示是否阻止观众在设备上的麦克风。|
|networkEscapeHatchAllowed|Boolean|指示在引导时设备是否允许连接到临时网络连接。|
|nfcBlockOutgoingBeam|Boolean|指示是否阻止 NFC 传出横梁。|
|passwordBlockKeyguard|Boolean|指示是否禁用 keyguard。|
|passwordBlockKeyguardFeatures|[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)集合|要阻止的设备 keyguard 功能的列表。 该集合最多可包含 7 个元素。|
|passwordExpirationDays|Int32|指示在密码过期之前可以设置密码的时间量（以秒为单位）以及需要新密码的时间（以秒为单位）。 有效值为 1 至 365。|
|passwordMinimumLength|Int32|指示设备上所需密码的最小长度。 有效值为 4 至 16|
|passwordMinimumLetterCharacters|Int32|指示设备密码所需的字母字符的最小数量。 有效值为1至16|
|passwordMinimumLowerCaseCharacters|Int32|指示设备密码所需的最小小写字符数。 有效值为1至16|
|passwordMinimumNonLetterCharacters|Int32|指示设备密码所需的最小非字母字符数。 有效值为1至16|
|passwordMinimumNumericCharacters|Int32|指示设备密码所需的最小数字字符数。 有效值为1至16|
|passwordMinimumSymbolCharacters|Int32|指示设备密码所需的最小符号字符数。 有效值为1至16|
|passwordMinimumUpperCaseCharacters|Int32|指示设备密码所需的最小上限 caseletter 字符数。 有效值为1至16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动时间（毫秒）。|
|passwordPreviousPasswordCountToBlock|Int32|指示密码历史记录的长度，其中用户将不能输入与历史记录中的任何密码相同的新密码。 有效值为 0 至 24|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|指示设备上所需的最小密码质量。 可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|指示用户在擦除设备之前可以输入不正确密码的次数。 有效值为 4 至 11|
|playStoreMode|[androidDeviceOwnerPlayStoreMode](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|指示设备的播放存储模式。 可取值为：`notConfigured`、`allowList`、`blockList`。|
|safeBootBlocked|Boolean|指示是否禁用重新启动设备到安全启动。|
|screenCaptureBlocked|Boolean|指示是否禁用获取屏幕截图的功能。|
|securityAllowDebuggingFeatures|Boolean|指示是否阻止用户启用设备上的调试功能。|
|securityRequireVerifyApps|Boolean|指示是否需要验证应用。|
|statusBarBlocked|Boolean|指示是否禁用状态栏，包括通知、快速设置和其他屏幕重叠。|
|stayOnModes|[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)集合|设备的显示将保持开机状态的模式列表。 此集合最多可包含4个元素。|
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
|vpnAlwaysOnPackageIdentifier|字符串|将处理永不启用 VPN 连接的应用程序的 Android 应用程序包名称。|
|vpnAlwaysOnLockdownMode|Boolean|如果指定了 always on VPN 包名称，则在断开 VPN 连接时是否锁定网络流量。|
|wifiBlockEditConfigurations|Boolean|指示是否阻止用户编辑 wifi 连接设置。|
|wifiBlockEditPolicyDefinedConfigurations|Boolean|指示是否阻止用户仅编辑策略定义的网络。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|按用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
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
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "String"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 1024,
  "systemUpdateWindowEndMinutesAfterMidnight": 1024,
  "systemUpdateInstallType": "String",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "String",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```



