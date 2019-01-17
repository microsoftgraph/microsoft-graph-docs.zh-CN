---
title: macOSGeneralDeviceConfiguration 资源类型
description: 本主题提供由 macOSGeneralDeviceConfiguration 资源公开的已声明方法、属性和关系的说明。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 02bdcf72a9b01c9fd2ec0dcb45f7c743e51f941b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983924"
---
# <a name="macosgeneraldeviceconfiguration-resource-type"></a>macOSGeneralDeviceConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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
|roleScopeTagIds|String 集合|此实体实例范围标记的列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础的设备配置支持分配的范围标记。 此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。 这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
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
|passwordRequired|Boolean|是否需要密码。|
|keychainBlockCloudSync|Boolean|指示 iCloud 钥匙链同步阻止 (macOS 10.12 及更高版本)。|
|airPrintBlocked|Boolean|指示 AirPrint 阻止 (macOS 10.12 及更高版本)。|
|airPrintForceTrustedTLS|Boolean|指示受信任的证书是否需要 TLS 打印通信 (macOS 10.13 及更高版本)。|
|airPrintBlockiBeaconDiscovery|Boolean|指示阻止 iBeacon 发现 AirPrint 打印机。 这样可以防止在从网络流量 (macOS 10.3 及更高版本) 的网络钓鱼的虚假 AirPrint 蓝牙信号。|
|safariBlockAutofill|Boolean|指示在 Safari 中是否阻止用户使用自动填充。|
|cameraBlocked|Boolean|指示是否阻止用户访问设备的照相机。|
|iTunesBlockMusicService|Boolean|指示阻止音乐服务并还原为经典模式的音乐应用程序。|
|spotlightBlockInternetResults|Boolean|指示阻止聚焦从 Internet 搜索返回任何结果。|
|keyboardBlockDictation|Boolean|指示阻止用户使用口述输入。|
|definitionLookupBlocked|Boolean|指示阻止定义查找。|
|appleWatchBlockAutoUnlock|Boolean|指示是否或阻止用户解锁与 Apple Watch 其 Mac。|
|iTunesBlockFileSharing|Boolean|指示阻止进行文件传输使用 iTunes。|
|iCloudBlockDocumentSync|Boolean|指示是否阻止 iCloud 文档同步。|
|iCloudBlockMail|Boolean|指示阻止 iCloud 从同步邮件。|
|iCloudBlockAddressBook|Boolean|指示阻止 iCloud 从同步联系人。|
|iCloudBlockCalendar|Boolean|指示阻止 iCloud 从同步日历。|
|iCloudBlockReminders|Boolean|指示阻止 iCloud 从同步提醒。|
|iCloudBlockBookmarks|Boolean|指示阻止 iCloud 从同步书签。|
|iCloudBlockNotes|Boolean|指示阻止 iCloud 从同步注释。|
|airDropBlocked|Boolean|指示允许 AirDrop。|
|passwordBlockModification|Boolean|指示允许密码修改。|
|passwordBlockFingerprintUnlock|Boolean|指示是否阻止指纹解锁。|

## <a name="relationships"></a>Relationships
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
  "passwordBlockFingerprintUnlock": true
}
```





