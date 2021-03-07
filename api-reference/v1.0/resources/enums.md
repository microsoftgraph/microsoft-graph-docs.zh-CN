---
title: 枚举值
description: Microsoft Graph 枚举值。
localization_priority: Normal
ms.prod: non-product-specific
author: MSGraphDocsvTeam
doc_type: enumPageType
ms.openlocfilehash: 0ca783518b3244230c776d33609bb6890d8a448c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516113"
---
# <a name="enum-values"></a>枚举值

命名空间：microsoft.graph

### <a name="activitytype-values"></a>activityType 值

|成员|
|:---|
|signin|
|user|
|unknownFutureValue|

### <a name="riskdetectiontimingtype-values"></a>riskDetectionTimingType 值

|成员|
|:---|
|notDefined|
|实时|
|nearRealtime|
|脱机|
|unknownFutureValue|

### <a name="tokenissuertype-values"></a>tokenIssuerType 值

|成员|
|:---|
|AzureAD|
|ADFederationServices|
|UnknownFutureValue|

### <a name="attachmenttype-values"></a>attachmentType 值

| 成员
|:--------------
| file
| 项
| 参考

### <a name="contactrelationship-values"></a>contactRelationship 值

|成员|值|Description|
|:---|:---|:---|
|父级|0|用户的父级。|
|relative|1 | 用户的相对位置。|
|aide|2 | 用户的助手。|
|一些|3 | 用户的医生。|
|保护者|4 | 用户的保护者。|
|Child|5 | 用户的子级。|
|other|6 | 与用户的未指定关系。|
|unknownFutureValue|7 | 用于将来兼容性的标记值。|

### <a name="scheduleentitytheme-values"></a>scheduleEntityTheme 值

| 成员
|:-------------------------
| white
| 蓝色
| 绿色
| 紫色
| 粉红色
| 黄色
| 灰色
| darkBlue
| darkGreen
| darkPurple
| darkPink
| darkYellow
| unknownFutureValue


### <a name="timeoffreasonicontype-values"></a>timeOffReasonIconType 值

|成员|
|:---|
|无|
|car|
|日历|
|正在运行|
|plane|
|firstAid|
|一些|
|notWorking|
|clock|
|juryDuty|
|全球|
|cup|
|phone|
|weather|
|umbrella|
|一个|
|狗|
|的|
|trafficCone|
|pin|
|一些|
|unknownFutureValue|

### <a name="timezonestandard-values"></a>timeZoneStandard 值

| 成员
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

| 成员
|:-------------------------
| 必需
| 可选
| resource


### <a name="externalaudiencescope-values"></a>externalAudienceScope 值

| 成员
|:-------------------------
| 无
| contactsOnly
| all


### <a name="automaticrepliesstatus-values"></a>automaticRepliesStatus 值

| 成员
|:-------------------------
| 已禁用
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

| 成员
|:-------------------------
| sis
| 手动
| unknownFutureValue


### <a name="educationgender-values"></a>educationGender 值

| 成员
|:-------------------------
| female
| male
| other
| unknownFutureValue


### <a name="eventtype-values"></a>eventType 值

| 成员
|:-------------------------
| singleInstance
| occurrence
| exception
| seriesMaster


### <a name="sensitivity-values"></a>敏感度值

| 成员
|:-------------------------
| normal
| personal
| private
| confidential


### <a name="importance-values"></a>重要性值

| 成员
|:-------------------------
| low
| normal
| high


### <a name="educationuserrole-values"></a>educationUserRole 值
| 成员
|:---------------------
| student
| teacher

### <a name="meetingmessagetype-values"></a>meetingMessageType 值

| 成员
|:-----------------
| 无
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTenativelyAccepted
| meetingDeclined


### <a name="followupflagstatus-values"></a>followupFlagStatus 值

| 成员
|:-------------------------
| notFlagged
| complete
| 已标记


### <a name="inferenceclassificationtype-values"></a>inferenceClassificationType 值

| 成员
|:-----------------
| 聚焦
| other


### <a name="iosnotificationalerttype-values"></a>iosNotificationAlertType 值

| 成员
|:-------------------------
| deviceDefault
| 横幅
| 模式
| 无

### <a name="deviceenrollmentfailurereason-values"></a>deviceEnrollmentFailureReason 值

| 成员
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
| 成员
|:---------
| text
| html


### <a name="locationtype-values"></a>locationType 值

| 成员
|:-------------------------
| 默认
| conferenceRoom
| homeAddress
| businessAddress
| geoCoordinates
| streetAddress
| 区
| 餐厅
| localBusiness
| postalAddress

### <a name="locationuniqueidtype-values"></a>locationUniqueIdType 值

| 成员
|:-------------------------
| unknown
| locationStore
| 目录
| private
| 必应


### <a name="messageactionflag-values"></a>messageActionFlag 值

| 成员
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

| 成员
|:-----------------
| NotStarted
| 正在运行
| Completed
| 已失败


### <a name="onenotepatchactiontype-values"></a>onenotePatchActionType 值

| 成员
|:-------------------------
| 替换
| Append
| 删除
| Insert
| Prepend

### <a name="onenotepatchinsertposition-values"></a>onenotePatchInsertPosition 值

| 成员
|:-------------------------
| 段后
| Before


### <a name="phonetype-values"></a>phoneType 值

| 成员
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

| 成员
|:-------------------------
| 自动
| noPreview
| checklist
| 说明
| 参考


### <a name="status-values"></a>状态值

| 成员
|:-----------------
| active
| updated
| deleted
| 忽略
| unknownFutureValue


### <a name="weekindex-values"></a>weekIndex 值

| 成员
|:-------------------------
| first
| second
| 第三个
| 第四个
| last


### <a name="dayofweek-values"></a>dayOfWeek 值

| 成员
|:-------------------------
| sunday
| monday
| 星期二
| 星期三
| 星期四
| 星期五
| saturday

### <a name="recurrencepatterntype-values"></a>recurrencePatternType 值

| 成员
|:-------------------------
| daily
| weekly
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>recurrenceRangeType 值

| 成员
|:-------------------------
| endDate
| noEnd
| 编号


### <a name="onenotesourceservice-values"></a>onenoteSourceService 值
| 成员
|:---------------------
| 未知
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### <a name="responsetype-values"></a>responseType 值

| 成员
|:-------------------------
| 无
| organizer － 组织者
| tentativelyAccepted
| accepted
| 拒绝
| notResponded


### <a name="activitydomain-values"></a>activityDomain 值

| 成员
|:-------------------------
| unknown
| 工时
| personal
| unrestricted


### <a name="websitetype-values"></a>websiteType 值

| 成员
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

分析员提供的警报可能的反馈值。

|成员|值|Description|
|:---|:---|:---|
|unknown|0|未知。|
|truePositive|1 |警报为 true-positive。|
|falsePositive|2 | 警报为误报。|
|benignPositive|3 | 警报是正性警报。|

### <a name="filehashtype-values"></a>fileHashType 值

文件哈希类型的枚举。

|成员|值|Description|
|:---|:---|:---|
|unknown|0|未知类型。|
|sha1|1 |SHA1 哈希类型。|
|sha256|2 | SHA256 哈希类型。|
|md5|3 | MD5 哈希类型。|
|authenticodeHash256|4 | AuthenticodeHash256 哈希类型。|
|lsHash|5 | LsHash 哈希类型。|
|ctph|6 | CTPH 哈希类型。|
|peSha1|7 | PESHA1 哈希类型。|
|peSha256|8 | PESHA256 哈希类型。|

### <a name="connectiondirection-values"></a>connectionDirection 值

网络连接方向的枚举 (/出站) 。

|成员|值|Description|
|:---|:---|:---|
|unknown|0|未知连接。|
|入站|1 |入站连接。|
|出站|2 | 出站连接。|

### <a name="connectionstatus-values"></a>connectionStatus 值

连接状态的枚举。

|成员|值|Description|
|:---|:---|:---|
|unknown|0|未知连接状态。|
|attempted|1 |已尝试连接。|
|succeeded|2 | 连接成功。|
|blocked|3 | 连接被阻止。|
|failed|4 | 连接失败。|

### <a name="processintegritylevel-values"></a>processIntegrityLevel 值

进程可能的完整性级别值。

|成员|值|Description|
|:---|:---|:---|
|unknown|0|未知。|
|不受信任的|10  |完整性级别不受信任。|
|low|20| 完整性级别较低。|
|中等|30| 完整性级别为"中等"。|
|high|40| 完整性级别为"高"。|
|system|50| 完整性级别为"系统"。|

### <a name="registryhive-values"></a>registryHive 值

由 [/windows/desktop/sysinfo/registry-hives 定义的注册表配置单元枚举](/windows/desktop/sysinfo/registry-hives)。

|成员|值|Description|
|:---|:---|:---|
|unknown|0|未知配置单元。|
|currentConfig|1 |HKEY_CURRENT_CONFIG配置单元。|
|currentUser|2 | HKEY_CURRENT_USER配置单元。|
|localMachineSam|3 | HKEY_LOCAL_MACHINE\SAM配置单元。|
|localMachineSamSoftware|4 | HKEY_LOCAL_MACHINE\Software配置单元。|
|localMachineSystem|5 | HKEY_LOCAL_MACHINE\System配置单元。|
|usersDefault|6 | HKEY_USERS \\ 。DEFAULT 配置单元。|

### <a name="registryoperation-values"></a>registryOperation 值

更改注册表项名称和/或值的操作。

|成员|值|Description|
|:---|:---|:---|
|unknown|0|未知的注册表值类型。|
|create|1 |创建注册表。|
|modify|2 |修改注册表。|
|delete|3 |删除注册表。|

### <a name="registryvaluetype-values"></a>registryValueType 值

由 [/windows/desktop/sysinfo/registry-value-types 定义的注册表值类型的枚举](/windows/desktop/sysinfo/registry-value-types)。

|成员|值|Description|
|:---|:---|:---|
|unknown|0|未知的注册表值类型。|
|binary|1 |REG_BINARY注册表值类型。|
|dword|2 | REG_DWORD注册表值类型。|
|dwordLittleEndian|3 | REG_DWORD_LITTLE_ENDIAN注册表值类型。|
|dwordBigEndian|4 | REG_DWORD_BIG_ENDIAN注册表值类型。|
|expandSz|5 | REG_EXPAND_SZ注册表值类型。|
|link|6 | REG_LINK注册表值类型。|
|multiSz|7 | REG_MULTI_SZ注册表值类型。|
|无|8 | REG_NONE注册表值类型。|
|qword|9 | REG_QWORD注册表值类型。|
|qwordlittleEndian|10  | REG_QWORD_LITTLE_ENDIAN注册表值类型。|
|sz|11| REG_SZ注册表值类型。|

### <a name="alertseverity-values"></a>alertSeverity 值

警报严重性枚举。

|成员|值|Description|
|:---|:---|:---|
|unknown|0|严重性未知。|
|信息|1 |严重性仅适用于信息。|
|low|2 | 严重性较低。|
|中等|3 | 严重性为中等。|
|high|4 | 严重性为高。|

### <a name="alertstatus-values"></a>alertStatus 值

警报生命周期状态可能的值 (阶段) 。

|成员|值|Description|
|:---|:---|:---|
|unknown|0|未知状态。|
|newAlert|10  | 警报是新增功能。|
|inProgress|20|警报正在进行中。|
|已解决|30|警报已解决。|

### <a name="emailrole-values"></a>emailRole 值
电子邮件角色的可能值。

|成员|值|Description|
|:---|:---|:---|
|unknown|0|未知角色。|
|sender|1 |电子邮件的发件人。|
|recipient|2 |电子邮件的收件人。|

### <a name="logontype-values"></a>logonType 值

用户登录方法的可能值。

|成员|值|Description|
|:---|:---|:---|
|unknown|-1|未知。|
|interactive|0|登录是交互式的。|
|remoteInteractive|1 | 登录是远程交互式登录。|
|网络|2 | 登录是网络。|
|batch|3 | 登录是批处理。|
|服务|4 | 登录是服务。|

### <a name="useraccountsecuritytype-values"></a>userAccountSecurityType 值

根据 Windows 定义，用户帐户类型 (组) 可能的值。

|成员|成员|说明|
|:---|:---|:---|
|unknown|-1|未知。|
|standard|0|标准用户组的成员。|
|power|1 | Power Users 组的成员。|
|administrator|2 | 组管理员组。|

### <a name="riskdetail-values"></a>riskDetail 值

| 成员
|:-------------------------
| adminGeneratedTemporaryPassword
| userPerformedSecuredPasswordChange
| userPerformedSecuredPasswordReset
| adminConfirmedSigninSafe
| aiConfirmedSigninSafe
| userPassedMFADrivenByRiskBasedPolicy
| adminDismissedAllRiskForUser
| adminConfirmedSigninCompromign
| unknownFutureValue

### <a name="riskeventtypes-values"></a>riskEventTypes 值

| 成员
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

|成员|
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
|adminConfirmedUserComprom工|
|mcasImpossibleTravel|
|mcasSuspiciousInboxManipulationRules|
|investigationsThreatIntelligenceSigninLinked|
|maliciousIPAddressValidCredentialsBlockedIP|
|unknownFutureValue|

### <a name="risklevel-values"></a>riskLevel 值

| 成员
|:-------------------------
| 无
| low
| 中等
| high
| hidden
| unknownFutureValue

### <a name="riskstate-values"></a>riskState 值

| 成员
|:-------------------------
| 无
| confirmedSafe
| 修正
| dismissed
| atRisk
| confirmedComprom confirmed
| unknownFutureValue

### <a name="exchangeidformat-values"></a>exchangeIdFormat 值

|成员|
|:---|
|entryId|
|ewsId|
|immutableEntryId|
|restId|
|restImmutableEntryId|

### <a name="onlinemeetingprovidertype-values"></a>onlineMeetingProviderType 值

|成员|
|:---|
|unknown|
|skypeForBusiness|
|skypeForConsumer|
|teamsForBusiness|

### <a name="delegatemeetingmessagedeliveryoptions-values"></a>delegateMeetingMessageDeliveryOptions 值

|成员|
|:---|
|sendToDelegateAndInformationToPrincipal|
|sendToDelegateAndPrincipal|
|sendToDelegateOnly|

### <a name="calendarroletype-values"></a>calendarRoleType 值

|成员|
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

| 成员 | 值 | Description             |
|:-------|:------|:------------------------|
| mail   | 1      | 邮件威胁。            |
| url    | 2      | URL 威胁。             |
| file   | 3      | 附件文件威胁。 |

### <a name="threatexpectedassessment-values"></a>threatExpectedAssessment 值

| 成员  | 值 | Description                       |
|:--------|:------|:----------------------------------|
| block   | 1      | 应阻止威胁。     |
| unblock | 2      | 不应阻止威胁。 |

### <a name="threatcategory-values"></a>threatCategory 值

| 成员             | 值 | Description        |
|:-------------------|:------|:-------------------|
| 垃圾邮件 (spam)               | 1      | 垃圾邮件威胁。       |
| 仿冒           | 2      | 网络钓鱼威胁。   |
| 恶意软件            | 3      | 恶意软件威胁。    |
| unknownFutureValue | 4      | sentinel 成员。 |

### <a name="threatassessmentstatus-values"></a>threatAssessmentStatus 值

| 成员    | 值 | Description                              |
|:----------|:------|:-----------------------------------------|
| 挂起   | 1      | 威胁评估仍在进行中。 |
| 已完成 | 2      | 威胁评估已完成。         |

### <a name="threatassessmentrequestsource-values"></a>threatAssessmentRequestSource 值

| 成员        | 值 | Description              |
|:--------------|:------|:-------------------------|
| undefined     | 0     | 尚不知道。            |
| user          | 1      | 用户提交。         |
| administrator | 2      | 租户管理员提交。 |

### <a name="threatassessmentresulttype-values"></a>threatAssessmentResultType 值

| 成员             | 值 | Description                                          |
|:-------------------|:------|:-----------------------------------------------------|
| checkPolicy        | 1      | 策略检查结果，仅适用于 `mail` 评估。 |
| rescan             | 2      | 重新扫描结果。                                   |
| unknownFutureValue | 3      | sentinel 成员。                                   |

### <a name="maildestinationroutingreason-values"></a>mailDestinationRoutingReason 值

| 成员                | 值 | Description                         |
|:----------------------|:------|:------------------------------------|
| 无                  | 0     | 尚不知道。                       |
| mailFlowRule          | 1      | Exchange 传输规则。            |
| safeSender            | 2      | 安全发件人列表。                   |
| blockedSender         | 3      | 阻止的发件人列表。                |
| advancedSpamFiltering | 4      | 高级垃圾邮件阻止选项。     |
| domainAllowList       | 5      | 发件人域允许列表。           |
| domainBlockList       | 6      | 发件人域阻止列表。           |
| notInAddressBook      | 7      | 排除不在通讯簿中的发件人。 |
| firstTimeSender       | 8      | 因第一次发送者而阻止。   |
| autoPurgeToInbox      | 9      | TimeTravel 将邮件移动到收件箱。   |
| autoPurgeToJunk       | 10      | TimeTravel 将邮件移动到垃圾邮件。    |
| autoPurgeToDeleted    | 11    | 要删除的 TimeTravel 移动消息。 |
| 出站              | 12     | 出站邮件。                      |
| notJunk               | 13     | 允许，因为不是垃圾邮件。              |
| 垃圾邮件                  | 14     | 因垃圾邮件被阻止。                |
| unknownFutureValue    | 15     | sentinel 成员。                  |

### <a name="chatmessagepolicyviolationdlpactiontype-values"></a>chatMessagePolicyViolationDlpActionType 值

| 值 |
|:-----------------|
| 无 |
| NotifySender |
| BlockAccess |
| BlockAccessExternal |

### <a name="chatmessagepolicyviolationuseractiontype-values"></a>chatMessagePolicyViolationUserActionType 值

| 成员   | Int 值 |  说明 |
|:---------------|:--------|:----------|
| 无 | 0 | 默认值。 当用户未对 DLP 阻止的邮件采取操作时，此值为邮件上的值。 |
| Override | 1  | 发件人已重写了邮件裁定，并发送了该邮件。|
| ReportFalsePositive | 2  | 发件人将邮件裁定报告给管理员为误报。|

### <a name="chatmessagepolicyviolationverdictdetailstype-values"></a>chatMessagePolicyViolationVerdictDetailsType 值

| 成员   | Int 值 |  说明 |
|:---------------|:--------|:----------|
| 无 | 0 |  不允许用户覆盖邮件。 如果未提供策略提示，则不允许用户将邮件报告为误报。 在所有其他方案中，用户可以将邮件报告为误报。|
| AllowFalsePositiveOverride | 1  |  除非此块与或标志组合在一起，否则不允许用户显式 `AllowOverrideWithoutJustification` 覆盖 `AllowOverrideWithJustification` 此块。 报告违反行为误报将自动覆盖阻止并发送邮件。 |
| AllowOverrideWithoutJustification | 2  | 允许用户覆盖阻止并发送邮件。 理由文本不是必需的。 独占到 `AllowOverrideWithJustification` 。 |
| AllowOverrideWithJustification | 4  |  允许用户覆盖阻止并发送邮件。 理由文本是必需的。 独占到 `AllowOverrideWithoutJustification` 。|

### <a name="channelmembershiptype-values"></a>channelMembershipType 值

| 成员             | 值 |Description|
| :----------------- | :---- |:-----------|
| standard           | 0     |频道继承父团队成员的列表。|
| private            | 1      |频道的成员可以是父团队中所有成员的子集。|
| unknownFutureValue | 2      |      |
### <a name="wellknownlistname-values"></a>wellknownListName 值
| 成员
|:----------------------
| 无
| defaultList
| flaggedEmails
| unknownFutureValue

### <a name="taskstatus-values"></a>taskStatus 值
| 成员
|:----------------------
| notStarted
| inProgress
| 已完成
| waitingOnOthers
| 延迟

### <a name="permissionclassificationtype-values"></a>permissionClassificationType 值

| 成员
|:-------
| low

### <a name="permissiontype-values"></a>permissionType 值

| 成员
|:-------------------------
| 应用程序
| delegated
| delegatedUserConsentable

### <a name="printcolormode-values"></a>printColorMode 值 

|成员|
|:---|
|blackAndWhite|
|灰度|
|颜色|
|自动|
|unknownFutureValue|

### <a name="printduplexmode-values"></a>printDuplexMode 值 

|成员|
|:---|
|flipOnLongEdge|
|flipOnShortEdge|
|oneSided|
|unknownFutureValue|

### <a name="printerfeedorientation-values"></a>printerFeedOrientation 值 

|成员|
|:---|
|longEdgeFirst|
|shortEdgeFirst|
|unknownFutureValue|

### <a name="printfinishing-values"></a>printFinishing 值 

|成员|
|:---|
|无|
|装订|
|60|
|cover|
|bind|
|itchstitch|
|所edge|
|装订TopLeft|
|装订BottomLeft|
|装订TopRight|
|装订BottomRight|
|stitchLeftEdge|
|将topEdge|
|将rightEdge|
|stitchBottomEdge|
|装订DualLeft|
|装订DualTop|
|装订DualRight|
|装订DualBottom|
|unknownFutureValue|

### <a name="printmultipagelayout-values"></a>printMultipageLayout 值 

|成员|
|:---|
|顺时针FromTopLeft|
|counterclockwiseFromTopLeft|
|counterclockwiseFromTopRight|
|顺时针FromTopRight|
|counterclockwiseFromBottomLeft|
|顺时针FromBottomLeft|
|counterclockwiseFromBottomRight|
|顺时针FromBottomRight|
|unknownFutureValue|

### <a name="printorientation-values"></a>printOrientation 值 

|成员|
|:---|
|纵向|
|landscape|
|reverseLandscape|
|reversePortrait|
|unknownFutureValue|

### <a name="printquality-values"></a>printQuality 值 

|成员|
|:---|
|low|
|中等|
|high|
|unknownFutureValue|

### <a name="printscaling-values"></a>printScaling 值 

|成员|
|:---|
|自动|
|shrinkToFit|
|fill|
|fit|
|无|
|unknownFutureValue|