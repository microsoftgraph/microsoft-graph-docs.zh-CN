---
title: 创建 iosGeneralDeviceConfiguration
description: 创建新的 iosGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e27adb28967d88519e9be6f29fbcf095cedbffa
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730860"
---
# <a name="create-iosgeneraldeviceconfiguration"></a>创建 iosGeneralDeviceConfiguration

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。

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
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 iosGeneralDeviceConfiguration 对象的 JSON 表示形式。

下表显示创建 iosGeneralDeviceConfiguration 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|说明|字符串|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
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
|appStoreBlocked|Boolean|指示是否阻止用户使用 App Store。 需要 iOS 13 及更高版本的监督设备。|
|appStoreBlockInAppPurchases|Boolean|指示是否阻止用户进行应用内购买。|
|appStoreBlockUIAppInstallation|Boolean|指示是否阻止 App Store 应用，而不通过主机应用限制安装。 仅适用于监督模式（iOS 9.0 及更高版本）。|
|appStoreRequirePassword|Boolean|指示使用 App Store 时是否需要密码。|
|bluetoothBlockModification|Boolean|指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。|
|cameraBlocked|Boolean|指示是否阻止用户访问设备的照相机。 需要 iOS 13 及更高版本的监督设备。|
|cellularBlockDataRoaming|Boolean|指示是否阻止数据漫游。|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Boolean|指示漫游时是否阻止全局背景提取。|
|cellularBlockPerAppDataModification|Boolean|指示设备处于监督模式时是否允许更改手机应用数据使用设置。|
|cellularBlockPersonalHotspot|Boolean|指示是否阻止个人热点。|
|cellularBlockVoiceRoaming|Boolean|指示是否阻止语音漫游。|
|certificatesBlockUntrustedTlsCertificates|Boolean|指示是否阻止不受信任的 TLS 证书。|
|classroomAppBlockRemoteScreenObservation|Boolean|指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。|
|classroomAppForceUnpromptedScreenObservation|Boolean|指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。|
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
|enterpriseAppBlockTrustModification|Boolean|\[已弃用\] 配置此设置并将值设置为“true”对设备没有影响。|
|faceTimeBlocked|Boolean|指示是否阻止用户使用 FaceTime。 需要 iOS 13 及更高版本的监督设备。|
|findMyFriendsBlocked|Boolean|指示在设备处于监督模式时是否阻止对“查找我的好友”的更改。|
|gamingBlockGameCenterFriends|Boolean|指示是否阻止用户在 Game Center 中拥有好友。 需要 iOS 13 及更高版本的监督设备。|
|gamingBlockMultiplayer|Boolean|指示是否阻止用户使用多人游戏。 需要 iOS 13 及更高版本的监督设备。|
|gameCenterBlocked|Boolean|指示设备处于监督模式时是否阻止用户使用 Game Center。|
|hostPairingBlocked|Boolean|指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。|
|iBooksStoreBlocked|Boolean|指示设备处于监督模式时是否阻止用户使用 iBooks Store。|
|iBooksStoreBlockErotica|Boolean|指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。|
|iCloudBlockActivityContinuation|Boolean|指示是否阻止用户继续在 iOS 设备上开始的工作到另一个 iOS 或 macOS 设备。|
|iCloudBlockBackup|Boolean|指示是否阻止 iCloud 备份。 需要 iOS 13 及更高版本的监督设备。|
|iCloudBlockDocumentSync|Boolean|指示是否阻止 iCloud 文档同步。需要 iOS 13 及更高版本的监督设备。|
|iCloudBlockManagedAppsSync|Boolean|指示是否阻止托管应用云同步。|
|iCloudBlockPhotoLibrary|Boolean|指示是否阻止 iCloud 照片库。|
|iCloudBlockPhotoStreamSync|Boolean|指示是否阻止 iCloud 照片流同步。|
|iCloudBlockSharedPhotoStream|Boolean|指示是否阻止共享照片流。|
|iCloudRequireEncryptedBackup|Boolean|指示是否要求加密备份到 iCloud 的数据。|
|iTunesBlockExplicitContent|Boolean|指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。 需要 iOS 13 及更高版本的监督设备。|
|iTunesBlockMusicService|Boolean|指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。|
|iTunesBlockRadio|Boolean|指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。|
|keyboardBlockAutoCorrect|Boolean|指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。|
|keyboardBlockDictation|Boolean|指示设备处于监督模式时是否阻止用户使用听写输入。|
|keyboardBlockPredictive|Boolean|指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。|
|keyboardBlockShortcuts|Boolean|指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。|
|keyboardBlockSpellCheck|Boolean|指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。|
|kioskModeAllowAssistiveSpeak|Boolean|指示在展台模式下是否允许辅助朗读。|
|kioskModeAllowAssistiveTouchSettings|Boolean|指示在展台模式下是否允许访问辅助触摸设置。|
|kioskModeAllowAutoLock|Boolean|指示在展台模式下是否允许设备自动锁定。 此属性的功能在 OS 默认情况下是冗余的，并且已弃用。 请改用 KioskModeBlockAutoLock。|
|kioskModeAllowColorInversionSettings|Boolean|指示在展台模式下是否允许访问颜色反转设置。|
|kioskModeAllowRingerSwitch|Boolean|指示在展台模式下是否允许使用响铃开关。 此属性的功能在 OS 默认情况下是冗余的，并且已弃用。 请改用 KioskModeBlockRingerSwitch。|
|kioskModeAllowScreenRotation|Boolean|指示在展台模式下是否允许屏幕旋转。 此属性的功能在 OS 默认情况下是冗余的，并且已弃用。 请改用 KioskModeBlockScreenRotation。|
|kioskModeAllowSleepButton|Boolean|指示在展台模式下是否允许使用睡眠按钮。 此属性的功能在 OS 默认情况下是冗余的，并且已弃用。 请改用 KioskModeBlockSleepButton。|
|kioskModeAllowTouchscreen|Boolean|指示在展台模式下是否允许使用触摸屏。 此属性的功能在 OS 默认情况下是冗余的，并且已弃用。 请改用 KioskModeBlockTouchscreen。|
|kioskModeAllowVoiceOverSettings|Boolean|指示在展台模式下是否允许访问语音插入设置。|
|kioskModeAllowVolumeButtons|Boolean|指示在展台模式下是否允许使用音量按钮。 此属性的功能在 OS 默认情况下是冗余的，并且已弃用。 请改用 KioskModeBlockVolumeButtons。|
|kioskModeAllowZoomSettings|Boolean|指示在展台模式下是否允许访问缩放设置。|
|kioskModeAppStoreUrl|String|指向 App Store 中要用于展台模式的应用的 URL。 如果 KioskModeManagedAppId 未知，请使用此方法。|
|kioskModeBuiltInAppId|String|用于展台模式的内置应用的 ID。 未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。|
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
|mediaContentRatingApps|[ratingAppsType](../resources/intune-deviceconfig-ratingappstype.md)|应用的媒体内容分级设置。 可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。|
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
|passcodeSignInFailureCountBeforeWipe|Int32|擦除设备前允许登录失败的次数。 有效值 2 到 11|
|passcodeRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|必需的密码类型。 可取值为：`deviceDefault`、`alphanumeric`、`numeric`。|
|passcodeRequired|Boolean|指示是否需要密码。|
|podcastsBlocked|Boolean|指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。|
|safariBlockAutofill|Boolean|指示在 Safari 中是否阻止用户使用自动填充。 需要 iOS 13 及更高版本的监督设备。|
|safariBlockJavaScript|Boolean|指示在 Safari 中是否阻止 JavaScript。|
|safariBlockPopups|Boolean|指示在 Safari 中是否阻止弹出窗口。|
|safariBlocked|Boolean|指示是否阻止用户使用 Safari。 需要 iOS 13 及更高版本的监督设备。|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Safari 的 Cookie 设置。 可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。|
|safariManagedDomains|String 集合|与此处列出的模式匹配的 URL 将被视为托管。|
|safariPasswordAutoFillDomains|String 集合|用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。 适用于处于监督模式下的设备（iOS 9.3 及更高版本）。|
|safariRequireFraudWarning|Boolean|指示在 Safari 中是否需要诈骗警告。|
|screenCaptureBlocked|Boolean|指示是否阻止用户进行屏幕截图。|
|siriBlocked|Boolean|指示是否阻止用户使用 Siri。|
|siriBlockedWhenLocked|Boolean|指示锁定时是否阻止用户使用 Siri。|
|siriBlockUserGeneratedContent|Boolean|指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。|
|siriRequireProfanityFilter|Boolean|指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。|
|spotlightBlockInternetResults|Boolean|指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。|
|voiceDialingBlocked|Boolean|指示是否阻止语音拨号。|
|wallpaperBlockModification|Boolean|指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。|
|wiFiConnectOnlyToConfiguredNetworks|Boolean|指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。 适用于运行 iOS 和 iPadOS 版本 14.4 及更低版本的设备。 运行 14.5+ 的设备应使用设置“WiFiConnectToAllowedNetworksOnlyForced”。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 7841

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
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
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
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
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 8013

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
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
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```





