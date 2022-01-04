---
title: 创建 macOSGeneralDeviceConfiguration
description: 创建新的 macOSGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa5afab21f38da8ce2a18c75ab295e439bf9a4e2
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/04/2022
ms.locfileid: "61711933"
---
# <a name="create-macosgeneraldeviceconfiguration"></a>创建 macOSGeneralDeviceConfiguration

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

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
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 macOSGeneralDeviceConfiguration 对象的 JSON 表示形式。

下表显示创建 macOSGeneralDeviceConfiguration 时所需的属性。

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
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
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
|touchIdTimeoutInHours|Int32|用户必须输入密码才能解锁设备（而不是使用触摸 ID）的最长小时数。 适用于运行 macOS 12 及更高版本的设备。 有效值为 0 到 2147483647|
|iCloudPrivateRelayBlocked|Boolean|iCloud 专用中继是一项 iCloud+ 服务，可防止网络和服务器通过 Internet 监视用户的活动。 通过阻止 iCloud 专用中继，Apple 不会加密离开设备的流量。 适用于运行 macOS 12 及更高版本的设备。|
|iCloudDesktopAndDocumentsBlocked|Boolean|如果为 TRUE，则阻止云桌面和文档的同步。 如果为 FALSE，则允许同步云桌面和文档。 适用于运行 macOS 10.12.4 及更高版本的设备。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 5014

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "passwordMaximumAttemptCount": 11,
  "passwordMinutesUntilFailedLoginReset": 4,
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
  "softwareUpdatesEnforcedDelayInDays": 2,
  "updateDelayPolicy": "delayOSUpdateVisibility",
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
      "displayName": "Display Name value",
      "identifier": "Identifier value",
      "identifierType": "path",
      "codeRequirement": "Code Requirement value",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "enabled",
      "accessibility": "enabled",
      "addressBook": "enabled",
      "calendar": "enabled",
      "reminders": "enabled",
      "photos": "enabled",
      "mediaLibrary": "enabled",
      "fileProviderPresence": "enabled",
      "systemPolicyAllFiles": "enabled",
      "systemPolicySystemAdminFiles": "enabled",
      "systemPolicyDesktopFolder": "enabled",
      "systemPolicyDocumentsFolder": "enabled",
      "systemPolicyDownloadsFolder": "enabled",
      "systemPolicyNetworkVolumes": "enabled",
      "systemPolicyRemovableVolumes": "enabled",
      "postEvent": "enabled",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "Code Requirement value",
          "identifier": "Identifier value",
          "identifierType": "path",
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
  "softwareUpdateMajorOSDeferredInstallDelayInDays": 15,
  "softwareUpdateMinorOSDeferredInstallDelayInDays": 15,
  "softwareUpdateNonOSDeferredInstallDelayInDays": 13,
  "touchIdTimeoutInHours": 5,
  "iCloudPrivateRelayBlocked": true,
  "iCloudDesktopAndDocumentsBlocked": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5186

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "passwordMaximumAttemptCount": 11,
  "passwordMinutesUntilFailedLoginReset": 4,
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
  "softwareUpdatesEnforcedDelayInDays": 2,
  "updateDelayPolicy": "delayOSUpdateVisibility",
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
      "displayName": "Display Name value",
      "identifier": "Identifier value",
      "identifierType": "path",
      "codeRequirement": "Code Requirement value",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "enabled",
      "accessibility": "enabled",
      "addressBook": "enabled",
      "calendar": "enabled",
      "reminders": "enabled",
      "photos": "enabled",
      "mediaLibrary": "enabled",
      "fileProviderPresence": "enabled",
      "systemPolicyAllFiles": "enabled",
      "systemPolicySystemAdminFiles": "enabled",
      "systemPolicyDesktopFolder": "enabled",
      "systemPolicyDocumentsFolder": "enabled",
      "systemPolicyDownloadsFolder": "enabled",
      "systemPolicyNetworkVolumes": "enabled",
      "systemPolicyRemovableVolumes": "enabled",
      "postEvent": "enabled",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "Code Requirement value",
          "identifier": "Identifier value",
          "identifierType": "path",
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
  "softwareUpdateMajorOSDeferredInstallDelayInDays": 15,
  "softwareUpdateMinorOSDeferredInstallDelayInDays": 15,
  "softwareUpdateNonOSDeferredInstallDelayInDays": 13,
  "touchIdTimeoutInHours": 5,
  "iCloudPrivateRelayBlocked": true,
  "iCloudDesktopAndDocumentsBlocked": true
}
```




