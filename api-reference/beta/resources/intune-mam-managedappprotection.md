---
title: managedAppProtection 资源类型
description: 用于为指定的一组应用配置详细管理设置的策略
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: abfe85e5d768fc7e8d99c6fbf310cc6bcd4ae2b6
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340651"
---
# <a name="managedappprotection-resource-type"></a>managedAppProtection 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于为指定的一组应用配置详细管理设置的策略


继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedAppProtections](../api/intune-mam-managedappprotection-list.md)|[managedAppProtection](../resources/intune-mam-managedappprotection.md) 集合|列出 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。|
|[Get managedAppProtection](../api/intune-mam-managedappprotection-get.md)|[managedAppProtection](../resources/intune-mam-managedappprotection.md)|读取 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。|
|[targetApps 操作](../api/intune-mam-managedappprotection-targetapps.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|策略显示名称。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|说明|String|策略的说明。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|roleScopeTagIds|字符串集合|此实体实例的范围标记列表。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|String|实体的键。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|实体的版本。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|Duration|设备未连接到 Internet 时在该时间段后检查访问权限。|
|periodOnlineBeforeAccessCheck|Duration|设备连接到 Internet 时在该时间段后检查访问权限。|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|允许传输其中的数据的源。 可取值为：`allApps`、`managedApps`、`none`。|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|允许向其传输数据的目标。 可取值为：`allApps`、`managedApps`、`none`。|
|organizationalCredentialsRequired|Boolean|指示是否需要组织凭据才能使用应用。|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|可以在托管设备上的应用之间共享剪贴板的级别。 可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。|
|dataBackupBlocked|Boolean|指示是否阻止备份托管应用的数据。|
|deviceComplianceRequired|Boolean|指示是否需要设备合规性。|
|managedBrowserToOpenLinksRequired|Boolean|指示是应在托管浏览器应用中打开 Internet 链接，还是应打开由 CustomBrowserProtocol (for iOS) 或 CustomBrowserPackageId/CustomBrowserDisplayName (for Android) |
|saveAsBlocked|Boolean|指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。|
|periodOfflineBeforeWipeIsEnforced|Duration|在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。|
|pinRequired|Boolean|指示是否需要应用级 pin。|
|maximumPinRetries|Int32|阻止或擦除托管应用之前的最大错误引脚重试次数。|
|simplePinBlocked|Boolean|指示是否阻止 simplePin。|
|minimumPinLength|Int32|PinRequired 设置为 True 时应用级 pin 所需的最小 pin 长度。|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|PinRequired 设置为 True 时可用于应用级 pin 的字符集。 可取值为：`numeric`、`alphanumericAndSymbol`。|
|periodBeforePinReset|Duration|TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 pin。|
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) 集合|用户可能存储托管数据的数据存储位置。|
|contactSyncBlocked|Boolean|指示联系人是否可以同步到用户的设备。|
|printBlocked|Boolean|指示是否允许从托管应用进行打印。|
|fingerprintBlocked|Boolean|指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 pin。|
|disableAppPinIfDevicePinIsSet|Boolean|指示如果设置了设备 PIN，是否需要使用应用 PIN。|
|maximumRequiredOsVersion|String|大于指定版本的版本将阻止托管应用访问公司数据。|
|maximumWarningOsVersion|String|大于指定版本的版本将阻止托管应用访问公司数据。|
|maximumWipeOsVersion|String|大于指定版本的版本将阻止托管应用访问公司数据。|
|minimumRequiredOsVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。|
|minimumWarningOsVersion|String|低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。|
|minimumRequiredAppVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。|
|minimumWarningAppVersion|String|低于指定版本的版本将导致托管应用出现警告消息。|
|minimumWipeOsVersion|String|小于或等于指定版本的版本将擦除托管应用和关联的公司数据。|
|minimumWipeAppVersion|String|小于或等于指定版本的版本将擦除托管应用和关联的公司数据。|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|如果 DeviceComplianceRequired 设置为 true，则定义设备取得 root 或越狱权限时可阻止或擦除的托管应用行为。 可取值为：`block`、`wipe`、`warn`。|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|根据错误的 pin 重试次数上限，定义托管应用行为（阻止或擦除）。 可取值为：`block`、`wipe`、`warn`。|
|pinRequiredInsteadOfBiometricTimeout|期限|应用 PIN（而不是非生物识别密码）的超时（分钟）|
|allowedOutboundClipboardSharingExceptionLength|Int32|指定可以剪切或从组织数据和帐户复制到任何应用程序的字符数。 此设置将覆盖 AllowedOutboundClipboardSharingLevel 限制。 默认值"0"表示不允许任何异常。|
|notificationRestriction|[managedAppNotificationRestriction](../resources/intune-mam-managedappnotificationrestriction.md)|指定应用通知限制。 可取值为：`allow`、`blockOrganizationalData`、`block`。|
|previousPinBlockCount|Int32|需要一个引脚与此属性中指定的数字唯一。|
|managedBrowser|[managedBrowserType](../resources/intune-mam-managedbrowsertype.md)|指示应打开 internet () 的托管浏览器。 配置此属性时，ManagedBrowserToOpenLinksRequired 应为 true。 可取值为：`notConfigured`、`microsoftEdge`。|
|maximumAllowedDeviceThreatLevel|[managedAppDeviceThreatLevel](../resources/intune-mam-managedappdevicethreatlevel.md)|MTD 应用报告的最大允许设备威胁级别。 可取值为：`notConfigured`、`secured`、`low`、`medium`、`high`。|
|mobileThreatDefenseRemediationAction|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|确定在未达到移动威胁防护威胁阈值时要采取什么操作。 警告不是此属性支持的值。 可取值为：`block`、`wipe`、`warn`。|
|blockDataIngestionIntoOrganizationDocuments|Boolean|指示用户是否可以将数据引入组织文档。|
|allowedDataIngestionLocations|[managedAppDataIngestionLocation](../resources/intune-mam-managedappdataingestionlocation.md) 集合|用户可能存储托管数据的数据存储位置。|
|appActionIfUnableToAuthenticateUser|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|如果设置，它将指定在用户由于身份验证令牌无效而无法签入时要执行哪些操作。 当用户在邮件中删除或禁用时AAD。 可取值为：`block`、`wipe`、`warn`。|
|dialerRestrictionLevel|[managedAppPhoneNumberRedirectLevel](../resources/intune-mam-managedappphonenumberredirectlevel.md)|允许单击打开电话号码的拨号程序应用的类。 可能的值是：`allApps`、`managedApps`、`customApp`、`blocked`。|
|gracePeriodToBlockAppsDuringOffClockHours|期限|在非时钟时段阻止应用访问前的宽限期。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppProtection",
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
  "gracePeriodToBlockAppsDuringOffClockHours": "String (duration)"
}
```




