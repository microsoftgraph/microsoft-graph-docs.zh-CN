---
title: 创建 androidDeviceOwnerGeneralDeviceConfiguration
description: 创建新的 androidDeviceOwnerGeneralDeviceConfiguration 对象。
author: tfitzmac
ms.openlocfilehash: 404233f1c9eba62021b5ba019a9f3bb049c272c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333256"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a>创建 androidDeviceOwnerGeneralDeviceConfiguration

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

创建新的[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。
## <a name="prerequisites"></a>先决条件
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。


|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

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
|授权|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 androidDeviceOwnerGeneralDeviceConfiguration 对象的 JSON 表示形式。

下表显示时创建 androidDeviceOwnerGeneralDeviceConfiguration 所需的属性。

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
|bluetoothBlockConfiguration|Boolean|指示阻止用户与配置蓝牙。|
|bluetoothBlockContactSharing|Boolean|指示阻止用户与共享通过蓝牙的联系人。|
|cameraBlocked|Boolean|指示禁用照相机使用。|
|cellularBlockWiFiTethering|Boolean|指示是否阻止 Wi-Fi 网络共享。|
|dataRoamingBlocked|Boolean|指示阻止用户与漫游数据。|
|dateTimeConfigurationBlocked|Boolean|指示阻止用户手动更改日期或设备上的时间|
|factoryResetDeviceAdministratorEmails|String 集合|需要进行身份验证后设备出厂重置之前可以设置它的 Google 帐户电子邮件的列表。|
|factoryResetBlocked|Boolean|指示禁用中设置的出厂重置选项。|
|kioskModeApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|将以展台模式，该设备时显示的托管应用程序的列表。 该集合最多可包含 500 个元素。|
|microphoneForceMute|Boolean|指示阻止 unmuting 麦克风设备上。|
|networkEscapeHatchAllowed|Boolean|指示将允许设备连接到在启动时的临时网络连接。|
|nfcBlockOutgoingBeam|Boolean|指示阻止 NFC 传出无线发送。|
|passwordBlockKeyguard|Boolean|指示禁用 keyguard。|
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
|stayOnModes|[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)集合|在其中设备的显示将保持电模式的列表。 4 元素的最多可以包含此集合。 可取值为：`notConfigured`、`ac`、`usb`、`wireless`。|
|storageAllowUsb|Boolean|指示允许 USB 大容量存储。|
|storageBlockExternalMedia|Boolean|指示阻止外部介质。|
|storageBlockUsbFileTransfer|Boolean|指示阻止 USB 文件传输。|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|指示系统更新窗口启动的午夜后的分钟数。 0 到 1440 之间的有效值|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|指示系统更新窗口结束的午夜后的分钟数。 0 到 1440 之间的有效值|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|系统更新配置的类型。 可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。|
|usersBlockAdd|Boolean|指示将用户和配置文件添加被禁用。|
|usersBlockRemove|Boolean|指示禁用从设备中删除其他用户。|
|volumeBlockAdjustment|Boolean|指示调整主音量被禁用。|
|wifiBlockEditConfigurations|Boolean|指示阻止用户编辑 wifi 连接设置。|
|wifiBlockEditPolicyDefinedConfigurations|Boolean|指示阻止用户编辑只策略定义的网络。|



## <a name="response"></a>响应
如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2156

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2264

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```





