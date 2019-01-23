---
title: androidDeviceOwnerGeneralDeviceConfiguration 资源类型
description: 本主题提供的声明方法属性和公开 androidDeviceOwnerGeneralDeviceConfiguration 资源的关系的说明。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ac403bd13091a9db61b7f27462caecf6934b452
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403747"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>androidDeviceOwnerGeneralDeviceConfiguration 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

本主题提供的声明方法属性和公开 androidDeviceOwnerGeneralDeviceConfiguration 资源的关系的说明。


继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 androidDeviceOwnerGeneralDeviceConfigurations](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)集合|列出属性和[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象之间的关系。|
|[获取 androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|读取属性和[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的关系。|
|[创建 androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|创建新的[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。|
|[删除 androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|无|删除[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)。|
|[更新 androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|更新[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String 集合|此实体实例范围标记的列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础的设备配置支持分配的范围标记。 此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。 这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|accountsBlockModification|Boolean|指示添加或删除帐户被禁用。|
|appsAllowInstallFromUnknownSources|Boolean|指示允许用户启用到未知源设置。|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|指示应用程序自动更新策略的值。 可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|如果一个未定义应用程序专门，指示运行时权限请求的权限策略。 可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。|
|appsRecommendSkippingFirstUseHints|Boolean|建议所有应用程序，请跳过它们可能已添加任何首次使用提示。|
|bluetoothBlockConfiguration|Boolean|指示阻止用户与配置蓝牙。|
|bluetoothBlockContactSharing|Boolean|指示阻止用户与共享通过蓝牙的联系人。|
|cameraBlocked|Boolean|指示禁用照相机使用。|
|cellularBlockWiFiTethering|Boolean|指示是否阻止 Wi-Fi 网络共享。|
|dataRoamingBlocked|Boolean|指示阻止用户与漫游数据。|
|dateTimeConfigurationBlocked|Boolean|指示阻止用户手动更改日期或设备上的时间|
|factoryResetDeviceAdministratorEmails|String 集合|需要进行身份验证后设备出厂重置之前可以设置它的 Google 帐户电子邮件的列表。|
|factoryResetBlocked|Boolean|指示禁用中设置的出厂重置选项。|
|kioskModeApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|将以展台模式，该设备时显示的托管应用程序的列表。 该集合最多可包含 500 个元素。|
|kioskModeWallpaperUrl|String|要以展台模式设备时，可用于墙纸可公开访问图像 URL。|
|kioskModeExitCode|String|退出代码以允许用户以展台模式设备时转义从展台模式。|
|kioskModeVirtualHomeButtonEnabled|Boolean|是否以展台模式设备时显示虚拟主页按钮。|
|microphoneForceMute|Boolean|指示阻止 unmuting 麦克风设备上。|
|networkEscapeHatchAllowed|Boolean|指示将允许设备连接到在启动时的临时网络连接。|
|nfcBlockOutgoingBeam|Boolean|指示阻止 NFC 传出无线发送。|
|passwordBlockKeyguard|Boolean|指示禁用 keyguard。|
|passwordBlockKeyguardFeatures|[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)集合|要阻止的设备 keyguard 功能的列表。 该集合最多可包含 7 个元素。|
|passwordExpirationDays|Int32|指示该帐户到期和新密码需要之前，可以为设置密码以秒为单位的时间量。 有效值为 1 至 365。|
|passwordMinimumLength|Int32|指示在设备上所需的密码的最小长度。 有效值为 4 至 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时前的不活动毫秒。|
|passwordPreviousPasswordCountToBlock|Int32|指示密码历史记录，其中用户将无法输入的历史记录中任何密码相同的新密码的长度。 有效值为 0 至 24|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|指示在设备上所需的最短密码质量。 可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|指示擦除设备之前，用户可以输入密码不正确的次数。 有效值为 4 至 11|
|safeBootBlocked|Boolean|指示重新启动设备插入安全启动的被禁用。|
|screenCaptureBlocked|Boolean|指示禁用的功能，才能屏幕截图。|
|securityAllowDebuggingFeatures|Boolean|指示阻止用户启用设备上的调试功能。|
|securityRequireVerifyApps|Boolean|指示是否验证应用程序，则需要。|
|statusBarBlocked|Boolean|指示是否或状态栏已禁用，包括通知、 快速设置和其他屏幕覆盖。|
|stayOnModes|[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)集合|在其中设备的显示将保持电模式的列表。 4 元素的最多可以包含此集合。|
|storageAllowUsb|Boolean|指示允许 USB 大容量存储。|
|storageBlockExternalMedia|Boolean|指示阻止外部介质。|
|storageBlockUsbFileTransfer|Boolean|指示阻止 USB 文件传输。|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|指示系统更新窗口启动的午夜后的分钟数。 0 到 1440 之间的有效值|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|指示系统更新窗口结束的午夜后的分钟数。 0 到 1440 之间的有效值|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|系统更新配置的类型。 可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。|
|systemWindowsBlocked|Boolean|阻止 Android 系统提示窗口中的，如 toast、 电话活动和系统通知。|
|usersBlockAdd|Boolean|指示将用户和配置文件添加被禁用。|
|usersBlockRemove|Boolean|指示禁用从设备中删除其他用户。|
|volumeBlockAdjustment|Boolean|指示调整主音量被禁用。|
|vpnAlwaysOnPackageIdentifier|String|在 android 应用包将用来处理始终打开的 VPN 连接的应用程序的名称。|
|vpnAlwaysOnLockdownMode|Boolean|如果始终在 VPN 包名称指定了，锁定网络流量时断开连接的 VPN。|
|wifiBlockEditConfigurations|Boolean|指示阻止用户编辑 wifi 连接设置。|
|wifiBlockEditPolicyDefinedConfigurations|Boolean|指示阻止用户编辑只策略定义的网络。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

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
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "String"
  ],
  "factoryResetBlocked": true,
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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "String"
  ],
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordCountToBlock": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
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




