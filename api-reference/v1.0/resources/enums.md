---
title: 枚举值
description: Microsoft Graph枚举值。
ms.localizationpriority: medium
ms.prod: non-product-specific
author: MSGraphDocsvTeam
doc_type: enumPageType
ms.openlocfilehash: abf5a95ccc6c19bcb656d84c9d6cf4d9891cbea6
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420570"
---
# <a name="enum-values"></a>枚举值

命名空间：microsoft.graph

### <a name="expirationpatterntype-values"></a>expirationPatternType 值 

|成员|
|:---|
|notSpecified|
|noExpiration|
|afterDateTime|
|afterDuration|

### <a name="recurrencepatterntype-values"></a>recurrencePatternType 值 

|成员|
|:---|
|日常|
|每周|
|absoluteMonthly|
|relativeMonthly|
|absoluteYearly|
|relativeYearly|

### <a name="roleassignmentschedulefilterbycurrentuseroptions-values"></a>roleAssignmentScheduleFilterByCurrentUserOptions 值 

|成员|
|:---|
|主要|
|unknownFutureValue|

### <a name="roleassignmentscheduleinstancefilterbycurrentuseroptions-values"></a>roleAssignmentScheduleInstanceFilterByCurrentUserOptions 值 

|成员|
|:---|
|主要|
|unknownFutureValue|

### <a name="roleassignmentschedulerequestfilterbycurrentuseroptions-values"></a>roleAssignmentScheduleRequestFilterByCurrentUserOptions 值 

|成员|
|:---|
|主要|
|createdBy|
|审批者|
|unknownFutureValue|

### <a name="roleeligibilityschedulefilterbycurrentuseroptions-values"></a>roleEligibilityScheduleFilterByCurrentUserOptions 值 

|成员|
|:---|
|主要|
|unknownFutureValue|

### <a name="roleeligibilityscheduleinstancefilterbycurrentuseroptions-values"></a>roleEligibilityScheduleInstanceFilterByCurrentUserOptions 值 

|成员|
|:---|
|主要|
|unknownFutureValue|

### <a name="roleeligibilityschedulerequestfilterbycurrentuseroptions-values"></a>roleEligibilityScheduleRequestFilterByCurrentUserOptions 值 

|成员|
|:---|
|主要|
|createdBy|
|审批者|
|unknownFutureValue|

### <a name="unifiedrolemanagementpolicyruletargetoperations-values"></a>unifiedRoleManagementPolicyRuleTargetOperations 值 

|成员|
|:---|
|全部|
|激活|
|关闭|
|分配|
|更新|
|删除|
|扩展|
|续订|
|unknownFutureValue|

### <a name="unifiedroleschedulerequestactions-values"></a>unifiedRoleScheduleRequestActions 值 

|成员|
|:---|
|adminAssign|
|adminUpdate|
|adminRemove|
|selfActivate|
|selfDeactivate|
|adminExtend|
|adminRenew|
|selfExtend|
|selfRenew|
|unknownFutureValue|

### <a name="approvalfilterbycurrentuseroptions-values"></a>approvalFilterByCurrentUserOptions 值 

|成员|
|:---|
|target|
|createdBy|
|审批者|
|unknownFutureValue|

### <a name="accessreviewexpirationbehavior-values"></a>accessReviewExpirationBehavior 值

|成员|
|:---|
|keepAccess|
|removeAccess|
|acceptAccessRecommendation|
|unknownFutureValue|

### <a name="allowedtargetscope-values"></a>allowedTargetScope 值

|成员|
|:---|
|notSpecified|
|specificDirectoryUsers|
|specificConnectedOrganizationUsers|
|specificDirectoryServicePrincipals|
|allMemberUsers|
|allDirectoryUsers|
|allDirectoryServicePrincipals|
|allConfiguredConnectedOrganizationUsers|
|allExternalUsers|
|unknownFutureValue|

### <a name="approvalfilterbycurrentuseroptions-values"></a>approvalFilterByCurrentUserOptions 值 

|成员|
|:---|
|target|
|createdBy|
|审批者|
|unknownFutureValue|

### <a name="accesspackageassignmentfilterbycurrentuseroptions-values"></a>accessPackageAssignmentFilterByCurrentUserOptions 值

|成员|
|:---|
|target|
|createdBy|
|unknownFutureValue|

### <a name="accesspackageassignmentrequestfilterbycurrentuseroptions-values"></a>accessPackageAssignmentRequestFilterByCurrentUserOptions 值

|成员|
|:---|
|target|
|createdBy|
|审批者|
|unknownFutureValue|

### <a name="accesspackageassignmentstate-values"></a>accessPackageAssignmentState 值

|成员|
|:---|
|提供|
|partiallyDelivered|
|交付|
|过期|
|deliveryFailed|
|unknownFutureValue|

### <a name="accesspackagecatalogstate-values"></a>accessPackageCatalogState 值

|成员|
|:---|
|发表|
|发表|
|unknownFutureValue|

### <a name="accesspackagecatalogtype-values"></a>accessPackageCatalogType 值

|成员|
|:---|
|userManaged|
|serviceDefault|
|serviceManaged|
|unknownFutureValue|

### <a name="accesspackageexternaluserlifecycleaction-values"></a>accessPackageExternalUserLifecycleAction 值

|成员|
|:---|
|无|
|blockSignIn|
|blockSignInAndDelete|
|unknownFutureValue|

### <a name="accesspackagefilterbycurrentuseroptions-values"></a>accessPackageFilterByCurrentUserOptions 值

|成员|
|:---|
|allowedRequestor|
|unknownFutureValue|

### <a name="accesspackagerequeststate-values"></a>accessPackageRequestState 值

|成员|
|:---|
|提交|
|pendingApproval|
|提供|
|交付|
|deliveryFailed|
|denied|
|scheduled|
|取消|
|partiallyDelivered|
|unknownFutureValue|

### <a name="accesspackagerequesttype-values"></a>accessPackageRequestType 值

|成员|
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

|成员|
|:---|
|notSpecified|
|用户|
|servicePrincipal|
|unknownFutureValue|

### <a name="connectedorganizationstate-values"></a>connectedOrganizationState 值

|成员|
|:---|
|配置|
|提出|

### <a name="accessreviewinstancedecisionitemfilterbycurrentuseroptions-values"></a>accessReviewInstanceDecisionItemFilterByCurrentUserOptions 值 

|成员|
|:---|
|评论家|
|unknownFutureValue|

### <a name="volumetype-values"></a>volumeType 值

|成员|
|:---|
|operatingSystemVolume|
|fixedDataVolume|
|removableDataVolume|
|unknownFutureValue|

### <a name="filtermode-values"></a>filterMode 值

|成员|
|:---|
|包括|
|排除|

### <a name="lifecycleeventtype-values"></a>lifecycleEventType 值

|成员|
|:---|
|错过|
|subscriptionRemoved|
|reauthorizationRequired|

### <a name="changetype-values"></a>changeType 值

|成员|
|:---|
|clientIpAddress|
|authenticatorAppGps|

### <a name="countrylookupmethodtype-values"></a>countryLookupMethodType 值

|成员|
|:---|
|clientIpAddress|
|authenticatorAppGps|

### <a name="consentrequestfilterbycurrentuseroptions-values"></a>consentRequestFilterByCurrentUserOptions 值 

|成员|
|:---|
|评论家|
|unknownFutureValue|

### <a name="externalemailotpstate-values"></a>externalEmailOtpState 值

|成员|
|:---|
|默认|
|enabled|
|禁用|
|unknownFutureValue|

### <a name="educationaddedstudentaction-values"></a>educationAddedStudentAction 值

|成员|
|:---|
|无|
|assignIfOpen|
|unknownFutureValue|

### <a name="fido2restrictionenforcementtype-values"></a>fido2RestrictionEnforcementType 值

|成员|
|:---|
|允许|
|块|

### <a name="attestationlevel-values"></a>attestationLevel 值

|成员|
|:---|
|证明|
|notAttested|

### <a name="authenticationmethodtargettype-values"></a>authenticationMethodTargetType 值

|成员|
|:---|
|用户|
|组|

### <a name="authenticationmethodstate-values"></a>authenticationMethodState 值

|成员|
|:---|
|enabled|
|禁用|

### <a name="microsoftauthenticatorauthenticationmode-values"></a>microsoftAuthenticatorAuthenticationMode 值

|成员|
|:---|
|任意|
|推|
|deviceBasedPush|

### <a name="keystrength-values"></a>keyStrength 值

|成员|
|:---|
|正常|
|弱|
|unknown|

### <a name="authenticationmethodkeystrength-values"></a>authenticationMethodKeyStrength 值

|成员|
|:---|
|正常|
|弱|
|unknown|

### <a name="allowinvitesfrom-values"></a>allowInvitesFrom 值

|成员|
|:---|
|无|
|adminsAndGuestInviters|
|adminsGuestInvitersAndAllMembers|
|每个人 都|
|unknownFutureValue|

### <a name="datapolicyoperationstatus-values"></a>dataPolicyOperationStatus 值

|成员|
|:---|
|notStarted|
|运行|
|complete|
|失败|
|unknownFutureValue|

### <a name="conditionalaccessdeviceplatform-values"></a>conditionalAccessDevicePlatform 值

| 成员       |
|:--------------|
|Android|
|iOS|
|windows|
|windowsPhone|
|macOS|
|全部|
|unknownFutureValue|

### <a name="signinfrequencytype-values"></a>signinFrequencyType 值

| 成员       |
|:--------------|
|天|
|小时|

### <a name="persistentbrowsersessionmode-values"></a>persistentBrowserSessionMode 值

| 成员       |
|:--------------|
|总是|
|从来 没有|

### <a name="cloudappsecuritysessioncontroltype-values"></a>cloudAppSecuritySessionControlType 值

| 成员       |
|:--------------|
|mcasConfigured|
|monitorOnly|
|blockDownloads|
|unknownFutureValue|

### <a name="conditionalaccessgrantcontrol-values"></a>conditionalAccessGrantControl 值

| 成员       |
|:--------------|
|块|
|Mfa|
|compliantDevice|
|domainJoinedDevice|
|approvedApplication|
|compliantApplication|
|passwordChange|
|unknownFutureValue|

### <a name="conditionalaccessclientapp-values"></a>conditionalAccessClientApp 值

|成员|
|:---|
|全部|
|浏览器|
|mobileAppsAndDesktopClients|
|exchangeActiveSync|
|easSupported|
|其他|
|unknownFutureValue|

### <a name="conditionalaccesspolicystate-values"></a>conditionalAccessPolicyState 值

|成员|
|:---|
|enabled|
|禁用|
|enabledForReportingButNotEnforced|

#### <a name="deviceprofiletype-values"></a>deviceProfileType 值
|成员|
|:---|
|RegisteredDevice|
|SecureVM|
|Printer|
|共享的内容|
|IoT|

### <a name="appliedconditionalaccesspolicyresult-values"></a>appliedConditionalAccessPolicyResult 值 

|成员|
|:---|
|success|
|失败|
|notApplied|
|notEnabled|
|unknown|
|unknownFutureValue|

### <a name="grouptype-values"></a>groupType 值 

|成员|
|:---|
|unifiedGroups|
|azureAD|
|unknownFutureValue|

### <a name="conditionalaccessstatus-values"></a>conditionalAccessStatus 值

|成员|
|:---|
|success|
|失败|
|notApplied|
|unknownFutureValue|

### <a name="operationresult-values"></a>operationResult 值

|成员|
|:---|
|success|
|失败|
|timeout|
|unknownFutureValue|

### <a name="tone-values"></a>音调值

|成员|
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
|明星|
|磅|
|a|
|b|
|c|
|d|
|闪光|

### <a name="mediastate-values"></a>mediaState 值

|成员|
|:---|
|积极|
|无效|
|unknownFutureValue|

### <a name="basicstatus-values"></a>basicStatus 值

|成员|
|:---|
|积极|
|无效|

### <a name="callstate-values"></a>callState 值

|成员|
|:---|
|传入|
|建立|
|响|
|建立|
|hold|
|转移|
|transferAccepted|
|重 定向|
|终止|
|终止|

### <a name="calltype-values"></a>callType 值

|成员|
|:---|
|unknown|
|groupCall|
|peerToPeer|
|unknownFutureValue|

### <a name="educationaddtocalendaroptions-values"></a>educationAddToCalendarOptions 值
|成员|
|:---|
|无|
|studentsAndPublisher|
|studentsAndTeamOwners|
|unknownFutureValue|
|studentsOnly|

### <a name="educationsubmissionstatus-values"></a>educationSubmissionStatus 值
|成员|
|:---|
|工作|
|提交|
|释放|
|返回|
|unknownFutureValue|
|分配|

### <a name="onlinemeetingrole-values"></a>onlineMeetingRole 值

|成员|
|:---|
|attendee|
|主持人|
|unknownFutureValue|

### <a name="modality-values"></a>模式值 

|成员|
|:---|
|audio|
|video|
|videoBasedScreenSharing|
|data|
|screenSharing|
|unknownFutureValue|

### <a name="calldirection-values"></a>callDirection 值

|成员|
|:---|
|传入|
|外向|

### <a name="signinaudience-values"></a>signInAudience 值

|成员|
|:---|
|AzureADMyOrg|
|AzureADMultleOrgs|
|AzureADandPersonalMicrosoftAccount|
|PersonalMicrosoftAccount|

### <a name="groupmembershipclaims-values"></a>groupMembershipClaims 值

|成员|
|:---|
|无|
|SecurityGroup|
|所有|

### <a name="recipientscopetype-values"></a>recipientScopeType 值

|成员|
|:---|
|无|
|内部|
|外部|
|externalPartner|
|externalNonPartner|

### <a name="activitytype-values"></a>activityType 值

|成员|
|:---|
|signin|
|用户|
|unknownFutureValue|

### <a name="riskdetectiontimingtype-values"></a>riskDetectionTimingType 值

|成员|
|:---|
|notDefined|
|实时|
|nearRealtime|
|离线|
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

|成员|值|说明|
|:---|:---|:---|
|父级|0|用户的父级。|
|相对|1| 用户的相对。|
|助手|2| 用户的助手。|
|医生|3| 用户的医生。|
|监护人|4| 用户的监护人。|
|Child|5| 用户的子级。|
|其他|6 | 与用户的未指定关系。|
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
|车|
|日历|
|运行|
|飞机|
|firstAid|
|医生|
|notWorking|
|时钟|
|juryDuty|
|全球|
|杯|
|phone|
|天气|
|伞|
|piggyBank|
|狗|
|蛋糕|
|trafficCone|
|针|
|阳光|
|unknownFutureValue|

### <a name="workforceintegrationencryptionprotocol-values"></a>workforceIntegrationEncryptionProtocol 值

| 成员
|:----------------------------
|sharedSecret
|unknownFutureValue

### <a name="workforceintegrationsupportedentities-values"></a>workforceIntegrationSupportedEntities 值

|成员|
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

| 成员
|:-----------------
| windows
| Iana


### <a name="freebusystatus-values"></a>freeBusyStatus 值

| 成员            |值
|:------------------|:-------
| 自由              | 0
| 初步         | 1
| 忙              | 2
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
| 全部


### <a name="automaticrepliesstatus-values"></a>automaticRepliesStatus 值

| 成员
|:-------------------------
| 禁用
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

| 成员             |
| :----------------- |
| 姐姐                |
| 手动             |
| unknownFutureValue |

### <a name="educationgender-values"></a>educationGender 值

| 成员
|:-------------------------
| 女性
| 男性
| 其他
| unknownFutureValue


### <a name="eventtype-values"></a>eventType 值

| 成员
|:-------------------------
| singleInstance
| 发生
| 例外
| seriesMaster


### <a name="sensitivity-values"></a>敏感度值

| 成员
|:-------------------------
| 正常
| personal
| 私人
| 机密


### <a name="importance-values"></a>重要性值

| 成员
|:-------------------------
| 低
| 正常
| 高

### <a name="educationuserrole-values"></a>educationUserRole 值

| 成员             |
| :----------------- |
| student            |
| teacher            |
| 无               |
| unknownFutureValue |

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
| 标记


### <a name="inferenceclassificationtype-values"></a>inferenceClassificationType 值

| 成员
|:-----------------
| 集中
| 其他


### <a name="iosnotificationalerttype-values"></a>iosNotificationAlertType 值

| 成员
|:-------------------------
| deviceDefault
| 旗帜
| 模 态
| 无

### <a name="deviceenrollmentfailurereason-values"></a>deviceEnrollmentFailureReason 值

| 成员
|:-------------
| unknown
| 身份验证
| 授权
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
| 酒店
| 餐厅
| localBusiness
| postalAddress

### <a name="locationuniqueidtype-values"></a>locationUniqueIdType 值

| 成员
|:-------------------------
| unknown
| locationStore
| 目录
| 私人
| 必应


### <a name="messageactionflag-values"></a>messageActionFlag 值

| 成员
|:-------------------------
| 任意
| 通话
| doNotForward
| 随访
| fyi
| 转发
| noResponseNecessary
| 阅读
| 回复
| replyToAll
| 检讨


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
|NotStarted
|正在运行
|已完成
|已失败


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
| 活动后
| 活动前


### <a name="phonetype-values"></a>phoneType 值

| 成员
|:-------------------------
| 家
| 业务
| mobile
| 其他
| 助理
| homeFax
| businessFax
| otherFax
| pager
| 无线电


### <a name="plannercontainertype-values"></a>plannerContainerType 值

|成员|
|:---|
|组|
|unknownFutureValue|
|名册|


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
| 积极
| 更新
| deleted
| 忽略
| unknownFutureValue


### <a name="weekindex-values"></a>weekIndex 值

| 成员
|:-------------------------
| 第一
| 第二
| 第三
| 四
| 最后


### <a name="dayofweek-values"></a>dayOfWeek 值

| 成员
|:-------------------------
| 星期天
| 星期一
| 星期二
| 星期三
| 星期四
| 星期五
| 星期六

### <a name="recurrencepatterntype-values"></a>recurrencePatternType 值

| 成员
|:-------------------------
| 日常
| 每周
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
| 组织者
| 暂定Accepted
| 接受
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
| 其他
| 家
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

有关分析人员提供的警报的可能反馈值。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知。|
|truePositive|1|警报为 true-positive。|
|falsePositive|2| 警报为误报。|
|benignPositive|3| 警报是良性正的。|

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

枚举网络连接 (入站/出站) 的方向。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知连接。|
|入境|1|入站连接。|
|出境|2| 出站连接。|

### <a name="connectionstatus-values"></a>connectionStatus 值

连接状态的枚举。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知的连接状态。|
|企图|1|尝试连接。|
|成功|2| 连接成功。|
|封锁|3| 连接被阻止。|
|失败|4| 连接失败。|

### <a name="processintegritylevel-values"></a>processIntegrityLevel 值

进程的可能完整性级别值。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知。|
|可信|10|完整性级别不受信任。|
|低|20| 完整性级别较低。|
|中等|30| 完整性级别为中等。|
|高|40| 完整性级别较高。|
|system|50| 完整性级别为 System。|

### <a name="registryhive-values"></a>registryHive 值

由 [/windows/desktop/sysinfo/registry-hives 定义的注册表 hiv 的枚举](/windows/desktop/sysinfo/registry-hives)。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知 hive。|
|currentConfig|1|HKEY_CURRENT_CONFIG hive。|
|currentUser|2| HKEY_CURRENT_USER hive。|
|localMachineSam|3| HKEY_LOCAL_MACHINE\SAM hive。|
|localMachineSamSoftware|4| HKEY_LOCAL_MACHINE\Software hive。|
|localMachineSystem|5| HKEY_LOCAL_MACHINE\System hive。|
|usersDefault|6 | \\HKEY_USERS。DEFAULT hive。|

### <a name="registryoperation-values"></a>registryOperation 值

更改注册表项名称和/或值的操作。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知的注册表值类型。|
|create|1|创建注册表。|
|修改|2|修改注册表。|
|delete|3|删除注册表。|

### <a name="registryvaluetype-values"></a>registryValueType 值

由 [/windows/desktop/sysinfo/registry-value-types](/windows/desktop/sysinfo/registry-value-types) 定义的注册表值类型的枚举。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知的注册表值类型。|
|二 进 制|1|REG_BINARY注册表值类型。|
|Dword|2| REG_DWORD注册表值类型。|
|dwordLittleEndian|3| REG_DWORD_LITTLE_ENDIAN注册表值类型。|
|dwordBigEndian|4| REG_DWORD_BIG_ENDIAN注册表值类型。|
|expandSz|5| REG_EXPAND_SZ注册表值类型。|
|链接|6 | REG_LINK注册表值类型。|
|multiSz|7 | REG_MULTI_SZ注册表值类型。|
|无|8 | REG_NONE注册表值类型。|
|qword|9 | REG_QWORD注册表值类型。|
|qwordlittleEndian|10| REG_QWORD_LITTLE_ENDIAN注册表值类型。|
|深圳|11| REG_SZ注册表值类型。|

### <a name="alertseverity-values"></a>alertSeverity 值

警报严重性的枚举。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|严重性未知。|
|信息|1|严重性仅适用于信息。|
|低|2| 严重性较低。|
|中等|3| 严重性是中等的。|
|高|4| 严重性很高。|

### <a name="alertstatus-values"></a>alertStatus 值

警报生命周期状态的可能值 (阶段) 。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知状态。|
|newAlert|10| 警报是新的。|
|inProgress|20|警报正在进行中。|
|已解决|30|警报已解决。|

### <a name="emailrole-values"></a>emailRole 值
电子邮件角色的可能值。

|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知角色。|
|sender|1|电子邮件的发件人。|
|recipient|2|电子邮件收件人。|

### <a name="logontype-values"></a>logonType 值

用户登录方法的可能值。

|成员|值|说明|
|:---|:---|:---|
|unknown|-1|未知。|
|互动|0|登录是交互式的。|
|remoteInteractive|1| 登录是远程交互式登录。|
|网络|2| 登录是网络。|
|batch|3| 登录是批处理的。|
|服务|4| 登录是服务。|

### <a name="useraccountsecuritytype-values"></a>userAccountSecurityType 值

根据Windows定义，用户帐户类型的可能值 (组成员身份) 。

|成员|成员|说明|
|:---|:---|:---|
|unknown|-1|未知。|
|标准|0|标准用户组的成员。|
|权力|1| Power Users 组的成员。|
|管理员|2| 管理员组的成员。|

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
| 通用
| unknownFutureValue

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
|通用|
|adminConfirmedUserCompromised|
|mcasImpossibleTravel|
|mcasSuspiciousInboxManipulationRules|
|investigationsThreatIntelligenceSigninLinked|
|maliciousIPAddressValidCredentialsBlockedIP|
|unknownFutureValue|

### <a name="risklevel-values"></a>riskLevel 值

| 成员
|:-------------------------
| 无
| 低
| 中等
| 高
| hidden
| unknownFutureValue

### <a name="riskstate-values"></a>riskState 值

| 成员
|:-------------------------
| 无
| confirmedSafe
| 修正
| 解雇
| atRisk
| confirmedCompromised
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
|自 定义|

### <a name="threatassessmentcontenttype-values"></a>threatAssessmentContentType 值

| 成员 | 值 | 说明             |
|:-------|:------|:------------------------|
| mail   | 1     | 邮件威胁。            |
| url    | 2     | URL 威胁。             |
| file   | 3     | 附件文件威胁。 |

### <a name="threatexpectedassessment-values"></a>threatExpectedAssessment 值

| 成员  | 值 | 说明                       |
|:--------|:------|:----------------------------------|
| 块   | 1     | 应阻止威胁。     |
| 疏通 | 2     | 不应阻止威胁。 |

### <a name="threatcategory-values"></a>threatCategory 值

| 成员             | 值 | 说明        |
|:-------------------|:------|:-------------------|
| 垃圾邮件 (spam)               | 1     | 垃圾邮件威胁。       |
| 仿冒           | 2     | 网络钓鱼威胁。   |
| 恶意软件            | 3     | 恶意软件威胁。    |
| unknownFutureValue | 4     | 一个 sentinel 成员。 |

### <a name="threatassessmentstatus-values"></a>threatAssessmentStatus 值

| 成员    | 值 | 说明                              |
|:----------|:------|:-----------------------------------------|
| 等待   | 1     | 威胁评估仍在进行中。 |
| 完成 | 2     | 威胁评估已完成。         |

### <a name="threatassessmentrequestsource-values"></a>threatAssessmentRequestSource 值

| 成员        | 值 | 说明              |
|:--------------|:------|:-------------------------|
| 定义     | 0     | 还不知道            |
| 用户          | 1     | 用户提交。         |
| 管理员 | 2     | 租户管理员提交。 |

### <a name="threatassessmentresulttype-values"></a>threatAssessmentResultType 值

| 成员             | 值 | 说明                                          |
|:-------------------|:------|:-----------------------------------------------------|
| checkPolicy        | 1     | 策略检查结果，仅用于 `mail` 评估。 |
| rescan             | 2     | 重新扫描结果。                                   |
| unknownFutureValue | 3     | 一个 sentinel 成员。                                   |

### <a name="maildestinationroutingreason-values"></a>mailDestinationRoutingReason 值

| 成员                | 值 | 说明                         |
|:----------------------|:------|:------------------------------------|
| 无                  | 0     | 还不知道                       |
| mailFlowRule          | 1     | Exchange传输规则。            |
| safeSender            | 2     | 保险箱发件人列表。                   |
| blockedSender         | 3     | 阻止的发件人列表。                |
| advancedSpamFiltering | 4     | 高级垃圾邮件飞溅选项。     |
| domainAllowList       | 5     | 发送方域允许列表。           |
| domainBlockList       | 6      | 发送方域块列表。           |
| notInAddressBook      | 7      | 排除未在通讯簿中的发件人。 |
| firstTimeSender       | 8      | 由于第一次发送者而被阻止。   |
| autoPurgeToInbox      | 9      | TimeTravel 将消息移动到收件箱。   |
| autoPurgeToJunk       | 10    | TimeTravel 将消息移动到垃圾邮件。    |
| autoPurgeToDeleted    | 11    | 要删除的 TimeTravel 移动消息。 |
| 出境              | 12     | 出站邮件。                      |
| notJunk               | 13    | 允许由于不是垃圾。              |
| 垃圾                  | 14    | 因垃圾而被阻止。                |
| unknownFutureValue    | 15    | 一个 sentinel 成员。                  |

### <a name="chatmessagetype-values"></a>chatMessageType 值

| 值 |
|:-----------------|
| 消息 |
| chatEvent |
| 打字 |
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

| 成员   | Int 值 |  说明 |
|:---------------|:--------|:----------|
| 无 | 0 | 默认值。 当用户尚未对被 DLP 阻止的消息执行操作时，这是消息上的值。 |
| Override | 1 | 发送方已重写消息判决，并发送了该消息。|
| ReportFalsePositive | 2 | 发件人已将消息判决报告给管理员为误报。|

### <a name="chatmessagepolicyviolationverdictdetailstype-values"></a>chatMessagePolicyViolationVerdictDetailsType 值

| 成员   | Int 值 |  说明 |
|:---------------|:--------|:----------|
| 无 | 0 |  不允许用户重写消息。 如果未提供策略提示，则不允许用户将消息报告为误报。 在所有其他情况下，用户可以将消息报告为误报。|
| AllowFalsePositiveOverride | 1 |  不允许用户显式重写块，除非该块与标志或`AllowOverrideWithJustification`标志组合在一起`AllowOverrideWithoutJustification`。 报告违规的误报会自动覆盖块并发送消息。 |
| AllowOverrideWithoutJustification | 2 | 允许用户重写块并发送消息。 不需要理由文本。 独占到 `AllowOverrideWithJustification`. |
| AllowOverrideWithJustification | 4 |  允许用户重写块并发送消息。 需要有理由文本。 独占到 `AllowOverrideWithoutJustification`.|

### <a name="channelmembershiptype-values"></a>channelMembershipType 值

| 成员             | 值 |说明|
| :----------------- | :---- |:-----------|
| 标准           | 0     |频道继承父团队成员的列表。|
| 私人            | 1     |频道可以包含成员，这些成员是父团队中所有成员的子集。|
| unknownFutureValue | 2     |      |
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
| 完成
| waitingOnOthers
| 递 延

### <a name="columntypes-values"></a>columnTypes 值

|成员|说明|
|:-------|:------
|注意| 多行文本。 |
|text | 单行文本。 |
|选择 | 选项列 |
|multichoice | 多选列。 |
|number | 数字列。 |
|货币 | 货币列。 |
|dateTime | DateTime 列。 |
|查找 | 查阅列。 |
|boolean | 是/否列。 |
|用户 | 人员或组列。 |
|url | 超链接或图片列。 |
|计算 | 计算列。 |
|位置 | 位置列。 |
|地理位置 | 地理位置列。 |
|term | 托管元数据列。 |
|multiterm | 接受多个值的托管元数据列。 |
|缩略 图 | 图像列。 |
|approvalStatus | 内容审批状态列。 |
|unknownFutureValue | UnknownFuturevalue |

### <a name="permissionclassificationtype-values"></a>permissionClassificationType 值

| 成员
|:-------
| 低

### <a name="permissiontype-values"></a>permissionType 值

| 成员
|:-------------------------
| 应用程序
| 委托
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
|短|
|冲床|
|覆盖|
|绑定|
|saddleStitch|
|stitchEdge|
|stapleTopLeft|
|stapleBottomLeft|
|stapleTopRight|
|stapleBottomRight|
|stitchLeftEdge|
|stitchTopEdge|
|stitchRightEdge|
|stitchBottomEdge|
|stapleDualLeft|
|stapleDualTop|
|stapleDualRight|
|stapleDualBottom|
|unknownFutureValue|

### <a name="printmultipagelayout-values"></a>printMultipageLayout 值 

|成员|
|:---|
|clockwiseFromTopLeft|
|counterclockwiseFromTopLeft|
|counterclockwiseFromTopRight|
|clockwiseFromTopRight|
|counterclockwiseFromBottomLeft|
|clockwiseFromBottomLeft|
|counterclockwiseFromBottomRight|
|clockwiseFromBottomRight|
|unknownFutureValue|

### <a name="printorientation-values"></a>printOrientation 值 

|成员|
|:---|
|肖像|
|景观|
|reverseLandscape|
|reversePortrait|
|unknownFutureValue|

### <a name="printquality-values"></a>printQuality 值 

|成员|
|:---|
|低|
|中等|
|高|
|unknownFutureValue|

### <a name="printscaling-values"></a>printScaling 值 

|成员|
|:---|
|自动|
|shrinkToFit|
|fill|
|适合|
|无|
|unknownFutureValue|

### <a name="userflowtype-values"></a>userFlowType 值

|成员
|:----------------------
| 注册
| signIn
| signUpOrSignIn
| passwordReset
| profileUpdate
| resourceOwner
| unknownFutureValue

### <a name="identityuserflowattributedatatype-values"></a>identityUserFlowAttributeDataType 值

| 成员                |
|:----------------------|
| string                |
| boolean               |
| int64                 |
| stringCollection      |
| dateTime              |
| unknownFutureValue    |

### <a name="identityuserflowattributetype-values"></a>identityUserFlowAttributeType 值

| 成员                |
|:----------------------|
| 内置               |
| 自 定义                |
| 必需              |
| unknownFutureValue    |

### <a name="identityuserflowattributeinputtype-values"></a>identityUserFlowAttributeInputType 值

| 成员                |
|:----------------------|
| Textbox               |
| dateTimeDropDown      |
| radioSingleSelect     |
| dropdownSingleSelect  |
| emailBox              |
| checkboxMultiSelect   |

### <a name="teamworkactivitytopicsource-values"></a>teamworkActivityTopicSource 值 

| 成员    |
| :-------- |
| entityUrl |
| text      |


### <a name="provisioningresult-values"></a>provisioningResult 值 

|成员|
|:---|
|success|
|失败|
|跳|
|警告|
|unknownFutureValue|

### <a name="provisioningsteptype-values"></a>provisioningStepType 值 

|成员|
|:---|
|进口|
|范围|
|匹配|
|处理|
|referenceResolution|
|出口|
|unknownFutureValue|

### <a name="provisioningstatuserrorcategory-values"></a>provisioningStatusErrorCategory 值 

|成员|
|:---|
|失败|
|nonServiceFailure|
|success|
|unknownFutureValue|

### <a name="provisioningaction-values"></a>provisioningAction 值 

|成员|
|:---|
|其他|
|create|
|delete|
|disable|
|更新|
|stagedDelete|
|unknownFutureValue|


### <a name="initiatortype-values"></a>initiatorType 值 

|成员|
|:---|
|用户|
|应用程序|
|system|
|unknownFutureValue|

### <a name="teamworkapplicationidentitytype-values"></a>teamworkApplicationIdentityType 值 

|成员|
|:---|
|aadApplication|
|自动程序|
|tenantBot|
|office365Connector|
|outgoingWebhook|
|unknownFutureValue|

### <a name="teamworkconversationidentitytype-values"></a>teamworkConversationIdentityType 值 

|成员|
|:---|
|团队|
|通道|
|聊天|
|unknownFutureValue|

### <a name="teamworkuseridentitytype-values"></a>teamworkUserIdentityType 值 

|成员|
|:---|
|aadUser|
|onPremiseAadUser|
|anonymousGuest|
|federatedUser|
|personalMicrosoftAccountUser|
|skypeUser|
|phoneUser|
|unknownFutureValue|
|emailUser|

### <a name="posttype-values"></a>postType 值 

|成员|
|:---|
|定期|
|快速|
|战略|
|unknownFutureValue|

### <a name="searchalterationtype-values"></a>searchAlterationType 值

| 成员 |
|:---------------|
|修改|
|建议|

### <a name="servicehealthclassificationtype-values"></a>serviceHealthClassificationType 值 

|成员|
|:---|
|咨询|
|事件|
|unknownFutureValue|

### <a name="servicehealthorigin-values"></a>serviceHealthOrigin 值 

|成员|
|:---|
|微软|
|thirdParty|
|客户|
|unknownFutureValue|

### <a name="servicehealthstatus-values"></a>serviceHealthStatus 值 

|成员|
|:---|
|serviceOperational|
|正在调查|
|restoreService|
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
|减轻|
|resolvedExternal|
|证实|
|报道|
|unknownFutureValue|

### <a name="serviceupdatecategory-values"></a>serviceUpdateCategory 值 

|成员|
|:---|
|preventOrFixIssue|
|planForChange|
|stayInformed|
|unknownFutureValue|

### <a name="serviceupdateseverity-values"></a>serviceUpdateSeverity 值 

|成员|
|:---|
|正常|
|高|
|关键|
|unknownFutureValue|

### <a name="subjectrightsrequeststage-values"></a>subjectRightsRequestStage 值 

|成员|
|:---|
|contentRetrieval|
|contentReview|
|generateReport|
|contentDeletion|
|caseResolved|
|unknownFutureValue|

### <a name="subjectrightsrequeststagestatus-values"></a>subjectRightsRequestStageStatus 值 

|成员|
|:---|
|notStarted|
|当前| 
|完成| 
|失败|
|unknownFutureValue|

### <a name="subjectrightsrequeststatus-values"></a>subjectRightsRequestStatus 值 

|成员|
|:---|
|积极|
|关闭|
|unknownFutureValue|

### <a name="subjectrightsrequesttype-values"></a>subjectRightsRequestType 值 

|成员|
|:---|
|出口|
|delete|
|访问|
|tagForAction|
|unknownFutureValue|

### <a name="datasubjecttype-values"></a>dataSubjectType 值 

|成员|
|:---|
|客户|
|currentEmployee|
|formerEmployee|
|prospectiveEmployee|
|student|
|teacher|
|教师|
|其他|
|unknownFutureValue|

### <a name="advancedconfigstate-values"></a>advancedConfigState 值 

|成员|
|:---|
|默认|
|enabled|
|禁用|
|unknownFutureValue|

### <a name="callrecordingstatus-values"></a>callRecordingStatus 值 

|成员|
|:---|
|success|
|失败|
|初始|
|chunkFinished|
|unknownFutureValue|

### <a name="teamworkcalleventtype-values"></a>teamworkCallEventType 值 

|成员|
|:---|
|通话|
|会议|
|screenShare|
|unknownFutureValue|

### <a name="bookingreminderrecipients-values"></a>bookingReminderRecipients 值 

|成员|
|:---|
|allAttendees|
|员工|
|客户|
|unknownFutureValue|

### <a name="bookingstaffrole-values"></a>bookingStaffRole 值 

|成员|
|:---|
|客人|
|管理员|
|观众|
|externalGuest|
|unknownFutureValue|

### <a name="answerinputtype-values"></a>answerInputType 值 

|成员|
|:---|
|text|
|radioButton|
|unknownFutureValue|

### <a name="bookingpricetype-values"></a>bookingPriceType 值

|成员|
|:---|
|定义|
|fixedPrice|
|startingAt|
|小时|
|自由|
|priceVaries|
|愈 伤 组织|
|notSet|
|unknownFutureValue|

### <a name="accessreviewhistorystatus-values"></a>accessReviewHistoryStatus 值

| 成员|
|:-----------------|
|done|
|inprogress|
|error|
|要求|
|unknownFutureValue|

### <a name="accessreviewhistorydecisionfilter-values"></a>accessReviewHistoryDecisionFilter 值

| 成员|
|:-----------------|
|批准|
|否认|
|notReviewed|
|dontKnow|
|notNotified|
|unknownFutureValue|

### <a name="authenticationprotocol-values"></a>authenticationProtocol 值 

|成员|
|:---|
|wsFed|
|Saml|

### <a name="longrunningoperationstatus-values"></a>longRunningOperationStatus 值

| 成员|
|:-----------------|
|notStarted|
|运行|
|成功|
|失败|
|unknownFutureValue|
