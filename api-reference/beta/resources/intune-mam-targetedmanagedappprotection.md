---
title: targetedManagedAppProtection 资源类型
description: 用于配置针对特定安全组的详细管理设置的策略
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a2a17f6417d61721be87636ed624bc1c15ba9809
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670805"
---
# <a name="targetedmanagedappprotection-resource-type"></a>targetedManagedAppProtection 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于配置针对特定安全组的详细管理设置的策略


继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List targetedManagedAppProtections](../api/intune-mam-targetedmanagedappprotection-list.md)|[targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) 集合|列出 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) 对象的属性和关系。|
|[Get targetedManagedAppProtection](../api/intune-mam-targetedmanagedappprotection-get.md)|[targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)|读取 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) 对象的属性和关系。|
|[assign 操作](../api/intune-mam-targetedmanagedappprotection-assign.md)|无|尚未记录|
|[targetApps 操作](../api/intune-mam-targetedmanagedappprotection-targetapps.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|策略显示名称。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
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
|managedBrowserToOpenLinksRequired|Boolean|指示是应在托管浏览器应用中打开 Internet 链接，还是应在适用于 iOS) 的 CustomBrowserProtocol (或 CustomBrowserPackageId/CustomBrowserDisplayName (中为 Android 指定的任何自定义浏览器) 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|saveAsBlocked|Boolean|指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duration|在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinRequired|Boolean|指示是否需要应用级 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumPinRetries|Int32|阻止或擦除托管应用之前，最大错误的引脚重试尝试次数。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|simplePinBlocked|Boolean|指示是否阻止 simplePin。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumPinLength|Int32|PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|PinRequired 设置为 True 时可用于应用级 PIN 的字符集。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`numeric`、`alphanumericAndSymbol`。|
|periodBeforePinReset|Duration|TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) 集合|用户可能存储托管数据的数据存储位置。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|contactSyncBlocked|Boolean|指示联系人是否可以同步到用户的设备。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|printBlocked|Boolean|指示是否允许从托管应用进行打印。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|fingerprintBlocked|Boolean|指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Boolean|指示如果设置了设备 PIN，是否需要使用应用 PIN。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumRequiredOsVersion|String|大于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumWarningOsVersion|字符串|大于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumWipeOsVersion|String|大于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredOsVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningOsVersion|String|低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredAppVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningAppVersion|String|低于指定版本的版本将导致托管应用出现警告消息。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeOsVersion|字符串|小于或等于指定版本的版本将擦除托管应用和关联的公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeAppVersion|字符串|小于或等于指定版本的版本将擦除托管应用和关联的公司数据。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|如果 DeviceComplianceRequired 设置为 true，则定义当设备处于根基或越狱状态时，托管应用行为（阻止或擦除）。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`block`、`wipe`、`warn`。|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|根据错误的引脚重试尝试次数定义托管应用行为（阻止或擦除）。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`block`、`wipe`、`warn`。|
|pinRequiredInstedOfBiometricTimeout|持续时间|应用引脚的超时（以分钟为单位），而不是从 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 继承的非生物识别密码|
|allowedOutboundClipboardSharingExceptionLength|Int32|指定可从组织数据和帐户剪切或复制到任何应用程序的字符数。 此设置替代 AllowedOutboundClipboardSharingLevel 限制。 默认值“0”表示不允许出现异常。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|notificationRestriction|[managedAppNotificationRestriction](../resources/intune-mam-managedappnotificationrestriction.md)|指定从 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 继承的应用通知限制。 可取值为：`allow`、`blockOrganizationalData`、`block`。|
|previousPinBlockCount|Int32|需要从此属性中指定的数字中唯一一个引脚。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|managedBrowser|[managedBrowserType](../resources/intune-mam-managedbrowsertype.md)|指示在哪个托管浏览器 () 应打开 Internet 链接。 配置此属性时，ManagedBrowserToOpenLinksRequired 应为 true。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`notConfigured`、`microsoftEdge`。|
|maximumAllowedDeviceThreatLevel|[managedAppDeviceThreatLevel](../resources/intune-mam-managedappdevicethreatlevel.md)|允许的最大设备威胁级别，由从 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 继承的 MTD 应用报告。 可取值为：`notConfigured`、`secured`、`low`、`medium`、`high`。|
|mobileThreatDefenseRemediationAction|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|确定如果未达到移动威胁防御威胁阈值，将执行哪些操作。 对于从 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 继承的此属性，警告不是受支持的值。 可取值为：`block`、`wipe`、`warn`。|
|blockDataIngestionIntoOrganizationDocuments|Boolean|指示用户是否可以将数据引入组织文档。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedDataIngestionLocations|[managedAppDataIngestionLocation](../resources/intune-mam-managedappdataingestionlocation.md) 集合|用户可能存储托管数据的数据存储位置。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|appActionIfUnableToAuthenticateUser|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|如果设置，它将指定在用户因身份验证令牌无效而无法签入的情况下要采取的操作。 当用户在 AAD 中被删除或禁用时，会发生这种情况。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可取值为：`block`、`wipe`、`warn`。|
|dialerRestrictionLevel|[managedAppPhoneNumberRedirectLevel](../resources/intune-mam-managedappphonenumberredirectlevel.md)|允许单击打开电话号码的拨号应用类。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。 可能的值是：`allApps`、`managedApps`、`customApp`、`blocked`。|
|gracePeriodToBlockAppsDuringOffClockHours|持续时间|在非时钟时间阻止应用访问之前的宽限期。 继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|isAssigned|Boolean|指示策略是否部署到任何包含组。|
|targetedAppManagementLevels|[appManagementLevel](../resources/intune-mam-appmanagementlevel.md)|此策略的预期应用管理级别。 可取值为：`unspecified`、`unmanaged`、`mdm`、`androidEnterprise`、`androidEnterpriseDedicatedDevicesWithAzureAdSharedMode`、`androidOpenSourceProjectUserAssociated` 或 `androidOpenSourceProjectUserless`。|
|appGroupType|[targetedManagedAppGroupType](../resources/intune-mam-targetedmanagedappgrouptype.md)|公共应用选择：组或个人。 可取值为：`selectedPublicApps`、`allCoreMicrosoftApps`、`allMicrosoftApps`、`allApps`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合|策略部署到的包含组和排除组列表的导航属性。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "String",
  "appGroupType": "String"
}
```




