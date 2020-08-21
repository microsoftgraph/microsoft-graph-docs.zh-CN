---
title: 枚举值
description: Microsoft Graph 枚举值
doc_type: enumPageType
localization_priority: Normal
ms.prod: non-product-specific
author: MSGraphDocsvTeam
ms.openlocfilehash: 06e117900adca3dd12a31e222a98bda58969621e
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849511"
---
# <a name="enum-values"></a>枚举值

命名空间：microsoft.graph

### <a name="allowedaudiences-values"></a>allowedAudiences 值

|成员|
|:---|
|me|
|family|
|contacts|
|groupMembers|
|组织|
|federatedOrganizations|
|任何人|
|unknownFutureValue|

### <a name="emailtype-values"></a>emailType 值

|成员|
|:---|
|unknown|
|工时|
|personal|
|main|
|other|

### <a name="anniversarytype-values"></a>anniversaryType 值 

|成员|
|:---|
|birthday|
|wedding|
|unknownFutureValue|

### <a name="skillproficiencylevel-values"></a>skillProficiencyLevel 值 

|成员|
|:---|
|elementary|
|limitedWorking|
|generalProfessional|
|advancedProfessional|
|expert|
|unknownFutureValue|

### <a name="languageproficiencylevel-values"></a>languageProficiencyLevel 值 

|成员|
|:---|
|elementary|
|conversational|
|limitedWorking|
|professionalWorking|
|fullProfessional|
|nativeOrBilingual|
|unknownFutureValue|

### <a name="personrelationship-values"></a>personRelationship 值 

|成员|
|:---|
|manager|
|同事|
|directReport|
|dotLineReport|
|assistant|
|dotLineManager|
|alternateContact|
|friend|
|配对|
|sibling|
|child|
|父级|
|sponsor|
|emergencyContact|
|other|
|unknownFutureValue|

### <a name="attachmenttype-values"></a>attachmentType 值

| 成员
|:--------------
| file
| 项
| reference

### <a name="analyticsactivitytype-values"></a>analyticsActivityType 值

| 成员
|:--------------
| 通话
| 聊天
| 电子邮件
| 焦点
| meeting

### <a name="registrationauthmethod-values"></a>registrationAuthMethod 值

|成员|
|:---|
|电子邮件|
|mobilePhone|
|officePhone|
|securityQuestion|
|appNotification|
|appCode|
|alternateMobilePhone|

### <a name="entitytypes-values"></a>entityTypes 值

|成员|
|:---|
|event|
|message|
|driveItem|
|externalItem|

### <a name="contactrelationship-values"></a>contactRelationship 值

| 成员             | 值 | 说明                              |
| :----------------- | :---- | :--------------------------------------- |
| 父级             | 0     | 用户的父级。                       |
| 相对           | 1     | 用户的相对位置。                     |
| aide               | 2     | 用户的意。                         |
| doctor             | 3     | 用户的文档。                       |
| 防护者           | 4      | 用户的监护者。                     |
| child              | 5      | 用户的子级。                        |
| other              | 6      | 与用户的未指定关系。 |
| unknownFutureValue | 7      | 用于将来兼容性的标记值。   |

### <a name="scheduleentitytheme-values"></a>scheduleEntityTheme 值

| 成员
|:-------------------------
| white
| 蓝色
| 绿色
| 紫色
| 粉色
| 黄色
| 灰色
| 深蓝色
| darkGreen
| 深紫
| 深色
| darkYellow
| unknownFutureValue


### <a name="timeoffreasonicontype-values"></a>timeOffReasonIconType 值

|成员|
|:---|
|无|
|car|
|calendar|
|running|
|plane|
|firstAid|
|doctor|
|notWorking|
|时钟|
|juryDuty|
|globe|
|cup|
|phone|
|天气|
|umbrella|
|piggyBank|
|狗|
|cake|
|trafficCone|
|pin|
|sunny|
|unknownFutureValue|

### <a name="schedulechangestate-values"></a>scheduleChangeState 值

| 成员
|:----------------------------
|pending
|已批准
|declined
|unknownFutureValue

### <a name="schedulechangerequestactor-values"></a>scheduleChangeRequestActor 值

| 成员
|:----------------------------
|sender
|recipient
|manager
|system
|unknownFutureValue

### <a name="workforceintegrationencryptionprotocol-values"></a>workforceIntegrationEncryptionProtocol 值

| 成员
|:----------------------------
|sharedSecret
|unknownFutureValue

### <a name="workforceintegrationsupportedentities-values"></a>workforceIntegrationSupportedEntities 值

| 成员
|:----------------------------
|无
|Shift
|swapRequest
|openShift
|openShiftRequest
|userShiftPreferences

### <a name="timezonestandard-values"></a>timeZoneStandard 值

| 成员
|:-----------------
| windows
| iana


### <a name="freebusystatus-values"></a>freeBusyStatus 值

| 成员           | 值 |
| :--------------- | :---- |
| free             | 0     |
| 暂定        | 1     |
| 忙             | 2     |
| oof              | 3     |
| workingElsewhere | 4      |
| unknown          | -1    |


### <a name="physicaladdresstype-values"></a>physicalAddressType 值

| 成员
|:-------------------------
| unknown
| home
| 商用版
| other


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
| 全部


### <a name="automaticrepliesstatus-values"></a>automaticRepliesStatus 值

| 成员
|:-------------------------
| Disabled
| alwaysEnabled
| scheduled


### <a name="calendarcolor-values"></a>calendarColor 值

| 成员      | 值 |
| :---------- | :---- |
| 自动        | -1    |
| lightBlue   | 0     |
| lightGreen  | 1     |
| lightOrange | 2     |
| lightGray   | 3     |
| lightYellow | 4      |
| lightTeal   | 5      |
| lightPink   | 6      |
| lightBrown  | 7      |
| lightRed    | 8      |
| maxColor    | 9      |


### <a name="educationsynchronizationprofilestate-values"></a>educationSynchronizationProfileState 值

| 成员             | 值 |
| :----------------- | :---- |
| 删除           | 2     |
| deletionFailed     | 3     |
| provisioningFailed | 5      |
| 已设置        | 6      |
| provisioning       | 7      |
| unknownFutureValue | 8      |


### <a name="educationsynchronizationstatus-values"></a>educationSynchronizationStatus 值

| 成员             | 值 |
| :----------------- | :---- |
| 已暂停             | 0     |
| inProgress         | 1     |
| success            | 2     |
| error              | 3     |
| validationError    | 4      |
| 已隔离        | 5      |
| unknownFutureValue | 6      |

### <a name="educationexternalsource-values"></a>educationExternalSource 值

| 成员
|:-------------------------
| sis
| lms
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
| 一般
| personal
| private
| 机密


### <a name="importance-values"></a>重要性值

| 成员
|:-------------------------
| 低
| 一般
| high


### <a name="educationuserrole-values"></a>educationUserRole 值
| 成员
|:---------------------
| student
| teacher
| faculty


### <a name="meetingmessagetype-values"></a>meetingMessageType 值

| 成员
|:-----------------
| 无
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTentativelyAccepted
| meetingDeclined


### <a name="followupflagstatus-values"></a>followupFlagStatus 值

| 成员
|:-------------------------
| notFlagged
| complete
| flagged


### <a name="inferenceclassificationtype-values"></a>inferenceClassificationType 值

| 成员
|:-----------------
| focused - 具有焦点
| other


### <a name="iosnotificationalerttype-values"></a>iosNotificationAlertType 值

| 成员
|:-------------------------
| deviceDefault
| 横幅
| modal
| 无

### <a name="deviceenrollmentfailurereason-values"></a>deviceEnrollmentFailureReason 值

| 成员
|:-------------
| unknown
| authentication
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
| default
| conferenceRoom
| homeAddress
| businessAddress
| geoCoordinates
| streetAddress
| hotel
| restaurant
| localBusiness
| postalAddress

### <a name="locationuniqueidtype-values"></a>locationUniqueIdType 值

| 成员
|:-------------------------
| unknown
| locationStore
| directory
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

| 成员      | 值 |
| :---------- | :---- |
| 所有者       | 0     |
| 参与者 | 1     |
| 读者      | 2     |
| 无        | -1    |


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
| 预挂起

### <a name="onenotepatchinsertposition-values"></a>onenotePatchInsertPosition 值

| 成员
|:-------------------------
| 段后
| Before


### <a name="phonetype-values"></a>phoneType 值

| 成员
|:-------------------------
| home
| 商用版
| mobile
| other
| assistant
| homeFax
| businessFax
| otherFax
| pager
| 单选


### <a name="plannerpreviewtype-values"></a>plannerPreviewType 值

| 成员
|:-------------------------
| 自动
| noPreview
| checklist
| description
| reference


### <a name="status-values"></a>状态值

| 成员
|:-----------------
| active
| 已更新
| deleted
| 忽略
| unknownFutureValue


### <a name="weekindex-values"></a>weekIndex 值

| 成员
|:-------------------------
| first
| second
| third
| fourth
| last


### <a name="dayofweek-values"></a>dayOfWeek 值

| 成员
|:-------------------------
| sunday
| monday
| 星期二
| 星期三
| 星期四
| friday
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
| numbered


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
| 组织者
| tentativelyAccepted
| accepted
| declined
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

| 成员   | 值 |
| :------- | :---- |
| 无     | -1    |
| preset0  | 0     |
| preset1  | 1     |
| preset2  | 2     |
| preset3  | 3     |
| preset4  | 4      |
| preset5  | 5      |
| preset6  | 6      |
| preset7  | 7      |
| preset8  | 8      |
| preset9  | 9      |
| preset10 | 10     |
| preset11 | 11    |
| preset12 | 12     |
| preset13 | 13    |
| preset14 | 14     |
| preset15 | 15     |
| preset16 | 16     |
| preset17 | 17     |
| preset18 | 18     |
| preset19 | 19    |
| preset20 | 20    |
| preset21 |  21    |
| preset22 | 22    |
| preset23 | 23    |
| preset24 | 24    |

### <a name="alertfeedback-values"></a>alertFeedback 值

有关由一名或多信息学生提供的警报反馈值。

| 成员         | 值 | 说明               |
| :------------- | :---- | :------------------------ |
| unknown        | 0     | 未知。                  |
| truePositive   | 1     | 警报为正。   |
| falsePositive  | 2     | 警报为误报。  |
| benignPositive | 3     | 警报一定是正值的。 |

### <a name="filehashtype-values"></a>fileHashType 值

| 成员              | 值 | 说明                    |
| :------------------ | :---- | :----------------------------- |
| unknown             | 0     | 未知类型。                  |
| sha1                | 1     | SHA1 哈希类型。                |
| sha256              | 2     | SHA256 哈希类型。              |
| md5                 | 3     | MD5 哈希类型。                 |
| authenticodeHash256 | 4      | AuthenticodeHash256 哈希类型。 |
| lsHash              | 5      | LsHash 哈希类型。              |
| ctph                | 6      | CTPH 哈希类型。                |
| peSha1              | 7      | PESHA1 哈希类型。              |
| peSha256            | 8      | PESHA256 哈希类型。            |

### <a name="connectiondirection-values"></a>connectionDirection 值

| 成员   | 值 | 说明          |
| :------- | :---- | :------------------- |
| unknown  | 0     | 未知连接。  |
| 入站  | 1     | 入站连接。  |
| 出站 | 2     | 出站连接。 |

### <a name="connectionstatus-values"></a>connectionStatus 值

| 成员    | 值 | 说明                |
| :-------- | :---- | :------------------------- |
| unknown   | 0     | 未知连接状态。 |
| attempted | 1     | 已尝试连接。      |
| succeeded | 2     | 连接成功。      |
| blocked   | 3     | 连接被阻止。        |
| failed    | 4      | 连接失败。         |

### <a name="processintegritylevel-values"></a>processIntegrityLevel 值

| 成员    | 值 | 说明                   |
| :-------- | :---- | :---------------------------- |
| unknown   | 0     | 未知。                      |
| 不受信任 | 10     | 完整性级别为"不受信任"。 |
| 低       | 20    | 完整性级别为低。       |
| 中等    | 30    | 完整性级别为中。    |
| high      | 40    | 完整性级别为"高"。      |
| system    | 50    | 完整性级别为系统。    |

### <a name="registryhive-values"></a>registryHive 值

由定义的注册表配置配置器的枚举 [https://docs.microsoft.com/windows/desktop/sysinfo/registry-hives](https://docs.microsoft.com/windows/desktop/sysinfo/registry-hives) 。

| 成员                  | 值 | 说明                       |
| :---------------------- | :---- | :-------------------------------- |
| unknown                 | 0     | 未知配置单元。                     |
| currentConfig           | 1     | HKEY_CURRENT_CONFIG配置配置。         |
| currentUser             | 2     | HKEY_CURRENT_USER配置配置。           |
| localMachineSam         | 3     | HKEY_LOCAL_MACHINE\SAM 配置配置图。      |
| localMachineSamSoftware | 4      | HKEY_LOCAL_MACHINE\软件配置配置人员。 |
| localMachineSystem      | 5      | HKEY_LOCAL_MACHINE\系统配置配置配置人员。   |
| usersDefault            | 6      | HKEY_USERS \\ 。默认的配置分元。        |

### <a name="registryoperation-values"></a>registryOperation 值

更改了注册表项名称和/或值的操作。

| 成员  | 值 | 说明                  |
| :------ | :---- | :--------------------------- |
| unknown | 0     | 注册表值类型未知。 |
| create  | 1     | 创建注册表。             |
| 修改  | 2     | 修改注册表。             |
| delete  | 3     | 删除注册表。             |

### <a name="registryvaluetype-values"></a>registryValueType 值

注册表值类型定义的注册表 [值类型的枚举](https://docs.microsoft.com/windows/desktop/sysinfo/registry-value-types)。

| 成员            | 值 | 说明                                  |
| :---------------- | :---- | :------------------------------------------- |
| unknown           | 0     | 注册表值类型未知。                 |
| binary            | 1     | REG_BINARY注册表值类型。              |
| dword             | 2     | REG_DWORD注册表值类型。               |
| dwordLittleEndian | 3     | REG_DWORD_LITTLE_ENDIAN注册表值类型。 |
| dwordBigEndian    | 4      | REG_DWORD_BIG_ENDIAN注册表值类型。    |
| expandSz          | 5      | REG_EXPAND_SZ注册表值类型。           |
| link              | 6      | REG_LINK注册表值类型。                |
| multiSz           | 7      | REG_MULTI_SZ 注册表值类型。            |
| 无              | 8      | REG_NONE注册表值类型。                |
| qword             | 9      | REG_QWORD注册表值类型。               |
| qwordlittleEndian | 10     | REG_QWORD_LITTLE_ENDIAN注册表值类型。 |
| sz                | 11    | REG_SZ注册表值类型。                  |

### <a name="alertseverity-values"></a>alertSeverity 值

对严重性的枚举。

| 成员        | 值 | 说明                       |
| :------------ | :---- | :-------------------------------- |
| unknown       | 0     | 严重性未知。              |
| informational | 1     | 严重性仅用于信息。 |
| 低           | 2     | 严重性为低。                  |
| 中等        | 3     | 严重性是中等。               |
| high          | 4      | 严重性为高。                 |

### <a name="alertstatus-values"></a>alertStatus 值

警报生命周期状态的可能 (阶段) 。

| 成员     | 值 | 说明           |
| :--------- | :---- | :-------------------- |
| unknown    | 0     | 未知状态。       |
| newAlert   | 10     | 警报是新增功能。         |
| inProgress | 20    | 警报正在进行。 |
| 已解决   | 30    | 警报已解决。    |

### <a name="emailrole-values"></a>emailRole 值

电子邮件角色的可能值。

| 成员    | 值 | 说明             |
| :-------- | :---- | :---------------------- |
| unknown   | 0     | 未知角色。           |
| sender    | 1     | 电子邮件的发件人。    |
| recipient | 2     | 电子邮件的收件人。 |

### <a name="logontype-values"></a>logonType 值

用户登录方法的可能值。

| 成员            | 值 | 说明                  |
| :---------------- | :---- | :--------------------------- |
| unknown           | -1    | 未知。                     |
| interactive       | 0     | 登录是交互式的。        |
| remoteInteractive | 1     | 登录是远程交互式。 |
| 网络           | 2     | 登录是网络。            |
| batch             | 3     | 登录为批处理。              |
| service           | 4      | 登录为服务。            |

### <a name="useraccountsecuritytype-values"></a>userAccountSecurityType 值

基于 Windows 定义的组成员 (身份) 可能的值。

| 成员        | 值 | 说明                     |
| :------------ | :---- | :------------------------------ |
| unknown       | -1    | 未知。                        |
| standard      | 0     | Standard Users 组的成员。 |
| 电源         | 1     | Power Users 组的成员。    |
| 管理员 | 2     | 管理员组。 |

### <a name="scopeoperatormultivaluedcomparisontype-values"></a>scopeOperatorMultiValuedComparisonType 值

|成员|
|:---|
|全部|
|任意|

### <a name="risklevel-values"></a>riskLevel 值

|成员|
|:---|
|低|
|中等|
|high|
|hidden|
|无|
|unknownFutureValue|

### <a name="riskstate-values"></a>riskState 值

|成员|
|:---|
|无|
|confirmedSafe|
|已修正|
|dismissed|
|atRisk|
|confirmedCompromised|
|unknownFutureValue|

### <a name="riskdetail-values"></a>riskDetail 值

|成员|
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
|unknownFutureValue|

### <a name="referenceattachmentpermission-values"></a>referenceAttachmentPermission 值

|成员|
|:---|
|other|
|view|
|edit|
|anonymousView|
|anonymousEdit|
|organizationView|
|organizationEdit|

### <a name="referenceattachmentprovider-values"></a>referenceAttachmentProvider 值

|成员|
|:---|
|other|
|oneDriveBusiness|
|oneDriveConsumer|
|dropbox|

### <a name="riskeventtype-values"></a>riskEventType 值

|成员|
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
|unknownFutureValue|

### <a name="networktype-values"></a>networkType 值

|成员|
|:---|
|intranet|
|Extranet|
|namedNetwork|
|trusted|
|unknownFutureValue|

### <a name="exchangeidformat-values"></a>exchangeIdFormat 值

|成员|
|:---|
|entryId|
|ewsId|
|immutableEntryId|
|restId|
|restImmutableEntryId|

### <a name="attributeflowbehavior-values"></a>attributeFlowBehavior 值

|成员|
|:---|
|flowWhenChanged|
|flowAlways|

### <a name="attributeflowtype-values"></a>attributeFlowType 值

|成员|
|:---|
|始终|
|objectAddOnly|
|multiValueAddOnly|
|restId|

### <a name="objectflowtypes-values"></a>objectFlowTypes 值

| 成员 | 值 |
| :----- | :---- |
| 无   | 0     |
| 添加    | 1     |
| 更新 | 2     |
| 删除 | 4      |

### <a name="chatmessagetype-values"></a>chatMessageType 值

|成员|
|:---|
|message|

### <a name="chatmessageimportance-values"></a>chatMessageImportance 值

|成员|
|:---|
|一般|
|high|
|urgent|

### <a name="channelmembershiptype-values"></a>channelMembershipType 值

| 成员             | 值 |
| :----------------- | :---- |
| standard           | 0     |
| private            | 1     |
| unknownFutureValue | 2     |

### <a name="stagedfeaturename-values"></a>stagedFeatureName 值

| 成员                    | 说明                   |
| :------------------------ | :---------------------------- |
| passthroughAuthentication | 传递身份验证    |
| seamlessSso               | 无缝单一登录       |
| passwordHashSync          | 密码哈希同步 |

### <a name="tokenissuertype-values"></a>tokenIssuerType 值

|成员|
|:---|
|AzureAD|
|ADFederationServices|
|unknownFutureValue|

### <a name="riskdetectiontimingtype-values"></a>riskDetectionTimingType 值

|成员|
|:---|
|notDefined|
|realtime|
|nearRealtime|
|offline|
|unknownFutureValue|

### <a name="activitytype-values"></a>activityType 值

|成员|
|:---|
|signin|
|user|
|unknownFutureValue|

### <a name="entitytype-values"></a>entityType 值

| 成员       |
|:--------------|
|event|
|message|
|driveItem|
|externalFile|
|externalItem|

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

### <a name="contentformat-values"></a>contentFormat 值

| 成员  | 值 | 说明                          |
| :------ | :---- | :----------------------------------- |
| default | 0     | 内容是文件类型或非电子邮件类型。 |
| 电子邮件   | 1     | 内容是电子邮件。                 |

### <a name="contentstate-values"></a>contentState 值

| 成员 | 值 | 说明                                                                      |
| :----- | :---- | :------------------------------------------------------------------------------- |
| rest   | 0     | 数据处于其余中;例如，共享中的文件。                                 |
| 动作 | 1     | 数据处于动作状态。 传输网络设备截获的文件。         |
| use    | 2     | 数据正在使用中。 文件在客户端应用程序（如客户端应用程序）Microsoft Office。 |

### <a name="assignmentmethod-values"></a>assignmentMethod 值

| 成员     | 值 | 说明                                                                                                                      |
| :--------- | :---- | :------------------------------------------------------------------------------------------------------------------------------- |
| standard   | 0     | 该标签是由服务或策略条件设置的。                                                                              |
| privileged | 1     | 标签由用户显式设置。                                                                                          |
| 自动       | 2     | 允许替代任何现有标签。 降级时所需的理从性。 元数据 `standard` 中的工作分配方法的结果。 |

### <a name="actionsource-values"></a>actionSource 值

| 成员        | 值 | 说明                                                  |
| :------------ | :---- | :----------------------------------------------------------- |
| 手动        | 0     | 用户可以手动选择标签。                          |
| 自动     | 1     | 已通过策略条件选择标签。       |
| 建议   | 2     | 选择要应用建议标签。                    |
| policyDefault | 3     | 用户未执行任何操作，且已应用策略默认标签。 |
| 强制     | 4      | 用户在被限制后选择标签。         |

### <a name="contentalignment-values"></a>contentAlignment 值

| 成员 | 值 | 说明                         |
| :----- | :---- | :---------------------------------- |
| left   | 0     | 使内容标记向左对齐。  |
| 向  | 1     | 使内容标记向右对齐。 |
| 居中 | 2     | 居中内容标记。             |

### <a name="watermarklayout-values"></a>watermarkLayout 值

| 成员     | 值 | 说明                 |
| :--------- | :---- | :-------------------------- |
| 水平 | 0     | 使用水平水印。 |
| 对角线   | 1     | 使用对角水印。   |

### <a name="conditionalaccesspolicystate"></a>conditionalAccessPolicyState

|成员|
|:---|
|enabled|
|Disabled|

### <a name="conditionalaccessclientapp"></a>conditionalAccessClientApp

| 成员       |
|:--------------|
|浏览器|
|新式|
|easSupported|
|easUnsupported|
|other|

### <a name="conditionalaccessgrantcontrol"></a>conditionalAccessGrantControl

| 成员       |
|:--------------|
|block|
|mfa|
|compliantDevice|
|domainJoinedDevice|
|approvedApplication|
|compliantApplication|

### <a name="cloudappsecuritysessioncontroltype"></a>cloudAppSecuritySessionControlType

| 成员       |
|:--------------|
|mcasConfigured|
|monitorOnly|
|blockDownloads|

### <a name="signinfrequencytype"></a>signinFrequencyType

| 成员       |
|:--------------|
|days|
|hours|

### <a name="persistentbrowsersessionmode"></a>persistentBrowserSessionMode

| 成员       |
|:--------------|
|始终|
|从不|

### <a name="conditionalaccessdeviceplatform"></a>conditionalAccessDevicePlatform

| 成员       |
|:--------------|
|android|
|iOS|
|windows|
|windowsPhone|
|macOS|
|全部|

### <a name="priority-values"></a>priority values

|成员|值|
|:---|:---|
|无|0|
|高|1|
|低|2|

### <a name="threatassessmentcontenttype-values"></a>threatAssessmentContentType 值

| 成员 | 值 | 说明             |
|:-------|:------|:------------------------|
| mail   | 1     | 邮件威胁。            |
| url    | 2     | URL 威胁。             |
| file   | 3     | 附件文件威胁。 |

### <a name="threatexpectedassessment-values"></a>threatExpectedAssessment 值

| 成员  | 值 | 说明                       |
|:--------|:------|:----------------------------------|
| block   | 1     | 应该会阻止威胁。     |
| 取消阻止 | 2     | 不应阻止威胁。 |

### <a name="threatcategory-values"></a>threatCategory 值

| 成员             | 值 | 说明        |
|:-------------------|:------|:-------------------|
| 垃圾邮件 (spam)               | 1     | 垃圾邮件威胁。       |
| 仿冒           | 2     | 网络钓鱼威胁。   |
| 恶意软件            | 3     | 恶意软件威胁。    |
| unknownFutureValue | 4      | Sentinel 成员。 |

### <a name="threatassessmentstatus-values"></a>threatAssessmentStatus 值

| 成员    | 值 | 说明                              |
|:----------|:------|:-----------------------------------------|
| pending   | 1     | 仍在进行中的威胁评估。 |
| completed | 2     | 威胁评估已完成。         |

### <a name="threatassessmentrequestsource-values"></a>threatAssessmentRequestSource 值

| 成员        | 值 | 说明              |
|:--------------|:------|:-------------------------|
| undefined     | 0     | "Not yet know"。            |
| user          | 1     | 用户提交。         |
| 管理员 | 2     | 租户管理员提交。 |

### <a name="threatassessmentresulttype-values"></a>threatAssessmentResultType 值

| 成员             | 值 | 说明                                          |
|:-------------------|:------|:-----------------------------------------------------|
| checkPolicy        | 1     | 策略检查结果，仅适用于 `mail` 评估。 |
| rescan             | 2     | 重新扫描结果。                                   |
| unknownFutureValue | 3     | Sentinel 成员。                                   |

### <a name="maildestinationroutingreason-values"></a>mailDestinationRoutingReason 值

| 成员                | 值 | 说明                         |
|:----------------------|:------|:------------------------------------|
| 无                  | 0     | "Not yet know"。                       |
| mailFlowRule          | 1     | Exchange 传输规则。            |
| safeSender            | 2     | 安全发件人列表。                   |
| blockedSender         | 3     | 阻止发件人列表。                |
| advancedSpamFiltering | 4      | 高级垃圾邮件存档选项。     |
| domainAllowList       | 5      | 发件人域允许列表。           |
| domainBlockList       | 6      | 发件人域阻止列表。           |
| notInAddressBook      | 7      | 排除通讯簿不包括发件人。 |
| firstTimeSender       | 8      | 发件人第一次时阻止。   |
| autoPurgeToInbox      | 9      | TimeTravel 将邮件移动到收件箱。   |
| autoPurgeToJunk       | 10     | TimeTravel 将邮件移动到垃圾邮件。    |
| autoPurgeToDeleted    | 11    | TimeTravel 将邮件移动到已删除。 |
| 出站              | 12     | 出站邮件。                      |
| notJunk               | 13    | 非垃圾邮件，允许。              |
| 垃圾邮件                  | 14     | 垃圾邮件阻止。                |
| unknownFutureValue    | 15     | Sentinel 成员。                  |

### <a name="threatassessmentrequestpivotproperty-values"></a>threatAssessmentRequestPivotProperty 值

| 成员                       | 值 | 说明                                                            |
|:-----------------------------|:------|:-----------------------------------------------------------------------|
| threatCategory               | 1     | 将威胁评估聚合 `threatCategory` 请求。               |
| mailDestinationRoutingReason | 2     | 将威胁评估聚合 `mailDestinationRoutingReason` 请求。 |

### <a name="riskeventtypes-values"></a>riskEventTypes 值

| 成员
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
| unknownFutureValue

### <a name="openidconnectresponsemode-values"></a>openIdConnectResponseMode 值
| 成员                
|:----------------------
| 无
| form_post
| 查询 
| unknownFutureValue 

### <a name="openidconnectresponsetypes-values"></a>openIdConnectResponseTypes 值
| 成员                
|:----------------------
| 无
| code
| id_token
| 令牌

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
| completed
| waitingOnOthers
| deferred