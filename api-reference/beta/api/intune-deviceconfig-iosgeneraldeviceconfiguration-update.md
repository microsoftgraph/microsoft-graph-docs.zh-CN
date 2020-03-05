---
title: 更新 iosGeneralDeviceConfiguration
description: 更新 iosGeneralDeviceConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 824c4dccc62f40ff9f442ad5466509a8ae996ce8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448906"
---
# <a name="update-iosgeneraldeviceconfiguration"></a>更新 iosGeneralDeviceConfiguration

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。

下表显示创建 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String 集合|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|布尔|指示基础设备配置是否支持作用域标记的分配。 如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。 这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|适用于此策略的操作系统版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|accountBlockModification|布尔|指示设备处于监督模式时是否允许帐户修改。|
|activationLockAllowWhenSupervised|布尔|指示设备处于监督模式时是否允许激活锁定。|
|airDropBlocked|布尔|指示设备处于监督模式时是否允许 AirDrop。|
|airDropForceUnmanagedDropTarget|布尔|指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。|
|airPlayForcePairingPasswordForOutgoingRequests|布尔|指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。|
|appleWatchBlockPairing|布尔|指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。|
|appleWatchForceWristDetection|布尔|指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。|
|appleNewsBlocked|布尔|指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。|
|appsSingleAppModeList|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|获取或设置允许自主进入单个应用模式的 iOS 应用列表。 仅限监督模式。 iOS 7.0 及更高版本。 该集合最多可包含 500 个元素。|
|appsVisibilityList|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。 该集合最多可包含 10000 个元素。|
|appsVisibilityListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|位于 AppsVisibilityList 中的列表类型。 可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。|
|appStoreBlockAutomaticDownloads|布尔|指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。|
|appStoreBlocked|Boolean|指示是否阻止用户使用 App Store。 需要受监督设备的 iOS 13 及更高版本。|
|appStoreBlockInAppPurchases|布尔|指示是否阻止用户进行应用内购买。|
|appStoreBlockUIAppInstallation|布尔|指示是否阻止 App Store 应用，而不通过主机应用限制安装。 仅适用于监督模式（iOS 9.0 及更高版本）。|
|appStoreRequirePassword|布尔|指示使用 App Store 时是否需要密码。|
|autoFillForceAuthentication|布尔|指示在 Safari 中的 autofilling 密码和信用卡信息之前是否强制进行用户身份验证，以及受监督的设备上的其他应用。|
|bluetoothBlockModification|布尔|指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。|
|cameraBlocked|布尔|指示是否阻止用户访问设备的照相机。 需要受监督设备的 iOS 13 及更高版本。|
|cellularBlockDataRoaming|布尔|指示是否阻止数据漫游。|
|cellularBlockGlobalBackgroundFetchWhileRoaming|布尔|指示漫游时是否阻止全局背景提取。|
|cellularBlockPerAppDataModification|布尔|指示设备处于监督模式时是否允许更改手机应用数据使用设置。|
|cellularBlockPersonalHotspot|布尔|指示是否阻止个人热点。|
|cellularBlockPlanModification|布尔|指示是否允许用户在受监督的设备上更改移动电话计划的设置。|
|cellularBlockVoiceRoaming|布尔|指示是否阻止语音漫游。|
|certificatesBlockUntrustedTlsCertificates|布尔|指示是否阻止不受信任的 TLS 证书。|
|classroomAppBlockRemoteScreenObservation|布尔|指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。|
|classroomAppForceUnpromptedScreenObservation|布尔|指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。|
|classroomForceAutomaticallyJoinClasses|布尔|指示设备处于监督模式时是否自动向教师的请求授予权限，而不提示学生。|
|classroomForceUnpromptedAppAndDeviceLock|布尔|指示是否允许教师在不提示学生的情况下锁定应用或设备。 仅限监督模式。|
|compliantAppsList|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。 该集合最多可包含 10000 个元素。|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|位于 AppComplianceList 中的列表。 可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。|
|configurationProfileBlockChanges|布尔|指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。|
|definitionLookupBlocked|布尔|指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。|
|deviceBlockEnableRestrictions|布尔|指示设备处于监督模式时是否允许用户在设备设置中启用限制。|
|deviceBlockEraseContentAndSettings|布尔|指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。|
|deviceBlockNameModification|布尔|指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。|
|diagnosticDataBlockSubmission|布尔|指示是否阻止诊断数据提交。|
|diagnosticDataBlockSubmissionModification|布尔|指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。|
|documentsBlockManagedDocumentsInUnmanagedApps|布尔|指示是否阻止用户查看非托管应用中的托管文档。|
|documentsBlockUnmanagedDocumentsInManagedApps|布尔|指示是否阻止用户查看托管应用中的非托管文档。|
|emailInDomainSuffixes|String 集合|缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。|
|enterpriseAppBlockTrust|布尔|指示是否阻止用户信任企业应用。|
|enterpriseAppBlockTrustModification|Boolean|指示是否阻止用户修改企业应用信任设置。|
|esimBlockModification|布尔|指示是否允许在受监督的设备的 eSIM 卡上添加或删除手机网络计划。|
|faceTimeBlocked|布尔|指示是否阻止用户使用 FaceTime。 需要受监督设备的 iOS 13 及更高版本。|
|findMyFriendsBlocked|布尔|指示设备处于监督模式时是否阻止更改以查找我的好友。|
|gamingBlockGameCenterFriends|布尔|指示是否阻止用户在 Game Center 中拥有好友。 需要受监督设备的 iOS 13 及更高版本。|
|gamingBlockMultiplayer|布尔|指示是否阻止用户使用多人游戏。 需要受监督设备的 iOS 13 及更高版本。|
|gameCenterBlocked|布尔|指示设备处于监督模式时是否阻止用户使用 Game Center。|
|hostPairingBlocked|布尔|指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。|
|iBooksStoreBlocked|布尔|指示设备处于监督模式时是否阻止用户使用 iBooks Store。|
|iBooksStoreBlockErotica|布尔|指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。|
|iCloudBlockActivityContinuation|布尔|指示是否阻止用户将其在 iOS 设备上启动的工作继续到另一个 iOS 或 macOS 设备。|
|iCloudBlockBackup|布尔|指示是否阻止 iCloud 备份。 需要受监督设备的 iOS 13 及更高版本。|
|iCloudBlockDocumentSync|布尔|指示是否阻止 iCloud 文档同步。需要受监督设备的 iOS 13 及更高版本。|
|iCloudBlockManagedAppsSync|布尔|指示是否阻止托管应用云同步。|
|iCloudBlockPhotoLibrary|布尔|指示是否阻止 iCloud 照片库。|
|iCloudBlockPhotoStreamSync|布尔|指示是否阻止 iCloud 照片流同步。|
|iCloudBlockSharedPhotoStream|布尔|指示是否阻止共享照片流。|
|iCloudRequireEncryptedBackup|布尔|指示是否要求加密备份到 iCloud 的数据。|
|iTunesBlockExplicitContent|布尔|指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。 需要受监督设备的 iOS 13 及更高版本。|
|iTunesBlockMusicService|布尔|指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。|
|iTunesBlockRadio|布尔|指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。|
|keyboardBlockAutoCorrect|布尔|指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。|
|keyboardBlockDictation|布尔|指示设备处于监督模式时是否阻止用户使用听写输入。|
|keyboardBlockPredictive|布尔|指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。|
|keyboardBlockShortcuts|布尔|指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。|
|keyboardBlockSpellCheck|布尔|指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。|
|kioskModeAllowAssistiveSpeak|布尔|指示在展台模式下是否允许辅助朗读。|
|kioskModeAllowAssistiveTouchSettings|布尔|指示在展台模式下是否允许访问辅助触摸设置。|
|kioskModeAllowAutoLock|布尔|指示在展台模式下是否允许设备自动锁定。 此属性的功能对于 OS 默认值是多余的，已弃用。 请改用 KioskModeBlockAutoLock。|
|kioskModeBlockAutoLock|布尔|指示在展台模式下是否阻止设备自动锁定。|
|kioskModeAllowColorInversionSettings|布尔|指示在展台模式下是否允许访问颜色反转设置。|
|kioskModeAllowRingerSwitch|Boolean|指示在展台模式下是否允许使用响铃开关。 此属性的功能对于 OS 默认值是多余的，已弃用。 请改用 KioskModeBlockRingerSwitch。|
|kioskModeBlockRingerSwitch|布尔|指示在展台模式下是否阻止使用铃声开关。|
|kioskModeAllowScreenRotation|布尔|指示在展台模式下是否允许屏幕旋转。 此属性的功能对于 OS 默认值是多余的，已弃用。 请改用 KioskModeBlockScreenRotation。|
|kioskModeBlockScreenRotation|布尔|指示在展台模式下是否阻止屏幕旋转。|
|kioskModeAllowSleepButton|布尔|指示在展台模式下是否允许使用睡眠按钮。 此属性的功能对于 OS 默认值是多余的，已弃用。 请改用 KioskModeBlockSleepButton。|
|kioskModeBlockSleepButton|布尔|指示在展台模式下是否阻止使用 "睡眠" 按钮。|
|kioskModeAllowTouchscreen|布尔|指示在展台模式下是否允许使用触摸屏。 此属性的功能对于 OS 默认值是多余的，已弃用。 请改用 KioskModeBlockTouchscreen。|
|kioskModeBlockTouchscreen|布尔|指示在展台模式下是否阻止使用触摸屏。|
|kioskModeEnableVoiceControl|布尔|指示是否在展台模式下启用语音控制。|
|kioskModeAllowVoiceControlModification|布尔|指示是否允许用户在展台模式下切换语音控件。|
|kioskModeAllowVoiceOverSettings|布尔|指示在展台模式下是否允许访问语音插入设置。|
|kioskModeAllowVolumeButtons|布尔|指示在展台模式下是否允许使用音量按钮。 此属性的功能对于 OS 默认值是多余的，已弃用。 请改用 KioskModeBlockVolumeButtons。|
|kioskModeBlockVolumeButtons|布尔|指示在展台模式下是否阻止音量按钮。|
|kioskModeAllowZoomSettings|布尔|指示在展台模式下是否允许访问缩放设置。|
|kioskModeAppStoreUrl|String|指向 App Store 中要用于展台模式的应用的 URL。 如果 KioskModeManagedAppId 未知，请使用此方法。|
|kioskModeBuiltInAppId|String|用于展台模式的内置应用程序的 ID。 在未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。|
|kioskModeRequireAssistiveTouch|布尔|指示在展台模式下是否要求辅助触摸。|
|kioskModeRequireColorInversion|布尔|指示在展台模式下是否要求颜色反转。|
|kioskModeRequireMonoAudio|布尔|指示在展台模式下是否要求单声道音频。|
|kioskModeRequireVoiceOver|布尔|指示在展台模式下是否要求语音插入。|
|kioskModeRequireZoom|布尔|指示在展台模式下是否要求缩放。|
|kioskModeManagedAppId|String|用于展台模式的应用的托管应用 ID。 如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。|
|lockScreenBlockControlCenter|布尔|指示是否阻止用户在锁定屏幕上使用控制中心。|
|lockScreenBlockNotificationView|布尔|指示是否阻止用户在锁定屏幕上使用通知视图。|
|lockScreenBlockPassbook|布尔|指示设备处于锁定状态时是否阻止用户使用 Passbook。|
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
|messagesBlocked|布尔|指示是否阻止用户使用受监督设备上的消息应用。|
|notificationsBlockSettingsModification|布尔|指示是否允许修改通知设置（iOS 9.3 及更高版本）。|
|passcodeBlockFingerprintUnlock|布尔|指示是否阻止指纹解锁。|
|passcodeBlockFingerprintModification|布尔|在监督模式下阻止修改已注册的 Touch ID 指纹。|
|passcodeBlockModification|布尔|指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。|
|passcodeBlockSimple|布尔|指示是否阻止简单密码。|
|passcodeExpirationDays|Int32|密码过期前的天数。 有效值为 1 至 65535|
|passcodeMinimumLength|Int32|密码的最小长度。 有效值为 4 至 14|
|passcodeMinutesOfInactivityBeforeLock|Int32|需要密码之前的不活动分钟数。|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|passcodeMinimumCharacterSetCount|Int32|密码必须包含的字符集数。 有效值为 0 至 4|
|passcodePreviousPasscodeBlockCount|Int32|要阻止的以前密码的数量。 有效值为 1 至 24|
|passcodeSignInFailureCountBeforeWipe|Int32|擦除设备前允许登录失败的次数。 有效值为 4 至 11|
|passcodeRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|必需的密码类型。 可取值为：`deviceDefault`、`alphanumeric`、`numeric`。|
|passcodeRequired|布尔|指示是否需要密码。|
|podcastsBlocked|布尔|指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。|
|proximityBlockSetupToNewDevice|布尔|指示是否启用提示以在受监督的设备上安装附近设备。|
|safariBlockAutofill|布尔|指示在 Safari 中是否阻止用户使用自动填充。 需要受监督设备的 iOS 13 及更高版本。|
|safariBlockJavaScript|布尔|指示在 Safari 中是否阻止 JavaScript。|
|safariBlockPopups|布尔|指示在 Safari 中是否阻止弹出窗口。|
|safariBlocked|Boolean|指示是否阻止用户使用 Safari。 需要受监督设备的 iOS 13 及更高版本。|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Safari 的 Cookie 设置。 可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。|
|safariManagedDomains|String 集合|与此处列出的模式匹配的 URL 将被视为托管。|
|safariPasswordAutoFillDomains|String 集合|用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。 适用于处于监督模式下的设备（iOS 9.3 及更高版本）。|
|safariRequireFraudWarning|布尔|指示在 Safari 中是否需要诈骗警告。|
|screenCaptureBlocked|布尔|指示是否阻止用户进行屏幕截图。|
|siriBlocked|布尔|指示是否阻止用户使用 Siri。|
|siriBlockedWhenLocked|布尔|指示锁定时是否阻止用户使用 Siri。|
|siriBlockUserGeneratedContent|布尔|指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。|
|siriRequireProfanityFilter|布尔|指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。|
|softwareUpdatesEnforcedDelayInDays|Int32|设置受监督的设备 delyed 软件更新的天数。 有效值为 0 至 90|
|softwareUpdatesForceDelayed|布尔|指示设备处于监督模式时是否延迟用户对软件更新的可见性。|
|spotlightBlockInternetResults|布尔|指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。|
|voiceDialingBlocked|布尔|指示是否阻止语音拨号。|
|wallpaperBlockModification|布尔|指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。|
|wiFiConnectOnlyToConfiguredNetworks|Boolean|指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。|
|classroomForceRequestPermissionToLeaveClasses|布尔|指示在非托管课程中通过教室注册的学生是否会在尝试离开该课程（iOS 11.3 及更高版本）时向教师请求权限。|
|keychainBlockCloudSync|布尔|指示是否阻止 iCloud 密钥链同步。 需要受监督设备的 iOS 13 及更高版本。|
|pkiBlockOTAUpdates|布尔|指示是否阻止无线 PKI 更新。 将此限制设置为 false 不会禁用 CRL 和 OCSP 检查（iOS 7.0 及更高版本）。|
|privacyForceLimitAdTracking|布尔|指示广告跟踪是否受限制。（iOS 7.0 及更高版本）。|
|enterpriseBookBlockBackup|布尔|指示是否阻止企业书籍备份。|
|enterpriseBookBlockMetadataSync|布尔|指示是否阻止企业书籍笔记和突出显示同步。|
|airPrintBlocked|布尔|指示是否阻止 AirPrint （iOS 11.0 及更高版本）。|
|airPrintBlockCredentialsStorage|布尔|指示是否阻止 Airprint 的用户名和密码的密钥链存储（iOS 11.0 及更高版本）。|
|airPrintForceTrustedTLS|布尔|指示 TLS 打印通信是否需要受信任的证书（iOS 11.0 及更高版本）。|
|airPrintBlockiBeaconDiscovery|布尔|指示是否阻止 AirPrint 打印机的 iBeacon 发现。 这样可以防止虚假的 AirPrint 蓝牙信号免受网络流量（iOS 11.0 及更高版本）的欺骗。|
|filesNetworkDriveAccessBlocked|布尔|指示设备是否可以使用服务器消息块（SMB）协议访问网络服务器上的文件或其他资源。 适用于运行 iOS 和 iPadOS 版本13.0 及更高版本的设备。|
|filesUsbDriveAccessBlocked|布尔|指示带 access 的 sevices 是否可以连接到 USB 驱动器上的文件并打开文件。 适用于运行 iOS 和 iPadOS 版本13.0 及更高版本的设备。|
|wifiPowerOnForced|布尔|指示 Wi-fi 是否仍处于打开状态，即使设备处于飞行模式时也是如此。 适用于运行 iOS 和 iPadOS 版本13.0 及更高版本的设备。|
|blockSystemAppRemoval|布尔|指示是否在受监督的设备（iOS 11.0 及更高版本）上阻止从设备中删除系统应用程序。|
|vpnBlockCreation|布尔|指示是否阻止创建 VPN 配置（iOS 11.0 及更高版本）。|
|appRemovalBlocked|布尔|指示是否允许删除应用程序。|
|usbRestrictedModeBlocked|布尔|指示是否允许在锁定设备时连接到 USB 附件（iOS 11.4.1 及更高版本）。|
|passwordBlockAutoFill|布尔|指示是否允许自动填充密码功能（iOS 12.0 及更高版本）。|
|passwordBlockProximityRequests|布尔|指示是否阻止来自附近设备（iOS 12.0 及更高版本）发出请求的密码。|
|passwordBlockAirDropSharing|布尔|指示是否阻止使用 AirDrop 密码的共享密码功能 iOS 12.0 及更高版本）。|
|dateAndTimeForceSetAutomatically|布尔|指示是否启用日期和时间 "设置自动设置" 功能，以及用户是否无法关闭该功能（iOS 12.0 及更高版本）。|
|contactsAllowManagedToUnmanagedWrite|布尔|指示托管应用程序是否可以将联系人写入非托管联系人帐户（iOS 12.0 及更高版本）。|
|contactsAllowUnmanagedToManagedRead|布尔|指示非托管应用是否可以从托管联系人帐户读取（iOS 12.0 或更高版本）。|
|cellularBlockPersonalHotspotModification|布尔|指示是否阻止用户修改个人热点设置（iOS 12.2 或更高版本）。|
|continuousPathKeyboardBlocked|布尔|指示设备受到监督时是否阻止连续路径键盘（iOS 13 或更高版本）。|
|findMyDeviceInFindMyAppBlocked|布尔|指示设备受到监督时是否阻止查找我的设备（iOS 13 或更高版本）。|
|findMyFriendsInFindMyAppBlocked|布尔|指示设备受到监督时是否阻止查找我的好友（iOS 13 或更高版本）。|
|iTunesBlocked|布尔|指示是否阻止 iTunes 应用。 需要受监督设备的 iOS 13 及更高版本。|
|kioskModeAppType|[iosKioskModeAppType](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|在展台模式下运行的应用类型。 可取值为：`notConfigured`、`appStoreApp`、`managedApp`、`builtInApp`。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 10518

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
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
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
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
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
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
    "Email In Domain Suffixes value"
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
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
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
  "kioskModeAppType": "appStoreApp"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10690

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
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
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
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
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
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
    "Email In Domain Suffixes value"
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
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
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
  "kioskModeAppType": "appStoreApp"
}
```





