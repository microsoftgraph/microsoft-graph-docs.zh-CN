---
title: macOSGeneralDeviceConfiguration 资源类型
description: 本主题提供由 macOSGeneralDeviceConfiguration 资源公开的已声明方法、属性和关系的说明。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8fadc8f8aa91caec0596650765c1feada58cecc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146240"
---
# <a name="macosgeneraldeviceconfiguration-resource-type"></a>macOSGeneralDeviceConfiguration 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

本主题提供由 macOSGeneralDeviceConfiguration 资源公开的已声明方法、属性和关系的说明。


继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List macOSGeneralDeviceConfigurations](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-list.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 集合|列出 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的属性和关系。|
|[Get macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-get.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|读取 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的属性和关系。|
|[Create macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-create.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|创建新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。|
|[Delete macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-delete.md)|无|删除 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)。|
|[Update macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-update.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|更新 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|布尔|指示基础设备配置是否支持作用域标记的分配。 如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。 这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|compliantAppsList|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。 该集合最多可包含 10000 个元素。|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|位于 CompliantAppsList 中的列表。 可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。|
|emailInDomainSuffixes|String 集合|缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。|
|passwordBlockSimple|Boolean|阻止简单密码。|
|passwordExpirationDays|Int32|密码过期前的天数。|
|passwordMinimumCharacterSetCount|Int32|密码必须包含的字符集数。 有效值为 0 至 4|
|passwordMinimumLength|Int32|密码的最小长度。|
|passwordMinutesOfInactivityBeforeLock|Int32|在需要密码之前需要不活动的分钟数。|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|在屏幕超时之前需要不活动的分钟数。|
|passwordPreviousPasswordBlockCount|Int32|要阻止的以前密码的数量。|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|必需的密码类型。 可取值为：`deviceDefault`、`alphanumeric`、`numeric`。|
|passwordRequired|布尔|是否需要密码。|
|keychainBlockCloudSync|布尔|指示是否阻止 iCloud 密钥链同步 (macOS 10.12 及更高版本)。|
|airPrintBlocked|布尔|指示是否阻止 AirPrint (macOS 10.12 及更高版本)。|
|airPrintForceTrustedTLS|布尔|指示 TLS 打印通信是否需要受信任的证书 (macOS 10.13 及更高版本)。|
|airPrintBlockiBeaconDiscovery|布尔|指示是否阻止 AirPrint 打印机的 iBeacon 发现。 这可防止来自网络流量的虚假 AirPrint 蓝牙信号 (macOS 10.3 及更高版本)。|
|safariBlockAutofill|Boolean|指示在 Safari 中是否阻止用户使用自动填充。|
|cameraBlocked|Boolean|指示是否阻止用户访问设备的照相机。|
|iTunesBlockMusicService|布尔|指示是否阻止音乐服务并将音乐应用还原到经典模式。|
|spotlightBlockInternetResults|Boolean|指示是否阻止聚光灯从 Internet 搜索返回任何结果。|
|keyboardBlockDictation|布尔|指示是否阻止用户使用听写输入。|
|definitionLookupBlocked|布尔|指示是否阻止定义查找。|
|appleWatchBlockAutoUnlock|布尔|指示是否阻止用户使用 Apple Watch 解锁其 Mac。|
|iTunesBlockFileSharing|布尔|指示是否阻止使用 iTunes 传输文件。|
|iCloudBlockDocumentSync|布尔|指示是否阻止 iCloud 文档同步。|
|iCloudBlockMail|布尔|指示是否阻止 iCloud 同步邮件。|
|iCloudBlockAddressBook|布尔|指示是否阻止 iCloud 同步联系人。|
|iCloudBlockCalendar|布尔|指示是否阻止 iCloud 同步日历。|
|iCloudBlockReminders|布尔|指示是否阻止 iCloud 同步提醒。|
|iCloudBlockBookmarks|布尔|指示是否阻止 iCloud 同步书签。|
|iCloudBlockNotes|布尔|指示是否阻止 iCloud 同步笔记。|
|airDropBlocked|布尔|指示是否允许 AirDrop。|
|passwordBlockModification|布尔|指示是否允许修改密码。|
|passwordBlockFingerprintUnlock|布尔|指示是否阻止指纹解锁。|
|passwordBlockAutoFill|布尔|指示是否阻止自动填充密码功能。|
|passwordBlockProximityRequests|布尔|指示是否阻止来自附近设备的请求密码。|
|passwordBlockAirDropSharing|布尔|指示是否阻止使用 AirDrop 密码功能的共享密码。|
|softwareUpdatesEnforcedDelayInDays|Int32|设置受监督的设备 delyed 软件更新的天数。 有效值为 0 至 90|
|softwareUpdatesForceDelayed|布尔|指示设备处于监督模式时是否延迟用户对软件更新的可见性。|
|contentCachingBlocked|布尔|指示是否允许内容缓存。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|按用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "emailInDomainSuffixes": [
    "String"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 1024,
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true
}
```




