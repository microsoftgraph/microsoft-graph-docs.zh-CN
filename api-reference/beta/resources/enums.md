---
title: 枚举值
description: Microsoft Graph 枚举值
doc_type: enumPageType
localization_priority: Normal
ms.prod: non-product-specific
author: MSGraphDocsvTeam
ms.openlocfilehash: ef7e62be359faf7284d786ed1b0cbb300fd47b83
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581143"
---
# <a name="enum-values"></a>枚举值

命名空间：microsoft.graph

### <a name="volumetype-values"></a>volumeType 值

| Member
|:--------------
| operatingSystemVolume
| fixedDataVolume
| removableDataVolume
| 向 unknownfuturevalue

### <a name="allowedaudiences-values"></a>allowedAudiences 值

|Member|
|:---|
|me|
|家长|
|contacts|
|groupMembers|
|组织|
|federatedOrganizations|
|成员|
|向 unknownfuturevalue|

### <a name="attestationlevel-values"></a>attestationLevel 值

|Member|
|:---|
|证明|
|notAttested|

### <a name="emailtype-values"></a>emailType 值

|Member|
|:---|
|unknown|
|工时|
|personal|
|spy|
|相互|

### <a name="authenticationmethodtargettype-values"></a>authenticationMethodTargetType 值

|Member|
|:---|
|user|
|group|

### <a name="authenticationmethodstate-values"></a>authenticationMethodState 值

|Member|
|:---|
|enabled|
|禁用|

### <a name="fido2restrictionenforcementtype-values"></a>fido2RestrictionEnforcementType 值

|Member|
|:---|
|允许|
|数据|

### <a name="authenticatorappcontexttype-values"></a>authenticatorAppContextType 值

|Member|
|:---|
|位置|
|应用|

### <a name="anniversarytype-values"></a>anniversaryType 值

|Member|
|:---|
|birthday|
|筹划|
|向 unknownfuturevalue|

### <a name="skillproficiencylevel-values"></a>skillProficiencyLevel 值

|Member|
|:---|
|初级|
|limitedWorking|
|generalProfessional|
|advancedProfessional|
|处理器|
|向 unknownfuturevalue|

### <a name="languageproficiencylevel-values"></a>languageProficiencyLevel 值

|Member|
|:---|
|初级|
|对话|
|limitedWorking|
|professionalWorking|
|fullProfessional|
|nativeOrBilingual|
|向 unknownfuturevalue|

### <a name="personrelationship-values"></a>personRelationship 值

|Member|
|:---|
|manager|
|同事|
|directReport|
|dotLineReport|
|协助|
|dotLineManager|
|alternateContact|
|给|
|姓名|
|同辈|
|Child|
|父级|
|发起人|
|emergencyContact|
|相互|
|向 unknownfuturevalue|

### <a name="attachmenttype-values"></a>attachmentType 值

| Member
|:--------------
| file
| 项
| 参考

### <a name="analyticsactivitytype-values"></a>analyticsActivityType 值

| Member
|:--------------
| 通话
| 聊天
| email
| 焦点
| 要求

### <a name="registrationauthmethod-values"></a>registrationAuthMethod 值

|Member|
|:---|
|email|
|mobilePhone|
|officePhone|
|securityQuestion|
|appNotification|
|appCode|
|alternateMobilePhone|

### <a name="entitytypes-values"></a>entityTypes 值

|Member|
|:---|
|event|
|message|
|driveItem|
|externalItem|
|网站|
|list|
|listItem|
|驱动器|

### <a name="bucketaggregationsortproperty-values"></a>bucketAggregationSortProperty 值

|Member|
|:---|
|count|
|keyAsString|
|keyAsNumber|

### <a name="contactrelationship-values"></a>contactRelationship 值

| 成员             | 值 | Description                              |
| :----------------- | :---- | :--------------------------------------- |
| 父级             | 0     | 用户的父级。                       |
| 彼此           | 1      | 用户的相对路径。                     |
| aide               | 2      | 用户的 aide。                         |
| dr.             | 3      | 用户的医生。                       |
| 监护           | 4      | 用户的监护人。                     |
| Child              | 5      | 用户的子级。                        |
| 相互              | 6      | 与用户的未指定关系。 |
| 向 unknownfuturevalue | 7      | 用于将来兼容性的标记值。   |

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

### <a name="schedulechangestate-values"></a>scheduleChangeState 值

| Member
|:----------------------------
|决
|批准
|邀请
|向 unknownfuturevalue

### <a name="schedulechangerequestactor-values"></a>scheduleChangeRequestActor 值

| Member
|:----------------------------
|sender
|recipient
|manager
|system
|向 unknownfuturevalue

### <a name="workforceintegrationencryptionprotocol-values"></a>workforceIntegrationEncryptionProtocol 值

| Member
|:----------------------------
|sharedSecret
|向 unknownfuturevalue

### <a name="workforceintegrationsupportedentities-values"></a>workforceIntegrationSupportedEntities 值

| Member
|:----------------------------
|无
|Shift
|swapRequest
|openShift
|openShiftRequest
|userShiftPreferences

### <a name="timezonestandard-values"></a>timeZoneStandard 值

| Member
|:-----------------
| 时间
| iana


### <a name="freebusystatus-values"></a>freeBusyStatus 值

| 成员           | 值 |
| :--------------- | :---- |
| 任意             | 0     |
| 暂        | 1      |
| 空闲             | 2      |
| oof              | 3      |
| workingElsewhere | 4      |
| unknown          | -1    |


### <a name="physicaladdresstype-values"></a>: Physicaladdresstype 值

| Member
|:-------------------------
| unknown
| 回收
| 知情
| 相互


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

| 成员      | 值 |
| :---------- | :---- |
| 自动        | -1    |
| lightBlue   | 0     |
| lightGreen  | 1      |
| lightOrange | 2      |
| lightGray   | 3      |
| lightYellow | 4      |
| lightTeal   | 5      |
| lightPink   | 6      |
| lightBrown  | 7      |
| lightRed    | 8      |
| maxColor    | 9      |


### <a name="educationsynchronizationprofilestate-values"></a>educationSynchronizationProfileState 值

| 成员             | 值 |
| :----------------- | :---- |
| 删除           | 2      |
| deletionFailed     | 3      |
| provisioningFailed | 5      |
| 已设置        | 6      |
| 设置       | 7      |
| 向 unknownfuturevalue | 8      |


### <a name="educationsynchronizationstatus-values"></a>educationSynchronizationStatus 值

| 成员             | 值 |
| :----------------- | :---- |
| 停留             | 0     |
| inProgress         | 1      |
| success            | 2      |
| error              | 3      |
| validationError    | 4      |
| 隔离        | 5      |
| 向 unknownfuturevalue | 6      |

### <a name="educationexternalsource-values"></a>educationExternalSource 值

| Member
|:-------------------------
| sis
| lms
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
| 人员


### <a name="meetingmessagetype-values"></a>meetingMessageType 值

| Member
|:-----------------
| 无
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTentativelyAccepted
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
| 响应
| replyToAll
| 概述


### <a name="onenoteuserrole-values"></a>onenoteUserRole 值

| 成员      | 值 |
| :---------- | :---- |
| 所有者       | 0     |
| 参与者 | 1      |
| 读者      | 2      |
| 无        | -1    |


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
| Delete
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
| 说明
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
| 组织者
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

| 成员   | 值 |
| :------- | :---- |
| 无     | -1    |
| preset0  | 0     |
| preset1  | 1      |
| preset2  | 2      |
| preset3  | 3      |
| preset4  | 4      |
| preset5  | 5      |
| preset6  | 6      |
| preset7  | 7      |
| preset8  | 8      |
| preset9  | 9      |
| preset10 | 10     |
| preset11 | 11     |
| preset12 | 12     |
| preset13 | 13     |
| preset14 | 14     |
| preset15 | 15     |
| preset16 | 16     |
| preset17 | 17     |
| preset18 | 18     |
| preset19 | 合    |
| preset20 | 20    |
| preset21 |  21    |
| preset22 | 22    |
| preset23 | 上午    |
| preset24 | 24    |

### <a name="alertfeedback-values"></a>alertFeedback 值

由分析师提供的警报上可能的反馈值。

| 成员         | 值 | Description               |
| :------------- | :---- | :------------------------ |
| unknown        | 0     | 陌生.                  |
| truePositive   | 1      | 警报为 true-肯定。   |
| falsePositive  | 2      | 警报为 false-肯定。  |
| benignPositive | 3      | 警报为良性-肯定。 |

### <a name="filehashtype-values"></a>fileHashType 值

| 成员              | 值 | Description                    |
| :------------------ | :---- | :----------------------------- |
| unknown             | 0     | 未知类型。                  |
| sha1                | 1      | SHA1 哈希类型。                |
| sha256              | 2      | SHA256 哈希类型。              |
| md5                 | 3      | MD5 哈希类型。                 |
| authenticodeHash256 | 4      | AuthenticodeHash256 哈希类型。 |
| lsHash              | 5      | LsHash 哈希类型。              |
| ctph                | 6      | CTPH 哈希类型。                |
| peSha1              | 7      | PESHA1 哈希类型。              |
| peSha256            | 8      | PESHA256 哈希类型。            |

### <a name="connectiondirection-values"></a>connectionDirection 值

| 成员   | 值 | Description          |
| :------- | :---- | :------------------- |
| unknown  | 0     | 未知的连接。  |
| 进货  | 1      | 入站连接。  |
| 出站 | 2      | 出站连接。 |

### <a name="connectionstatus-values"></a>connectionStatus 值

| 成员    | 值 | Description                |
| :-------- | :---- | :------------------------- |
| unknown   | 0     | 未知的连接状态。 |
| 尝试 | 1      | 已尝试连接。      |
| 完成 | 2      | 连接成功。      |
| 堵塞   | 3      | 连接被阻止。        |
| 未能    | 4      | 连接失败。         |

### <a name="processintegritylevel-values"></a>processIntegrityLevel 值

| 成员    | 值 | Description                   |
| :-------- | :---- | :---------------------------- |
| unknown   | 0     | 陌生.                      |
| 可信 | 10     | 完整性级别不受信任。 |
| 降低       | 20    | 完整性级别较低。       |
| 中等    | 30    | 完整性级别为 "中"。    |
| 高效      | 40    | 完整性级别为 "高"。      |
| system    | 50    | 完整性级别为 "系统"。    |

### <a name="registryhive-values"></a>registryHive 值

由定义的注册表配置单元的枚举 [https://docs.microsoft.com/windows/desktop/sysinfo/registry-hives](/windows/desktop/sysinfo/registry-hives) 。

| 成员                  | 值 | Description                       |
| :---------------------- | :---- | :-------------------------------- |
| unknown                 | 0     | 未知配置单元。                     |
| currentConfig           | 1      | HKEY_CURRENT_CONFIG 配置单元。         |
| currentUser             | 2      | HKEY_CURRENT_USER 配置单元。           |
| localMachineSam         | 3      | HKEY_LOCAL_MACHINE\SAM 配置单元。      |
| localMachineSamSoftware | 4      | HKEY_LOCAL_MACHINE\Software 配置单元。 |
| localMachineSystem      | 5      | HKEY_LOCAL_MACHINE\System 配置单元。   |
| usersDefault            | 6      | HKEY_USERS \\ 。默认配置单元。        |

### <a name="registryoperation-values"></a>registryOperation 值

更改注册表项名称和/或值的操作。

| 成员  | 值 | Description                  |
| :------ | :---- | :--------------------------- |
| unknown | 0     | 未知的注册表值类型。 |
| create  | 1      | 创建注册表。             |
| modify  | 2      | 修改注册表。             |
| delete  | 3      | 删除注册表。             |

### <a name="registryvaluetype-values"></a>registryValueType 值

由 [注册表值类型](/windows/desktop/sysinfo/registry-value-types)定义的注册表值类型的枚举。

| 成员            | 值 | Description                                  |
| :---------------- | :---- | :------------------------------------------- |
| unknown           | 0     | 未知的注册表值类型。                 |
| 数字            | 1      | REG_BINARY 注册表值类型。              |
| 值             | 2      | REG_DWORD 注册表值类型。               |
| dwordLittleEndian | 3      | REG_DWORD_LITTLE_ENDIAN 注册表值类型。 |
| dwordBigEndian    | 4      | REG_DWORD_BIG_ENDIAN 注册表值类型。    |
| expandSz          | 5      | REG_EXPAND_SZ 注册表值类型。           |
| link              | 6      | REG_LINK 注册表值类型。                |
| multiSz           | 7      | REG_MULTI_SZ 注册表值类型。            |
| 无              | 8      | REG_NONE 注册表值类型。                |
| qword             | 9      | REG_QWORD 注册表值类型。               |
| qwordlittleEndian | 10     | REG_QWORD_LITTLE_ENDIAN 注册表值类型。 |
| sz                | 11     | REG_SZ 注册表值类型。                  |

### <a name="alertseverity-values"></a>alertSeverity 值

警报严重性的枚举。

| 成员        | 值 | Description                       |
| :------------ | :---- | :-------------------------------- |
| unknown       | 0     | 严重度未知。              |
| 之 | 1      | 严重性仅适用于信息。 |
| 降低           | 2      | 严重性为低。                  |
| 中等        | 3      | 严重性为 "中"。               |
| 高效          | 4      | 严重性为高。                 |

### <a name="alertstatus-values"></a>alertStatus 值

 (stage) 的警报生命周期状态的可能值。

| 成员     | 值 | Description           |
| :--------- | :---- | :-------------------- |
| unknown    | 0     | 未知状态。       |
| newAlert   | 10     | 警报是新的。         |
| inProgress | 20    | 警报正在进行中。 |
| 已解决   | 30    | 警报已解决。    |

### <a name="emailrole-values"></a>emailRole 值

电子邮件角色的可能值。

| 成员    | 值 | Description             |
| :-------- | :---- | :---------------------- |
| unknown   | 0     | 未知角色。           |
| sender    | 1      | 电子邮件的发件人。    |
| recipient | 2      | 电子邮件的收件人。 |

### <a name="logontype-values"></a>logonType 值

用户登录方法的可能值。

| 成员            | 值 | Description                  |
| :---------------- | :---- | :--------------------------- |
| unknown           | -1    | 陌生.                     |
| 式       | 0     | 登录是交互式的。        |
| remoteInteractive | 1      | 登录是远程交互的。 |
| network           | 2      | 登录为网络。            |
| batch             | 3      | 登录是批处理。              |
| 服务           | 4      | 登录为 "服务"。            |

### <a name="useraccountsecuritytype-values"></a>userAccountSecurityType 值

每个 Windows 定义 (组成员身份) 的用户帐户类型的可能值。

| 成员        | 值 | Description                     |
| :------------ | :---- | :------------------------------ |
| unknown       | -1    | 陌生.                        |
| 普通      | 0     | "标准用户" 组的成员。 |
| 能力         | 1      | Power Users 组的成员。    |
| 联系 | 2      | Administrators 组的成员。 |

### <a name="chatmessagepolicyviolationdlpactiontype-values"></a>chatMessagePolicyViolationDlpActionType 值

| 值 |
|:-----------------|
| 无 |
| NotifySender |
| BlockAccess |
| BlockAccessExternal |

### <a name="scopeoperatormultivaluedcomparisontype-values"></a>scopeOperatorMultiValuedComparisonType 值

|Member|
|:---|
|各种|
|任意|

### <a name="risklevel-values"></a>riskLevel 值

|Member|
|:---|
|降低|
|中等|
|高效|
|hidden|
|无|
|向 unknownfuturevalue|

### <a name="riskstate-values"></a>riskState 值

|Member|
|:---|
|无|
|confirmedSafe|
|得以|
|清除|
|atRisk|
|confirmedCompromised|
|向 unknownfuturevalue|

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
|adminConfirmedSigninCompromised|
|adminConfirmedUserCompromised|
|hidden|
|向 unknownfuturevalue|

### <a name="referenceattachmentpermission-values"></a>referenceAttachmentPermission 值

|Member|
|:---|
|相互|
|view|
|edit|
|anonymousView|
|anonymousEdit|
|organizationView|
|organizationEdit|

### <a name="referenceattachmentprovider-values"></a>: Referenceattachmentprovider 值

|Member|
|:---|
|相互|
|oneDriveBusiness|
|oneDriveConsumer|
|箱|

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

### <a name="networktype-values"></a>网络值

|Member|
|:---|
|在内|
|powerlink|
|namedNetwork|
|获得|
|向 unknownfuturevalue|

### <a name="exchangeidformat-values"></a>exchangeIdFormat 值

|Member|
|:---|
|entryId|
|ewsId|
|immutableEntryId|
|restId|
|restImmutableEntryId|

### <a name="attributeflowbehavior-values"></a>attributeFlowBehavior 值

|Member|
|:---|
|flowWhenChanged|
|flowAlways|

### <a name="attributeflowtype-values"></a>attributeFlowType 值

|Member|
|:---|
|都|
|objectAddOnly|
|multiValueAddOnly|
|restId|

### <a name="objectflowtypes-values"></a>objectFlowTypes 值

| 成员 | 值 |
| :----- | :---- |
| 无   | 0     |
| 添加    | 1      |
| 更新 | 2      |
| Delete | 4      |

### <a name="chatmessagetype-values"></a>chatMessageType 值

|Member|
|:---|
|message|

### <a name="chatmessageimportance-values"></a>chatMessageImportance 值

|Member|
|:---|
|通用|
|高效|
|紧急|

### <a name="channelmembershiptype-values"></a>channelMembershipType 值

| 成员             | 值 |
| :----------------- | :---- |
| 普通           | 0     |
| private            | 1      |
| 向 unknownfuturevalue | 2      |

### <a name="stagedfeaturename-values"></a>stagedFeatureName 值

| 成员                    | 说明                   |
| :------------------------ | :---------------------------- |
| passthroughAuthentication | 传递身份验证    |
| seamlessSso               | 无缝单一登录       |
| passwordHashSync          | 密码哈希同步 |

### <a name="tokenissuertype-values"></a>tokenIssuerType 值

|Member|
|:---|
|AzureAD|
|ADFederationServices|
|向 unknownfuturevalue|

### <a name="riskdetectiontimingtype-values"></a>riskDetectionTimingType 值

|Member|
|:---|
|notDefined|
|实时|
|nearRealtime|
|脱机|
|向 unknownfuturevalue|

### <a name="activitytype-values"></a>activityType 值

|Member|
|:---|
|登录|
|user|
|向 unknownfuturevalue|

### <a name="chatmessagepolicyviolationuseractiontype-values"></a>chatMessagePolicyViolationUserActionType 值

| Member   | Int 值 |  说明 |
|:---------------|:--------|:----------|
| 无 | 0 | 默认值。 这是用户未对 DLP 阻止的邮件执行操作时邮件上的值。 |
| Override | 1  | 发件人已覆盖邮件结论并发送邮件。|
| ReportFalsePositive | 2  | 发件人已将邮件 "肯定为" 作为 "误报" 的管理员报告。|

### <a name="chatmessagepolicyviolationverdictdetailstype-values"></a>chatMessagePolicyViolationVerdictDetailsType 值

| Member   | Int 值 |  说明 |
|:---------------|:--------|:----------|
| 无 | 0 |  不允许用户覆盖邮件。 如果未提供 policyTip，则不允许用户将邮件报告为误报。 在所有其他情况下，用户可以将邮件报告为误报。|
| AllowFalsePositiveOverride | 1  |  不允许用户显式重写 block，除非将其与 `AllowOverrideWithoutJustification` 或标志组合 `AllowOverrideWithJustification` 。 对违规报告误报会自动覆盖该阻止并发送邮件。 |
| AllowOverrideWithoutJustification | 2  | 允许用户替代阻止并发送邮件。 不需要对齐文本。 专用于 `AllowOverrideWithJustification` 。 |
| AllowOverrideWithJustification | 4  |  允许用户替代阻止并发送邮件。 需要理由文本。 专用于 `AllowOverrideWithoutJustification` 。|

### <a name="entitytype-values"></a>entityType 值

| Member       |
|:--------------|
|event|
|message|
|driveItem|
|externalFile|
|externalItem|

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

### <a name="contentformat-values"></a>contentFormat 值

| 成员  | 值 | Description                          |
| :------ | :---- | :----------------------------------- |
| 设置 | 0     | 内容是文件或非电子邮件类型。 |
| email   | 1      | 内容是一封电子邮件。                 |

### <a name="contentstate-values"></a>contentState 值

| 成员 | 值 | Description                                                                      |
| :----- | :---- | :------------------------------------------------------------------------------- |
| 完成   | 0     | 数据是静止的;共享中的文件，例如。                                 |
| 动作 | 1      | 数据是活动的。 由传输中的网络设备截获的文件。         |
| 改用    | 2      | 数据正在使用中。 在客户端应用程序（如 Microsoft Office）中打开一个文件。 |

### <a name="assignmentmethod-values"></a>assignmentMethod 值

| 成员     | 值 | Description                                                                                                                      |
| :--------- | :---- | :------------------------------------------------------------------------------------------------------------------------------- |
| 普通   | 0     | 标签是由服务或策略条件设置的。                                                                              |
| 严格 | 1      | 标签由用户显式设置。                                                                                          |
| 自动       | 2      | 允许覆盖任何现有标签。 降级时所需的理由。 `standard`元数据中的赋值方法的结果。 |

### <a name="actionsource-values"></a>actionSource 值

| 成员        | 值 | Description                                                  |
| :------------ | :---- | :----------------------------------------------------------- |
| 手动        | 0     | 用户手动选择标签。                          |
| 自动     | 1      | 策略条件的结果是选择了标签。       |
| 建议   | 2      | 要应用推荐的标签的选择。                    |
| policyDefault | 3      | 用户不执行任何操作且策略-默认标签已应用。 |
| 强制     | 4      | 用户在强制选择标签后选择了一个标签。         |

### <a name="contentalignment-values"></a>contentAlignment 值

| 成员 | 值 | Description                         |
| :----- | :---- | :---------------------------------- |
| left   | 0     | 将内容标记向左对齐。  |
| 左向右  | 1      | 将内容标记向右对齐。 |
| 置 | 2      | 居中内容标记。             |

### <a name="watermarklayout-values"></a>watermarkLayout 值

| 成员     | 值 | Description                 |
| :--------- | :---- | :-------------------------- |
| 横向 | 0     | 使用水平水印。 |
| 用作   | 1      | 使用斜向水印。   |

### <a name="conditionalaccesspolicystate"></a>conditionalAccessPolicyState

|Member|
|:---|
|enabled|
|禁用|

### <a name="conditionalaccessclientapp"></a>conditionalAccessClientApp

| Member       |
|:--------------|
|浏览器|
|新式|
|easSupported|
|easUnsupported|
|相互|

### <a name="conditionalaccessgrantcontrol"></a>conditionalAccessGrantControl

| Member       |
|:--------------|
|数据|
|mfa|
|compliantDevice|
|domainJoinedDevice|
|approvedApplication|
|compliantApplication|

### <a name="cloudappsecuritysessioncontroltype"></a>cloudAppSecuritySessionControlType

| Member       |
|:--------------|
|mcasConfigured|
|monitorOnly|
|blockDownloads|

### <a name="signinfrequencytype"></a>signinFrequencyType

| Member       |
|:--------------|
|之前|
|花费|

### <a name="persistentbrowsersessionmode"></a>persistentBrowserSessionMode

| Member       |
|:--------------|
|都|
|永不|

### <a name="conditionalaccessdeviceplatform"></a>conditionalAccessDevicePlatform

| Member       |
|:--------------|
|android|
|iOS|
|时间|
|windowsPhone|
|macOS|
|各种|

### <a name="priority-values"></a>优先级值

|成员|值|
|:---|:---|
|无|0|
|高|1 |
|低|2 |

### <a name="threatassessmentcontenttype-values"></a>threatAssessmentContentType 值

| 成员 | 值 | Description             |
|:-------|:------|:------------------------|
| mail   | 1      | 邮件威胁。            |
| url    | 2      | URL 威胁。             |
| file   | 3      | 附件文件威胁。 |

### <a name="threatexpectedassessment-values"></a>threatExpectedAssessment 值

| 成员  | 值 | Description                       |
|:--------|:------|:----------------------------------|
| 数据   | 1      | 应阻止该威胁。     |
| 阻塞 | 2      | 不应阻止该威胁。 |

### <a name="threatcategory-values"></a>threatCategory 值

| 成员             | 值 | Description        |
|:-------------------|:------|:-------------------|
| 垃圾邮件 (spam)               | 1      | 垃圾邮件威胁。       |
| 仿冒           | 2      | 网络钓鱼威胁。   |
| 受到            | 3      | 恶意软件威胁。    |
| 向 unknownfuturevalue | 4      | 一个 sentinel 成员。 |

### <a name="threatassessmentstatus-values"></a>threatAssessmentStatus 值

| 成员    | 值 | Description                              |
|:----------|:------|:-----------------------------------------|
| 决   | 1      | 威胁评估仍在进行中。 |
| 后 | 2      | 威胁评估已完成。         |

### <a name="threatassessmentrequestsource-values"></a>threatAssessmentRequestSource 值

| 成员        | 值 | Description              |
|:--------------|:------|:-------------------------|
| 取消     | 0     | 尚不知道。            |
| user          | 1      | 用户提交。         |
| 联系 | 2      | 租户管理员提交。 |

### <a name="threatassessmentresulttype-values"></a>threatAssessmentResultType 值

| 成员             | 值 | Description                                          |
|:-------------------|:------|:-----------------------------------------------------|
| checkPolicy        | 1      | 策略检查结果，仅用于 `mail` 评估。 |
| 重新扫描             | 2      | 重新扫描结果。                                   |
| 向 unknownfuturevalue | 3      | 一个 sentinel 成员。                                   |

### <a name="maildestinationroutingreason-values"></a>mailDestinationRoutingReason 值

| 成员                | 值 | Description                         |
|:----------------------|:------|:------------------------------------|
| 无                  | 0     | 尚不知道。                       |
| mailFlowRule          | 1      | Exchange 传输规则。            |
| safeSender            | 2      | 安全发件人列表。                   |
| blockedSender         | 3      | 阻止发件人列表。                |
| advancedSpamFiltering | 4      | 高级垃圾邮件 flitering 选项。     |
| domainAllowList       | 5      | 发件人域允许列表。           |
| domainBlockList       | 6      | 发件人域阻止列表。           |
| notInAddressBook      | 7      | 将发件人排除在通讯簿之外。 |
| firstTimeSender       | 8      | 由于第一次发件人而被阻止。   |
| autoPurgeToInbox      | 9      | TimeTravel 将邮件移动到收件箱。   |
| autoPurgeToJunk       | 10     | TimeTravel 将邮件移动到垃圾邮件。    |
| autoPurgeToDeleted    | 11     | TimeTravel 将邮件移动到 "已删除"。 |
| 出站              | 12     | 出站邮件。                      |
| notJunk               | 13     | 由于非垃圾邮件而启用。              |
| 可疑                  | 14     | 由于垃圾邮件而被阻止。                |
| 向 unknownfuturevalue    | 15     | 一个 sentinel 成员。                  |

### <a name="threatassessmentrequestpivotproperty-values"></a>threatAssessmentRequestPivotProperty 值

| 成员                       | 值 | Description                                                            |
|:-----------------------------|:------|:-----------------------------------------------------------------------|
| threatCategory               | 1      | 的聚合威胁评估请求 `threatCategory` 。               |
| mailDestinationRoutingReason | 2      | 的聚合威胁评估请求 `mailDestinationRoutingReason` 。 |

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

### <a name="userflowtype-values"></a>userFlowType 值

|Member
|:----------------------
| 注册
| 登录
| signUpOrSignIn
| passwordReset
| profileUpdate
| resourceOwner
| 向 unknownfuturevalue

### <a name="openidconnectresponsemode-values"></a>openIdConnectResponseMode 值

| Member
|:----------------------
| 无
| form_post
| 查询
| 向 unknownfuturevalue

### <a name="openidconnectresponsetypes-values"></a>openIdConnectResponseTypes 值

| Member
|:----------------------
| 无
| code
| id_token
| 令牌

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

### <a name="connectedorganizationstate-values"></a>connectedOrganizationState 值

| 成员                | 值 | Description                                                                                                                                                                                                        |
|:----------------------| :-----|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 尚未            | 0     | 具有此状态值的已连接组织包含在请求者范围类型的分配策略中 `AllConfiguredConnectedOrganizationSubjects` 。                                                          |
| 审批              | 1      | 系统自动创建的已连接组织具有此状态值。 它们不包含在请求程序范围类型的分配策略中 `AllConfiguredConnectedOrganizationSubjects` 。   |
| 向 unknownfuturevalue    | 2      | 一个 sentinel 成员。                                                                                                                                                                                                 |

### <a name="identitysourcetype-values"></a>identitySourceType 值

|Member|
|:---|
|azureActiveDirectory|
|对外|

### <a name="externalgroupmembertype-values"></a>externalGroupMemberType 值

|Member|
|:---|
|user|
|group|

### <a name="identityuserflowattributedatatype-values"></a>identityUserFlowAttributeDataType 值

| 成员                | 值 | 说明                         |
|:----------------------|:------|:------------------------------------|
| string                | 1      | String 数据类型                    |
| boolean               | 2      | Boolean 数据类型                   |
| int64                 | 3      | Int 数据类型                       |
| stringCollection      | 4      | 字符串集合数据类型         |
| 向 unknownfuturevalue    | 5      | 一个 sentinel 成员。                  |

### <a name="identityuserflowattributetype-values"></a>identityUserFlowAttributeType 值

| 成员                | 值 | Description                                                        |
|:----------------------|:------|:-------------------------------------------------------------------|
| 内置               | 1      | 此用户流属性类型表示它是由系统创建的 |
| 自                | 2      | 此用户流属性类型表示它是由用户创建的   |
| 向 unknownfuturevalue    | 3      | 一个 sentinel 成员。                                                 |

### <a name="connectionstate-values"></a>connectionState 值

|Member|
|:---|
|拟定|
|即可|
|过时|
|limitExceeded|

### <a name="permissionclassificationtype-values"></a>permissionClassificationType 值

| Member
|:-------
| 降低

### <a name="permissiontype-values"></a>permissionType 值

| Member
|:-------------------------
| 应用程序
| 被
| delegatedUserConsentable

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

| Member
|:---
| entityUrl
| text

### <a name="cloudpcdeviceimagestatus-values"></a>cloudPcDeviceImageStatus 值

|Member|
|:---|
|决|
|即可|
|未能|

### <a name="cloudpcdeviceimagestatusdetails-values"></a>cloudPcDeviceImageStatusDetails 值

|Member|
|:---|
|internalServerError|
|sourceImageNotFound|

### <a name="cloudpconpremisesconnectionhealthcheckerrortype-values"></a>cloudPcOnPremisesConnectionHealthCheckErrorType 值

|Member|
|:---|
|dnsCheckFqdnNotFound|
|dnsCheckUnknownError|
|adJoinCheckFqdnNotFound|
|adJoinCheckIncorrectCredentials|
|adJoinCheckOrganizationalUnitNotFound|
|adJoinCheckOrganizationalUnitIncorrectFormat|
|adJoinCheckUnknownError |
|endpointConnectivityCheckUrlNotWhitelisted|
|endpointConnectivityCheckUnknownError|
|aadConnectivityCheckUnknownError |
|resourceAvailabilityCheckNoSubnetIP |
|resourceAvailabilityCheckUnknownError |
|internalServerUnknownError |

### <a name="cloudpconpremisesconnectionstatus-values"></a>cloudPcOnPremisesConnectionStatus 值

|Member|
|:---|
|决|
|运行|
|已|
|未能|
|向 unknownfuturevalue|

### <a name="cloudpcprovisioningpolicyimagetype-values"></a>cloudPcProvisioningPolicyImageType 值

|Member|
|:---|
|自|
|之家|

### <a name="cloudpcstatus-values"></a>cloudPcStatus 值

|Member|
|:---|
|notProvisioned|
|设置|
|已设置|
|时会|
|inGracePeriod|
|解除|
|upgradeFailed|
|provisionFailed|
|deprovisionFailed|
|reprovisionFailed|
