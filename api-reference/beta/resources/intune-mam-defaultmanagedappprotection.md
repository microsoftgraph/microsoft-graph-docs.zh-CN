---
title: defaultManagedAppProtection 资源类型
description: 用于为 TargetedManagedAppProtection 策略未针对的所有用户配置指定的一组应用的详细管理设置的策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 264292aff3d79cee7b1561b4997fb915b1d6eba1
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695256"
---
# <a name="defaultmanagedappprotection-resource-type"></a>defaultManagedAppProtection 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于为 TargetedManagedAppProtection 策略未针对的所有用户配置指定的一组应用的详细管理设置的策略。


继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)

## <a name="methods"></a>Methods
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
|说明|String|策略的说明。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|String|实体的键。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|实体的版本。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|Duration|设备未连接到 Internet 时在该时间段后检查访问权限。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOnlineBeforeAccessCheck|Duration|设备连接到 Internet 时在该时间段后检查访问权限。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|允许传输其中的数据的源。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`allApps`、`managedApps`、`none`。|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|允许向其传输数据的目标。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`allApps`、`managedApps`、`none`。|
|organizationalCredentialsRequired|Boolean|指示是否需要组织凭据才能使用应用。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|可以在托管设备上的应用之间共享剪贴板的级别。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。|
|dataBackupBlocked|Boolean|指示是否阻止备份托管应用的数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|deviceComplianceRequired|Boolean|指示是否需要设备符合性。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|managedBrowserToOpenLinksRequired|Boolean|指示是应在托管浏览器应用中打开 Internet 链接，还是应在由 CustomBrowserProtocol (for iOS) 或 CustomBrowserPackageId/CustomBrowserDisplayName (for Android) 指定的任何自定义浏览器继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|saveAsBlocked|Boolean|指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duration|在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinRequired|Boolean|指示是否需要应用级 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumPinRetries|Int32|阻止或擦除托管应用之前的最大错误引脚重试次数。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|simplePinBlocked|Boolean|指示是否阻止 simplePin。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumPinLength|Int32|PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|PinRequired 设置为 True 时可用于应用级 PIN 的字符集。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`numeric`、`alphanumericAndSymbol`。|
|periodBeforePinReset|Duration|TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) 集合|用户可能存储托管数据的数据存储位置。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|contactSyncBlocked|Boolean|指示联系人是否可以同步到用户的设备。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|printBlocked|Boolean|指示是否允许从托管应用进行打印。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|fingerprintBlocked|Boolean|指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Boolean|指示如果设置了设备 PIN，是否需要使用应用 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumRequiredOsVersion|字符串|大于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumWarningOsVersion|String|大于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumWipeOsVersion|String|大于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredOsVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningOsVersion|String|低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredAppVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningAppVersion|String|低于指定版本的版本将导致托管应用出现警告消息。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeOsVersion|String|小于或等于指定版本的版本将擦除托管应用和关联的公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeAppVersion|字符串|小于或等于指定版本的版本将擦除托管应用和关联的公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|如果 DeviceComplianceRequired 设置为 true，则定义设备取得 root 或越狱权限时可阻止或擦除的托管应用行为。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`block`、`wipe`、`warn`。|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|根据错误的 pin 重试次数上限，定义托管应用行为（阻止或擦除）。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`block`、`wipe`、`warn`。|
|pinRequiredInsteadOfBiometricTimeout|期限|应用 PIN 而不是非生物识别密码的超时（分钟） 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedOutboundClipboardSharingExceptionLength|Int32|指定可以剪切或从组织数据和帐户复制到任何应用程序的字符数。 此设置将覆盖 AllowedOutboundClipboardSharingLevel 限制。 默认值"0"表示不允许任何异常。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|notificationRestriction|[managedAppNotificationRestriction](../resources/intune-mam-managedappnotificationrestriction.md)|指定应用通知限制 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`allow`、`blockOrganizationalData`、`block`。|
|previousPinBlockCount|Int32|需要一个引脚与此属性中指定的数字唯一。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|managedBrowser|[managedBrowserType](../resources/intune-mam-managedbrowsertype.md)|指示应打开 (浏览器) 的托管浏览器。 配置此属性时，ManagedBrowserToOpenLinksRequired 应为 true。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`notConfigured`、`microsoftEdge`。|
|maximumAllowedDeviceThreatLevel|[managedAppDeviceThreatLevel](../resources/intune-mam-managedappdevicethreatlevel.md)|允许的最大设备威胁级别，由 MTD 应用报告。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`notConfigured`、`secured`、`low`、`medium`、`high`。|
|mobileThreatDefenseRemediationAction|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|确定在未达到移动威胁防护威胁阈值时要采取什么操作。 警告不是此属性的受支持值 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`block`、`wipe`、`warn`。|
|blockDataIngestionIntoOrganizationDocuments|布尔值|指示用户是否可以将数据引入组织文档。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedDataIngestionLocations|[managedAppDataIngestionLocation](../resources/intune-mam-managedappdataingestionlocation.md) 集合|用户可能存储托管数据的数据存储位置。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|appActionIfUnableToAuthenticateUser|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|如果设置，它将指定在用户由于身份验证令牌无效而无法签入时要执行哪些操作。 当用户在邮件中删除或禁用时AAD。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`block`、`wipe`、`warn`。|
|dialerRestrictionLevel|[managedAppPhoneNumberRedirectLevel](../resources/intune-mam-managedappphonenumberredirectlevel.md)|允许单击打开电话号码的拨号程序应用的类。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可能的值是：`allApps`、`managedApps`、`customApp`、`blocked`。|
|gracePeriodToBlockAppsDuringOffClockHours|期限|在非时钟时段阻止应用访问前的宽限期。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|应该用于托管应用中的数据的加密类型。  (仅 iOS) 。 可能的值是：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。|
|screenCaptureBlocked|Boolean|指示是否阻止捕获屏幕。 （仅限 Android）|
|encryptAppData|Boolean|指示是否应加密托管应用数据。 （仅限 Android）|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|启用此设置后，如果启用了设备级别加密，则应用级别加密将被禁用。 （仅限 Android）|
|minimumRequiredSdkVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。  (仅 iOS) |
|customSettings|[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合|要发送给受影响用户的一组字符串键和字符串值对，不被此服务改变|
|deployedAppCount|Int32|当前策略部署到的应用的计数。|
|minimumRequiredPatchVersion|String|定义用户可以获得对应用的安全访问权限所需的最早的必需 Android 安全修补程序级别。 （仅限 Android）|
|minimumWarningPatchVersion|String|定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。 （仅限 Android）|
|exemptedAppProtocols|[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合|此列表中的 iOS 应用将免受策略的影响，并且将能够从托管应用接收数据。  (仅 iOS) |
|exemptedAppPackages|[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合|此列表中的 Android 应用包将免受策略的影响，并且将能够从托管应用接收数据。 （仅限 Android）|
|faceIdBlocked|Boolean|指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 PIN。  (仅 iOS) |
|minimumWipeSdkVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。|
|minimumWipePatchVersion|String|小于或等于指定值的 Android 安全修补程序级别将擦除托管应用和关联的公司数据。 （仅限 Android）|
|allowedIosDeviceModels|String|允许以字符串形式将设备型号的分号分隔列表用于托管应用。  (仅 iOS) |
|appActionIfIosDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管应用行为（阻止或擦除）（如果不允许指定的设备模型）。  (仅 iOS) 。 可取值为：`block`、`wipe`、`warn`。|
|allowedAndroidDeviceManufacturers|String|以字符串形式允许托管应用工作的设备制造商分号分隔列表。 （仅限 Android）|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管应用行为（阻止或擦除）（如果不允许指定的设备制造商）。  (Android) 。 可取值为：`block`、`wipe`、`warn`。|
|thirdPartyKeyboardsBlocked|布尔值|定义在访问托管应用时是否允许使用第三方键盘。  (仅 iOS) |
|filterOpenInToOnlyManagedApps|布尔值|定义是否支持从托管应用到所选文件共享位置的打开操作。 此设置仅在 AllowedOutboundDataTransferDestinations 设置为 ManagedApps 且 DisableProtectionOfManagedOutboundOpenInData 设置为 False 时适用。  (仅 iOS) |
|disableProtectionOfManagedOutboundOpenInData|布尔值|禁用对通过 IOS OpenIn 选项传输到其他应用的数据的保护。 只有在 AllowedOutboundDataTransferDestinations 设置为 ManagedApps 时，此设置才允许为 True。  (仅 iOS) |
|protectInboundDataFromUnknownSources|布尔值|保护来自未知源的传入数据。 只有在 AllowedInboundDataTransferSources 设置为 AllApps 时，此设置才允许为 True。  (仅 iOS) |
|requiredAndroidSafetyNetDeviceAttestationType|[androidManagedAppSafetyNetDeviceAttestationType](../resources/intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)|定义托管应用正常工作的 Android SafetyNet 设备证明要求。 可取值为：`none`、`basicIntegrity`、`basicIntegrityAndDeviceCertification`。|
|appActionIfAndroidSafetyNetDeviceAttestationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管应用行为，如果指定的 Android SafetyNet 证明要求失败，则发出警告或阻止。 可取值为：`block`、`wipe`、`warn`。|
|requiredAndroidSafetyNetAppsVerificationType|[androidManagedAppSafetyNetAppsVerificationType](../resources/intune-mam-androidmanagedappsafetynetappsverificationtype.md)|定义 Android SafetyNet 应用验证要求，使托管应用正常工作。 可取值为：`none`、`enabled`。|
|appActionIfAndroidSafetyNetAppsVerificationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管应用行为，如果指定的 Android 应用验证要求失败，则发出警告或阻止。 可取值为：`block`、`wipe`、`warn`。|
|customBrowserProtocol|String|在 iOS 上打开 Web 链接的自定义浏览器协议。  (iOS) |
|customBrowserPackageId|String|在 Android 上打开 Web 链接的自定义浏览器的唯一标识符。 （仅限 Android）|
|customBrowserDisplayName|String|在 Android 上打开 Web 链接的首选自定义浏览器的友好名称。 （仅限 Android）|
|minimumRequiredCompanyPortalVersion|字符串|必须安装在设备或应用访问上的公司门户的最低版本将被阻止|
|minimumWarningCompanyPortalVersion|String|必须安装在设备上或用户将收到警告的公司门户的最低版本|
|minimumWipeCompanyPortalVersion|字符串|必须安装在设备上或应用上的公司数据的最低版本公司门户将擦除|
|allowedAndroidDeviceModels|String collection|允许托管应用正常工作的设备型号列表（作为字符串）。  (Android) |
|appActionIfAndroidDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管应用行为（阻止或擦除）（如果不允许指定的设备模型）。  (Android) 。 可取值为：`block`、`wipe`、`warn`。|
|customDialerAppProtocol|String|在 iOS 上单击以打开电话号码的自定义拨号程序应用的协议，例如 skype：。|
|customDialerAppPackageId|String|在 Android 上单击以打开电话号码的自定义拨号程序应用的 PackageId。|
|customDialerAppDisplayName|String|在 Android 上单击以打开电话号码的自定义拨号程序应用的友好名称。|
|biometricAuthenticationBlocked|布尔值|指示 PinRequired 设置为 True 时是否允许使用生物识别身份验证来代表 PIN。  (Android) |
|requiredAndroidSafetyNetEvaluationType|[androidManagedAppSafetyNetEvaluationType](../resources/intune-mam-androidmanagedappsafetynetevaluationtype.md)|定义 Android SafetyNet 评估类型要求，使托管应用正常工作。  (Android 仅) 。 可取值为：`basic`、`hardwareBacked`。|
|blockAfterCompanyPortalUpdateDeferralInDays|Int32|在设备上公司门户更新可以延迟的最大天数，否则将阻止应用访问。|
|warnAfterCompanyPortalUpdateDeferralInDays|Int32|在设备上公司门户更新或用户将收到警告的最大天数|
|wipeAfterCompanyPortalUpdateDeferralInDays|Int32|在设备上公司门户更新的最大天数，或者将擦除应用上的公司数据|
|deviceLockRequired|布尔值|定义设备上是否必须要求任何类型的锁定。  (android) |
|appActionIfDeviceLockNotSet|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管应用行为（警告、阻止或擦除）（如果设备上需要屏幕锁定，但没有设置）。  (android) 。 可取值为：`block`、`wipe`、`warn`。|
|connectToVpnOnLaunch|布尔值|应用是否应该在启动时连接到配置的 VPN (Android) 。|

## <a name="relationships"></a>关系
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
  "roleScopeTagIds": [
    "String"
  ],
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
  "maximumRequiredOsVersion": "String",
  "maximumWarningOsVersion": "String",
  "maximumWipeOsVersion": "String",
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "minimumWipeOsVersion": "String",
  "minimumWipeAppVersion": "String",
  "appActionIfDeviceComplianceRequired": "String",
  "appActionIfMaximumPinRetriesExceeded": "String",
  "pinRequiredInsteadOfBiometricTimeout": "String (duration)",
  "allowedOutboundClipboardSharingExceptionLength": 1024,
  "notificationRestriction": "String",
  "previousPinBlockCount": 1024,
  "managedBrowser": "String",
  "maximumAllowedDeviceThreatLevel": "String",
  "mobileThreatDefenseRemediationAction": "String",
  "blockDataIngestionIntoOrganizationDocuments": true,
  "allowedDataIngestionLocations": [
    "String"
  ],
  "appActionIfUnableToAuthenticateUser": "String",
  "dialerRestrictionLevel": "String",
  "gracePeriodToBlockAppsDuringOffClockHours": "String (duration)",
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
  "protectInboundDataFromUnknownSources": true,
  "requiredAndroidSafetyNetDeviceAttestationType": "String",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
  "requiredAndroidSafetyNetAppsVerificationType": "String",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "String",
  "customBrowserProtocol": "String",
  "customBrowserPackageId": "String",
  "customBrowserDisplayName": "String",
  "minimumRequiredCompanyPortalVersion": "String",
  "minimumWarningCompanyPortalVersion": "String",
  "minimumWipeCompanyPortalVersion": "String",
  "allowedAndroidDeviceModels": [
    "String"
  ],
  "appActionIfAndroidDeviceModelNotAllowed": "String",
  "customDialerAppProtocol": "String",
  "customDialerAppPackageId": "String",
  "customDialerAppDisplayName": "String",
  "biometricAuthenticationBlocked": true,
  "requiredAndroidSafetyNetEvaluationType": "String",
  "blockAfterCompanyPortalUpdateDeferralInDays": 1024,
  "warnAfterCompanyPortalUpdateDeferralInDays": 1024,
  "wipeAfterCompanyPortalUpdateDeferralInDays": 1024,
  "deviceLockRequired": true,
  "appActionIfDeviceLockNotSet": "String",
  "connectToVpnOnLaunch": true
}
```



