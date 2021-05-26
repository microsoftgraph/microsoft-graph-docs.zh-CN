---
title: iosGeneralDeviceConfiguration 资源类型
description: 本主题提供由 iosGeneralDeviceConfiguration 资源公开的已声明方法、属性和关系的说明。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 740cb725c520024bd280470b11b19fb312f44b86
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665019"
---
# <a name="iosgeneraldeviceconfiguration-resource-type"></a>iosGeneralDeviceConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

本主题提供由 iosGeneralDeviceConfiguration 资源公开的已声明方法、属性和关系的说明。


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List iosGeneralDeviceConfigurations](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-list.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 集合|列出 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的属性和关系。|
|[Get iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-get.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|读取 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的属性和关系。|
|[Create iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-create.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|创建新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。|
|[Delete iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-delete.md)|无|删除 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)。|
|[Update iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-update.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|更新 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|布尔值|指示基础设备配置是否支持分配范围标记。 当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。 这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的操作系统版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|accountBlockModification|Boolean|指示设备处于监督模式时是否允许帐户修改。|
|activationLockAllowWhenSupervised|Boolean|指示设备处于监督模式时是否允许激活锁定。|
|airDropBlocked|Boolean|指示设备处于监督模式时是否允许 AirDrop。|
|airDropForceUnmanagedDropTarget|Boolean|指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。|
|airPlayForcePairingPasswordForOutgoingRequests|Boolean|指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。|
|appleWatchBlockPairing|Boolean|指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。|
|appleWatchForceWristDetection|Boolean|指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。|
|appleNewsBlocked|Boolean|指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。|
|appsSingleAppModeList|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|获取或设置允许自主进入单个应用模式的 iOS 应用列表。 仅限监督模式。 iOS 7.0 及更高版本。 该集合最多可包含 500 个元素。|
|appsVisibilityList|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。 该集合最多可包含 10000 个元素。|
|appsVisibilityListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|位于 AppsVisibilityList 中的列表类型。 可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。|
|appStoreBlockAutomaticDownloads|Boolean|指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。|
|appStoreBlocked|Boolean|指示是否阻止用户使用 App Store。 需要适用于 iOS 13 及更高版本的受监督设备。|
|appStoreBlockInAppPurchases|Boolean|指示是否阻止用户进行应用内购买。|
|appStoreBlockUIAppInstallation|Boolean|指示是否阻止 App Store 应用，而不通过主机应用限制安装。 仅适用于监督模式（iOS 9.0 及更高版本）。|
|appStoreRequirePassword|Boolean|指示使用 App Store 时是否需要密码。|
|autoFillForceAuthentication|布尔值|指示在 Safari 和其他受监督设备上应用自动填充密码和信用卡信息之前是否强制用户身份验证。|
|bluetoothBlockModification|Boolean|指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。|
|cameraBlocked|Boolean|指示是否阻止用户访问设备的照相机。 需要适用于 iOS 13 及更高版本的受监督设备。|
|cellularBlockDataRoaming|Boolean|指示是否阻止数据漫游。|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Boolean|指示漫游时是否阻止全局背景提取。|
|cellularBlockPerAppDataModification|Boolean|指示设备处于监督模式时是否允许更改手机应用数据使用设置。|
|cellularBlockPersonalHotspot|Boolean|指示是否阻止个人热点。|
|cellularBlockPlanModification|布尔值|指示是否允许用户在受监督的设备上更改手机网络计划的设置。|
|cellularBlockVoiceRoaming|Boolean|指示是否阻止语音漫游。|
|certificatesBlockUntrustedTlsCertificates|Boolean|指示是否阻止不受信任的 TLS 证书。|
|classroomAppBlockRemoteScreenObservation|Boolean|指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。|
|classroomAppForceUnpromptedScreenObservation|Boolean|指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。|
|classroomForceAutomaticallyJoinClasses|布尔值|指示设备在监督模式下时是否自动授予对教师请求的权限，而不提示学生。|
|classroomForceUnpromptedAppAndDeviceLock|布尔值|指示是否允许教师在不提示学生的情况下锁定应用或设备。 仅限监督模式。|
|compliantAppsList|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。 该集合最多可包含 10000 个元素。|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|位于 AppComplianceList 中的列表。 可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。|
|configurationProfileBlockChanges|Boolean|指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。|
|definitionLookupBlocked|Boolean|指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。|
|deviceBlockEnableRestrictions|Boolean|指示设备处于监督模式时是否允许用户在设备设置中启用限制。|
|deviceBlockEraseContentAndSettings|Boolean|指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。|
|deviceBlockNameModification|Boolean|指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。|
|diagnosticDataBlockSubmission|Boolean|指示是否阻止诊断数据提交。|
|diagnosticDataBlockSubmissionModification|Boolean|指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。|
|documentsBlockManagedDocumentsInUnmanagedApps|Boolean|指示是否阻止用户查看非托管应用中的托管文档。|
|documentsBlockUnmanagedDocumentsInManagedApps|Boolean|指示是否阻止用户查看托管应用中的非托管文档。|
|emailInDomainSuffixes|String 集合|缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。|
|enterpriseAppBlockTrust|Boolean|指示是否阻止用户信任企业应用。|
|enterpriseAppBlockTrustModification|Boolean|\[已弃用 \] 配置此设置，将值设置为"true"对设备没有影响。|
|esimBlockModification|布尔值|指示是否允许在受监督设备的 eSIM 上添加或删除手机网络计划。|
|faceTimeBlocked|Boolean|指示是否阻止用户使用 FaceTime。 需要适用于 iOS 13 及更高版本的受监督设备。|
|findMyFriendsBlocked|Boolean|指示设备在监督模式下时是否阻止对"查找我的好友"的更改。|
|gamingBlockGameCenterFriends|Boolean|指示是否阻止用户在 Game Center 中拥有好友。 需要适用于 iOS 13 及更高版本的受监督设备。|
|gamingBlockMultiplayer|Boolean|指示是否阻止用户使用多人游戏。 需要适用于 iOS 13 及更高版本的受监督设备。|
|gameCenterBlocked|Boolean|指示设备处于监督模式时是否阻止用户使用 Game Center。|
|hostPairingBlocked|Boolean|指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。|
|iBooksStoreBlocked|Boolean|指示设备处于监督模式时是否阻止用户使用 iBooks Store。|
|iBooksStoreBlockErotica|Boolean|指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。|
|iCloudBlockActivityContinuation|Boolean|指示是否阻止用户继续在 iOS 设备上启动的工作到其他 iOS 或 macOS 设备。|
|iCloudBlockBackup|Boolean|指示是否阻止 iCloud 备份。 需要适用于 iOS 13 及更高版本的受监督设备。|
|iCloudBlockDocumentSync|Boolean|指示是否阻止 iCloud 文档同步。需要适用于 iOS 13 及更高版本的受监督设备。|
|iCloudBlockManagedAppsSync|Boolean|指示是否阻止托管应用云同步。|
|iCloudBlockPhotoLibrary|Boolean|指示是否阻止 iCloud 照片库。|
|iCloudBlockPhotoStreamSync|Boolean|指示是否阻止 iCloud 照片流同步。|
|iCloudBlockSharedPhotoStream|Boolean|指示是否阻止共享照片流。|
|iCloudRequireEncryptedBackup|Boolean|指示是否要求加密备份到 iCloud 的数据。|
|iTunesBlockExplicitContent|Boolean|指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。 需要适用于 iOS 13 及更高版本的受监督设备。|
|iTunesBlockMusicService|Boolean|指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。|
|iTunesBlockRadio|Boolean|指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。|
|keyboardBlockAutoCorrect|Boolean|指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。|
|keyboardBlockDictation|Boolean|指示设备处于监督模式时是否阻止用户使用听写输入。|
|keyboardBlockPredictive|Boolean|指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。|
|keyboardBlockShortcuts|Boolean|指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。|
|keyboardBlockSpellCheck|Boolean|指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。|
|kioskModeAllowAssistiveSpeak|Boolean|指示在展台模式下是否允许辅助朗读。|
|kioskModeAllowAssistiveTouchSettings|Boolean|指示在展台模式下是否允许访问辅助触摸设置。|
|kioskModeAllowAutoLock|Boolean|指示在展台模式下是否允许设备自动锁定。 对于操作系统默认设置，此属性的功能是多余的，并且已弃用。 请改为使用 KioskModeBlockAutoLock。|
|kioskModeBlockAutoLock|布尔值|指示在展台模式下是否阻止设备自动锁定。|
|kioskModeAllowColorInversionSettings|Boolean|指示在展台模式下是否允许访问颜色反转设置。|
|kioskModeAllowRingerSwitch|Boolean|指示在展台模式下是否允许使用响铃开关。 对于操作系统默认设置，此属性的功能是多余的，并且已弃用。 请改为使用 KioskModeBlockRingerSwitch。|
|kioskModeBlockRingerSwitch|布尔值|指示在展台模式下是否阻止使用响铃开关。|
|kioskModeAllowScreenRotation|Boolean|指示在展台模式下是否允许屏幕旋转。 对于操作系统默认设置，此属性的功能是多余的，并且已弃用。 请改为使用 KioskModeBlockScreenRotation。|
|kioskModeBlockScreenRotation|布尔值|指示在展台模式下是否阻止屏幕旋转。|
|kioskModeAllowSleepButton|Boolean|指示在展台模式下是否允许使用睡眠按钮。 对于操作系统默认设置，此属性的功能是多余的，并且已弃用。 请改为使用 KioskModeBlockSleepButton。|
|kioskModeBlockSleepButton|Boolean|指示在展台模式下是否阻止使用睡眠按钮。|
|kioskModeAllowTouchscreen|Boolean|指示在展台模式下是否允许使用触摸屏。 对于操作系统默认设置，此属性的功能是多余的，并且已弃用。 请改为使用 KioskModeBlockTouchscreen。|
|kioskModeBlockTouchscreen|布尔值|指示在展台模式下是否阻止使用触摸屏。|
|kioskModeEnableVoiceControl|布尔值|指示是否在展台模式下启用语音控制。|
|kioskModeAllowVoiceControlModification|布尔值|指示是否允许用户在展台模式下切换语音控制。|
|kioskModeAllowVoiceOverSettings|Boolean|指示在展台模式下是否允许访问语音插入设置。|
|kioskModeAllowVolumeButtons|Boolean|指示在展台模式下是否允许使用音量按钮。 对于操作系统默认设置，此属性的功能是多余的，并且已弃用。 请改为使用 KioskModeBlockVolumeButtons。|
|kioskModeBlockVolumeButtons|Boolean|指示在展台模式下是否阻止音量按钮。|
|kioskModeAllowZoomSettings|Boolean|指示在展台模式下是否允许访问缩放设置。|
|kioskModeAppStoreUrl|String|指向 App Store 中要用于展台模式的应用的 URL。 如果 KioskModeManagedAppId 未知，请使用此方法。|
|kioskModeBuiltInAppId|String|用于展台模式的内置应用的 ID。 在未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。|
|kioskModeRequireAssistiveTouch|Boolean|指示在展台模式下是否要求辅助触摸。|
|kioskModeRequireColorInversion|Boolean|指示在展台模式下是否要求颜色反转。|
|kioskModeRequireMonoAudio|Boolean|指示在展台模式下是否要求单声道音频。|
|kioskModeRequireVoiceOver|Boolean|指示在展台模式下是否要求语音插入。|
|kioskModeRequireZoom|Boolean|指示在展台模式下是否要求缩放。|
|kioskModeManagedAppId|String|用于展台模式的应用的托管应用 ID。 如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。|
|lockScreenBlockControlCenter|Boolean|指示是否阻止用户在锁定屏幕上使用控制中心。|
|lockScreenBlockNotificationView|Boolean|指示是否阻止用户在锁定屏幕上使用通知视图。|
|lockScreenBlockPassbook|Boolean|指示设备处于锁定状态时是否阻止用户使用 Passbook。|
|lockScreenBlockTodayView|Boolean|指示是否阻止用户在锁定屏幕上使用今日视图。|
|mediaContentRatingAustralia|[mediaContentRatingAustralia](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|澳大利亚的媒体内容评级设置|
|mediaContentRatingCanada|[mediaContentRatingCanada](../resources/intune-deviceconfig-mediacontentratingcanada.md)|加拿大的媒体内容评级设置|
|mediaContentRatingFrance|[mediaContentRatingFrance](../resources/intune-deviceconfig-mediacontentratingfrance.md)|法国的媒体内容评级设置|
|mediaContentRatingGermany|[mediaContentRatingGermany](../resources/intune-deviceconfig-mediacontentratinggermany.md)|德国的媒体内容评级设置|
|mediaContentRatingIreland|[mediaContentRatingIreland](../resources/intune-deviceconfig-mediacontentratingireland.md)|爱尔兰的媒体内容评级设置|
|mediaContentRatingJapan|[mediaContentRatingJapan](../resources/intune-deviceconfig-mediacontentratingjapan.md)|日本的媒体内容评级设置|
|mediaContentRatingNewZealand|[mediaContentRatingNewZealand](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|新西兰的媒体内容评级设置|
|mediaContentRatingUnitedKingdom|[mediaContentRatingUnitedKingdom](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|英国的媒体内容评级设置|
|mediaContentRatingUnitedStates|[mediaContentRatingUnitedStates](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|美国的媒体内容评级设置|
|networkUsageRules|[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合|托管应用列表以及适用于它们的网络规则。 该集合最多可包含 1000 个元素。|
|mediaContentRatingApps|[ratingAppsType](../resources/intune-deviceconfig-ratingappstype.md)|应用的媒体内容评级设置。 可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。|
|messagesBlocked|Boolean|指示是否阻止用户使用受监督设备上的消息应用。|
|notificationsBlockSettingsModification|Boolean|指示是否允许修改通知设置（iOS 9.3 及更高版本）。|
|passcodeBlockFingerprintUnlock|Boolean|指示是否阻止指纹解锁。|
|passcodeBlockFingerprintModification|Boolean|在监督模式下阻止修改已注册的 Touch ID 指纹。|
|passcodeBlockModification|Boolean|指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。|
|passcodeBlockSimple|Boolean|指示是否阻止简单密码。|
|passcodeExpirationDays|Int32|密码过期前的天数。 有效值为 1 至 65535|
|passcodeMinimumLength|Int32|密码的最小长度。 有效值为 4 至 14|
|passcodeMinutesOfInactivityBeforeLock|Int32|需要密码之前的不活动分钟数。|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|passcodeMinimumCharacterSetCount|Int32|密码必须包含的字符集数。 有效值为 0 至 4|
|passcodePreviousPasscodeBlockCount|Int32|要阻止的以前密码的数量。 有效值为 1 至 24|
|passcodeSignInFailureCountBeforeWipe|Int32|擦除设备前允许登录失败的次数。 有效值为 2 至 11|
|passcodeRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|必需的密码类型。 可取值为：`deviceDefault`、`alphanumeric`、`numeric`。|
|passcodeRequired|Boolean|指示是否需要密码。|
|podcastsBlocked|Boolean|指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。|
|proximityBlockSetupToNewDevice|布尔值|指示是否启用提示以使用受监督的设备设置附近设备。|
|safariBlockAutofill|Boolean|指示在 Safari 中是否阻止用户使用自动填充。 需要适用于 iOS 13 及更高版本的受监督设备。|
|safariBlockJavaScript|Boolean|指示在 Safari 中是否阻止 JavaScript。|
|safariBlockPopups|Boolean|指示在 Safari 中是否阻止弹出窗口。|
|safariBlocked|Boolean|指示是否阻止用户使用 Safari。 需要适用于 iOS 13 及更高版本的受监督设备。|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Safari 的 Cookie 设置。 可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。|
|safariManagedDomains|String 集合|与此处列出的模式匹配的 URL 将被视为托管。|
|safariPasswordAutoFillDomains|String 集合|用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。 适用于处于监督模式下的设备（iOS 9.3 及更高版本）。|
|safariRequireFraudWarning|Boolean|指示在 Safari 中是否需要诈骗警告。|
|screenCaptureBlocked|Boolean|指示是否阻止用户进行屏幕截图。|
|siriBlocked|Boolean|指示是否阻止用户使用 Siri。|
|siriBlockedWhenLocked|Boolean|指示锁定时是否阻止用户使用 Siri。|
|siriBlockUserGeneratedContent|Boolean|指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。|
|siriRequireProfanityFilter|Boolean|指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。|
|softwareUpdatesEnforcedDelayInDays|Int32|设置对受监督设备取消软件更新的天数。 有效值为 0 至 90|
|softwareUpdatesForceDelayed|布尔值|指示设备在监督模式下时是否延迟软件更新的用户可见性。|
|spotlightBlockInternetResults|Boolean|指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。|
|voiceDialingBlocked|Boolean|指示是否阻止语音拨号。|
|wallpaperBlockModification|Boolean|指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。|
|wiFiConnectOnlyToConfiguredNetworks|Boolean|指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。 适用于运行 iOS 和 iPadOS 版本 14.4 及更早版本的设备。 运行 14.5+ 的设备应该使用设置"WiFiConnectToAllowedNetworksOnlyForced"。|
|classroomForceRequestPermissionToLeaveClasses|布尔值|指示通过 Classroom 参加非托管课程的学生在尝试离开 iOS 11.3 及更高版本的 (课程时是否将请求教师) 。|
|keychainBlockCloudSync|布尔值|指示是否阻止 iCloud 密钥链同步。 需要适用于 iOS 13 及更高版本的受监督设备。|
|pkiBlockOTAUpdates|布尔值|指示是否阻止非空 PKI 更新。 如果此限制设置为 false，将不会在 iOS 7.0 (禁用 CRL 和 OCSP 检查) 。|
|privacyForceLimitAdTracking|布尔值|指示广告跟踪是否受限。 (iOS 7.0 及更高版本) 。|
|enterpriseBookBlockBackup|布尔值|指示是否阻止Enterprise备份书籍。|
|enterpriseBookBlockMetadataSync|布尔值|指示是否阻止Enterprise备注和突出显示同步。|
|airPrintBlocked|布尔值|指示 iOS 11.0 (是否阻止 AirPrint) 。|
|airPrintBlockCredentialsStorage|布尔值|指示在 iOS 11.0 及更高版本 (是否阻止用于 Airprint 的用户名和密码的密钥链) 。|
|airPrintForceTrustedTLS|布尔值|指示在 iOS 11.0 及更高版本中，TLS 打印通信 (信任证书) 。|
|airPrintBlockiBeaconDiscovery|布尔值|指示是否阻止 iBeacon 发现 AirPrint 打印机。 这可以防止恶意的 AirPrint 蓝牙信号对 iOS 11.0 (及更高版本的网络通信进行网络钓鱼) 。|
|filesNetworkDriveAccessBlocked|布尔值|指示设备是否可以使用 SMB 协议中的服务器消息块访问网络 (或其他) 资源。 适用于运行 iOS 和 iPadOS 版本 13.0 及更高版本的设备。|
|filesUsbDriveAccessBlocked|布尔值|指示具有访问权限的设备能否连接到 USB 驱动器上并打开文件。 适用于运行 iOS 和 iPadOS 版本 13.0 及更高版本的设备。|
|wifiPowerOnForced|布尔值|指示设备是否Wi-Fi保持打开状态，即使设备处于飞行模式。 适用于运行 iOS 和 iPadOS 版本 13.0 及更高版本的设备。|
|blockSystemAppRemoval|布尔值|指示在受监督的设备 (iOS 11.0 及更高版本上是否阻止从设备删除系统) 。|
|vpnBlockCreation|布尔值|指示在 iOS 11.0 (或更高版本中是否阻止创建 VPN) 。|
|appRemovalBlocked|布尔值|指示是否允许删除应用。|
|usbRestrictedModeBlocked|布尔值|指示是否允许在 iOS 11.4.1 (设备锁定时连接到 USB) 。|
|passwordBlockAutoFill|布尔值|指示是否允许在 iOS 12.0 (自动填充密码) 。|
|passwordBlockProximityRequests|布尔值|指示是否阻止从 iOS 12.0 (及更高版本的附近设备请求) 。|
|passwordBlockAirDropSharing|布尔值|指示是否阻止使用 iOS 12.0 及更高版本的 AirDrop 密码功能共享) 。|
|dateAndTimeForceSetAutomatically|布尔值|指示日期和时间"自动设置"功能是否已启用，并且用户 (iOS 12.0 及更高版本) 。|
|contactsAllowManagedToUnmanagedWrite|布尔值|指示托管应用是否可以将联系人写入 iOS 12.0 及更高版本 (非托管联系人) 。|
|contactsAllowUnmanagedToManagedRead|布尔值|指示非托管应用是否可以从 iOS 12.0 (或更高版本的托管联系人帐户) 。|
|cellularBlockPersonalHotspotModification|布尔值|指示是否阻止用户修改 iOS 12.2 (或更高版本的个人热点) 。|
|continuousPathKeyboardBlocked|布尔值|指示在 iOS 13 或更高版本的设备受监督时 (连续路径) 。|
|findMyDeviceInFindMyAppBlocked|布尔值|指示在 iOS 13 或更高版本中监督设备时 (查找我的) 。|
|findMyFriendsInFindMyAppBlocked|布尔值|指示在 iOS 13 或更高版本中监督设备时是否 (查找我的好友) 。|
|iTunesBlocked|布尔值|指示是否阻止 iTunes 应用。 需要适用于 iOS 13 及更高版本的受监督设备。|
|sharedDeviceBlockTemporarySessions|布尔值|指示是否阻止 iOS 13.4 或更高版本上的共享 iPad (临时) 。|
|appClipsBlocked|布尔值|阻止用户添加任何应用剪辑并删除设备上的任何现有应用剪辑。|
|applePersonalizedAdsBlocked|布尔值|如果为 true，限制 Apple 个性化广告。 在 iOS 14 及更高版本中可用。|
|nfcBlocked|Boolean|禁用 NFC 以防止设备与其他支持 NFC 的设备配对。 适用于运行 14.2 及更高版本的 iOS/iPadOS 设备。|
|autoUnlockBlocked|布尔值|阻止用户使用 Apple Watch 解锁其设备。 适用于运行 iOS 和 iPadOS 版本 14.5 及更高版本的设备。|
|unpairedExternalBootToRecoveryAllowed|布尔值|允许用户使用未配对的设备将设备启动到恢复模式。 适用于运行 iOS 和 iPadOS 版本 14.5 及更高版本的设备。|
|onDeviceOnlyDictationForced|布尔值|禁用与 Siri 服务器的连接，以便用户不能使用 Siri 听写文本。 适用于运行 iOS 和 iPadOS 版本 14.5 及更高版本的设备。|
|kioskModeAppType|[iosKioskModeAppType](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|在展台模式下运行的应用类型。 可取值为：`notConfigured`、`appStoreApp`、`managedApp`、`builtInApp`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
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
  "@odata.type": "microsoft.graph.iosGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
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
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsVisibilityListType": "String",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "String"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "esimBlockModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeBlockAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeBlockRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeBlockScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeBlockTouchscreen": true,
  "kioskModeEnableVoiceControl": true,
  "kioskModeAllowVoiceControlModification": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "String",
  "kioskModeBuiltInAppId": "String",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "String",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "String",
    "tvRating": "String"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "String",
          "publisher": "String",
          "appStoreUrl": "String",
          "appId": "String"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "String",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 1024,
  "passcodeMinimumLength": 1024,
  "passcodeMinutesOfInactivityBeforeLock": 1024,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passcodeMinimumCharacterSetCount": 1024,
  "passcodePreviousPasscodeBlockCount": 1024,
  "passcodeSignInFailureCountBeforeWipe": 1024,
  "passcodeRequiredType": "String",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "String",
  "safariManagedDomains": [
    "String"
  ],
  "safariPasswordAutoFillDomains": [
    "String"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 1024,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "filesNetworkDriveAccessBlocked": true,
  "filesUsbDriveAccessBlocked": true,
  "wifiPowerOnForced": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "iTunesBlocked": true,
  "sharedDeviceBlockTemporarySessions": true,
  "appClipsBlocked": true,
  "applePersonalizedAdsBlocked": true,
  "nfcBlocked": true,
  "autoUnlockBlocked": true,
  "unpairedExternalBootToRecoveryAllowed": true,
  "onDeviceOnlyDictationForced": true,
  "kioskModeAppType": "String"
}
```




