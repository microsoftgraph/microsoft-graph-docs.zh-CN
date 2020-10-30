---
title: 枚举值
description: Microsoft Graph 枚举值。
localization_priority: Normal
ms.prod: non-product-specific
author: MSGraphDocsvTeam
doc_type: enumPageType
ms.openlocfilehash: 4e8cf9ceb5087d497f5ebb3464425fc945e672e7
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797135"
---
# <a name="enum-values"></a>枚举值

命名空间：microsoft.graph

### <a name="activitytype-values"></a>activityType 值

|Member|
|:---|
|登录|
|user|
|向 unknownfuturevalue|

### <a name="riskdetectiontimingtype-values"></a>riskDetectionTimingType 值

|Member|
|:---|
|notDefined|
|实时|
|nearRealtime|
|脱机|
|向 unknownfuturevalue|

### <a name="tokenissuertype-values"></a>tokenIssuerType 值

|Member|
|:---|
|AzureAD|
|ADFederationServices|
|向 unknownfuturevalue|

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
|彼此|1| 用户的相对路径。|
|aide|双面| 用户的 aide。|
|dr.|第三章| 用户的医生。|
|监护|4 | 用户的监护人。|
|Child|5 | 用户的子级。|
|相互|6 | 与用户的未指定关系。|
|向 unknownfuturevalue|7 | 用于将来兼容性的标记值。|

### <a name="scheduleentitytheme-values"></a>scheduleEntityTheme 值

| Member
|:-------------------------
| white
| 蓝色
| 绿色
| 紫色
| 粉色
| 黄色
| 底纹
| darkBlue
| darkGreen
| darkPurple
| darkPink
| darkYellow
| 向 unknownfuturevalue


### <a name="timeoffreasonicontype-values"></a>timeOffReasonIconType 值

|Member|
|:---|
|无|
|car|
|日历|
|运行|
|plane|
|firstAid|
|dr.|
|notWorking|
|构造|
|juryDuty|
|投放|
|cup of|
|phone|
|气候|
|防护|
|piggyBank|
|狗|
|桩|
|trafficCone|
|针|
|sunny|
|向 unknownfuturevalue|

### <a name="timezonestandard-values"></a>timeZoneStandard 值

| Member
|:-----------------
| 时间
| iana


### <a name="freebusystatus-values"></a>freeBusyStatus 值

| 成员            |值
|:------------------|:-------
| 任意              | 0
| 暂         | 1
| 空闲              | 双面
| oof               | 第三章
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
| 各种


### <a name="automaticrepliesstatus-values"></a>automaticRepliesStatus 值

| Member
|:-------------------------
| 禁用
| Alwaysenabled 启用
| scheduled


### <a name="calendarcolor-values"></a>calendarColor 值

| 成员     | 值
|:-----------|:----------
| 自动       | -1
| lightBlue  | 0
| lightGreen | 1
| lightOrange| 双面
| lightGray  | 第三章
| lightYellow| 4 
| lightTeal  | 5 
| lightPink  | 6 
| lightBrown | 7 
| lightRed   | 8 
| maxColor   | 9 


### <a name="educationexternalsource-values"></a>educationExternalSource 值

| Member
|:-------------------------
| sis
| 手动
| 向 unknownfuturevalue


### <a name="educationgender-values"></a>educationGender 值

| Member
|:-------------------------
| 接头
| 触点
| 相互
| 向 unknownfuturevalue


### <a name="eventtype-values"></a>事件的值

| Member
|:-------------------------
| singleInstance
| 重复
| 异常
| seriesMaster


### <a name="sensitivity-values"></a>敏感度值

| Member
|:-------------------------
| 通用
| personal
| private
| 秘密


### <a name="importance-values"></a>重要性值

| Member
|:-------------------------
| 降低
| 通用
| 高效


### <a name="educationuserrole-values"></a>educationUserRole 值
| Member
|:---------------------
| student
| teacher

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
| 带


### <a name="inferenceclassificationtype-values"></a>inferenceClassificationType 值

| Member
|:-----------------
| 介绍
| 相互


### <a name="iosnotificationalerttype-values"></a>iosNotificationAlertType 值

| Member
|:-------------------------
| deviceDefault
| 分隔
| 适合
| 无

### <a name="deviceenrollmentfailurereason-values"></a>deviceEnrollmentFailureReason 值

| Member
|:-------------
| unknown
| authentication
| 批准
| accountValidation
| userValidation
| deviceNotSupported
| inMaintenance
| badRequest
| featureNotSupported
| enrollmentRestrictionsEnforced
| clientDisconnected


### <a name="bodytype-values"></a>Office.mailboxenums.bodytype 值
| Member
|:---------
| text
| html


### <a name="locationtype-values"></a>locationType 值

| Member
|:-------------------------
| 设置
| conferenceRoom
| homeAddress
| businessAddress
| geoCoordinates
| streetAddress
| 住
| 餐馆
| localBusiness
| postalAddress

### <a name="locationuniqueidtype-values"></a>locationUniqueIdType 值

| Member
|:-------------------------
| unknown
| locationStore
| 文件夹
| private
| 必应


### <a name="messageactionflag-values"></a>messageActionFlag 值

| Member
|:-------------------------
| 任意
| 通话
| doNotForward
| 努力
| 仅供参考
| 转发
| noResponseNecessary
| 阅读
| 回复
| replyToAll
| 概述


### <a name="onenoteuserrole-values"></a>onenoteUserRole 值

| 成员      | 值
|:------------|:------------
| 所有者       | 0
| 参与者 | 1
| 读者      | 双面
| 无        | -1


### <a name="operationstatus-values"></a>operationStatus 值

| Member
|:-----------------
| NotStarted
| 正在运行
| Completed
| 已失败


### <a name="onenotepatchactiontype-values"></a>onenotePatchActionType 值

| Member
|:-------------------------
| 替换
| Append
| 删除
| Insert
| 计算

### <a name="onenotepatchinsertposition-values"></a>onenotePatchInsertPosition 值

| Member
|:-------------------------
| 段后
| Before


### <a name="phonetype-values"></a>phoneType 值

| Member
|:-------------------------
| 回收
| 知情
| mobile
| 相互
| 协助
| homeFax
| businessFax
| otherFax
| pager
| 无线电台


### <a name="plannerpreviewtype-values"></a>plannerPreviewType 值

| Member
|:-------------------------
| 自动
| noPreview
| checklist
| description
| 参考


### <a name="status-values"></a>status 值

| Member
|:-----------------
| 工作
| updated
| deleted
| 忽略
| 向 unknownfuturevalue


### <a name="weekindex-values"></a>weekIndex 值

| Member
|:-------------------------
| 前
| 第二个
| 次
| 四分之一
| 末


### <a name="dayofweek-values"></a>dayOfWeek 值

| Member
|:-------------------------
| 日
| 星期一
| 2001
| 星期三
| 星期三
| 之前
| 星期六

### <a name="recurrencepatterntype-values"></a>recurrencePatternType 值

| Member
|:-------------------------
| 每日
| 周历
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>recurrenceRangeType 值

| Member
|:-------------------------
| endDate
| noEnd
| 数字化


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
| organizer － 组织者
| tentativelyAccepted
| 接受
| 邀请
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
| 相互
| 回收
| 工时
| 博客
| 个人资料


### <a name="categorycolor-values"></a>categoryColor 值

| 成员   |值
|:---------|:--------
| 无     | -1
| preset0  | 0
| preset1  | 1
| preset2  | 双面
| preset3  | 第三章
| preset4  | 4 
| preset5  | 5 
| preset6  | 6 
| preset7  | 7 
| preset8  | 8 
| preset9  | 9 
| preset10 | 10  
| preset11 | 11x17
| preset12 | 12 
| preset13 | 13 
| preset14 | 14 
| preset15 | 15 
| preset16 | 16 
| preset17 | 17 
| preset18 | 18 
| preset19 | 合
| preset20 | 20
| preset21 |  21
| preset22 | 22
| preset23 | 上午
| preset24 | 24

### <a name="alertfeedback-values"></a>alertFeedback 值

由分析师提供的警报上可能的反馈值。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|陌生.|
|truePositive|1|警报为 true-肯定。|
|falsePositive|双面| 警报为 false-肯定。|
|benignPositive|第三章| 警报为良性-肯定。|

### <a name="filehashtype-values"></a>fileHashType 值

文件哈希类型的枚举。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知类型。|
|sha1|1|SHA1 哈希类型。|
|sha256|双面| SHA256 哈希类型。|
|md5|第三章| MD5 哈希类型。|
|authenticodeHash256|4 | AuthenticodeHash256 哈希类型。|
|lsHash|5 | LsHash 哈希类型。|
|ctph|6 | CTPH 哈希类型。|
|peSha1|7 | PESHA1 哈希类型。|
|peSha256|8 | PESHA256 哈希类型。|

### <a name="connectiondirection-values"></a>connectionDirection 值

 (入站/出站) 的网络连接的方向的枚举。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知的连接。|
|进货|1|入站连接。|
|出站|双面| 出站连接。|

### <a name="connectionstatus-values"></a>connectionStatus 值

连接状态的枚举。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知的连接状态。|
|尝试|1|已尝试连接。|
|完成|双面| 连接成功。|
|堵塞|第三章| 连接被阻止。|
|未能|4 | 连接失败。|

### <a name="processintegritylevel-values"></a>processIntegrityLevel 值

进程的可能完整性级别值。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|陌生.|
|可信|10  |完整性级别不受信任。|
|降低|20| 完整性级别较低。|
|中等|30| 完整性级别为 "中"。|
|高效|40| 完整性级别为 "高"。|
|system|50| 完整性级别为 "系统"。|

### <a name="registryhive-values"></a>registryHive 值

由 [/windows/desktop/sysinfo/registry-hives](/windows/desktop/sysinfo/registry-hives)定义的注册表配置单元的枚举。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知配置单元。|
|currentConfig|1|HKEY_CURRENT_CONFIG 配置单元。|
|currentUser|双面| HKEY_CURRENT_USER 配置单元。|
|localMachineSam|第三章| HKEY_LOCAL_MACHINE\SAM 配置单元。|
|localMachineSamSoftware|4 | HKEY_LOCAL_MACHINE\Software 配置单元。|
|localMachineSystem|5 | HKEY_LOCAL_MACHINE\System 配置单元。|
|usersDefault|6 | HKEY_USERS \\ 。默认配置单元。|

### <a name="registryoperation-values"></a>registryOperation 值

更改注册表项名称和/或值的操作。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知的注册表值类型。|
|create|1|创建注册表。|
|modify|双面|修改注册表。|
|delete|第三章|删除注册表。|

### <a name="registryvaluetype-values"></a>registryValueType 值

由 [/windows/desktop/sysinfo/registry-value-types](/windows/desktop/sysinfo/registry-value-types)定义的注册表值类型的枚举。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知的注册表值类型。|
|数字|1|REG_BINARY 注册表值类型。|
|值|双面| REG_DWORD 注册表值类型。|
|dwordLittleEndian|第三章| REG_DWORD_LITTLE_ENDIAN 注册表值类型。|
|dwordBigEndian|4 | REG_DWORD_BIG_ENDIAN 注册表值类型。|
|expandSz|5 | REG_EXPAND_SZ 注册表值类型。|
|link|6 | REG_LINK 注册表值类型。|
|multiSz|7 | REG_MULTI_SZ 注册表值类型。|
|无|8 | REG_NONE 注册表值类型。|
|qword|9 | REG_QWORD 注册表值类型。|
|qwordlittleEndian|10  | REG_QWORD_LITTLE_ENDIAN 注册表值类型。|
|sz|11x17| REG_SZ 注册表值类型。|

### <a name="alertseverity-values"></a>alertSeverity 值

警报严重性的枚举。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|严重度未知。|
|之|1|严重性仅适用于信息。|
|降低|双面| 严重性为低。|
|中等|第三章| 严重性为 "中"。|
|高效|4 | 严重性为高。|

### <a name="alertstatus-values"></a>alertStatus 值

 (stage) 的警报生命周期状态的可能值。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知状态。|
|newAlert|10  | 警报是新的。|
|inProgress|20|警报正在进行中。|
|已解决|30|警报已解决。|

### <a name="emailrole-values"></a>emailRole 值
电子邮件角色的可能值。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知角色。|
|sender|1|电子邮件的发件人。|
|recipient|双面|电子邮件的收件人。|

### <a name="logontype-values"></a>logonType 值

用户登录方法的可能值。

|成员|值|说明|
|:---|:---|:---|
|unknown|-1|陌生.|
|式|0|登录是交互式的。|
|remoteInteractive|1| 登录是远程交互的。|
|network|双面| 登录为网络。|
|batch|第三章| 登录是批处理。|
|服务|4 | 登录为 "服务"。|

### <a name="useraccountsecuritytype-values"></a>userAccountSecurityType 值

每个 Windows 定义 (组成员身份) 的用户帐户类型的可能值。

|Member|成员|说明|
|:---|:---|:---|
|unknown|-1|陌生.|
|普通|0|"标准用户" 组的成员。|
|能力|1| Power Users 组的成员。|
|联系|双面| Administrators 组的成员。|

### <a name="riskdetail-values"></a>riskDetail 值

| Member
|:-------------------------
| adminGeneratedTemporaryPassword
| userPerformedSecuredPasswordChange
| userPerformedSecuredPasswordReset
| adminConfirmedSigninSafe
| aiConfirmedSigninSafe
| userPassedMFADrivenByRiskBasedPolicy
| adminDismissedAllRiskForUser
| adminConfirmedSigninCompromised
| 向 unknownfuturevalue

### <a name="riskeventtypes-values"></a>riskEventTypes 值

| Member
|:-------------------------
| unlikelyTravel
| anonymizedIPAddress
| maliciousIPAddress
| unfamiliarFeatures
| malwareInfectedIPAddress
| suspiciousIPAddress
| leakedCredentials
| investigationsThreatIntelligence
| 泛型
| 向 unknownfuturevalue

### <a name="riskeventtype-values"></a>riskEventType 值

|Member|
|:---|
|unlikelyTravel|
|anonymizedIPAddress|
|maliciousIPAddress|
|unfamiliarFeatures|
|malwareInfectedIPAddress|
|suspiciousIPAddress|
|leakedCredentials|
|investigationsThreatIntelligence|
|泛型|
|adminConfirmedUserCompromised|
|mcasImpossibleTravel|
|mcasSuspiciousInboxManipulationRules|
|investigationsThreatIntelligenceSigninLinked|
|maliciousIPAddressValidCredentialsBlockedIP|
|向 unknownfuturevalue|

### <a name="risklevel-values"></a>riskLevel 值

| Member
|:-------------------------
| 无
| 降低
| 中等
| 高效
| hidden
| 向 unknownfuturevalue

### <a name="riskstate-values"></a>riskState 值

| Member
|:-------------------------
| 无
| confirmedSafe
| 得以
| 清除
| atRisk
| confirmedCompromised
| 向 unknownfuturevalue

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
|自|

### <a name="threatassessmentcontenttype-values"></a>threatAssessmentContentType 值

| 成员 | 值 | 说明             |
|:-------|:------|:------------------------|
| mail   | 1     | 邮件威胁。            |
| url    | 双面     | URL 威胁。             |
| file   | 第三章     | 附件文件威胁。 |

### <a name="threatexpectedassessment-values"></a>threatExpectedAssessment 值

| 成员  | 值 | 说明                       |
|:--------|:------|:----------------------------------|
| 数据   | 1     | 应阻止该威胁。     |
| 阻塞 | 双面     | 不应阻止该威胁。 |

### <a name="threatcategory-values"></a>threatCategory 值

| 成员             | 值 | 说明        |
|:-------------------|:------|:-------------------|
| 垃圾邮件 (spam)               | 1     | 垃圾邮件威胁。       |
| 仿冒           | 双面     | 网络钓鱼威胁。   |
| 受到            | 第三章     | 恶意软件威胁。    |
| 向 unknownfuturevalue | 4      | 一个 sentinel 成员。 |

### <a name="threatassessmentstatus-values"></a>threatAssessmentStatus 值

| 成员    | 值 | 说明                              |
|:----------|:------|:-----------------------------------------|
| 决   | 1     | 威胁评估仍在进行中。 |
| 后 | 双面     | 威胁评估已完成。         |

### <a name="threatassessmentrequestsource-values"></a>threatAssessmentRequestSource 值

| 成员        | 值 | 说明              |
|:--------------|:------|:-------------------------|
| 取消     | 0     | 尚不知道。            |
| user          | 1     | 用户提交。         |
| 联系 | 双面     | 租户管理员提交。 |

### <a name="threatassessmentresulttype-values"></a>threatAssessmentResultType 值

| 成员             | 值 | 说明                                          |
|:-------------------|:------|:-----------------------------------------------------|
| checkPolicy        | 1     | 策略检查结果，仅用于 `mail` 评估。 |
| 重新扫描             | 双面     | 重新扫描结果。                                   |
| 向 unknownfuturevalue | 第三章     | 一个 sentinel 成员。                                   |

### <a name="maildestinationroutingreason-values"></a>mailDestinationRoutingReason 值

| 成员                | 值 | 说明                         |
|:----------------------|:------|:------------------------------------|
| 无                  | 0     | 尚不知道。                       |
| mailFlowRule          | 1     | Exchange 传输规则。            |
| safeSender            | 双面     | 安全发件人列表。                   |
| blockedSender         | 第三章     | 阻止发件人列表。                |
| advancedSpamFiltering | 4      | 高级垃圾邮件 flitering 选项。     |
| domainAllowList       | 5      | 发件人域允许列表。           |
| domainBlockList       | 6      | 发件人域阻止列表。           |
| notInAddressBook      | 7      | 将发件人排除在通讯簿之外。 |
| firstTimeSender       | 8      | 由于第一次发件人而被阻止。   |
| autoPurgeToInbox      | 9      | TimeTravel 将邮件移动到收件箱。   |
| autoPurgeToJunk       | 10      | TimeTravel 将邮件移动到垃圾邮件。    |
| autoPurgeToDeleted    | 11x17    | TimeTravel 将邮件移动到 "已删除"。 |
| 出站              | 12     | 出站邮件。                      |
| notJunk               | 13     | 由于非垃圾邮件而启用。              |
| 可疑                  | 14     | 由于垃圾邮件而被阻止。                |
| 向 unknownfuturevalue    | 15     | 一个 sentinel 成员。                  |

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
| 无 | 0 | 默认值。 这是用户未对 DLP 阻止的邮件执行操作时邮件上的值。 |
| Override | 1 | 发件人已覆盖邮件结论并发送邮件。|
| ReportFalsePositive | 双面 | 发件人已将邮件 "肯定为" 作为 "误报" 的管理员报告。|

### <a name="chatmessagepolicyviolationverdictdetailstype-values"></a>chatMessagePolicyViolationVerdictDetailsType 值

| Member   | Int 值 |  说明 |
|:---------------|:--------|:----------|
| 无 | 0 |  不允许用户覆盖邮件。 如果未提供 policyTip，则不允许用户将邮件报告为误报。 在所有其他情况下，用户可以将邮件报告为误报。|
| AllowFalsePositiveOverride | 1 |  不允许用户显式重写 block，除非将其与 `AllowOverrideWithoutJustification` 或标志组合 `AllowOverrideWithJustification` 。 对违规报告误报会自动覆盖该阻止并发送邮件。 |
| AllowOverrideWithoutJustification | 双面 | 允许用户替代阻止并发送邮件。 不需要对齐文本。 专用于 `AllowOverrideWithJustification` 。 |
| AllowOverrideWithJustification | 4  |  允许用户替代阻止并发送邮件。 需要理由文本。 专用于 `AllowOverrideWithoutJustification` 。|

### <a name="wellknownlistname-values"></a>wellknownListName 值
| Member
|:----------------------
| 无
| defaultList
| flaggedEmails
| 向 unknownfuturevalue

### <a name="taskstatus-values"></a>taskStatus 值
| Member
|:----------------------
| notStarted
| inProgress
| 后
| waitingOnOthers
| 关联表
