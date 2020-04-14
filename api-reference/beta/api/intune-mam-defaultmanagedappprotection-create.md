---
title: 创建 defaultManagedAppProtection
description: 创建新的 defaultManagedAppProtection 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c0f74866c130ad59d62fe92fb261551cd762fc8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444576"
---
# <a name="create-defaultmanagedappprotection"></a>创建 defaultManagedAppProtection

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 defaultManagedAppProtection 对象的 JSON 表示形式。

下表显示创建 defaultManagedAppProtection 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|策略显示名称。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|description|String|策略的说明。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|roleScopeTagIds|String 集合|此实体实例的范围标记列表。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|字符串|实体的键。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|实体的版本。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|持续时间|设备未连接到 Internet 时在该时间段后检查访问权限。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOnlineBeforeAccessCheck|持续时间|设备连接到 Internet 时在该时间段后检查访问权限。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
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
|maximumPinRetries|Int32|在阻止或擦除托管应用之前，不正确 pin 重试的最大次数。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|simplePinBlocked|Boolean|指示是否阻止 simplePin。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumPinLength|Int32|PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|PinRequired 设置为 True 时可用于应用级 PIN 的字符集。 继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`numeric`、`alphanumericAndSymbol`。|
|periodBeforePinReset|Duration|TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合|用户可能存储托管数据的数据存储位置。 继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。|
|contactSyncBlocked|Boolean|指示联系人是否可以同步到用户的设备。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|printBlocked|Boolean|指示是否允许从托管应用进行打印。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|fingerprintBlocked|Boolean|指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Boolean|指示如果设置了设备 PIN，是否需要使用应用 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredOsVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningOsVersion|String|低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredAppVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningAppVersion|String|低于指定版本的版本将导致托管应用出现警告消息。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeOsVersion|String|小于或等于指定版本的版本将擦除托管应用和关联的公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeAppVersion|String|小于或等于指定版本的版本将擦除托管应用和关联的公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|如果将 DeviceComplianceRequired 设置为 true，则定义在设备为根或已越狱时的托管应用行为（阻止或擦除）。 继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`block`、`wipe`、`warn`。|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|根据最大错误 pin 重试次数定义托管应用行为，即阻止或擦除。 继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`block`、`wipe`、`warn`。|
|pinRequiredInsteadOfBiometricTimeout|持续时间|以分钟为单位的应用程序 pin （而不是从[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)继承的无生物特征密码）超时|
|allowedOutboundClipboardSharingExceptionLength|Int32|指定可以从组织数据和帐户中剪切或复制到任何应用程序的字符数。 此设置将覆盖 AllowedOutboundClipboardSharingLevel 限制。 默认值为 "0" 表示不允许异常。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|notificationRestriction|[managedAppNotificationRestriction](../resources/intune-mam-managedappnotificationrestriction.md)|指定从[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)继承的应用程序通知限制。 可取值为：`allow`、`blockOrganizationalData`、`block`。|
|previousPinBlockCount|Int32|需要 pin 才能与此属性中指定的编号唯一。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|managedBrowser|[managedBrowserType](../resources/intune-mam-managedbrowsertype.md)|指示应在哪个托管浏览器中打开 internet 链接。 继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`notConfigured`、`microsoftEdge`。|
|maximumAllowedDeviceThreatLevel|[managedAppDeviceThreatLevel](../resources/intune-mam-managedappdevicethreatlevel.md)|允许的最大设备威胁级别，由从[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)继承的 MTD 应用程序报告。 可取值为：`notConfigured`、`secured`、`low`、`medium`、`high`。|
|mobileThreatDefenseRemediationAction|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|确定在不满足移动威胁防御威胁阈值时要采取的操作。 警告不是从[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)继承的此属性的受支持的值。 可取值为：`block`、`wipe`、`warn`。|
|blockDataIngestionIntoOrganizationDocuments|Boolean|指示用户是否可以将数据导入到组织文档中。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedDataIngestionLocations|[managedAppDataIngestionLocation](../resources/intune-mam-managedappdataingestionlocation.md)集合|用户可能存储托管数据的数据存储位置。 继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`oneDriveForBusiness`、`sharePoint`、`camera`。|
|appActionIfUnableToAuthenticateUser|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|如果设置，则它将指定在用户因其身份验证令牌无效而无法签入的情况下要执行的操作。 当用户在 AAD 中被删除或禁用时，会发生这种情况。 继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`block`、`wipe`、`warn`。|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|应该用于托管应用中的数据的加密类型。 （仅限 iOS）。 可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。|
|screenCaptureBlocked|Boolean|指示是否阻止捕获屏幕。 （仅限 Android）|
|encryptAppData|Boolean|指示是否应加密托管应用数据。 （仅限 Android）|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|如果启用此设置，则在启用设备级加密的情况下禁用应用级加密。 （仅限 Android）|
|minimumRequiredSdkVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 （仅限 iOS）|
|customSettings|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|要发送给受影响用户的一组字符串键和字符串值对，不被此服务改变|
|deployedAppCount|Int32|当前策略部署到的应用的计数。|
|minimumRequiredPatchVersion|String|定义用户可以获得对应用的安全访问权限所需的最早的必需 Android 安全修补程序级别。 （仅限 Android）|
|minimumWarningPatchVersion|String|定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。 （仅限 Android）|
|exemptedAppProtocols|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|此列表中的 iOS 应用程序将不受策略的阻止，并且将能够从托管应用接收数据。 （仅限 iOS）|
|exemptedAppPackages|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|此列表中的 Android 应用程序包将从该策略中排除，并且将能够从托管应用接收数据。 （仅限 Android）|
|faceIdBlocked|Boolean|指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 PIN。 （仅限 iOS）|
|minimumWipeSdkVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。|
|minimumWipePatchVersion|String|Android 安全修补程序级别小于或等于指定值将擦除托管应用和关联的公司数据。 （仅限 Android）|
|allowedIosDeviceModels|String|允许托管应用使用的设备模型的以分号分隔的列表（以字符串形式）。 （仅限 iOS）|
|appActionIfIosDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管应用程序行为，如果不允许指定的设备模型，则要么阻止，也可以擦除。 （仅限 iOS）。 可取值为：`block`、`wipe`、`warn`。|
|allowedAndroidDeviceManufacturers|String|允许托管应用使用的设备制造商以分号分隔的列表，以字符串形式提供。 （仅限 Android）|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|如果不允许指定的设备制造商，则定义托管应用行为（无论是阻止还是擦除）。 （仅限 Android）。 可取值为：`block`、`wipe`、`warn`。|
|thirdPartyKeyboardsBlocked|Boolean|定义在访问托管应用程序时是否允许使用第三方键盘。 （仅限 iOS）|
|filterOpenInToOnlyManagedApps|Boolean|定义是否支持从受管理的应用程序到所选的可共享位置的打开入点操作。 此设置仅适用于将 AllowedOutboundDataTransferDestinations 设置为 ManagedApps 和 DisableProtectionOfManagedOutboundOpenInData 设置为 False 的情况。 （仅限 iOS）|
|disableProtectionOfManagedOutboundOpenInData|Boolean|禁用通过 IOS OpenIn 选项传输到其他应用程序的数据保护。 仅当 AllowedOutboundDataTransferDestinations 设置为 ManagedApps 时，此设置才允许为 True。 （仅限 iOS）|
|protectInboundDataFromUnknownSources|Boolean|保护来自未知源的传入数据。 仅当 AllowedInboundDataTransferSources 设置为 AllApps 时，此设置才允许为 True。 （仅限 iOS）|
|requiredAndroidSafetyNetDeviceAttestationType|[androidManagedAppSafetyNetDeviceAttestationType](../resources/intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)|定义要使用的托管应用的 Android SafetyNet 设备证明要求。 可取值为：`none`、`basicIntegrity`、`basicIntegrityAndDeviceCertification`。|
|appActionIfAndroidSafetyNetDeviceAttestationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管应用程序行为（如果指定的 Android SafetyNet 认证 requirment 失败，则为 "警告" 或 "阻止"）。 可取值为：`block`、`wipe`、`warn`。|
|requiredAndroidSafetyNetAppsVerificationType|[androidManagedAppSafetyNetAppsVerificationType](../resources/intune-mam-androidmanagedappsafetynetappsverificationtype.md)|定义要使用的受管理的应用程序的 Android SafetyNet 应用验证要求。 可取值为：`none`、`enabled`。|
|appActionIfAndroidSafetyNetAppsVerificationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管应用程序行为（如果指定的 Android 应用验证 requirment 失败，则为警告或阻止）。 可取值为：`block`、`wipe`、`warn`。|
|customBrowserProtocol|String|用于在 iOS 上打开 weblink 的自定义浏览器协议。 （仅限 iOS）|
|customBrowserPackageId|String|在 Android 上打开 weblink 的自定义浏览器的唯一标识符。 （仅限 Android）|
|customBrowserDisplayName|String|首选自定义浏览器的友好名称，以在 Android 上打开 weblink。 （仅限 Android）|
|minimumRequiredCompanyPortalVersion|String|必须在设备或应用程序访问上安装的公司门户的最低版本将被阻止|
|minimumWarningCompanyPortalVersion|String|必须在设备上安装的公司门户的最低版本或用户将收到警告|
|minimumWipeCompanyPortalVersion|String|必须在设备上安装的公司门户的最低版本或应用程序上的公司数据将被擦除|
|allowedAndroidDeviceModels|String 集合|允许托管应用使用的设备模型列表，以字符串形式表示。 （仅限 Android）|
|appActionIfAndroidDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管应用程序行为，如果不允许指定的设备模型，则要么阻止，也可以擦除。 （仅限 Android）。 可取值为：`block`、`wipe`、`warn`。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections
Content-type: application/json
Content-length: 4523

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
  "allowedOutboundClipboardSharingExceptionLength": 14,
  "notificationRestriction": "blockOrganizationalData",
  "previousPinBlockCount": 5,
  "managedBrowser": "microsoftEdge",
  "maximumAllowedDeviceThreatLevel": "secured",
  "mobileThreatDefenseRemediationAction": "wipe",
  "blockDataIngestionIntoOrganizationDocuments": true,
  "allowedDataIngestionLocations": [
    "sharePoint"
  ],
  "appActionIfUnableToAuthenticateUser": "wipe",
  "appDataEncryptionType": "afterDeviceRestart",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
  "requiredAndroidSafetyNetAppsVerificationType": "enabled",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe",
  "customBrowserProtocol": "Custom Browser Protocol value",
  "customBrowserPackageId": "Custom Browser Package Id value",
  "customBrowserDisplayName": "Custom Browser Display Name value",
  "minimumRequiredCompanyPortalVersion": "Minimum Required Company Portal Version value",
  "minimumWarningCompanyPortalVersion": "Minimum Warning Company Portal Version value",
  "minimumWipeCompanyPortalVersion": "Minimum Wipe Company Portal Version value",
  "allowedAndroidDeviceModels": [
    "Allowed Android Device Models value"
  ],
  "appActionIfAndroidDeviceModelNotAllowed": "wipe"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4695

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "77064c51-4c51-7706-514c-0677514c0677",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
  "allowedOutboundClipboardSharingExceptionLength": 14,
  "notificationRestriction": "blockOrganizationalData",
  "previousPinBlockCount": 5,
  "managedBrowser": "microsoftEdge",
  "maximumAllowedDeviceThreatLevel": "secured",
  "mobileThreatDefenseRemediationAction": "wipe",
  "blockDataIngestionIntoOrganizationDocuments": true,
  "allowedDataIngestionLocations": [
    "sharePoint"
  ],
  "appActionIfUnableToAuthenticateUser": "wipe",
  "appDataEncryptionType": "afterDeviceRestart",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
  "requiredAndroidSafetyNetAppsVerificationType": "enabled",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe",
  "customBrowserProtocol": "Custom Browser Protocol value",
  "customBrowserPackageId": "Custom Browser Package Id value",
  "customBrowserDisplayName": "Custom Browser Display Name value",
  "minimumRequiredCompanyPortalVersion": "Minimum Required Company Portal Version value",
  "minimumWarningCompanyPortalVersion": "Minimum Warning Company Portal Version value",
  "minimumWipeCompanyPortalVersion": "Minimum Wipe Company Portal Version value",
  "allowedAndroidDeviceModels": [
    "Allowed Android Device Models value"
  ],
  "appActionIfAndroidDeviceModelNotAllowed": "wipe"
}
```



