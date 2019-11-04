---
title: 枚举值
description: Microsoft Graph 枚举值
doc_type: enumPageType
localization_priority: Normal
ms.prod: non-product-specific
author: MSGraphDocsvTeam
ms.openlocfilehash: f7f6d2d71e2a6c3ec1be01d308109cd07cf9076e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939633"
---
# <a name="enum-values"></a>枚举值

### <a name="attachmenttype-values"></a>attachmentType 值

| Member
|:--------------
| file
| item
| reference

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
|microsoft. graph. 事件|
|microsoft. graph. 邮件|
|driveItem|
|externalFile|
|externalItem|

### <a name="contactrelationship-values"></a>contactRelationship 值

| 成员             | 值 | 说明                              |
| :----------------- | :---- | :--------------------------------------- |
| 母语             | 0     | 用户的父级。                       |
| 彼此           | 1     | 用户的相对路径。                     |
| aide               | 双面     | 用户的 aide。                         |
| dr.             | 第三章     | 用户的医生。                       |
| 监护           | 4     | 用户的监护人。                     |
| 该子              | 5     | 用户的子级。                        |
| 相互              | 型     | 与用户的未指定关系。 |
| 向 unknownfuturevalue | 步     | 用于将来兼容性的标记值。   |

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
|calendar|
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

| 成员           | 值 |
| :--------------- | :---- |
| 任意             | 0     |
| 暂        | 1     |
| 空闲             | 双面     |
| oof              | 第三章     |
| workingElsewhere | 4     |
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
| lightGreen  | 1     |
| lightOrange | 双面     |
| lightGray   | 第三章     |
| lightYellow | 4     |
| lightTeal   | 5     |
| lightPink   | 型     |
| lightBrown  | 步     |
| lightRed    | utf-8     |
| maxColor    | 第     |


### <a name="educationsynchronizationprofilestate-values"></a>educationSynchronizationProfileState 值

| 成员             | 值 |
| :----------------- | :---- |
| 删除           | 双面     |
| deletionFailed     | 第三章     |
| provisioningFailed | 5     |
| 已设置        | 型     |
| 设置       | 步     |
| 向 unknownfuturevalue | utf-8     |


### <a name="educationsynchronizationstatus-values"></a>educationSynchronizationStatus 值

| 成员             | 值 |
| :----------------- | :---- |
| 停留             | 0     |
| inProgress         | 1     |
| success            | 双面     |
| error              | 第三章     |
| validationError    | 4     |
| 隔离        | 5     |
| 向 unknownfuturevalue | 型     |

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
| 前后
| noResponseNecessary
| 自述
| 响应
| replyToAll
| 概述


### <a name="onenoteuserrole-values"></a>onenoteUserRole 值

| 成员      | 值 |
| :---------- | :---- |
| Owner       | 0     |
| 参与者 | 1     |
| 读者      | 双面     |
| 无        | -1    |


### <a name="operationstatus-values"></a>operationStatus 值

| Member
|:-----------------
| NotStarted
| 运行
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
| 流动
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
| reference


### <a name="status-values"></a>status 值

| Member
|:-----------------
| 工作
| updated
| deleted
| 忽视
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
| 配置文件


### <a name="categorycolor-values"></a>categoryColor 值

| 成员   | 值 |
| :------- | :---- |
| 无     | -1    |
| preset0  | 0     |
| preset1  | 1     |
| preset2  | 双面     |
| preset3  | 第三章     |
| preset4  | 4     |
| preset5  | 5     |
| preset6  | 型     |
| preset7  | 步     |
| preset8  | utf-8     |
| preset9  | 第     |
| preset10 | 10    |
| preset11 | 11x17    |
| preset12 | 12    |
| preset13 | 13    |
| preset14 | 日    |
| preset15 | 个    |
| preset16 | 16     |
| preset17 | ×    |
| preset18 | 18    |
| preset19 | 合    |
| preset20 | 20    |
| preset21 | 不足    |
| preset22 | 22    |
| preset23 | 上午    |
| preset24 | 24    |

### <a name="alertfeedback-values"></a>alertFeedback 值

由分析师提供的警报上可能的反馈值。

| 成员         | 值 | 说明               |
| :------------- | :---- | :------------------------ |
| unknown        | 0     | 陌生.                  |
| truePositive   | 1     | 警报为 true-肯定。   |
| falsePositive  | 双面     | 警报为 false-肯定。  |
| benignPositive | 第三章     | 警报为良性-肯定。 |

### <a name="filehashtype-values"></a>fileHashType 值

| 成员              | 值 | 说明                    |
| :------------------ | :---- | :----------------------------- |
| unknown             | 0     | 未知类型。                  |
| sha1                | 1     | SHA1 哈希类型。                |
| sha256              | 双面     | SHA256 哈希类型。              |
| md5                 | 第三章     | MD5 哈希类型。                 |
| authenticodeHash256 | 4     | AuthenticodeHash256 哈希类型。 |
| lsHash              | 5     | LsHash 哈希类型。              |
| ctph                | 型     | CTPH 哈希类型。                |
| peSha1              | 步     | PESHA1 哈希类型。              |
| peSha256            | utf-8     | PESHA256 哈希类型。            |

### <a name="connectiondirection-values"></a>connectionDirection 值

| 成员   | 值 | 说明          |
| :------- | :---- | :------------------- |
| unknown  | 0     | 未知的连接。  |
| 进货  | 1     | 入站连接。  |
| 出站 | 双面     | 出站连接。 |

### <a name="connectionstatus-values"></a>connectionStatus 值

| 成员    | 值 | 说明                |
| :-------- | :---- | :------------------------- |
| unknown   | 0     | 未知的连接状态。 |
| 尝试 | 1     | 已尝试连接。      |
| 完成 | 双面     | 连接成功。      |
| 堵塞   | 第三章     | 连接被阻止。        |
| 未能    | 4     | 连接失败。         |

### <a name="processintegritylevel-values"></a>processIntegrityLevel 值

| 成员    | 值 | 说明                   |
| :-------- | :---- | :---------------------------- |
| unknown   | 0     | 陌生.                      |
| 可信 | 10    | 完整性级别不受信任。 |
| 降低       | 20    | 完整性级别较低。       |
| 中等    | 30    | 完整性级别为 "中"。    |
| 高效      | 40    | 完整性级别为 "高"。      |
| system    | 50    | 完整性级别为 "系统"。    |

### <a name="registryhive-values"></a>registryHive 值

由定义的[https://docs.microsoft.com/windows/desktop/sysinfo/registry-hives](https://docs.microsoft.com/windows/desktop/sysinfo/registry-hives)注册表配置单元的枚举。

| 成员                  | 值 | 说明                       |
| :---------------------- | :---- | :-------------------------------- |
| unknown                 | 0     | 未知配置单元。                     |
| currentConfig           | 1     | HKEY_CURRENT_CONFIG 配置单元。         |
| currentUser             | 双面     | HKEY_CURRENT_USER 配置单元。           |
| localMachineSam         | 第三章     | HKEY_LOCAL_MACHINE\SAM 配置单元。      |
| localMachineSamSoftware | 4     | HKEY_LOCAL_MACHINE\Software 配置单元。 |
| localMachineSystem      | 5     | HKEY_LOCAL_MACHINE\System 配置单元。   |
| usersDefault            | 型     | HKEY_USERS\\。默认配置单元。        |

### <a name="registryoperation-values"></a>registryOperation 值

更改注册表项名称和/或值的操作。

| 成员  | 值 | 说明                  |
| :------ | :---- | :--------------------------- |
| unknown | 0     | 未知的注册表值类型。 |
| create  | 1     | 创建注册表。             |
| modify  | 双面     | 修改注册表。             |
| delete  | 第三章     | 删除注册表。             |

### <a name="registryvaluetype-values"></a>registryValueType 值

由[注册表值类型](https://docs.microsoft.com/windows/desktop/sysinfo/registry-value-types)定义的注册表值类型的枚举。

| 成员            | 值 | 说明                                  |
| :---------------- | :---- | :------------------------------------------- |
| unknown           | 0     | 未知的注册表值类型。                 |
| 数字            | 1     | REG_BINARY 注册表值类型。              |
| 值             | 双面     | REG_DWORD 注册表值类型。               |
| dwordLittleEndian | 第三章     | REG_DWORD_LITTLE_ENDIAN 注册表值类型。 |
| dwordBigEndian    | 4     | REG_DWORD_BIG_ENDIAN 注册表值类型。    |
| expandSz          | 5     | REG_EXPAND_SZ 注册表值类型。           |
| link              | 型     | REG_LINK 注册表值类型。                |
| multiSz           | 步     | REG_MULTI_SZ 注册表值类型。            |
| 无              | utf-8     | REG_NONE 注册表值类型。                |
| qword             | 第     | REG_QWORD 注册表值类型。               |
| qwordlittleEndian | 10    | REG_QWORD_LITTLE_ENDIAN 注册表值类型。 |
| sz                | 11x17    | REG_SZ 注册表值类型。                  |

### <a name="alertseverity-values"></a>alertSeverity 值

警报严重性的枚举。

| 成员        | 值 | 说明                       |
| :------------ | :---- | :-------------------------------- |
| unknown       | 0     | 严重度未知。              |
| 之 | 1     | 严重性仅适用于信息。 |
| 降低           | 双面     | 严重性为低。                  |
| 中等        | 第三章     | 严重性为 "中"。               |
| 高效          | 4     | 严重性为高。                 |

### <a name="alertstatus-values"></a>alertStatus 值

警报生命周期状态（阶段）的可能值。

| 成员     | 值 | 说明           |
| :--------- | :---- | :-------------------- |
| unknown    | 0     | 未知状态。       |
| newAlert   | 10    | 警报是新的。         |
| inProgress | 20    | 警报正在进行中。 |
| 经过   | 30    | 警报已解决。    |

### <a name="emailrole-values"></a>emailRole 值

电子邮件角色的可能值。

| 成员    | 值 | 说明             |
| :-------- | :---- | :---------------------- |
| unknown   | 0     | 未知角色。           |
| sender    | 1     | 电子邮件的发件人。    |
| recipient | 双面     | 电子邮件的收件人。 |

### <a name="logontype-values"></a>logonType 值

用户登录方法的可能值。

| 成员            | 值 | 说明                  |
| :---------------- | :---- | :--------------------------- |
| unknown           | -1    | 陌生.                     |
| 式       | 0     | 登录是交互式的。        |
| remoteInteractive | 1     | 登录是远程交互的。 |
| network           | 双面     | 登录为网络。            |
| batch             | 第三章     | 登录是批处理。              |
| service           | 4     | 登录为 "服务"。            |

### <a name="useraccountsecuritytype-values"></a>userAccountSecurityType 值

每个 Windows 定义的用户帐户类型（组成员身份）可能的值。

| 成员        | 值 | 说明                     |
| :------------ | :---- | :------------------------------ |
| unknown       | -1    | 陌生.                        |
| 普通      | 0     | "标准用户" 组的成员。 |
| 能力         | 1     | Power Users 组的成员。    |
| 联系 | 双面     | Administrators 组的成员。 |

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
| 加法    | 1     |
| Update | 双面     |
| Delete | 4     |

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
| private            | 1     |
| 向 unknownfuturevalue | 双面     |

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
|自述|
|销帐|
|delegateWithoutPrivateEventAccess|
|delegateWithPrivateEventAccess|
|自|

### <a name="contentformat-values"></a>contentFormat 值

| 成员  | 值 | 说明                          |
| :------ | :---- | :----------------------------------- |
| 设置 | 0     | 内容是文件或非电子邮件类型。 |
| email   | 1     | 内容是一封电子邮件。                 |

### <a name="contentstate-values"></a>contentState 值

| 成员 | 值 | 说明                                                                      |
| :----- | :---- | :------------------------------------------------------------------------------- |
| 完成   | 0     | 数据是静止的;共享中的文件，例如。                                 |
| 动作 | 1     | 数据是活动的。 由传输中的网络设备截获的文件。         |
| 改用    | 双面     | 数据正在使用中。 在客户端应用程序（如 Microsoft Office）中打开一个文件。 |

### <a name="assignmentmethod-values"></a>assignmentMethod 值

| 成员     | 值 | 说明                                                                                                                      |
| :--------- | :---- | :------------------------------------------------------------------------------------------------------------------------------- |
| 普通   | 0     | 标签是由服务或策略条件设置的。                                                                              |
| 严格 | 1     | 标签由用户显式设置。                                                                                          |
| 自动       | 双面     | 允许覆盖任何现有标签。 降级时所需的理由。 元数据`standard`中的赋值方法的结果。 |

### <a name="actionsource-values"></a>actionSource 值

| 成员        | 值 | 说明                                                  |
| :------------ | :---- | :----------------------------------------------------------- |
| 手动        | 0     | 用户手动选择标签。                          |
| 自动     | 1     | 策略条件的结果是选择了标签。       |
| 建议   | 双面     | 要应用推荐的标签的选择。                    |
| policyDefault | 第三章     | 用户不执行任何操作且策略-默认标签已应用。 |
| 强制     | 4     | 用户在强制选择标签后选择了一个标签。         |

### <a name="contentalignment-values"></a>contentAlignment 值

| 成员 | 值 | 说明                         |
| :----- | :---- | :---------------------------------- |
| left   | 0     | 将内容标记向左对齐。  |
| 左向右  | 1     | 将内容标记向右对齐。 |
| 置 | 双面     | 居中内容标记。             |

### <a name="watermarklayout-values"></a>watermarkLayout 值

| 成员     | 值 | 说明                 |
| :--------- | :---- | :-------------------------- |
| 横向 | 0     | 使用水平水印。 |
| 用作   | 1     | 使用斜向水印。   |

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
|高|1|
|低|双面|

