---
title: managedAppProtection 资源类型
description: 用于为指定的一组应用配置详细管理设置的策略
ms.openlocfilehash: 565ec8b2658ba93f6163845f5bb79255bf3d45f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042572"
---
# <a name="managedappprotection-resource-type"></a>managedAppProtection 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

用于为指定的一组应用配置详细管理设置的策略

继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedAppProtections](../api/intune-mam-managedappprotection-list.md)|[managedAppProtection](../resources/intune-mam-managedappprotection.md) 集合|列出 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。|
|[Get managedAppProtection](../api/intune-mam-managedappprotection-get.md)|[managedAppProtection](../resources/intune-mam-managedappprotection.md)|读取 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。|
|[targetApps 操作](../api/intune-mam-managedappprotection-targetapps.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|策略显示名称。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|description|String|策略的说明。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
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
|managedBrowserToOpenLinksRequired|Boolean|指示是否应在托管浏览器应用中打开 Internet 链接。|
|saveAsBlocked|Boolean|指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。|
|periodOfflineBeforeWipeIsEnforced|Duration|在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。|
|pinRequired|Boolean|指示是否需要应用级 pin。|
|maximumPinRetries|Int32|最大不正确的 pin 重试次数之前阻止或之前托管的应用程序。|
|simplePinBlocked|Boolean|指示是否阻止 simplePin。|
|minimumPinLength|Int32|PinRequired 设置为 True 时应用级 pin 所需的最小 pin 长度。|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|PinRequired 设置为 True 时可用于应用级 pin 的字符集。 可取值为：`numeric`、`alphanumericAndSymbol`。|
|periodBeforePinReset|Duration|TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 pin。|
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合|用户可能存储托管数据的数据存储位置。|
|contactSyncBlocked|Boolean|指示联系人是否可以同步到用户的设备。|
|printBlocked|Boolean|指示是否允许从托管应用进行打印。|
|fingerprintBlocked|Boolean|指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 pin。|
|disableAppPinIfDevicePinIsSet|Boolean|指示如果设置了设备 pin，是否需要使用应用 pin。|
|minimumRequiredOsVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。|
|minimumWarningOsVersion|String|低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。|
|minimumRequiredAppVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。|
|minimumWarningAppVersion|String|低于指定版本的版本将导致托管应用出现警告消息。|
|minimumWipeOsVersion|字符串|小于或等于指定的版本将擦除托管应用程序和关联的公司数据的版本。|
|minimumWipeAppVersion|字符串|小于或等于指定的版本将擦除托管应用程序和关联的公司数据的版本。|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管的应用程序行为，阻止或擦除时也根设备, 或 jailbroken，如果 DeviceComplianceRequired 设置为 true。 可取值为：`block`、`wipe`。|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|定义托管的应用程序行为，或者是阻止或擦除，基于最大数量的不正确的 pin 重试次数。 可取值为：`block`、`wipe`。|
|pinRequiredInsteadOfBiometricTimeout|Duration|以分钟为单位的应用程序 pin，而不是非生物密码超时|

## <a name="relationships"></a>Relationships
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
  "pinRequiredInsteadOfBiometricTimeout": "String (duration)"
}
```





