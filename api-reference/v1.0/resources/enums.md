---
title: 枚举值
description: Microsoft Graph枚举值。
ms.localizationpriority: medium
ms.prod: non-product-specific
author: MSGraphDocsvTeam
doc_type: enumPageType
ms.openlocfilehash: 1288bddd70c1ee82ed3f8056a295ecf3dfbc183c
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525384"
---
# <a name="enum-values"></a>枚举值

命名空间：microsoft.graph

### <a name="accesspackageassignmentfilterbycurrentuseroptions-values"></a>accessPackageAssignmentFilterByCurrentUserOptions 值

|Member|
|:---|
|target|
|createdBy|
|unknownFutureValue|

### <a name="accesspackageassignmentrequestfilterbycurrentuseroptions-values"></a>accessPackageAssignmentRequestFilterByCurrentUserOptions 值

|Member|
|:---|
|target|
|createdBy|
|审批者|
|unknownFutureValue|

### <a name="accesspackageassignmentstate-values"></a>accessPackageAssignmentState 值

|Member|
|:---|
|delivering|
|partiallyDelivered|
|delivered|
|已过期|
|deliveryFailed|
|unknownFutureValue|

### <a name="accesspackagecatalogstate-values"></a>accessPackageCatalogState 值

|Member|
|:---|
|unpublished|
|published|
|unknownFutureValue|

### <a name="accesspackagecatalogtype-values"></a>accessPackageCatalogType 值

|Member|
|:---|
|userManaged|
|serviceDefault|
|serviceManaged|
|unknownFutureValue|

### <a name="accesspackageexternaluserlifecycleaction-values"></a>accessPackageExternalUserLifecycleAction 值

|Member|
|:---|
|无|
|blockSignIn|
|blockSignInAndDelete|
|unknownFutureValue|

### <a name="accesspackagefilterbycurrentuseroptions-values"></a>accessPackageFilterByCurrentUserOptions 值

|Member|
|:---|
|allowedRequestor|
|unknownFutureValue|

### <a name="accesspackagerequeststate-values"></a>accessPackageRequestState 值

|Member|
|:---|
|submitted|
|pendingApproval|
|delivering|
|delivered|
|deliveryFailed|
|denied|
|scheduled|
|canceled|
|partiallyDelivered|
|unknownFutureValue|

### <a name="accesspackagerequesttype-values"></a>accessPackageRequestType 值

|Member|
|:---|
|notSpecified|
|userAdd|
|userUpdate|
|userRemove|
|adminAdd|
|adminUpdate|
|adminRemove|
|systemAdd|
|systemUpdate|
|systemRemove|
|onBehalfAdd|
|unknownFutureValue|

### <a name="accesspackagesubjecttype-values"></a>accessPackageSubjectType 值

|Member|
|:---|
|notSpecified|
|用户|
|servicePrincipal|
|unknownFutureValue|

### <a name="connectedorganizationstate-values"></a>connectedOrganizationState 值

|Member|
|:---|
|已配置|
|已建议|

### <a name="accessreviewinstancedecisionitemfilterbycurrentuseroptions-values"></a>accessReviewInstanceDecisionItemFilterByCurrentUserOptions 值 

|Member|
|:---|
|reviewer|
|unknownFutureValue|

### <a name="volumetype-values"></a>volumeType 值

|Member|
|:---|
|operatingSystemVolume|
|fixedDataVolume|
|removableDataVolume|
|unknownFutureValue|

### <a name="filtermode-values"></a>filterMode 值

|Member|
|:---|
|include|
|exclude|

### <a name="lifecycleeventtype-values"></a>lifecycleEventType 值

|Member|
|:---|
|错过|
|subscriptionRemoved|
|reauthorizationRequired|

### <a name="changetype-values"></a>changeType 值

|Member|
|:---|
|clientIpAddress|
|authenticatorApp提供|

### <a name="countrylookupmethodtype-values"></a>countryLookupMethodType 值

|Member|
|:---|
|clientIpAddress|
|authenticatorApp提供|

### <a name="consentrequestfilterbycurrentuseroptions-values"></a>consentRequestFilterByCurrentUserOptions 值 

|Member|
|:---|
|reviewer|
|unknownFutureValue|

### <a name="externalemailotpstate-values"></a>externalEmailOtpState 值

|Member|
|:---|
|default|
|enabled|
|disabled|
|unknownFutureValue|

### <a name="educationaddedstudentaction-values"></a>educationAddedStudentAction 值

|Member|
|:---|
|无|
|assignIfOpen|
|unknownFutureValue|

### <a name="fido2restrictionenforcementtype-values"></a>fido2RestrictionEnforcementType 值

|Member|
|:---|
|allow|
|block|

### <a name="attestationlevel-values"></a>attestationLevel 值

|Member|
|:---|
|已证明|
|notAttested|

### <a name="authenticationmethodtargettype-values"></a>authenticationMethodTargetType 值

|Member|
|:---|
|用户|
|组|

### <a name="authenticationmethodstate-values"></a>authenticationMethodState 值

|Member|
|:---|
|enabled|
|disabled|

### <a name="microsoftauthenticatorauthenticationmode-values"></a>microsoftAuthenticatorAuthenticationMode 值

|Member|
|:---|
|任意|
|push|
|deviceBasedPush|

### <a name="keystrength-values"></a>keyStrength 值

|Member|
|:---|
|normal|
|weak|
|unknown|

### <a name="authenticationmethodkeystrength-values"></a>authenticationMethodKeyStrength 值

|Member|
|:---|
|normal|
|weak|
|unknown|

### <a name="allowinvitesfrom-values"></a>allowInvitesFrom 值

|Member|
|:---|
|无|
|adminsAndGuestInviters|
|adminsGuestInvitersAndAllMembers|
|everyone|
|unknownFutureValue|

### <a name="datapolicyoperationstatus-values"></a>dataPolicyOperationStatus 值

|Member|
|:---|
|notStarted|
|running|
|complete|
|failed|
|unknownFutureValue|

### <a name="conditionalaccessdeviceplatform-values"></a>conditionalAccessDevicePlatform 值

| Member       |
|:--------------|
|android|
|iOS|
|windows|
|windowsPhone|
|macOS|
|all|
|unknownFutureValue|

### <a name="signinfrequencytype-values"></a>signinFrequencyType 值

| Member       |
|:--------------|
|days|
|hours|

### <a name="persistentbrowsersessionmode-values"></a>persistentBrowserSessionMode 值

| Member       |
|:--------------|
|始终|
|从不|

### <a name="cloudappsecuritysessioncontroltype-values"></a>cloudAppSecuritySessionControlType 值

| Member       |
|:--------------|
|mcasConfigured|
|monitorOnly|
|blockDownloads|
|unknownFutureValue|

### <a name="conditionalaccessgrantcontrol-values"></a>conditionalAccessGrantControl 值

| Member       |
|:--------------|
|block|
|mfa|
|compliantDevice|
|domainJoinedDevice|
|approvedApplication|
|compliantApplication|
|passwordChange|
|unknownFutureValue|

### <a name="conditionalaccessclientapp-values"></a>conditionalAccessClientApp 值

|Member|
|:---|
|all|
|浏览器|
|mobileAppsAndDesktopClients|
|exchangeActiveSync|
|easSupported|
|other|
|unknownFutureValue|

### <a name="conditionalaccesspolicystate-values"></a>conditionalAccessPolicyState 值

|Member|
|:---|
|enabled|
|disabled|
|enabledForReportingButNotEnforced|

#### <a name="deviceprofiletype-values"></a>deviceProfileType 值
|Member|
|:---|
|RegisteredDevice|
|SecureVM|
|Printer|
|共享的内容|
|IoT|

### <a name="appliedconditionalaccesspolicyresult-values"></a>appliedConditionalAccessPolicyResult 值 

|Member|
|:---|
|success|
|failure|
|notApplied|
|notEnabled|
|unknown|
|unknownFutureValue|

### <a name="grouptype-values"></a>groupType 值 

|Member|
|:---|
|unifiedGroups|
|azureAD|
|unknownFutureValue|

### <a name="conditionalaccessstatus-values"></a>conditionalAccessStatus 值

|Member|
|:---|
|success|
|failure|
|notApplied|
|unknownFutureValue|

### <a name="operationresult-values"></a>operationResult 值

|Member|
|:---|
|success|
|failure|
|timeout|
|unknownFutureValue|

### <a name="tone-values"></a>音调值

|Member|
|:---|
|tone0|
|tone1|
|tone2|
|tone3|
|tone4|
|tone5|
|tone6|
|tone7|
|tone8|
|tone9|
|星形|
|井号|
|a|
|b|
|c|
|d|
|flash|

### <a name="mediastate-values"></a>mediaState 值

|Member|
|:---|
|active|
|inactive|
|unknownFutureValue|

### <a name="basicstatus-values"></a>basicStatus 值

|Member|
|:---|
|active|
|inactive|

### <a name="callstate-values"></a>callState 值

|Member|
|:---|
|incoming|
|建立|
|响铃|
|established|
|hold|
|传输|
|transferAccepted|
|重定向|
|终止|
|已终止|

### <a name="calltype-values"></a>callType 值

|Member|
|:---|
|unknown|
|groupCall|
|peerToPeer|
|unknownFutureValue|

### <a name="onlinemeetingrole-values"></a>onlineMeetingRole 值

|Member|
|:---|
|attendee|
|演示者|
|unknownFutureValue|

### <a name="modality-values"></a>形式值 

|Member|
|:---|
|audio|
|video|
|videoBasedScreenSharing|
|data|
|screenSharing|
|unknownFutureValue|

### <a name="calldirection-values"></a>callDirection 值

|Member|
|:---|
|incoming|
|传出|

### <a name="signinaudience-values"></a>signInAudience 值

|Member|
|:---|
|AzureADMyOrg|
|AzureADMultleOrgs|
|AzureADandPersonalMicrosoftAccount|
|PersonalMicrosoftAccount|

### <a name="groupmembershipclaims-values"></a>groupMembershipClaims 值

|Member|
|:---|
|无|
|SecurityGroup|
|全部|

### <a name="recipientscopetype-values"></a>recipientScopeType 值

|Member|
|:---|
|无|
|internal|
|external|
|externalPartner|
|externalNonPartner|

### <a name="activitytype-values"></a>activityType 值

|Member|
|:---|
|signin|
|用户|
|unknownFutureValue|

### <a name="riskdetectiontimingtype-values"></a>riskDetectionTimingType 值

|Member|
|:---|
|notDefined|
|realtime|
|nearRealtime|
|offline|
|unknownFutureValue|

### <a name="tokenissuertype-values"></a>tokenIssuerType 值

|Member|
|:---|
|AzureAD|
|ADFederationServices|
|UnknownFutureValue|

### <a name="attachmenttype-values"></a>attachmentType 值

| Member
|:--------------
| file
| 项
| 参考

### <a name="contactrelationship-values"></a>contactRelationship 值

|成员|值|说明|
|:---|:---|:---|
|父级|0|用户的父级。|
|relative|1| 用户的相对。|
|aide|2| 用户的助手。|
|一个|3| 用户的。|
|保护者|4| 用户的保护者。|
|Child|5| 用户的子级。|
|other|6 | 与用户未指定的关系。|
|unknownFutureValue|7 | 用于将来兼容性的标记值。|

### <a name="scheduleentitytheme-values"></a>scheduleEntityTheme 值

| Member
|:-------------------------
| white
| 蓝色
| 绿色
| 紫色
| 粉色
| 黄色
| 灰色
| darkBlue
| darkGreen
| darkPurple
| darkPink
| darkYellow
| unknownFutureValue


### <a name="timeoffreasonicontype-values"></a>timeOffReasonIconType 值

|Member|
|:---|
|无|
|car|
|日历|
|running|
|plane|
|firstAid|
|一个|
|notWorking|
|clock|
|将duty|
|globe|
|cup|
|phone|
|weather|
|umbrella|
|和/|
|狗|
|的|
|trafficCone|
|pin|
|一些|
|unknownFutureValue|

### <a name="workforceintegrationencryptionprotocol-values"></a>workforceIntegrationEncryptionProtocol 值

| Member
|:----------------------------
|sharedSecret
|unknownFutureValue

### <a name="workforceintegrationsupportedentities-values"></a>workforceIntegrationSupportedEntities 值

|Member|
|:---|
|无|
|Shift|
|swapRequest|
|userShiftPreferences|
|openShift|
|openShiftRequest|
|offerShiftRequest|
|unknownFutureValue|

### <a name="timezonestandard-values"></a>timeZoneStandard 值

| Member
|:-----------------
| windows
| iana


### <a name="freebusystatus-values"></a>freeBusyStatus 值

| 成员            |值
|:------------------|:-------
| free              | 0
| 暂定         | 1
| 忙碌              | 2
| oof               | 3
| workingElsewhere  | 4
| unknown           | -1


### <a name="attendeetype-values"></a>attendeeType 值

| Member
|:-------------------------
| 必需
| 可选
| resource


### <a name="externalaudiencescope-values"></a>externalAudienceScope 值

| Member
|:-------------------------
| 无
| contactsOnly
| all


### <a name="automaticrepliesstatus-values"></a>automaticRepliesStatus 值

| Member
|:-------------------------
| disabled
| alwaysEnabled
| scheduled


### <a name="calendarcolor-values"></a>calendarColor 值

| 成员     | 值
|:-----------|:----------
| 自动       | -1
| lightBlue  | 0
| lightGreen | 1
| lightOrange| 2
| lightGray  | 3
| lightYellow| 4
| lightTeal  | 5
| lightPink  | 6 
| lightBrown | 7 
| lightRed   | 8 
| maxColor   | 9 

### <a name="educationexternalsource-values"></a>educationExternalSource 值

| Member             |
| :----------------- |
| sis                |
| 手动             |
| unknownFutureValue |

### <a name="educationgender-values"></a>educationGender 值

| Member
|:-------------------------
| female
| male
| other
| unknownFutureValue


### <a name="eventtype-values"></a>eventType 值

| Member
|:-------------------------
| singleInstance
| occurrence
| 异常
| seriesMaster


### <a name="sensitivity-values"></a>敏感度值

| Member
|:-------------------------
| normal
| personal
| private
| confidential


### <a name="importance-values"></a>重要性值

| Member
|:-------------------------
| low
| normal
| high

### <a name="educationuserrole-values"></a>educationUserRole 值

| Member             |
| :----------------- |
| student            |
| teacher            |
| 无               |
| unknownFutureValue |

### <a name="meetingmessagetype-values"></a>meetingMessageType 值

| Member
|:-----------------
| 无
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTenativelyAccepted
| meetingDeclined


### <a name="followupflagstatus-values"></a>followupFlagStatus 值

| Member
|:-------------------------
| notFlagged
| complete
| 已标记


### <a name="inferenceclassificationtype-values"></a>inferenceClassificationType 值

| Member
|:-----------------
| 聚焦
| other


### <a name="iosnotificationalerttype-values"></a>iosNotificationAlertType 值

| Member
|:-------------------------
| deviceDefault
| 横幅
| modal
| 无

### <a name="deviceenrollmentfailurereason-values"></a>deviceEnrollmentFailureReason 值

| Member
|:-------------
| unknown
| 身份验证
| authorization
| accountValidation
| userValidation
| deviceNotSupported
| inMaintenance
| badRequest
| featureNotSupported
| enrollmentRestrictionsEnforced
| clientDisconnected


### <a name="bodytype-values"></a>bodyType 值
| Member
|:---------
| text
| html


### <a name="locationtype-values"></a>locationType 值

| Member
|:-------------------------
| default
| conferenceRoom
| homeAddress
| businessAddress
| geoCoordinates
| streetAddress
| 区
| restaurant
| localBusiness
| postalAddress

### <a name="locationuniqueidtype-values"></a>locationUniqueIdType 值

| Member
|:-------------------------
| unknown
| locationStore
| directory
| private
| 必应


### <a name="messageactionflag-values"></a>messageActionFlag 值

| Member
|:-------------------------
| 任意
| 通话
| doNotForward
| followUp
| fyi
| 转发
| noResponseNecessary
| 阅读
| 回复
| replyToAll
| review


### <a name="onenoteuserrole-values"></a>onenoteUserRole 值

| 成员      | 值
|:------------|:------------
| 所有者       | 0
| 参与者 | 1
| 读者      | 2
| 无        | -1


### <a name="operationstatus-values"></a>operationStatus 值

| Member
|:-----------------
|NotStarted
|正在运行
|已完成
|已失败


### <a name="onenotepatchactiontype-values"></a>onenotePatchActionType 值

| Member
|:-------------------------
| 替换
| Append
| 删除
| Insert
| Prepend

### <a name="onenotepatchinsertposition-values"></a>onenotePatchInsertPosition 值

| Member
|:-------------------------
| 活动后
| 活动前


### <a name="phonetype-values"></a>phoneType 值

| Member
|:-------------------------
| home
| business
| mobile
| other
| assistant
| homeFax
| businessFax
| otherFax
| pager
| radio


### <a name="plannerpreviewtype-values"></a>plannerPreviewType 值

| Member
|:-------------------------
| 自动
| noPreview
| checklist
| description
| 参考


### <a name="status-values"></a>状态值

| Member
|:-----------------
| active
| updated
| deleted
| 忽略
| unknownFutureValue


### <a name="weekindex-values"></a>weekIndex 值

| Member
|:-------------------------
| first
| second
| 第三
| fourth
| last


### <a name="dayofweek-values"></a>dayOfWeek 值

| Member
|:-------------------------
| sunday
| monday
| tuesday
| 星期三
| thursday
| 星期五
| saturday

### <a name="recurrencepatterntype-values"></a>recurrencePatternType 值

| Member
|:-------------------------
| daily
| weekly
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>recurrenceRangeType 值

| Member
|:-------------------------
| endDate
| noEnd
| 编号


### <a name="onenotesourceservice-values"></a>onenoteSourceService 值
| Member
|:---------------------
| 未知
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### <a name="responsetype-values"></a>responseType 值

| Member
|:-------------------------
| 无
| 组织者
| tentativelyAccepted
| accepted
| declined
| notResponded


### <a name="activitydomain-values"></a>activityDomain 值

| Member
|:-------------------------
| unknown
| 工时
| personal
| unrestricted


### <a name="websitetype-values"></a>websiteType 值

| Member
|:-------------------------
| other
| home
| 工时
| 博客
| 个人资料


### <a name="categorycolor-values"></a>categoryColor 值

| 成员   |值
|:---------|:--------
| 无     | -1
| preset0  | 0
| preset1  | 1
| preset2  | 2
| preset3  | 3
| preset4  | 4
| preset5  | 5
| preset6  | 6 
| preset7  | 7 
| preset8  | 8 
| preset9  | 9 
| preset10 | 10 
| preset11 | 11
| preset12 | 12 
| preset13 | 13
| preset14 | 14 
| preset15 | 15 
| preset16 | 16
| preset17 | 17 
| preset18 | 18 
| preset19 | 19
| preset20 | 20
| preset21 |  21
| preset22 | 22
| preset23 | 23
| preset24 | 24

### <a name="alertfeedback-values"></a>alertFeedback 值

分析员提供的警报的可能反馈值。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知。|
|truePositive|1|警报为正数。|
|falsePositive|2| 警报为误报。|
|将positive|3| 警报是正性警报。|

### <a name="filehashtype-values"></a>fileHashType 值

文件哈希类型的枚举。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知类型。|
|sha1|1|SHA1 哈希类型。|
|sha256|2| SHA256 哈希类型。|
|md5|3| MD5 哈希类型。|
|authenticodeHash256|4| AuthenticodeHash256 哈希类型。|
|lsHash|5| LsHash 哈希类型。|
|ctph|6 | CTPH 哈希类型。|
|peSha1|7 | PESHA1 哈希类型。|
|peSha256|8 | PESHA256 哈希类型。|

### <a name="connectiondirection-values"></a>connectionDirection 值

用于入站/出站 (网络连接方向的枚举) 。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知连接。|
|inbound|1|入站连接。|
|出站|2| 出站连接。|

### <a name="connectionstatus-values"></a>connectionStatus 值

连接状态的枚举。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|连接状态未知。|
|attempted|1|已尝试连接。|
|succeeded|2| 连接成功。|
|blocked|3| 连接被阻止。|
|failed|4| 连接失败。|

### <a name="processintegritylevel-values"></a>processIntegrityLevel 值

进程可能的完整性级别值。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知。|
|不受信任的|10 |完整性级别不受信任。|
|low|20| 完整性级别为"低"。|
|中等|30| 完整性级别为"中"。|
|high|40| 完整性级别为"高"。|
|system|50| 完整性级别为系统。|

### <a name="registryhive-values"></a>registryHive 值

由 [/windows/desktop/sysinfo/registry-hives 定义的注册表配置单元的枚举](/windows/desktop/sysinfo/registry-hives)。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知配置单元。|
|currentConfig|1|HKEY_CURRENT_CONFIG配置单元。|
|currentUser|2| HKEY_CURRENT_USER配置单元。|
|localMachineSam|3| HKEY_LOCAL_MACHINE\SAM配置单元。|
|localMachineSamSoftware|4| HKEY_LOCAL_MACHINE\Software配置单元。|
|localMachineSystem|5| HKEY_LOCAL_MACHINE\System配置单元。|
|usersDefault|6 | HKEY_USERS \\ 。DEFAULT 配置单元。|

### <a name="registryoperation-values"></a>registryOperation 值

更改注册表项名称和/或值的操作。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知的注册表值类型。|
|create|1|创建注册表。|
|modify|2|修改注册表。|
|delete|3|删除注册表。|

### <a name="registryvaluetype-values"></a>registryValueType 值

由 [/windows/desktop/sysinfo/registry-value-types 定义的注册表值类型的枚举](/windows/desktop/sysinfo/registry-value-types)。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知的注册表值类型。|
|binary|1|REG_BINARY注册表值类型。|
|dword|2| REG_DWORD注册表值类型。|
|dwordLittleEndian|3| REG_DWORD_LITTLE_ENDIAN注册表值类型。|
|dwordBigEndian|4| REG_DWORD_BIG_ENDIAN注册表值类型。|
|expandSz|5| REG_EXPAND_SZ注册表值类型。|
|link|6 | REG_LINK注册表值类型。|
|multiSz|7 | REG_MULTI_SZ注册表值类型。|
|无|8 | REG_NONE注册表值类型。|
|qword|9 | REG_QWORD注册表值类型。|
|qwordlittleEndian|10 | REG_QWORD_LITTLE_ENDIAN注册表值类型。|
|sz|11| REG_SZ注册表值类型。|

### <a name="alertseverity-values"></a>alertSeverity 值

警报严重性枚举。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|严重性未知。|
|informational|1|严重性仅适用于信息。|
|low|2| 严重性较低。|
|中等|3| 严重性为中等。|
|high|4| 严重性较高。|

### <a name="alertstatus-values"></a>alertStatus 值

警报生命周期状态的可能值 (阶段) 。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知状态。|
|newAlert|10 | 警报是新警报。|
|inProgress|20|警报正在进行中。|
|已解决|30|警报已解决。|

### <a name="emailrole-values"></a>emailRole 值
电子邮件角色的可能值。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知角色。|
|sender|1|电子邮件的发件人。|
|recipient|2|电子邮件的收件人。|

### <a name="logontype-values"></a>logonType 值

用户登录方法的可能值。

|成员|值|说明|
|:---|:---|:---|
|unknown|-1|未知。|
|interactive|0|登录是交互式的。|
|remoteInteractive|1| 登录是远程交互的。|
|network|2| 登录是网络。|
|batch|3| 登录是批处理。|
|服务|4| 登录是服务。|

### <a name="useraccountsecuritytype-values"></a>userAccountSecurityType 值

根据组定义， (用户帐户) 类型的Windows值。

|Member|成员|说明|
|:---|:---|:---|
|unknown|-1|未知。|
|standard|0|标准用户组的成员。|
|power|1| Power Users 组的成员。|
|administrator|2| 组管理员组。|

### <a name="riskdetail-values"></a>riskDetail 值

|Member|
|:---|
|无|
|adminGeneratedTemporaryPassword|
|userPerformedSecuredPasswordChange|
|userPerformedSecuredPasswordReset|
|adminConfirmedSigninSafe|
|aiConfirmedSigninSafe|
|userPassedMFADrivenByRiskBasedPolicy|
|adminDismissedAllRiskForUser|
|adminConfirmedSigninComprom一|
|adminConfirmedUserComprom一|
|hidden|
|unknownFutureValue|

### <a name="riskeventtypes-values"></a>riskEventTypes 值

| Member
|:-------------------------
| unlikelyTravel
| 匿名IPAddress
| maliciousIPAddress
| unfamiliarFeatures
| malwareInfectedIPAddress
| suspiciousIPAddress
| leakedCredentials
| investigationsThreatIntelligence
| generic
| unknownFutureValue

### <a name="riskeventtype-values"></a>riskEventType 值

|Member|
|:---|
|unlikelyTravel|
|匿名IPAddress|
|maliciousIPAddress|
|unfamiliarFeatures|
|malwareInfectedIPAddress|
|suspiciousIPAddress|
|leakedCredentials|
|investigationsThreatIntelligence|
|generic|
|adminConfirmedUserComprom一|
|mcasImpossibleTravel|
|mcasSuspiciousInboxManipulationRules|
|investigationsThreatIntelligenceSigninLinked|
|maliciousIPAddressValidCredentialsBlockedIP|
|unknownFutureValue|

### <a name="risklevel-values"></a>riskLevel 值

| Member
|:-------------------------
| 无
| low
| 中等
| high
| hidden
| unknownFutureValue

### <a name="riskstate-values"></a>riskState 值

| Member
|:-------------------------
| 无
| confirmedSafe
| 修正
| dismissed
| atRisk
| confirmedComprom一
| unknownFutureValue

### <a name="exchangeidformat-values"></a>exchangeIdFormat 值

|Member|
|:---|
|entryId|
|ewsId|
|immutableEntryId|
|restId|
|restImmutableEntryId|

### <a name="onlinemeetingprovidertype-values"></a>onlineMeetingProviderType 值

|Member|
|:---|
|unknown|
|skypeForBusiness|
|skypeForConsumer|
|teamsForBusiness|

### <a name="delegatemeetingmessagedeliveryoptions-values"></a>delegateMeetingMessageDeliveryOptions 值

|Member|
|:---|
|sendToDelegateAndInformationToPrincipal|
|sendToDelegateAndPrincipal|
|sendToDelegateOnly|

### <a name="calendarroletype-values"></a>calendarRoleType 值

|Member|
|:---|
|无|
|freeBusyRead|
|limitedRead|
|阅读|
|写入|
|delegateWithoutPrivateEventAccess|
|delegateWithPrivateEventAccess|
|custom|

### <a name="threatassessmentcontenttype-values"></a>threatAssessmentContentType 值

| 成员 | 值 | 说明             |
|:-------|:------|:------------------------|
| mail   | 1     | 邮件威胁。            |
| url    | 2     | URL 威胁。             |
| file   | 3     | 附件文件威胁。 |

### <a name="threatexpectedassessment-values"></a>threatExpectedAssessment 值

| 成员  | 值 | 说明                       |
|:--------|:------|:----------------------------------|
| block   | 1     | 应阻止威胁。     |
| unblock | 2     | 不应阻止威胁。 |

### <a name="threatcategory-values"></a>threatCategory 值

| 成员             | 值 | 说明        |
|:-------------------|:------|:-------------------|
| 垃圾邮件 (spam)               | 1     | 垃圾邮件威胁。       |
| 仿冒           | 2     | 网络钓鱼威胁。   |
| 恶意软件 (malware)            | 3     | 恶意软件威胁。    |
| unknownFutureValue | 4     | sentinel 成员。 |

### <a name="threatassessmentstatus-values"></a>threatAssessmentStatus 值

| 成员    | 值 | 说明                              |
|:----------|:------|:-----------------------------------------|
| pending   | 1     | 威胁评估仍在进行中。 |
| 已完成 | 2     | 已完成威胁评估。         |

### <a name="threatassessmentrequestsource-values"></a>threatAssessmentRequestSource 值

| 成员        | 值 | 说明              |
|:--------------|:------|:-------------------------|
| undefined     | 0     | 尚不知道。            |
| 用户          | 1     | 用户提交。         |
| administrator | 2     | 租户管理员提交。 |

### <a name="threatassessmentresulttype-values"></a>threatAssessmentResultType 值

| 成员             | 值 | 说明                                          |
|:-------------------|:------|:-----------------------------------------------------|
| checkPolicy        | 1     | 策略检查结果，仅适用于 `mail` 评估。 |
| rescan             | 2     | 重新扫描结果。                                   |
| unknownFutureValue | 3     | sentinel 成员。                                   |

### <a name="maildestinationroutingreason-values"></a>mailDestinationRoutingReason 值

| 成员                | 值 | 说明                         |
|:----------------------|:------|:------------------------------------|
| 无                  | 0     | 尚不知道。                       |
| mailFlowRule          | 1     | Exchange传输规则。            |
| safeSender            | 2     | 保险箱发件人列表。                   |
| blockedSender         | 3     | 阻止的发件人列表。                |
| advancedSpamFiltering | 4     | 高级垃圾邮件筛选选项。     |
| domainAllowList       | 5     | 发件人域允许列表。           |
| domainBlockList       | 6      | 发件人域阻止列表。           |
| notInAddressBook      | 7      | 排除不在通讯簿中的发件人。 |
| firstTimeSender       | 8      | 因第一次发送者被阻止。   |
| autoPurgeToInbox      | 9      | TimeTravel 将邮件移动到收件箱。   |
| autoPurgeToJunk       | 10     | TimeTravel 将邮件移动到垃圾邮件。    |
| autoPurgeToDeleted    | 11    | TimeTravel 要删除的移动消息。 |
| 出站              | 12     | 出站邮件。                      |
| notJunk               | 13    | 允许，因为不是垃圾邮件。              |
| junk                  | 14     | 因垃圾邮件被阻止。                |
| unknownFutureValue    | 15     | sentinel 成员。                  |

### <a name="chatmessagetype-values"></a>chatMessageType 值

| 值 |
|:-----------------|
| message |
| chatEvent |
| 键入 |
| unknownFutureValue |
| systemEventMessage |

### <a name="chatmessagepolicyviolationdlpactiontype-values"></a>chatMessagePolicyViolationDlpActionType 值

| 值 |
|:-----------------|
| 无 |
| NotifySender |
| BlockAccess |
| BlockAccessExternal |

### <a name="chatmessagepolicyviolationuseractiontype-values"></a>chatMessagePolicyViolationUserActionType 值

| Member   | Int 值 |  说明 |
|:---------------|:--------|:----------|
| 无 | 0 | 默认值。 当用户未对 DLP 阻止的邮件采取操作时，此值为邮件上的值。 |
| Override | 1 | 发件人已覆盖邮件裁定并发送了该邮件。|
| ReportFalsePositive | 2 | 发件人将邮件裁定报告给管理员为误报。|

### <a name="chatmessagepolicyviolationverdictdetailstype-values"></a>chatMessagePolicyViolationVerdictDetailsType 值

| Member   | Int 值 |  说明 |
|:---------------|:--------|:----------|
| 无 | 0 |  不允许用户覆盖邮件。 如果未提供策略提示，则不允许用户将邮件报告为误报。 在所有其他方案中，用户可以将邮件报告为误报。|
| AllowFalsePositiveOverride | 1 |  除非此块与 或 标志组合在一起，否则不允许用户显式 `AllowOverrideWithoutJustification` 替代 `AllowOverrideWithJustification` 块。 报告违反误报会自动覆盖阻止并发送邮件。 |
| AllowOverrideWithoutJustification | 2 | 允许用户覆盖块并发送邮件。 理由文本不是必需的。 独占到 `AllowOverrideWithJustification` 。 |
| AllowOverrideWithJustification | 4 |  允许用户覆盖块并发送邮件。 理由文本是必需的。 独占到 `AllowOverrideWithoutJustification` 。|

### <a name="channelmembershiptype-values"></a>channelMembershipType 值

| 成员             | 值 |说明|
| :----------------- | :---- |:-----------|
| standard           | 0     |Channel 继承父团队成员的列表。|
| private            | 1     |频道的成员可以是父团队中所有成员的子集。|
| unknownFutureValue | 2     |      |
### <a name="wellknownlistname-values"></a>wellknownListName 值
| Member
|:----------------------
| 无
| defaultList
| flaggedEmails
| unknownFutureValue

### <a name="taskstatus-values"></a>taskStatus 值
| Member
|:----------------------
| notStarted
| inProgress
| 已完成
| waitingOnOthers
| deferred

### <a name="columntypes-values"></a>columnTypes 值

|成员|说明|
|:-------|:------
|note| 多行文本。 |
|text | 单行文本。 |
|choice | 选项列 |
|multichoice | 多选择列。 |
|number | 数字列。 |
|currency | 货币列。 |
|dateTime | DateTime 列。 |
|查找 | 查找列。 |
|boolean | 是/否列。 |
|用户 | 人员或组列。 |
|url | 超链接或图片列。 |
|calculated | 计算列。 |
|位置 | 位置列。 |
|地理位置 | "地理位置"列。 |
|term | 托管元数据列。 |
|multiterm | 接受多个值的托管元数据列。 |
|thumbnail | 图像列。 |
|approvalStatus | 内容审批状态列。 |
|unknownFutureValue | UnknownFuturevalue |

### <a name="permissionclassificationtype-values"></a>permissionClassificationType 值

| Member
|:-------
| low

### <a name="permissiontype-values"></a>permissionType 值

| Member
|:-------------------------
| 应用程序
| delegated
| delegatedUserConsentable

### <a name="printcolormode-values"></a>printColorMode 值 

|Member|
|:---|
|blackAndWhite|
|灰度|
|颜色|
|自动|
|unknownFutureValue|

### <a name="printduplexmode-values"></a>printDuplexMode 值 

|Member|
|:---|
|flipOnLongEdge|
|flipOnShortEdge|
|oneSided|
|unknownFutureValue|

### <a name="printerfeedorientation-values"></a>printerFeedOrientation 值 

|Member|
|:---|
|longEdgeFirst|
|shortEdgeFirst|
|unknownFutureValue|

### <a name="printfinishing-values"></a>printFinishing 值 

|Member|
|:---|
|无|
|装订|
|一个|
|cover|
|bind|
|一些|
|一些|
|stapleTopLeft|
|装订BottomLeft|
|stapleTopRight|
|装订BottomRight|
|将leftEdge|
|将topEdge|
|将rightEdge|
|将bottomEdge|
|stapleDualLeft|
|stapleDualTop|
|stapleDualRight|
|stapleDualBottom|
|unknownFutureValue|

### <a name="printmultipagelayout-values"></a>printMultipageLayout 值 

|Member|
|:---|
|顺时针FromTopLeft|
|counterclockwiseFromTopLeft|
|counterclockwiseFromTopRight|
|clockwiseFromTopRight|
|counterclockwiseFromBottomLeft|
|顺时针FromBottomLeft|
|counterclockwiseFromBottomRight|
|顺时针FromBottomRight|
|unknownFutureValue|

### <a name="printorientation-values"></a>printOrientation 值 

|Member|
|:---|
|纵向|
|横向|
|reverseLandscape|
|reversePortrait|
|unknownFutureValue|

### <a name="printquality-values"></a>printQuality 值 

|Member|
|:---|
|low|
|中等|
|high|
|unknownFutureValue|

### <a name="printscaling-values"></a>printScaling 值 

|Member|
|:---|
|自动|
|shrinkToFit|
|fill|
|fit|
|无|
|unknownFutureValue|

### <a name="userflowtype-values"></a>userFlowType 值

|Member
|:----------------------
| signUp
| signIn
| signUpOrSignIn
| passwordReset
| profileUpdate
| resourceOwner
| unknownFutureValue

### <a name="identityuserflowattributedatatype-values"></a>identityUserFlowAttributeDataType 值

| Member                |
|:----------------------|
| string                |
| boolean               |
| int64                 |
| stringCollection      |
| dateTime              |
| unknownFutureValue    |

### <a name="identityuserflowattributetype-values"></a>identityUserFlowAttributeType 值

| Member                |
|:----------------------|
| builtIn               |
| custom                |
| 必需              |
| unknownFutureValue    |

### <a name="identityuserflowattributeinputtype-values"></a>identityUserFlowAttributeInputType 值

| Member                |
|:----------------------|
| textBox               |
| dateTimeDropDown      |
| radioSingleSelect     |
| dropdownSingleSelect  |
| emailBox              |
| checkboxMultiSelect   |

### <a name="teamworkactivitytopicsource-values"></a>teamworkActivityTopicSource 值 

| Member    |
| :-------- |
| entityUrl |
| text      |


### <a name="provisioningresult-values"></a>provisioningResult 值 

|Member|
|:---|
|success|
|failure|
|已跳过|
|警告|
|unknownFutureValue|

### <a name="provisioningsteptype-values"></a>provisioningStepType 值 

|Member|
|:---|
|import|
|范围|
|匹配|
|processing|
|referenceResolution|
|export|
|unknownFutureValue|

### <a name="provisioningstatuserrorcategory-values"></a>provisioningStatusErrorCategory 值 

|Member|
|:---|
|failure|
|nonServiceFailure|
|success|
|unknownFutureValue|

### <a name="provisioningaction-values"></a>provisioningAction 值 

|Member|
|:---|
|other|
|create|
|delete|
|disable|
|update|
|stagedDelete|
|unknownFutureValue|


### <a name="initiatortype-values"></a>initiatorType 值 

|Member|
|:---|
|用户|
|应用程序|
|system|
|unknownFutureValue|

### <a name="teamworkapplicationidentitytype-values"></a>teamworkApplicationIdentityType 值 

|Member|
|:---|
|aadApplication|
|bot|
|tenantBot|
|office365Connector|
|outgoingWebhook|
|unknownFutureValue|

### <a name="teamworkconversationidentitytype-values"></a>teamworkConversationIdentityType 值 

|Member|
|:---|
|团队|
|channel|
|聊天|
|unknownFutureValue|

### <a name="teamworkuseridentitytype-values"></a>teamworkUserIdentityType 值 

|Member|
|:---|
|aadUser|
|onPremiseAadUser|
|anonymousGuest|
|federatedUser|
|personalMicrosoftAccountUser|
|skypeUser|
|phoneUser|
|unknownFutureValue|

### <a name="posttype-values"></a>postType 值 

|Member|
|:---|
|regular|
|quick|
|strategic|
|unknownFutureValue|

### <a name="servicehealthclassificationtype-values"></a>serviceHealthClassificationType 值 

|Member|
|:---|
|advisory|
|incident|
|unknownFutureValue|

### <a name="servicehealthorigin-values"></a>serviceHealthOrigin 值 

|Member|
|:---|
|microsoft|
|thirdParty|
|customer|
|unknownFutureValue|

### <a name="servicehealthstatus-values"></a>serviceHealthStatus 值 

|Member|
|:---|
|serviceOperational|
|正在调查|
|restoringService|
|verifyingService|
|serviceRestored|
|postIncidentReviewPublished|
|serviceDegradation|
|serviceInterruption|
|extendedRecovery|
|falsePositive|
|investigationSuspended|
|已解决|
|mitigatedExternal|
|已缓解|
|resolvedExternal|
|confirmed|
|reported|
|unknownFutureValue|

### <a name="serviceupdatecategory-values"></a>serviceUpdateCategory 值 

|Member|
|:---|
|preventOrFixIssue|
|planForChange|
|stayInformed|
|unknownFutureValue|

### <a name="serviceupdateseverity-values"></a>serviceUpdateSeverity 值 

|Member|
|:---|
|normal|
|high|
|critical|
|unknownFutureValue|

### <a name="subjectrightsrequeststage-values"></a>subjectRightsRequestStage 值 

|Member|
|:---|
|contentRetrieval|
|contentReview|
|generateReport|
|contentDeletion|
|caseResolved|
|unknownFutureValue|

### <a name="subjectrightsrequeststagestatus-values"></a>subjectRightsRequestStageStatus 值 

|Member|
|:---|
|notStarted|
|current| 
|已完成| 
|failed|
|unknownFutureValue|

### <a name="subjectrightsrequeststatus-values"></a>subjectRightsRequestStatus 值 

|Member|
|:---|
|active|
|closed|
|unknownFutureValue|

### <a name="subjectrightsrequesttype-values"></a>subjectRightsRequestType 值 

|Member|
|:---|
|export|
|delete|
|access|
|tagForAction|
|unknownFutureValue|

### <a name="datasubjecttype-values"></a>dataSubjectType 值 

|Member|
|:---|
|customer|
|currentEmployee|
|formerEmployee|
|prospectiveEmployee|
|student|
|teacher|
|教职员工|
|other|
|unknownFutureValue|

### <a name="advancedconfigstate-values"></a>advancedConfigState 值 

|Member|
|:---|
|default|
|enabled|
|disabled|
|unknownFutureValue|

### <a name="callrecordingstatus-values"></a>callRecordingStatus 值 

|Member|
|:---|
|success|
|failure|
|initial|
|chunkFinished|
|unknownFutureValue|

### <a name="teamworkcalleventtype-values"></a>teamworkCallEventType 值 

|Member|
|:---|
|通话|
|meeting|
|screenShare|
|unknownFutureValue|

### <a name="bookingreminderrecipients-values"></a>bookingReminderRecipients 值 

|Member|
|:---|
|allAttendees|
|staff|
|customer|
|unknownFutureValue|

### <a name="bookingstaffrole-values"></a>bookingStaffRole 值 

|Member|
|:---|
|来宾|
|administrator|
|viewer|
|externalGuest|
|unknownFutureValue|

### <a name="answerinputtype-values"></a>answerInputType 值 

|Member|
|:---|
|text|
|radioButton|
|unknownFutureValue|

### <a name="bookingpricetype-values"></a>bookingPriceType 值

|Member|
|:---|
|undefined|
|fixedPrice|
|startingAt|
|hourly|
|free|
|priceVaries|
|callUs|
|notSet|
|unknownFutureValue|
