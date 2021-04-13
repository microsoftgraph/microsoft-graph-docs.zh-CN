---
title: 枚举值
description: Microsoft Graph 枚举值
doc_type: enumPageType
localization_priority: Normal
ms.prod: non-product-specific
author: MSGraphDocsvTeam
ms.openlocfilehash: 42ee6a9363efd868085cecb62a9a6aa5ac5600d4
ms.sourcegitcommit: fdd69d362d1debc7b08e78269d59b531f9dfdaae
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697205"
---
# <a name="enum-values"></a>枚举值

命名空间：microsoft.graph

### <a name="countrylookupmethodtype-values"></a>countryLookupMethodType 值

|Member|
|:---|
|clientIpAddress|
|authenticatorApp提供|

### <a name="approvalstate-values"></a>approvalState 值

|Member|
|:---|
|pending|
|已批准|
|denied|
|aborted|
|canceled|

### <a name="rolesummarystatus-values"></a>roleSummaryStatus 值

|Member|
|:---|
|还行|
|bad|

### <a name="datapolicyoperationstatus-values"></a>dataPolicyOperationStatus 值

|Member|
|:---|
|notStarted|
|running|
|complete|
|failed|
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

### <a name="consentrequestfilterbycurrentuseroptions-values"></a>consentRequestFilterByCurrentUserOptions 值 

|Member|
|:---|
|reviewer|
|unknownFutureValue|

### <a name="attributetype-values"></a>attributeType 值

|Member|
|:---|
|String|
|整数|
|参考|
|二进制|
|Boolean|
|日期时间|

### <a name="mutability-values"></a>可变值

|Member|
|:---|
|读写|
|ReadOnly|
|不可变|
|WriteOnly|

### <a name="directorydefinitiondiscoverabilities-values"></a>directoryDefinitionDiscoverabilities 值

|Member|
|:---|
|无|
|AttributeNames|
|AttributeDataTypes|
|AttributeReadOnly|
|ReferenceAttributes|
|UnknownFutureValue|

### <a name="connectorgroupregion-values"></a>connectorGroupRegion 值

|Member|
|:---|
|nam|
|eur|
|aus|
|asia|
|ind|
|unknownFutureValue|

### <a name="connectorgrouptype-values"></a>connectorGroupType 值

|Member|
|:---|
|applicationProxy|

### <a name="onpremisespublishingtype-values"></a>onPremisesPublishingType 值

|Member|
|:---|
|applicationProxy|
|exchangeOnline|
|身份验证|
|预配|
|intunePfx|
|oflineDomainJoin|
|unknownFutureValue|

### <a name="agentstatus-values"></a>agentStatus 值

|Member|
|:---|
|active|
|inactive|

### <a name="connectorstatus-values"></a>connectorStatus 值

|Member|
|:---|
|active|
|inactive|

### <a name="calltype-values"></a>callType 值

|Member|
|:---|
|unknown|
|groupCall|
|peerToPeer|
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

### <a name="routingpolicy-values"></a>routingPolicy 值

|Member|
|:---|
|无|
|noMissedCall|
|disableForwardingExceptPhone|
|disableForwarding|
|preferSkypeForBusiness|
|unknownFutureValue|

### <a name="meetingcapabilities-values"></a>meetingCapabilities 值

|Member|
|:---|
|questionAndAnswer|
|unknownFutureValue|

### <a name="onlinemeetingrole-values"></a>onlineMeetingRole 值

|Member|
|:---|
|attendee|
|演示者|
|producer|
|unknownFutureValue|

### <a name="autoadmitteduserstype-values"></a>autoAdmittedUsersType 值

|Member|
|:---|
|everyoneInCompany|
|everyone|

### <a name="mediastate-values"></a>mediaState 值

|Member|
|:---|
|active|
|inactive|
|unknownFutureValue|

### <a name="calldirection-values"></a>callDirection 值 

|Member|
|:---|
|incoming|
|传出|

### <a name="modality-values"></a>形式值 

|Member|
|:---|
|audio|
|video|
|videoBasedScreenSharing|
|data|
|screenSharing|
|unknownFutureValue|

### <a name="kerberossignonmappingattributetype-values"></a>kerberosSignOnMappingAttributeType 值 

|Member|
|:---|
|userPrincipalName|
|onPremisesUserPrincipalName|
|userPrincipalUsername|
|onPremisesUserPrincipalUsername|
|onPremisesSAMAccountName|

### <a name="externalauthenticationtype-values"></a>externalAuthenticationType 值 

|Member|
|:---|
|passthru|
|aadPreAuthentication|

### <a name="recipientscopetype-values"></a>recipientScopeType 值
|Member|
|:---|
|无|
|internal|
|external|
|externalPartner|
|externalNonPartner|

### <a name="appliedconditionalaccesspolicyresult-values"></a>appliedConditionalAccessPolicyResult 值 

|Member|
|:---|
|success|
|failure|
|notApplied|
|notEnabled|
|unknown|
|unknownFutureValue|
|reportOnlySuccess|
|reportOnlyFailure|
|reportOnlyNotApplied|
|reportOnlyInterrupted|


### <a name="microsoftauthenticatorauthenticationmode-values"></a>microsoftAuthenticatorAuthenticationMode 值

 

|Member|
|:---|
|任意|
|push|
|deviceBasedPush|


### <a name="authenticationmethodfeature-values"></a>authenticationMethodFeature 值 

|Member|
|:---|
|ssprRegistered|
|ssprEnabled|
|ssprCapable|
|passwordlessCapable|
|mfaCapable|

### <a name="authenticatorappfeaturesettings-values"></a>authenticatorAppFeatureSettings 值 



|Member|
|:---|
|requireNumberMatching|
|unknownFutureValue|

### <a name="authmethodstype-values"></a>authMethodsType 值 

|Member|
|:---|
|email|
|mobileSMS|
|mobilePhone|
|officePhone|
|securityQuestion|
|appNotification|
|appNotificationCode|
|appNotificationAndCode|
|appPassword|
|fido|
|alternateMobilePhone|
|mobilePhoneAndSMS|
|unknownFutureValue|

### <a name="azureadlicensetype-values"></a>azureADLicenseType 值 

|Member|
|:---|
|无|
|free|
|basic|
|premiumP1|
|premiumP2|
|unknownFutureValue|

### <a name="conditionalaccessconditions-values"></a>conditionalAccessConditions 值 

|Member|
|:---|
|无|
|应用程序|
|users|
|devicePlatform|
|位置|
|clientType|
|signInRisk|
|userRisk|
|time|
|deviceState|
|client|

### <a name="conditionalaccessstatus-values"></a>conditionalAccessStatus 值 

|Member|
|:---|
|success|
|failure|
|notApplied|
|unknownFutureValue|

### <a name="featuretype-values"></a>featureType 值 

|Member|
|:---|
|注册|
|重置|
|unknownFutureValue|

### <a name="grouptype-values"></a>groupType 值 

|Member|
|:---|
|unifiedGroups|
|azureAD|
|unknownFutureValue|

### <a name="includeduserroles-values"></a>includedUserRoles 值 

|Member|
|:---|
|all|
|privilegedAdmin|
|admin|
|user|
|unknownFutureValue|

### <a name="includedusertypes-values"></a>includedUserTypes 值 

|Member|
|:---|
|all|
|成员|
|来宾|
|unknownFutureValue|

### <a name="initiatortype-values"></a>initiatorType 值 

|Member|
|:---|
|user|
|应用|
|system|
|unknownFutureValue|

### <a name="migrationstatus-values"></a>migrationStatus 值 

|Member|
|:---|
|ready|
|needsReview|
|additionalStepsRequired|
|unknownFutureValue|

### <a name="networktype-values"></a>networkType 值 

|Member|
|:---|
|Intranet|
|Extranet|
|namedNetwork|
|trusted|
|unknownFutureValue|

### <a name="operationresult-values"></a>operationResult 值 

|Member|
|:---|
|success|
|failure|
|timeout|
|unknownFutureValue|

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
|fido|
|appPassword|
|unknownFutureValue|

### <a name="registrationstatustype-values"></a>registrationStatusType 值 

|Member|
|:---|
|registered|
|enabled|
|capable|
|mfaRegistered|
|unknownFutureValue|

### <a name="requirementprovider-values"></a>requirementProvider 值 

|Member|
|:---|
|MFA|
|CA|
|unknownFutureValue|


### <a name="riskdetail-values"></a>riskDetail 值 

|Member|
|:---|
|无|
|internal|
|external|
|externalPartner|
|externalNonPartner|
|adminGeneratedTemporaryPassword|
|userPerformedSecuredPasswordChange|
|userPerformedSecuredPasswordReset|
|adminConfirmedSigninSafe|
|aiConfirmedSigninSafe|
|userPassedMFADrivenByRiskBasedPolicy|
|adminDismissedAllRiskForUser|
|adminConfirmedSigninComprom一|
|hidden|
|adminConfirmedUserComprom一|
|unknownFutureValue|

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

|Member|
|:---|
|low|
|中等|
|high|
|hidden|
|无|
|unknownFutureValue|

### <a name="riskstate-values"></a>riskState 值 

|Member|
|:---|
|无|
|confirmedSafe|
|修正|
|dismissed|
|atRisk|
|confirmedComprom一|
|unknownFutureValue|

### <a name="tokenissuertype-values"></a>tokenIssuerType 值 

|Member|
|:---|
|AzureAD|
|ADFederationServices|
|UnknownFutureValue|

### <a name="usageauthmethod-values"></a>usageAuthMethod 值 

|Member|
|:---|
|email|
|mobileSMS|
|mobileCall|
|officePhone|
|securityQuestion|
|appNotification|
|appCode|
|alternateMobileCall|
|fido|
|appPassword|
|unknownFutureValue|

### <a name="authenticationmethodkeystrength-values"></a>authenticationMethodKeyStrength 值

|Member|
|:---|
|normal|
|weak|
|unknown|

### <a name="educationaddedstudentaction-values"></a>educationAddedStudentAction 值

|Member|
|:---|
|无|
|assignIfOpen|
|unknownFutureValue|

### <a name="externalemailotpstate-values"></a>externalEmailOtpState 值

|Member|
|:---|
|default|
|enabled|
|disabled|
|unknownFutureValue|

### <a name="replyrestriction-values"></a>replyRestriction 值

| Member
|:--------------
| everyone
| authorAndModerators
| unknownFutureValue

### <a name="usernewmessagerestriction-values"></a>userNewMessageRestriction 值

| Member
|:--------------
|everyone
|everyoneExceptGuests
|审阅人
|unknownFutureValue

### <a name="volumetype-values"></a>volumeType 值

|Member|
|:---|
|operatingSystemVolume|
|fixedDataVolume|
|removableDataVolume|
|unknownFutureValue|

### <a name="allowedaudiences-values"></a>allowedAudiences 值

|Member|
|:---|
|me|
|family|
|contacts|
|groupMembers|
|组织|
|federatedOrganizations|
|everyone|
|unknownFutureValue|

### <a name="attestationlevel-values"></a>attestationLevel 值

|Member|
|:---|
|已证明|
|notAttested|
|unknownFutureValue|

### <a name="emailtype-values"></a>emailType 值

|Member|
|:---|
|unknown|
|工时|
|personal|
|main|
|other|

### <a name="authenticationmethodsigninstate-values"></a>authenticationMethodSignInState 值

|Member|
|:---|
|notSupported|
|notAllowedByPolicy|
|notEnabled|
|phoneNumberNotUnique|
|ready|
|notConfigured|
|unknownFutureValue|

### <a name="authenticationphonetype-values"></a>authenticationPhoneType 值

|Member|
|:---|
|mobile|
|alternateMobile|
|办公室|
|unknownFutureValue|


### <a name="authenticationmethodtargettype-values"></a>authenticationMethodTargetType 值

|Member|
|:---|
|user|
|group|

### <a name="authenticationmethodstate-values"></a>authenticationMethodState 值

|Member|
|:---|
|enabled|
|disabled|

### <a name="fido2restrictionenforcementtype-values"></a>fido2RestrictionEnforcementType 值

|Member|
|:---|
|allow|
|block|
|unknownFutureValue|

### <a name="authenticatorappcontexttype-values"></a>authenticatorAppContextType 值

|Member|
|:---|
|位置|
|应用|

### <a name="anniversarytype-values"></a>anniversaryType 值

|Member|
|:---|
|birthday|
|的|
|unknownFutureValue|

### <a name="skillproficiencylevel-values"></a>skillProficiencyLevel 值

|Member|
|:---|
|一些|
|limitedWorking|
|generalProfessional|
|advancedProfessional|
|expert|
|unknownFutureValue|

### <a name="languageproficiencylevel-values"></a>languageProficiencyLevel 值

|Member|
|:---|
|一些|
|conversational|
|limitedWorking|
|professionalWorking|
|fullProfessional|
|nativeOrBilingual|
|unknownFutureValue|

### <a name="personrelationship-values"></a>personRelationship 值

|Member|
|:---|
|manager|
|同事|
|directReport|
|dotLineReport|
|assistant|
|dotLineManager|
|alternateContact|
|friend|
|配偶|
|同级|
|Child|
|父级|
|发起人|
|emergencyContact|
|other|
|unknownFutureValue|

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
| meeting

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

| 成员             | 值 | 说明                              |
| :----------------- | :---- | :--------------------------------------- |
| 父级             | 0     | 用户的父级。                       |
| relative           | 1     | 用户的相对。                     |
| aide               | 2     | 用户的助手。                         |
| 一个             | 3     | 用户的 <3> <2> <2>。                       |
| 保护者           | 4      | 用户的保护者。                     |
| Child              | 5      | 用户的子级。                        |
| other              | 6      | 与用户未指定的关系。 |
| unknownFutureValue | 7      | 用于将来兼容性的标记值。   |

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

### <a name="schedulechangestate-values"></a>scheduleChangeState 值

| Member
|:----------------------------
|pending
|已批准
|declined
|unknownFutureValue

### <a name="schedulechangerequestactor-values"></a>scheduleChangeRequestActor 值

| Member
|:----------------------------
|sender
|recipient
|manager
|system
|unknownFutureValue

### <a name="workforceintegrationencryptionprotocol-values"></a>workforceIntegrationEncryptionProtocol 值

| Member
|:----------------------------
|sharedSecret
|unknownFutureValue

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
| windows
| iana


### <a name="freebusystatus-values"></a>freeBusyStatus 值

| 成员           | 值 |
| :--------------- | :---- |
| free             | 0     |
| 暂定        | 1     |
| 忙碌             | 2     |
| oof              | 3     |
| workingElsewhere | 4      |
| unknown          | -1    |


### <a name="physicaladdresstype-values"></a>physicalAddressType 值

| Member
|:-------------------------
| unknown
| home
| business
| other


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
| 预配       | 7      |
| unknownFutureValue | 8      |


### <a name="educationsynchronizationstatus-values"></a>educationSynchronizationStatus 值

| 成员             | 值 |
| :----------------- | :---- |
| paused             | 0     |
| inProgress         | 1     |
| success            | 2     |
| error              | 3     |
| validationError    | 4      |
| quarantined        | 5      |
| unknownFutureValue | 6      |

### <a name="educationexternalsource-values"></a>educationExternalSource 值

| Member
|:-------------------------
| sis
| lms
| 手动
| unknownFutureValue

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
| Member
|:---------------------
| student
| teacher
| 教职员工


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
| forward
| noResponseNecessary
| 阅读
| reply
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

| Member
|:-----------------
|NotStarted
|正在运行
|Completed
|已失败


### <a name="onenotepatchactiontype-values"></a>onenotePatchActionType 值

| Member
|:-------------------------
| 替换
| Append
| Delete
| Insert
| Prepend

### <a name="onenotepatchinsertposition-values"></a>onenotePatchInsertPosition 值

| Member
|:-------------------------
| 段后
| Before


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
| 说明
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
| organizer － 组织者
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
| preset10 | 10      |
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

分析员提供的警报的可能反馈值。

| 成员         | 值 | 说明               |
| :------------- | :---- | :------------------------ |
| unknown        | 0     | 未知。                  |
| truePositive   | 1     | 警报为正数。   |
| falsePositive  | 2     | 警报为误报。  |
| 将positive | 3     | 警报是正性警报。 |

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
| inbound  | 1     | 入站连接。  |
| 出站 | 2     | 出站连接。 |

### <a name="connectionstatus-values"></a>connectionStatus 值

| 成员    | 值 | 说明                |
| :-------- | :---- | :------------------------- |
| unknown   | 0     | 连接状态未知。 |
| attempted | 1     | 已尝试连接。      |
| succeeded | 2     | 连接成功。      |
| blocked   | 3     | 连接被阻止。        |
| failed    | 4      | 连接失败。         |

### <a name="processintegritylevel-values"></a>processIntegrityLevel 值

| 成员    | 值 | 说明                   |
| :-------- | :---- | :---------------------------- |
| unknown   | 0     | 未知。                      |
| 不受信任的 | 10      | 完整性级别不受信任。 |
| low       | 20    | 完整性级别为"低"。       |
| 中等    | 30    | 完整性级别为"中"。    |
| high      | 40    | 完整性级别为"高"。      |
| system    | 50    | 完整性级别为系统。    |

### <a name="registryhive-values"></a>registryHive 值

由 定义的注册表配置单元的枚举 [https://docs.microsoft.com/windows/desktop/sysinfo/registry-hives](/windows/desktop/sysinfo/registry-hives) 。

| 成员                  | 值 | 说明                       |
| :---------------------- | :---- | :-------------------------------- |
| unknown                 | 0     | 未知配置单元。                     |
| currentConfig           | 1     | HKEY_CURRENT_CONFIG配置单元。         |
| currentUser             | 2     | HKEY_CURRENT_USER配置单元。           |
| localMachineSam         | 3     | HKEY_LOCAL_MACHINE\SAM配置单元。      |
| localMachineSamSoftware | 4      | HKEY_LOCAL_MACHINE\Software配置单元。 |
| localMachineSystem      | 5      | HKEY_LOCAL_MACHINE\System配置单元。   |
| usersDefault            | 6      | HKEY_USERS \\ 。DEFAULT 配置单元。        |

### <a name="registryoperation-values"></a>registryOperation 值

更改注册表项名称和/或值的操作。

| 成员  | 值 | 说明                  |
| :------ | :---- | :--------------------------- |
| unknown | 0     | 未知的注册表值类型。 |
| create  | 1     | 创建注册表。             |
| modify  | 2     | 修改注册表。             |
| delete  | 3     | 删除注册表。             |

### <a name="registryvaluetype-values"></a>registryValueType 值

由注册表值类型定义的注册表 [值类型的枚举](/windows/desktop/sysinfo/registry-value-types)。

| 成员            | 值 | 说明                                  |
| :---------------- | :---- | :------------------------------------------- |
| unknown           | 0     | 未知的注册表值类型。                 |
| binary            | 1     | REG_BINARY注册表值类型。              |
| dword             | 2     | REG_DWORD注册表值类型。               |
| dwordLittleEndian | 3     | REG_DWORD_LITTLE_ENDIAN注册表值类型。 |
| dwordBigEndian    | 4      | REG_DWORD_BIG_ENDIAN注册表值类型。    |
| expandSz          | 5      | REG_EXPAND_SZ注册表值类型。           |
| link              | 6      | REG_LINK注册表值类型。                |
| multiSz           | 7      | REG_MULTI_SZ注册表值类型。            |
| 无              | 8      | REG_NONE注册表值类型。                |
| qword             | 9      | REG_QWORD注册表值类型。               |
| qwordlittleEndian | 10      | REG_QWORD_LITTLE_ENDIAN注册表值类型。 |
| sz                | 11    | REG_SZ注册表值类型。                  |

### <a name="alertseverity-values"></a>alertSeverity 值

警报严重性枚举。

| 成员        | 值 | 说明                       |
| :------------ | :---- | :-------------------------------- |
| unknown       | 0     | 严重性未知。              |
| informational | 1     | 严重性仅适用于信息。 |
| low           | 2     | 严重性较低。                  |
| 中等        | 3     | 严重性为中等。               |
| high          | 4      | 严重性较高。                 |

### <a name="alertstatus-values"></a>alertStatus 值

警报生命周期状态的可能值 (阶段) 。

| 成员     | 值 | 说明           |
| :--------- | :---- | :-------------------- |
| unknown    | 0     | 未知状态。       |
| newAlert   | 10      | 警报是新警报。         |
| inProgress | 20    | 警报正在进行中。 |
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
| remoteInteractive | 1     | 登录是远程交互的。 |
| network           | 2     | 登录是网络。            |
| batch             | 3     | 登录是批处理。              |
| 服务           | 4      | 登录是服务。            |

### <a name="useraccountsecuritytype-values"></a>userAccountSecurityType 值

根据 Windows 定义，用户帐户类型 (组) 的可能值。

| 成员        | 值 | 说明                     |
| :------------ | :---- | :------------------------------ |
| unknown       | -1    | 未知。                        |
| standard      | 0     | 标准用户组的成员。 |
| power         | 1     | Power Users 组的成员。    |
| administrator | 2     | 组管理员组。 |

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
|all|
|任意|

### <a name="risklevel-values"></a>riskLevel 值

|Member|
|:---|
|low|
|中等|
|high|
|hidden|
|无|
|unknownFutureValue|

### <a name="riskstate-values"></a>riskState 值

|Member|
|:---|
|无|
|confirmedSafe|
|修正|
|dismissed|
|atRisk|
|confirmedComprom一|
|unknownFutureValue|

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

### <a name="referenceattachmentpermission-values"></a>referenceAttachmentPermission 值

|Member|
|:---|
|other|
|view|
|edit|
|anonymousView|
|anonymousEdit|
|organizationView|
|organizationEdit|

### <a name="referenceattachmentprovider-values"></a>referenceAttachmentProvider 值

|Member|
|:---|
|other|
|oneDriveBusiness|
|oneDriveConsumer|
|收存箱|

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

### <a name="networktype-values"></a>networkType 值

|Member|
|:---|
|Intranet|
|Extranet|
|namedNetwork|
|trusted|
|unknownFutureValue|

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
| Delete | 4      |

### <a name="chatmessagetype-values"></a>chatMessageType 值

|Member|
|:---|
|message|

### <a name="chatmessageimportance-values"></a>chatMessageImportance 值

|Member|
|:---|
|normal|
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
| passthroughAuthentication | Passthrough 身份验证    |
| seamlessSso               | 无缝单一登录       |
| passwordHashSync          | 密码哈希同步 |
| emailAsAlternateId        | 作为备用 ID 的电子邮件      |
| unknownFutureValue        | sentinel 成员             |

### <a name="tokenissuertype-values"></a>tokenIssuerType 值

|Member|
|:---|
|AzureAD|
|ADFederationServices|
|unknownFutureValue|

### <a name="riskdetectiontimingtype-values"></a>riskDetectionTimingType 值

|Member|
|:---|
|notDefined|
|realtime|
|nearRealtime|
|offline|
|unknownFutureValue|

### <a name="activitytype-values"></a>activityType 值

|Member|
|:---|
|signin|
|user|
|unknownFutureValue|

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
| AllowFalsePositiveOverride | 1 |  除非此块与 或 标志组合在一起，否则不允许用户显式 `AllowOverrideWithoutJustification` 覆盖 `AllowOverrideWithJustification` 块。 报告违反误报会自动覆盖阻止并发送邮件。 |
| AllowOverrideWithoutJustification | 2 | 允许用户覆盖块并发送邮件。 理由文本不是必需的。 独占到 `AllowOverrideWithJustification` 。 |
| AllowOverrideWithJustification | 4  |  允许用户覆盖块并发送邮件。 理由文本是必需的。 独占到 `AllowOverrideWithoutJustification` 。|

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
|custom|

### <a name="contentformat-values"></a>contentFormat 值

| 成员  | 值 | 说明                          |
| :------ | :---- | :----------------------------------- |
| default | 0     | 内容是文件或非电子邮件类型。 |
| email   | 1     | 内容是电子邮件。                 |

### <a name="contentstate-values"></a>contentState 值

| 成员 | 值 | 说明                                                                      |
| :----- | :---- | :------------------------------------------------------------------------------- |
| rest   | 0     | 数据处于其余;例如，共享中的文件。                                 |
| 动作 | 1     | 数据在运动中。 在传输过程中被网络设备截获的文件。         |
| use    | 2     | 数据在使用中。 文件在客户端应用程序（如客户端应用程序）中Microsoft Office。 |

### <a name="assignmentmethod-values"></a>assignmentMethod 值

| 成员     | 值 | 说明                                                                                                                      |
| :--------- | :---- | :------------------------------------------------------------------------------------------------------------------------------- |
| standard   | 0     | 标签由服务或策略条件设置。                                                                              |
| privileged | 1     | 标签是由用户显式设置的。                                                                                          |
| 自动       | 2     | 允许覆盖任何现有标签。 降级所需的理由。 结果为 `standard` 元数据中的分配方法。 |

### <a name="actionsource-values"></a>actionSource 值

| 成员        | 值 | 说明                                                  |
| :------------ | :---- | :----------------------------------------------------------- |
| 手动        | 0     | 用户手动选择了标签。                          |
| 自动     | 1     | 该标签是策略条件的结果。       |
| 建议   | 2     | 选择应用推荐的标签。                    |
| policyDefault | 3     | 用户没有操作，并且应用了策略默认标签。 |
| mandatory     | 4      | 用户在被强制选择后选择了标签。         |

### <a name="contentalignment-values"></a>contentAlignment 值

| 成员 | 值 | 说明                         |
| :----- | :---- | :---------------------------------- |
| left   | 0     | 将内容标记向左对齐。  |
| right  | 1     | 将内容标记向右对齐。 |
| center | 2     | 居中内容标记。             |

### <a name="watermarklayout-values"></a>watermarkLayout 值

| 成员     | 值 | 说明                 |
| :--------- | :---- | :-------------------------- |
| horizontal | 0     | 使用水平水印。 |
| 对角线   | 1     | 使用对角线水印。   |

### <a name="conditionalaccesspolicystate-values"></a>conditionalAccessPolicyState 值

|Member|
|:---|
|enabled|
|disabled|
|enabledForReportingButNotEnforced|

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

### <a name="priority-values"></a>优先级值

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
| block   | 1     | 应阻止威胁。     |
| unblock | 2     | 不应阻止威胁。 |

### <a name="threatcategory-values"></a>threatCategory 值

| 成员             | 值 | 说明        |
|:-------------------|:------|:-------------------|
| 垃圾邮件               | 1     | 垃圾邮件威胁。       |
| 仿冒           | 2     | 网络钓鱼威胁。   |
| 恶意软件            | 3     | 恶意软件威胁。    |
| unknownFutureValue | 4      | sentinel 成员。 |

### <a name="threatassessmentstatus-values"></a>threatAssessmentStatus 值

| 成员    | 值 | 说明                              |
|:----------|:------|:-----------------------------------------|
| pending   | 1     | 威胁评估仍在进行中。 |
| 已完成 | 2     | 已完成威胁评估。         |

### <a name="threatassessmentrequestsource-values"></a>threatAssessmentRequestSource 值

| 成员        | 值 | 说明              |
|:--------------|:------|:-------------------------|
| undefined     | 0     | 尚不知道。            |
| user          | 1     | 用户提交。         |
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
| mailFlowRule          | 1     | Exchange 传输规则。            |
| safeSender            | 2     | 安全发件人列表。                   |
| blockedSender         | 3     | 阻止的发件人列表。                |
| advancedSpamFiltering | 4      | 高级垃圾邮件筛选选项。     |
| domainAllowList       | 5      | 发件人域允许列表。           |
| domainBlockList       | 6      | 发件人域阻止列表。           |
| notInAddressBook      | 7      | 排除不在通讯簿中的发件人。 |
| firstTimeSender       | 8      | 因第一次发送者被阻止。   |
| autoPurgeToInbox      | 9      | TimeTravel 将邮件移动到收件箱。   |
| autoPurgeToJunk       | 10      | TimeTravel 将邮件移动到垃圾邮件。    |
| autoPurgeToDeleted    | 11    | TimeTravel 要删除的移动消息。 |
| 出站              | 12     | 出站邮件。                      |
| notJunk               | 13    | 允许，因为不是垃圾邮件。              |
| junk                  | 14     | 因垃圾邮件被阻止。                |
| unknownFutureValue    | 15     | sentinel 成员。                  |

### <a name="threatassessmentrequestpivotproperty-values"></a>threatAssessmentRequestPivotProperty 值

| 成员                       | 值 | 说明                                                            |
|:-----------------------------|:------|:-----------------------------------------------------------------------|
| threatCategory               | 1     | 聚合威胁评估请求 `threatCategory` 。               |
| mailDestinationRoutingReason | 2     | 聚合威胁评估请求 `mailDestinationRoutingReason` 。 |

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

### <a name="openidconnectresponsemode-values"></a>openIdConnectResponseMode 值

| Member
|:----------------------
| form_post
| 查询
| unknownFutureValue

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
|choice | choice 列 |
|multichoice | multichoice 列。 |
|number | 数字列。 |
|currency | currency 列。 |
|dateTime | dateTime 列。 |
|查找 | 查找列。 |
|boolean | 是/否列。 |
|user | 人员或组列。 |
|url | 超链接或图片列。 |
|calculated | 计算列。 |
|位置 | location 列。 |
|地理位置 | 地理位置列。 |
|term | 托管元数据列。 |
|multiterm | 接受多个值的托管元数据列。 |
|thumbnail | 图像列。 |
|approvalStatus | 内容审批状态列。 |
|unknownFutureValue | unknownFuturevalue |

### <a name="connectedorganizationstate-values"></a>connectedOrganizationState 值

| 成员                | 值 | 说明                                                                                                                                                                                                        |
|:----------------------| :-----|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 已配置            | 0     | 具有此状态值的已连接组织包含在具有请求者作用域类型的分配策略中 `AllConfiguredConnectedOrganizationSubjects` 。                                                          |
| 已建议              | 1     | 由系统自动创建的已连接组织具有此状态值。 它们不包含在具有请求者作用域类型的分配策略中 `AllConfiguredConnectedOrganizationSubjects` 。   |
| unknownFutureValue    | 2     | sentinel 成员。                                                                                                                                                                                                 |

### <a name="identitysourcetype-values"></a>identitySourceType 值

|Member|
|:---|
|azureActiveDirectory|
|external|

### <a name="externalgroupmembertype-values"></a>externalGroupMemberType 值

|Member|
|:---|
|user|
|group|

### <a name="identityuserflowattributedatatype-values"></a>identityUserFlowAttributeDataType 值

| 成员                | 值 | 说明                         |
|:----------------------|:------|:------------------------------------|
| string                | 1     | String 数据类型                    |
| boolean               | 2     | Boolean 数据类型                   |
| int64                 | 3     | Int 数据类型                       |
| stringCollection      | 4      | 字符串集合数据类型         |
|dateTime|5 ||
| unknownFutureValue    | 6      | sentinel 成员。                  |

### <a name="identityuserflowattributetype-values"></a>identityUserFlowAttributeType 值

| 成员                | 值 | 说明                                                        |
|:----------------------|:------|:-------------------------------------------------------------------|
| builtIn               | 1     | 此用户流属性类型表示它是由系统创建的 |
| custom                | 2     | 此用户流属性类型表示它是由用户创建的   |
|必需|3||
| unknownFutureValue    | 4      | sentinel 成员。                                                 |

### <a name="connectionstate-values"></a>connectionState 值

|Member|
|:---|
|draft|
|ready|
|已过时|
|limitExceeded|

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

### <a name="cloudpcprovisioningpolicyimagetype-values"></a>cloudPcProvisioningPolicyImageType 值

|Member|
|:---|
|custom|
|库|

### <a name="chattype-values"></a>chatType 值 

| 成员             | 值 | 说明               |
| :----------------- | :---- | :------------------------ |
|oneOnOne            | 0     | 指示聊天为一对一聊天。 对于此类聊天，名单大小是固定的，无法删除/添加成员。                  |
|group               | 1     | 指示聊天是群聊。 可以针对 (聊天至少 2 人) 名单大小。 稍后可以删除/添加成员。   |
|meeting             | 2     | 指示聊天是会议聊天，创建为创建 OnlineMeeting 的副作用。  |
|unknownFutureValue  | 3     | Sentinel 值，用于指示未来值。 |

### <a name="singlesignonmode-values"></a>singleSignOnMode 值

|Member|
|:---|
|无|
|onPremisesKerberos|
|aadHeaderBased|
|pingHeaderBased|

### <a name="plannercontainertype-values"></a>plannerContainerType 值 

|Member|
|:---|
|group|
|unknownFutureValue|

### <a name="plannerplancontexttype-values"></a>plannerPlanContextType 值 

|Member|
|:---|
|teamsTab|
|sharePointPage|
|meetingNotes|
|other|
|unknownFutureValue|

### <a name="teamsappinstallationscope-values"></a>teamsAppInstallationScope 值

|成员    |值    |说明 |
|:---------|:--------|:----------- |
|团队      |0        |指示 Teams 应用可以安装在团队中，并有权访问该团队的数据。|
|groupChat |1        |指示 Teams 应用可以安装在群聊中，并有权访问该群聊的数据。|
|personal  |2        |指示 Teams 应用可以安装在用户的个人范围内，并有权访问该用户的数据。|