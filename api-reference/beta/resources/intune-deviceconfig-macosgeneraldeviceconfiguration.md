---
title: macOSGeneralDeviceConfiguration 资源类型
description: 本主题提供由 macOSGeneralDeviceConfiguration 资源公开的已声明方法、属性和关系的说明。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e858605f49471bd70e9c79730f39497d5051e9f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064271"
---
# <a name="macosgeneraldeviceconfiguration-resource-type"></a>macOSGeneralDeviceConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

本主题提供由 macOSGeneralDeviceConfiguration 资源公开的已声明方法、属性和关系的说明。


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

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
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持分配范围标记。 当此值为 false 且实体对范围用户不可见时，不允许分配给 ScopeTags 属性。 这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的操作系统版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
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
|passwordMaximumAttemptCount|Int32|在设备的锁屏界面上输入密码的允许失败尝试次数。 有效值为 2 至 11|
|passwordMinutesUntilFailedLoginReset|Int32|达到最大登录尝试失败次数后重置登录前的分钟数。|
|keychainBlockCloudSync|Boolean|指示在 macOS 10.12 (是否阻止 iCloud 密钥链) 。|
|safariBlockAutofill|Boolean|指示在 Safari 中是否阻止用户使用自动填充。|
|cameraBlocked|Boolean|指示是否阻止用户访问设备的照相机。|
|iTunesBlockMusicService|Boolean|指示是否阻止音乐服务，音乐应用恢复为经典模式。|
|spotlightBlockInternetResults|Boolean|指示是否阻止聚焦从 Internet 搜索返回任何结果。|
|keyboardBlockDictation|Boolean|指示是否阻止用户使用听写输入。|
|definitionLookupBlocked|Boolean|指示是否阻止定义查找。|
|appleWatchBlockAutoUnlock|Boolean|指示是否阻止用户使用 Apple Watch 解锁其 Mac。|
|iTunesBlockFileSharing|Boolean|指示是否阻止使用 iTunes 传输文件。|
|iCloudBlockDocumentSync|Boolean|指示是否阻止 iCloud 文档同步。|
|iCloudBlockMail|Boolean|指示是否阻止 iCloud 同步邮件。|
|iCloudBlockAddressBook|Boolean|指示是否阻止 iCloud 同步联系人。|
|iCloudBlockCalendar|Boolean|指示是否阻止 iCloud 同步日历。|
|iCloudBlockReminders|Boolean|指示是否阻止 iCloud 同步提醒。|
|iCloudBlockBookmarks|Boolean|指示是否阻止 iCloud 同步书签。|
|iCloudBlockNotes|Boolean|指示是否阻止 iCloud 同步笔记。|
|airDropBlocked|Boolean|指示是否允许 AirDrop。|
|passwordBlockModification|Boolean|指示是否允许修改密码。|
|passwordBlockFingerprintUnlock|Boolean|指示是否阻止指纹解锁。|
|passwordBlockAutoFill|Boolean|指示是否阻止"自动填充密码"功能。|
|passwordBlockProximityRequests|Boolean|指示是否阻止从附近设备请求密码。|
|passwordBlockAirDropSharing|Boolean|指示是否阻止与 AirDrop 密码功能共享密码。|
|softwareUpdatesEnforcedDelayInDays|Int32|设置对受监督设备取消软件更新的天数。 有效值为 0 至 90|
|updateDelayPolicy|[macOSSoftwareUpdateDelayPolicy](../resources/intune-deviceconfig-macossoftwareupdatedelaypolicy.md)|确定是否延迟 macOS 的操作系统和/或应用更新。 可取值为：`none`、`delayOSUpdateVisibility`、`delayAppUpdateVisibility`、`unknownFutureValue`、`delayMajorOsUpdateVisibility`。|
|contentCachingBlocked|Boolean|指示是否允许内容缓存。|
|iCloudBlockPhotoLibrary|Boolean|指示是否阻止 iCloud 照片库。|
|screenCaptureBlocked|Boolean|指示是否阻止用户进行屏幕截图。|
|classroomAppBlockRemoteScreenObservation|Boolean|指示是否允许 Classroom 应用进行远程屏幕观察。 需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。|
|classroomAppForceUnpromptedScreenObservation|Boolean|指示是否自动授予课堂应用上托管课程的教师查看学生屏幕的权限，而不提示。 需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。|
|classroomForceAutomaticallyJoinClasses|Boolean|指示是否自动授予对教师请求的权限，而不提示学生。 需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。|
|classroomForceRequestPermissionToLeaveClasses|Boolean|指示在尝试离开课程时，是否要求通过 Classroom 在非托管课程注册的学生向教师请求权限。 需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。|
|classroomForceUnpromptedAppAndDeviceLock|Boolean|指示是否允许教师在不提示学生的情况下锁定应用或设备。 需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。|
|iCloudBlockActivityContinuation|Boolean|指示是否阻止用户继续在另一个 iOS 或 MacOS 设备 (MacOS 10.15 或更高版本的 MacOS 设备上) 。|
|privacyAccessControls|[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md) 集合|隐私首选项策略控件的列表。 该集合最多可包含 10000 个元素。|
|addingGameCenterFriendsBlocked|Boolean|是，禁止用户将好友添加到游戏中心。 适用于运行 macOS 版本 10.13 和更高版本的设备。|
|gameCenterBlocked|Boolean|是 禁用游戏中心，游戏中心图标从主屏幕中删除。 适用于运行 macOS 版本 10.13 和更高版本的设备。|
|multiplayerGamingBlocked|Boolean|如果为 TRUE，则使用游戏中心时阻止多人游戏。 如果为 FALSE，则使用游戏中心时允许多人游戏。 适用于运行 macOS 版本 10.13 和更高版本的设备。|
|wallpaperModificationBlocked|Boolean|如果为 TRUE，可防止更改墙纸。 FALSE 允许更改墙纸。 适用于运行 macOS 版本 10.13 和更高版本的设备。|
|eraseContentAndSettingsBlocked|Boolean|如果为 TRUE，则禁用受监督设备的重置选项。 如果为 FALSE，则启用受监督设备的重置选项。 适用于运行 macOS 版本 12.0 和更高版本的设备。|
|softwareUpdateMajorOSDeferredInstallDelayInDays|Int32|指定 1 (1-90) 延迟主要操作系统软件更新的可见性的天数。 适用于运行 macOS 版本 11.3 和更高版本的设备。 有效值为 0 至 90|
|softwareUpdateMinorOSDeferredInstallDelayInDays|Int32|指定延迟次要操作系统软件更新 (1-90) 的天数。 适用于运行 macOS 版本 11.3 和更高版本的设备。 有效值为 0 至 90|
|softwareUpdateNonOSDeferredInstallDelayInDays|Int32|指定 1 (1-90) 延迟非操作系统软件更新的可见性的天数。 适用于运行 macOS 版本 11.3 和更高版本的设备。 有效值为 0 至 90|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|

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
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
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
  "passwordMaximumAttemptCount": 1024,
  "passwordMinutesUntilFailedLoginReset": 1024,
  "keychainBlockCloudSync": true,
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
  "updateDelayPolicy": "String",
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true,
  "privacyAccessControls": [
    {
      "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem",
      "displayName": "String",
      "identifier": "String",
      "identifierType": "String",
      "codeRequirement": "String",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "String",
      "accessibility": "String",
      "addressBook": "String",
      "calendar": "String",
      "reminders": "String",
      "photos": "String",
      "mediaLibrary": "String",
      "fileProviderPresence": "String",
      "systemPolicyAllFiles": "String",
      "systemPolicySystemAdminFiles": "String",
      "systemPolicyDesktopFolder": "String",
      "systemPolicyDocumentsFolder": "String",
      "systemPolicyDownloadsFolder": "String",
      "systemPolicyNetworkVolumes": "String",
      "systemPolicyRemovableVolumes": "String",
      "postEvent": "String",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "String",
          "identifier": "String",
          "identifierType": "String",
          "allowed": true
        }
      ]
    }
  ],
  "addingGameCenterFriendsBlocked": true,
  "gameCenterBlocked": true,
  "multiplayerGamingBlocked": true,
  "wallpaperModificationBlocked": true,
  "eraseContentAndSettingsBlocked": true,
  "softwareUpdateMajorOSDeferredInstallDelayInDays": 1024,
  "softwareUpdateMinorOSDeferredInstallDelayInDays": 1024,
  "softwareUpdateNonOSDeferredInstallDelayInDays": 1024
}
```



