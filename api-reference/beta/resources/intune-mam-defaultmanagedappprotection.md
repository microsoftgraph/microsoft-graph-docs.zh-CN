---
title: defaultManagedAppProtection 资源类型
description: 用于为 TargetedManagedAppProtection 策略未针对的所有用户配置指定的一组应用的详细管理设置的策略。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 907a313e9a5dd399ece3deec2be171b0a87e4713
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849243"
---
# <a name="defaultmanagedappprotection-resource-type"></a>defaultManagedAppProtection 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

用于为 TargetedManagedAppProtection 策略未针对的所有用户配置指定的一组应用的详细管理设置的策略。

继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List defaultManagedAppProtections](../api/intune-mam-defaultmanagedappprotection-list.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 集合|列出 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的属性和关系。|
|[Get defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-get.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|读取 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的属性和关系。|
|[Create defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-create.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|创建新的 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。|
|[Delete defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-delete.md)|无|删除 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)。|
|[Update defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-update.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|更新 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|策略显示名称。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|description|String|策略的说明。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|String|实体的键。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|实体的版本。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|Duration|设备未连接到 Internet 时在该时间段后检查访问权限。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOnlineBeforeAccessCheck|Duration|设备连接到 Internet 时在该时间段后检查访问权限。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|允许传输其中的数据的源。 继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`allApps`、`managedApps`、`none`。|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|允许向其传输数据的目标。 继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`allApps`、`managedApps`、`none`。|
|organizationalCredentialsRequired|Boolean|指示是否需要组织凭据才能使用应用。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|可以在托管设备上的应用之间共享剪贴板的级别。 继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。|
|dataBackupBlocked|Boolean|指示是否阻止备份托管应用的数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|deviceComplianceRequired|Boolean|指示是否需要设备符合性。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|managedBrowserToOpenLinksRequired|Boolean|指示是否应在托管浏览器应用中打开 Internet 链接。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|saveAsBlocked|Boolean|指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duration|在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinRequired|Boolean|指示是否需要应用级 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumPinRetries|Int32|最大不正确的 pin 重试次数之前阻止或之前托管的应用程序。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|simplePinBlocked|Boolean|指示是否阻止 simplePin。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumPinLength|Int32|PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|PinRequired 设置为 True 时可用于应用级 PIN 的字符集。 继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`numeric`、`alphanumericAndSymbol`。|
|periodBeforePinReset|Duration|PinRequired 设置为 True 时，在此时间段之后必须重置所有级别的 PIN。
 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合|用户可能存储托管数据的数据存储位置。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|contactSyncBlocked|Boolean|指示联系人是否可以同步到用户的设备。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|printBlocked|Boolean|指示是否允许从托管应用进行打印。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|fingerprintBlocked|Boolean|指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Boolean|指示如果设置了设备 PIN，是否需要使用应用 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredOsVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningOsVersion|String|低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredAppVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningAppVersion|String|低于指定版本的版本将导致托管应用出现警告消息。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeOsVersion|字符串|小于或等于指定的版本将擦除托管应用程序和关联的公司数据的版本。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeAppVersion|字符串|小于或等于指定的版本将擦除托管应用程序和关联的公司数据的版本。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管的应用程序行为，阻止或擦除时也根设备, 或 jailbroken，如果 DeviceComplianceRequired 设置为 true。 继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`block`、`wipe`。|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管的应用程序行为，或者是阻止或擦除，基于最大数量的不正确的 pin 重试次数。 继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`block`、`wipe`。|
|pinRequiredInsteadOfBiometricTimeout|Duration|以分钟为单位的而不是从[managedAppProtection](../resources/intune-mam-managedappprotection.md)非生物密码继承应用程序 pin 超时|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|应该用于托管应用中的数据的加密类型。 (仅 iOS)。 可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。|
|screenCaptureBlocked|Boolean|指示是否阻止屏幕截图。 （仅限 Android）|
|encryptAppData|Boolean|指示是否应加密托管应用数据。 （仅限 Android）|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|启用此设置后，如果启用设备加密，则禁用应用程序级别的加密。 （仅限 Android）|
|minimumRequiredSdkVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 (仅适用于 iOS)|
|customSettings|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|要发送给受影响用户的一组字符串键和字符串值对，不被此服务改变|
|deployedAppCount|Int32|当前策略部署到的应用的计数。|
|minimumRequiredPatchVersion|String|定义用户可以拥有的最早的必需 Android 安全修补程序级别，用户可借此获得对应用的安全访问权限。
 （仅限 Android）|
|minimumWarningPatchVersion|String|定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。 （仅限 Android）|
|exemptedAppProtocols|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|此列表中的 iOS 应用程序将从策略中排除和都将能够从托管的应用程序接收数据。 (仅适用于 iOS)|
|exemptedAppPackages|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|此列表中的 android 应用程序包将从策略中排除并且能够接收从托管的应用程序的数据。 （仅限 Android）|
|faceIdBlocked|Boolean|指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 pin。 (仅适用于 iOS)|
|minimumWipeSdkVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。|
|minimumWipePatchVersion|字符串|托管的应用程序和关联的公司数据，将擦除 android 安全修补程序级别小于或等于指定值。 （仅限 Android）|
|allowedIosDeviceModels|字符串|作为字符串的托管的应用程序，以允许的设备模型的分号分隔列表。 (仅适用于 iOS)|
|appActionIfIosDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管的应用程序行为，阻止或擦除，如果不允许指定的设备模型。 (仅 iOS)。 可取值为：`block`、`wipe`。|
|allowedAndroidDeviceManufacturers|字符串|作为字符串的托管的应用程序，以允许的设备制造商的分号分隔列表。 （仅限 Android）|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管的应用程序行为，阻止或擦除，如果不允许指定的设备制造商。 (仅 android)。 可取值为：`block`、`wipe`。|
|thirdPartyKeyboardsBlocked|布尔|如果第三方键盘允许访问托管的应用程序时，定义。 (仅适用于 iOS)|
|filterOpenInToOnlyManagedApps|布尔|如果到所选的文件共享位置从托管的应用程序支持打开项操作，定义。 此设置仅适用于 AllowedOutboundDataTransferDestinations 设置为 ManagedApps 并且 DisableProtectionOfManagedOutboundOpenInData 设置为 False。 (仅适用于 iOS)|
|disableProtectionOfManagedOutboundOpenInData|布尔|禁用传输到 IOS OpenIn 选项通过其他应用程序的数据保护。 此设置只允许为 True 时 AllowedOutboundDataTransferDestinations 设置为 ManagedApps。 (仅适用于 iOS)|
|protectInboundDataFromUnknownSources|布尔|从未知源保护传入的数据。 此设置只允许为 True 时 AllowedInboundDataTransferSources 设置为 AllApps。 (仅适用于 iOS)|

## <a name="relationships"></a>Relationships
|关系|类型|说明|
|:---|:---|:---|
|apps|[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合|策略部署到的应用的列表。|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|配置的部署摘要的导航属性。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": true,
  "maximumPinRetries": 1024,
  "simplePinBlocked": true,
  "minimumPinLength": 1024,
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "minimumWipeOsVersion": "String",
  "minimumWipeAppVersion": "String",
  "appActionIfDeviceComplianceRequired": "String",
  "appActionIfMaximumPinRetriesExceeded": "String",
  "pinRequiredInsteadOfBiometricTimeout": "String (duration)",
  "appDataEncryptionType": "String",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "minimumRequiredPatchVersion": "String",
  "minimumWarningPatchVersion": "String",
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "String",
  "minimumWipePatchVersion": "String",
  "allowedIosDeviceModels": "String",
  "appActionIfIosDeviceModelNotAllowed": "String",
  "allowedAndroidDeviceManufacturers": "String",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true
}
```





