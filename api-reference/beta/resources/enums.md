---
title: 枚举值
description: Microsoft Graph枚举值
doc_type: enumPageType
ms.localizationpriority: medium
ms.prod: non-product-specific
author: MSGraphDocsvTeam
ms.openlocfilehash: af7a53c81bc1adf8a4e5571c69b1e63e457254b6
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755423"
---
# <a name="enum-values"></a>枚举值

命名空间：microsoft.graph

### <a name="bookingsavailabilitystatus-values"></a>bookingsAvailabilityStatus 值

|成员|
|:-----|
|可用|
|忙|
|slotsAvailable|
|outOfOffice|
|unknownFutureValue|

### <a name="accesspackagecustomextensionhandlerstatus-values"></a>accessPackageCustomExtensionHandlerStatus 值 

|成员|
|:---|
|requestSent|
|requestReceived|
|unknownFutureValue|

### <a name="accesspackagecustomextensionstage-values"></a>accessPackageCustomExtensionStage 值 

|成员|
|:---|
|assignmentRequestCreated|
|assignmentRequestApproved|
|assignmentRequestGranted|
|assignmentRequestRemoved|
|assignmentFourteenDaysBeforeExpiration|
|assignmentOneDayBeforeExpiration|
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


### <a name="accessreviewhistorystatus-values"></a>accessReviewHistoryStatus 值

|成员|
|:---|
|done|
|inprogress|
|error|
|要求|
|unknownFutureValue|

### <a name="crosstenantaccesspolicytargetconfigurationaccesstype-values"></a>crossTenantAccessPolicyTargetConfigurationAccessType 值

|成员|
|:---|
|允许|
|封锁|
|unknownFutureValue|

### <a name="crosstenantaccesspolicytargettype-values"></a>crossTenantAccessPolicyTargetType 值

|成员|
|:---|
|用户|
|组|

### <a name="accesspackagefilterbycurrentuseroptions-values"></a>accessPackageFilterByCurrentUserOptions 值

|成员|
|:---|
|allowedRequestor|
|unknownFutureValue|

### <a name="usersigninrecommendationscope-values"></a>userSignInRecommendationScope 值 

|成员|
|:---|
|租户|
|应用程序|

### <a name="incomingtokentype-values"></a>incomingTokenType 值 

|成员|
|:---|
|无|
|primaryRefreshToken|
|saml11|
|saml20|
|unknownFutureValue|

### <a name="protocoltype-values"></a>protocolType 值 

|成员|
|:---|
|无|
|oAuth2|
|ropc|
|wsFederation|
|saml20|
|deviceCode|
|unknownFutureValue|

### <a name="accessreviewinstancedecisionitemfilterbycurrentuseroptions-values"></a>accessReviewInstanceDecisionItemFilterByCurrentUserOptions 值 

|成员|
|:---|
|评论家|
|unknownFutureValue|

### <a name="accessreviewstagefilterbycurrentuseroptions-values"></a>accessReviewStageFilterByCurrentUserOptions 值 

|成员|
|:---|
|评论家|
|unknownFutureValue|

### <a name="continuousaccessevaluationmode-values"></a>continuousAccessEvaluationMode 值 

|成员|
|:---|
|strictEnforcement|
|禁用|
|unknownFutureValue|

### <a name="multifactorauthconfiguration-values"></a>multiFactorAuthConfiguration 值

| 成员             | 值 | 说明 |
|:-------------------|:------| :------|
| notRequired        | 0     | 用户无需进行多重身份验证即可完成设备注册。|
| 必需           | 1     | 用户必须进行多重身份验证才能完成设备注册。|
| unknownFutureValue | 2     | 可变枚举 sentinel 值。 请勿使用。|

### <a name="policyscope-values"></a>policyScope 值

| 成员             | 值 | 说明 |
|:-------------------|:------| :------|
| 无               | 0     | 该策略不适用于组织中的任何用户或组。 |
| 所有                | 1     | 该策略适用于组织中的所有用户和组。 默认值。 |
| 选择           | 2     | 该策略适用于组织中的特定用户或组。 |
| unknownFutureValue | 3     | 可变枚举 sentinel 值。 请勿使用。 |

### <a name="appcredentialrestrictiontype-values"></a>appCredentialRestrictionType 值

| 成员                 |
| :--------------------- |
| passwordAddition       |
| passwordLifetime       |
| symmetricKeyAddition   |
| symmetricKeyLifetime   |
| customPasswordAddition |
| unknownFutureValue     |

### <a name="appkeycredentialrestrictiontype-values"></a>appKeyCredentialRestrictionType 值

|成员|
|:-----|
|asymmetricKeyLifetime|
|unknownFutureValue|

### <a name="synchronizationsecret-values"></a>synchronizationSecret 值

|成员|
|:----|
|无|
|UserName|
|Password|
|SecretToken|
|AppKey|
|BaseAddress|
|ClientIdentifier|
|ClientSecret|
|SingleSignOnType|
|沙 箱|
|URL|
|Domain|
|ConsumerKey|
|ConsumerSecret|
|TokenKey|
|TokenExpiration|
|Oauth2AccessToken|
|Oauth2AccessTokenCreationTime|
|Oauth2RefreshToken|
|SyncAll|
|InstanceName|
|Oauth2ClientId|
|Oauth2ClientSecret|
|CompanyId|
|UpdateKeyOnSoftDelete|
|SynchronizationSchedule|
|SystemOfRecord|
|SandboxName|
|EnforceDomain|
|SyncNotificationSettings|
|SkipOutOfScopeDeletions|
|Oauth2AuthorizationCode|
|Oauth2RedirectUri|
|ApplicationTemplateIdentifier|
|服务器|
|PerformInboundEntitlementGrants|
|HardDeletesEnabled|
|SyncAgentCompatibilityKey|
|SyncAgentADContainer|
|ValidateDomain|
|TestReferences|

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
|已创建|
|更新|
|deleted|


### <a name="countrylookupmethodtype-values"></a>countryLookupMethodType 值

|成员|
|:---|
|clientIpAddress|
|authenticatorAppGps|

### <a name="approvalstate-values"></a>approvalState 值

|成员|
|:---|
|等待|
|批准|
|denied|
|中止|
|取消|

### <a name="rolesummarystatus-values"></a>roleSummaryStatus 值

|成员|
|:---|
|还行|
|坏|

### <a name="datapolicyoperationstatus-values"></a>dataPolicyOperationStatus 值

|成员|
|:---|
|notStarted|
|运行|
|complete|
|失败|
|unknownFutureValue|

### <a name="conditionalaccessclientapp-values"></a>conditionalAccessClientApp 值

|成员|
|:---|
|所有|
|浏览器|
|mobileAppsAndDesktopClients|
|exchangeActiveSync|
|easSupported|
|其他|

### <a name="consentrequestfilterbycurrentuseroptions-values"></a>consentRequestFilterByCurrentUserOptions 值

|成员|
|:---|
|评论家|
|unknownFutureValue|

### <a name="attributetype-values"></a>attributeType 值

|成员|
|:---|
|String|
|整数|
|参考|
|Binary|
|Boolean|
|日期时间|

### <a name="mutability-values"></a>可变性值

|成员|
|:---|
|读写|
|ReadOnly|
|变|
|WriteOnly|

### <a name="directorydefinitiondiscoverabilities-values"></a>directoryDefinitionDiscoverabilities 值

|成员|
|:---|
|无|
|AttributeNames|
|AttributeDataTypes|
|AttributeReadOnly|
|ReferenceAttributes|
|UnknownFutureValue|

### <a name="connectorgroupregion-values"></a>connectorGroupRegion 值

|成员|
|:---|
|南|
|欧元|
|澳大利亚|
|亚洲|
|工业|
|unknownFutureValue|

### <a name="connectorgrouptype-values"></a>connectorGroupType 值

|成员|
|:---|
|applicationProxy|

### <a name="onpremisespublishingtype-values"></a>onPremisesPublishingType 值

|成员|
|:---|
|applicationProxy|
|exchangeOnline|
|身份验证|
|供应|
|intunePfx|
|oflineDomainJoin|
|unknownFutureValue|

### <a name="agentstatus-values"></a>agentStatus 值

|成员|
|:---|
|积极|
|无效|

### <a name="connectorstatus-values"></a>connectorStatus 值

|成员|
|:---|
|积极|
|无效|

### <a name="calltype-values"></a>callType 值

|成员|
|:---|
|unknown|
|groupCall|
|peerToPeer|
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

### <a name="routingpolicy-values"></a>routingPolicy 值

|成员|
|:---|
|无|
|noMissedCall|
|disableForwardingExceptPhone|
|disableForwarding|
|preferSkypeForBusiness|
|unknownFutureValue|

### <a name="meetingcapabilities-values"></a>meetingCapabilities 值

|成员|
|:---|
|questionAndAnswer|
|unknownFutureValue|

### <a name="onlinemeetingrole-values"></a>onlineMeetingRole 值

|成员|
|:---|
|attendee|
|主持人|
|生产者|
|unknownFutureValue|

### <a name="autoadmitteduserstype-values"></a>autoAdmittedUsersType 值

|成员|
|:---|
|everyoneInCompany|
|每个人 都|

### <a name="mediastate-values"></a>mediaState 值

|成员|
|:---|
|积极|
|无效|
|unknownFutureValue|

### <a name="calldirection-values"></a>callDirection 值

|成员|
|:---|
|传入|
|外向|

### <a name="modality-values"></a>模式值

|成员|
|:---|
|audio|
|video|
|videoBasedScreenSharing|
|data|
|screenSharing|
|unknownFutureValue|

### <a name="kerberossignonmappingattributetype-values"></a>kerberosSignOnMappingAttributeType 值

|成员|
|:---|
|userPrincipalName|
|onPremisesUserPrincipalName|
|userPrincipalUsername|
|onPremisesUserPrincipalUsername|
|onPremisesSAMAccountName|

### <a name="externalauthenticationtype-values"></a>externalAuthenticationType 值

|成员|
|:---|
|passthru|
|aadPreAuthentication|

### <a name="recipientscopetype-values"></a>recipientScopeType 值
|成员|
|:---|
|无|
|内部|
|外部|
|externalPartner|
|externalNonPartner|

### <a name="appliedconditionalaccesspolicyresult-values"></a>appliedConditionalAccessPolicyResult 值

|成员|
|:---|
|success|
|失败|
|notApplied|
|notEnabled|
|unknown|
|unknownFutureValue|
|reportOnlySuccess|
|reportOnlyFailure|
|reportOnlyNotApplied|
|reportOnlyInterrupted|


### <a name="microsoftauthenticatorauthenticationmode-values"></a>microsoftAuthenticatorAuthenticationMode 值



|成员|
|:---|
|任意|
|推|
|deviceBasedPush|


### <a name="authenticationmethodfeature-values"></a>authenticationMethodFeature 值

|成员|
|:---|
|ssprRegistered|
|ssprEnabled|
|ssprCapable|
|passwordlessCapable|
|mfaCapable|


### <a name="authmethodstype-values"></a>authMethodsType 值

|成员|
|:---|
|电子邮件|
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

|成员|
|:---|
|无|
|自由|
|基本|
|premiumP1|
|premiumP2|
|unknownFutureValue|

### <a name="conditionalaccessconditions-values"></a>conditionalAccessConditions 值

|成员|
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
|客户|
|ipAddressSeenByAzureAD|
|ipAddressSeenByResourceProvider|
|unknownFutureValue|
|servicePrincipals|
|servicePrincipalRisk|

### <a name="conditionalaccessstatus-values"></a>conditionalAccessStatus 值

|成员|
|:---|
|success|
|失败|
|notApplied|
|unknownFutureValue|

### <a name="featuretype-values"></a>featureType 值

|成员|
|:---|
|注册|
|重置|
|unknownFutureValue|

### <a name="grouptype-values"></a>groupType 值

|成员|
|:---|
|unifiedGroups|
|azureAD|
|unknownFutureValue|

### <a name="includeduserroles-values"></a>includedUserRoles 值

|成员|
|:---|
|所有|
|privilegedAdmin|
|管理|
|用户|
|unknownFutureValue|

### <a name="includedusertypes-values"></a>includedUserTypes 值

|成员|
|:---|
|所有|
|成员|
|客人|
|unknownFutureValue|

### <a name="initiatortype-values"></a>initiatorType 值

|成员|
|:---|
|用户|
|应用|
|system|
|unknownFutureValue|

### <a name="migrationstatus-values"></a>migrationStatus 值

|成员|
|:---|
|准备|
|needsReview|
|additionalStepsRequired|
|unknownFutureValue|

### <a name="networktype-values"></a>networkType 值

|成员|
|:---|
|网|
|extranet|
|namedNetwork|
|信任|
|unknownFutureValue|

### <a name="operationresult-values"></a>operationResult 值

|成员|
|:---|
|success|
|失败|
|timeout|
|unknownFutureValue|

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
|fido|
|appPassword|
|unknownFutureValue|

### <a name="registrationstatustype-values"></a>registrationStatusType 值

|成员|
|:---|
|注册|
|enabled|
|能够|
|mfaRegistered|
|unknownFutureValue|


### <a name="signinidentifiertype-values"></a>signInIdentifierType 值 

|成员|
|:---|
|userPrincipalName|
|phoneNumber|
|proxyAddress|
|qrCode|
|onPremisesUserPrincipalName|
|unknownFutureValue|


### <a name="signinusertype-values"></a>signInUserType 值 

|成员|
|:---|
|成员|
|客人|
|unknownFutureValue|

### <a name="requirementprovider-values"></a>requirementProvider 值 


|成员|
|:---|
|用户|
|请求|
|servicePrincipal|
|v1ConditionalAccess|
|multiConditionalAccess|
|tenantSessionRiskPolicy|
|accountCompromisePolicies|
|v1ConditionalAccessDependency|
|v1ConditionalAccessPolicyIdRequested|
|mfaRegistrationRequiredByIdentityProtectionPolicy|
|baselineProtection|
|mfaRegistrationRequiredByBaselineProtection|
|mfaRegistrationRequiredByMultiConditionalAccess|
|enforcedForCspAdmins|
|securityDefaults|
|mfaRegistrationRequiredBySecurityDefaults|
|proofUpCodeRequest|
|crossTenantOutboundRule|
|gpsLocationCondition|
|riskBasedPolicy|
|unknownFutureValue|


### <a name="riskdetail-values"></a>riskDetail 值

|成员|
|:---|
|无|
|内部|
|外部|
|externalPartner|
|externalNonPartner|
|adminGeneratedTemporaryPassword|
|userPerformedSecuredPasswordChange|
|userPerformedSecuredPasswordReset|
|adminConfirmedSigninSafe|
|aiConfirmedSigninSafe|
|userPassedMFADrivenByRiskBasedPolicy|
|adminDismissedAllRiskForUser|
|adminConfirmedSigninCompromised|
|hidden|
|adminConfirmedUserCompromised|
|unknownFutureValue|
|adminConfirmedServicePrincipalCompromised|
|adminDismissedAllRiskForServicePrincipal|


<!-- maintenance comment: Do not delete enum delcaration for riskEventType until all properties of this type are marked as deleted. Dec 28, 2021: Pending eventTypes (in riskUserActivity) and riskType (in riskDetection)-->
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

### <a name="usageauthmethod-values"></a>usageAuthMethod 值

|成员|
|:---|
|电子邮件|
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

|成员|
|:---|
|正常|
|弱|
|unknown|

### <a name="authenticationcontextdetail-values"></a>authenticationContextDetail 值

|成员|
|:---|
|必需|
|previouslySatisfied|
|notApplicable|
|unknownFutureValue|

### <a name="educationaddedstudentaction-values"></a>educationAddedStudentAction 值

|成员|
|:---|
|无|
|assignIfOpen|
|unknownFutureValue|

### <a name="educationaddtocalendaroptions-values"></a>educationAddToCalendarOptions 值
|成员|
|:---|
|无|
|studentsAndPublisher|
|studentsAndTeamOwners|
|unknownFutureValue|
|studentsOnly|

### <a name="educationassignmentstatus-values"></a>educationAssignmentStatus 值
|成员|
|:---|
|草案|
|发表|
|分配|
|unknownFutureValue|

### <a name="educationsubmissionstatus-values"></a>educationSubmissionStatus 值
|成员|
|:---|
|工作|
|提交|
|释放|
|返回|
|unknownFutureValue|
|分配|

### <a name="externalemailotpstate-values"></a>externalEmailOtpState 值

|成员|
|:---|
|默认|
|enabled|
|禁用|
|unknownFutureValue|

### <a name="expirationrequirement-values"></a>expirationRequirement 值

|成员|
|:---|
|rememberMultifactorAuthenticationOnTrustedDevices|
|tenantTokenLifetimePolicy|
|audienceTokenLifetimePolicy|
|signInFrequencyPeriodicReauthentication|
|ngcMfa|
|signInFrequencyEveryTime|
|unknownFutureValue|


### <a name="replyrestriction-values"></a>replyRestriction 值

| 成员
|:--------------
| 每个人 都
| authorAndModerators
| unknownFutureValue

### <a name="usernewmessagerestriction-values"></a>userNewMessageRestriction 值

| 成员
|:--------------
|每个人 都
|everyoneExceptGuests
|版主
|unknownFutureValue

### <a name="volumetype-values"></a>volumeType 值

|成员|
|:---|
|operatingSystemVolume|
|fixedDataVolume|
|removableDataVolume|
|unknownFutureValue|

### <a name="allowedaudiences-values"></a>allowedAudiences 值

|成员|
|:---|
|me|
|家庭|
|contacts|
|groupMembers|
|组织|
|federatedOrganizations|
|每个人 都|
|unknownFutureValue|

### <a name="attestationlevel-values"></a>attestationLevel 值

|成员|
|:---|
|证明|
|notAttested|
|unknownFutureValue|

### <a name="emailtype-values"></a>emailType 值

|成员|
|:---|
|unknown|
|工时|
|personal|
|主要|
|其他|

### <a name="authenticationmethodsigninstate-values"></a>authenticationMethodSignInState 值

|成员|
|:---|
|notSupported|
|notAllowedByPolicy|
|notEnabled|
|phoneNumberNotUnique|
|准备|
|notConfigured|
|unknownFutureValue|

### <a name="authenticationphonetype-values"></a>authenticationPhoneType 值

|成员|
|:---|
|mobile|
|alternateMobile|
|办公室|
|unknownFutureValue|


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

### <a name="fido2restrictionenforcementtype-values"></a>fido2RestrictionEnforcementType 值

|成员|
|:---|
|允许|
|块|
|unknownFutureValue|

### <a name="x509certificateauthenticationmode-values"></a>x509CertificateAuthenticationMode 值
|成员|
|:---|
|x509CertificateSingleFactor|
|x509CertificateMultiFactor|
|unknownFutureValue|

### <a name="x509certificateruletype-values"></a>x509CertificateRuleType 值
|成员|
|:---|
|issuerSubject|
|policyOID|
|unknownFutureValue|

### <a name="anniversarytype-values"></a>anniversaryType 值

|成员|
|:---|
|birthday|
|婚礼|
|unknownFutureValue|

### <a name="skillproficiencylevel-values"></a>skillProficiencyLevel 值

|成员|
|:---|
|基本|
|limitedWorking|
|generalProfessional|
|advancedProfessional|
|专家|
|unknownFutureValue|

### <a name="languageproficiencylevel-values"></a>languageProficiencyLevel 值

|成员|
|:---|
|基本|
|会话|
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
|助理|
|dotLineManager|
|alternateContact|
|朋友|
|配偶|
|兄弟|
|Child|
|父级|
|赞助|
|emergencyContact|
|其他|
|unknownFutureValue|

### <a name="attachmenttype-values"></a>attachmentType 值

| 成员
|:--------------
| file
| 项
| 参考

### <a name="analyticsactivitytype-values"></a>analyticsActivityType 值

| 成员
|:--------------
| 通话
| 聊天
| 电子邮件
| 焦点
| 会议

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
|消息|
|driveItem|
|externalItem|
|网站|
|list|
|listItem|
|drive|
|unknownFutureValue|

### <a name="searchalterationtype-values"></a>searchAlterationType 值

| 成员 |
|:---------------|
|修改|
|建议|

### <a name="bucketaggregationsortproperty-values"></a>bucketAggregationSortProperty 值

|成员|
|:---|
|count|
|keyAsString|
|keyAsNumber|

### <a name="contactrelationship-values"></a>contactRelationship 值

| 成员             | 值 | 说明                              |
| :----------------- | :---- | :--------------------------------------- |
| 父级             | 0     | 用户的父级。                       |
| 相对           | 1     | 用户的相对。                     |
| 助手               | 2     | 用户的助手。                         |
| 医生             | 3     | 用户的医生。                       |
| 监护人           | 4     | 用户的监护人。                     |
| Child              | 5     | 用户的子级。                        |
| 其他              | 6      | 与用户的未指定关系。 |
| unknownFutureValue | 7      | 用于将来兼容性的标记值。   |

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

### <a name="timecardstate-values"></a>timeCardState 值

|成员|
|:---|
|clockedIn|
|onBreak|
|clockedOut|
|unknownFutureValue|

### <a name="schedulechangestate-values"></a>scheduleChangeState 值

| 成员
|:----------------------------
|等待
|批准
|拒绝
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
|timeCard|
|timeOffReason|
|timeOff|
|timeOffRequest|

### <a name="confirmedby-values"></a>confirmedBy 值

| 成员
|:-----------------
| 无|
| 用户|
| manager|
| unknownFutureValue|

### <a name="timezonestandard-values"></a>timeZoneStandard 值

| 成员
|:-----------------
| windows
| Iana


### <a name="freebusystatus-values"></a>freeBusyStatus 值

| 成员           | 值 |
| :--------------- | :---- |
| 自由             | 0     |
| 初步        | 1     |
| 忙             | 2     |
| oof              | 3     |
| workingElsewhere | 4     |
| unknown          | -1    |


### <a name="physicaladdresstype-values"></a>physicalAddressType 值

| 成员
|:-------------------------
| unknown
| 家
| 业务
| 其他


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
| 所有


### <a name="automaticrepliesstatus-values"></a>automaticRepliesStatus 值

| 成员
|:-------------------------
| 禁用
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
| lightYellow | 4     |
| lightTeal   | 5     |
| lightPink   | 6      |
| lightBrown  | 7      |
| lightRed    | 8      |
| maxColor    | 9      |


### <a name="educationsynchronizationprofilestate-values"></a>educationSynchronizationProfileState 值

| 成员             | 值 |
| :----------------- | :---- |
| 删除           | 2     |
| deletionFailed     | 3     |
| provisioningFailed | 5     |
| 已设置        | 6      |
| 供应       | 7      |
| unknownFutureValue | 8      |


### <a name="educationsynchronizationstatus-values"></a>educationSynchronizationStatus 值

| 成员             |
| :----------------- |
| 暂停             |
| inProgress         |
| success            |
| error              |
| validationError    |
| 隔离        |
| unknownFutureValue |
| 提取         |
| 验证         |

### <a name="educationexternalsource-values"></a>educationExternalSource 值

| 成员
|:-------------------------
| 姐姐
| Lms
| 手动
| unknownFutureValue

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
| 成员
|:---------------------
| student
| teacher
| 教师


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

| 成员      | 值 |
| :---------- | :---- |
| 所有者       | 0     |
| 参与者 | 1     |
| 读者      | 2     |
| 无        | -1    |


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

| 成员   | 值 |
| :------- | :---- |
| 无     | -1    |
| preset0  | 0     |
| preset1  | 1     |
| preset2  | 2     |
| preset3  | 3     |
| preset4  | 4     |
| preset5  | 5     |
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
| preset16 | 16    |
| preset17 | 17     |
| preset18 | 18     |
| preset19 | 19    |
| preset20 | 20    |
| preset21 |  21    |
| preset22 | 22    |
| preset23 | 23    |
| preset24 | 24    |

### <a name="alertfeedback-values"></a>alertFeedback 值

有关分析人员提供的警报的可能反馈值。

| 成员         | 值 | 说明               |
| :------------- | :---- | :------------------------ |
| unknown        | 0     | 未知。                  |
| truePositive   | 1     | 警报为 true-positive。   |
| falsePositive  | 2     | 警报为误报。  |
| benignPositive | 3     | 警报是良性正的。 |

### <a name="filehashtype-values"></a>fileHashType 值

| 成员              | 值 | 说明                    |
| :------------------ | :---- | :----------------------------- |
| unknown             | 0     | 未知类型。                  |
| sha1                | 1     | SHA1 哈希类型。                |
| sha256              | 2     | SHA256 哈希类型。              |
| md5                 | 3     | MD5 哈希类型。                 |
| authenticodeHash256 | 4     | AuthenticodeHash256 哈希类型。 |
| lsHash              | 5     | LsHash 哈希类型。              |
| ctph                | 6      | CTPH 哈希类型。                |
| peSha1              | 7      | PESHA1 哈希类型。              |
| peSha256            | 8      | PESHA256 哈希类型。            |

### <a name="connectiondirection-values"></a>connectionDirection 值

| 成员   | 值 | 说明          |
| :------- | :---- | :------------------- |
| unknown  | 0     | 未知连接。  |
| 入境  | 1     | 入站连接。  |
| 出境 | 2     | 出站连接。 |

### <a name="connectionstatus-values"></a>connectionStatus 值

| 成员    | 值 | 说明                |
| :-------- | :---- | :------------------------- |
| unknown   | 0     | 未知的连接状态。 |
| 企图 | 1     | 尝试连接。      |
| 成功 | 2     | 连接成功。      |
| 封锁   | 3     | 连接被阻止。        |
| 失败    | 4     | 连接失败。         |

### <a name="processintegritylevel-values"></a>processIntegrityLevel 值

| 成员    | 值 | 说明                   |
| :-------- | :---- | :---------------------------- |
| unknown   | 0     | 未知。                      |
| 可信 | 10     | 完整性级别不受信任。 |
| 低       | 20    | 完整性级别较低。       |
| 中等    | 30    | 完整性级别为中等。    |
| 高      | 40    | 完整性级别较高。      |
| system    | 50    | 完整性级别为 System。    |

### <a name="registryhive-values"></a>registryHive 值

注册 [表 Hives](/windows/desktop/sysinfo/registry-hives) 定义的注册表 hiv 的枚举。

| 成员                  | 值 | 说明                       |
| :---------------------- | :---- | :-------------------------------- |
| unknown                 | 0     | 未知 hive。                     |
| currentConfig           | 1     | HKEY_CURRENT_CONFIG hive。         |
| currentUser             | 2     | HKEY_CURRENT_USER hive。           |
| localMachineSam         | 3     | HKEY_LOCAL_MACHINE\SAM hive。      |
| localMachineSamSoftware | 4     | HKEY_LOCAL_MACHINE\Software hive。 |
| localMachineSystem      | 5     | HKEY_LOCAL_MACHINE\System hive。   |
| usersDefault            | 6      | \\HKEY_USERS。DEFAULT hive。        |

### <a name="registryoperation-values"></a>registryOperation 值

更改注册表项名称和/或值的操作。

| 成员  | 值 | 说明                  |
| :------ | :---- | :--------------------------- |
| unknown | 0     | 未知的注册表值类型。 |
| create  | 1     | 创建注册表。             |
| 修改  | 2     | 修改注册表。             |
| delete  | 3     | 删除注册表。             |

### <a name="registryvaluetype-values"></a>registryValueType 值

注册表值类型定义的注册 [表值类型的](/windows/desktop/sysinfo/registry-value-types)枚举。

| 成员            | 值 | 说明                                  |
| :---------------- | :---- | :------------------------------------------- |
| unknown           | 0     | 未知的注册表值类型。                 |
| 二 进 制            | 1     | REG_BINARY注册表值类型。              |
| Dword             | 2     | REG_DWORD注册表值类型。               |
| dwordLittleEndian | 3     | REG_DWORD_LITTLE_ENDIAN注册表值类型。 |
| dwordBigEndian    | 4     | REG_DWORD_BIG_ENDIAN注册表值类型。    |
| expandSz          | 5     | REG_EXPAND_SZ注册表值类型。           |
| link              | 6      | REG_LINK注册表值类型。                |
| multiSz           | 7      | REG_MULTI_SZ注册表值类型。            |
| 无              | 8      | REG_NONE注册表值类型。                |
| qword             | 9      | REG_QWORD注册表值类型。               |
| qwordlittleEndian | 10     | REG_QWORD_LITTLE_ENDIAN注册表值类型。 |
| 深圳                | 11    | REG_SZ注册表值类型。                  |

### <a name="alertseverity-values"></a>alertSeverity 值

警报严重性的枚举。

| 成员        | 值 | 说明                       |
| :------------ | :---- | :-------------------------------- |
| unknown       | 0     | 严重性未知。              |
| 信息 | 1     | 严重性仅适用于信息。 |
| 低           | 2     | 严重性较低。                  |
| 中等        | 3     | 严重性是中等的。               |
| 高          | 4     | 严重性很高。                 |

### <a name="alertstatus-values"></a>alertStatus 值

警报生命周期状态的可能值 (阶段) 。

| 成员     | 值 | 说明           |
| :--------- | :---- | :-------------------- |
| unknown    | 0     | 未知状态。       |
| newAlert   | 10     | 警报是新的。         |
| inProgress | 20    | 警报正在进行中。 |
| 已解决   | 30    | 警报已解决。    |

### <a name="emailrole-values"></a>emailRole 值

电子邮件角色的可能值。

| 成员    | 值 | 说明             |
| :-------- | :---- | :---------------------- |
| unknown   | 0     | 未知角色。           |
| sender    | 1     | 电子邮件的发件人。    |
| recipient | 2     | 电子邮件收件人。 |

### <a name="logontype-values"></a>logonType 值

用户登录方法的可能值。

| 成员            | 值 | 说明                  |
| :---------------- | :---- | :--------------------------- |
| unknown           | -1    | 未知。                     |
| 互动       | 0     | 登录是交互式的。        |
| remoteInteractive | 1     | 登录是远程交互式登录。 |
| 网络           | 2     | 登录是网络。            |
| batch             | 3     | 登录是批处理的。              |
| 服务           | 4     | 登录是服务。            |

### <a name="useraccountsecuritytype-values"></a>userAccountSecurityType 值

根据Windows定义，用户帐户类型的可能值 (组成员身份) 。

| 成员        | 值 | 说明                     |
| :------------ | :---- | :------------------------------ |
| unknown       | -1    | 未知。                        |
| 标准      | 0     | 标准用户组的成员。 |
| 权力         | 1     | Power Users 组的成员。    |
| 管理员 | 2     | 管理员组的成员。 |

### <a name="chatmessagepolicyviolationdlpactiontype-values"></a>chatMessagePolicyViolationDlpActionType 值

| 值 |
|:-----------------|
| 无 |
| NotifySender |
| BlockAccess |
| BlockAccessExternal |

### <a name="scopeoperatormultivaluedcomparisontype-values"></a>scopeOperatorMultiValuedComparisonType 值

|成员|
|:---|
|所有|
|任意|

### <a name="risklevel-values"></a>riskLevel 值

|成员|
|:---|
|低|
|中等|
|高|
|hidden|
|无|
|unknownFutureValue|

### <a name="riskstate-values"></a>riskState 值

|成员|
|:---|
|无|
|confirmedSafe|
|修正|
|解雇|
|atRisk|
|confirmedCompromised|
|unknownFutureValue|

### <a name="advancedconfigstate-values"></a>advancedConfigState 值

|成员|
|:---|
|默认|
|enabled|
|禁用|
|unknownFutureValue|

### <a name="referenceattachmentpermission-values"></a>referenceAttachmentPermission 值

|成员|
|:---|
|其他|
|view|
|edit|
|anonymousView|
|anonymousEdit|
|organizationView|
|organizationEdit|

### <a name="referenceattachmentprovider-values"></a>referenceAttachmentProvider 值

|成员|
|:---|
|其他|
|oneDriveBusiness|
|oneDriveConsumer|
|Dropbox|

### <a name="networktype-values"></a>networkType 值

|成员|
|:---|
|网|
|extranet|
|namedNetwork|
|信任|
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
|总是|
|objectAddOnly|
|multiValueAddOnly|
|restId|

### <a name="objectflowtypes-values"></a>objectFlowTypes 值

| 成员 | 值 |
| :----- | :---- |
| 无   | 0     |
| 添加    | 1     |
| 更新 | 2     |
| 删除 | 4     |

### <a name="chatmessagetype-values"></a>chatMessageType 值

|成员|
|:---|
|消息|
|chatEvent |
|打字 |
|unknownFutureValue|
|systemEventMessage|

### <a name="chatmessageimportance-values"></a>chatMessageImportance 值

|成员|
|:---|
|正常|
|高|
|紧急|

### <a name="channelmembershiptype-values"></a>channelMembershipType 值

| 成员             |
| :----------------- |
| 标准           |
| 私人            |
| unknownFutureValue |
| shared             |

### <a name="stagedfeaturename-values"></a>stagedFeatureName 值

| 成员                    | 说明                   |
| :------------------------ | :---------------------------- |
| passthroughAuthentication | 直通身份验证    |
| seamlessSso               | 无缝单一登录       |
| passwordHashSync          | 密码哈希同步 |
| emailAsAlternateId        | 电子邮件作为备用 ID      |
| unknownFutureValue        | Sentinel 成员             |

### <a name="tokenissuertype-values"></a>tokenIssuerType 值

|成员|
|:---|
|AzureAD|
|ADFederationServices|
|unknownFutureValue|
|AzureADBackupAuth|
|ADFederationServicesMFAAdapter|
|NPSExtension|


### <a name="riskdetectiontimingtype-values"></a>riskDetectionTimingType 值

|成员|
|:---|
|notDefined|
|实时|
|nearRealtime|
|离线|
|unknownFutureValue|

### <a name="activitytype-values"></a>activityType 值

|成员|
|:---|
|signin|
|用户|
|unknownFutureValue|
|servicePrincipal|

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

### <a name="entitytype-values"></a>entityType 值

| 成员       |
|:--------------|
|event|
|消息|
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
|自 定义|

### <a name="contentformat-values"></a>contentFormat 值

| 成员  | 值 | 说明                          |
| :------ | :---- | :----------------------------------- |
| 默认 | 0     | 内容是文件或非电子邮件类型。 |
| 电子邮件   | 1     | 内容是一封电子邮件。                 |

### <a name="contentstate-values"></a>contentState 值

| 成员 | 值 | 说明                                                                      |
| :----- | :---- | :------------------------------------------------------------------------------- |
| 休息   | 0     | 数据处于静态;例如，共享中的文件。                                 |
| 运动 | 1     | 数据正在移动。 传输中网络设备截获的文件。         |
| 使用    | 2     | 数据正在使用中。 文件在客户端应用程序（如Microsoft Office）中打开。 |

### <a name="assignmentmethod-values"></a>assignmentMethod 值

| 成员     | 值 | 说明                                                                                                                      |
| :--------- | :---- | :------------------------------------------------------------------------------------------------------------------------------- |
| 标准   | 0     | 标签由服务或策略条件设置。                                                                              |
| 特权 | 1     | 该标签由用户显式设置。                                                                                          |
| 自动       | 2     | 允许重写任何现有标签。 降级时需要理由。 在 `standard` 元数据中生成赋值方法。 |

### <a name="actionsource-values"></a>actionSource 值

| 成员        | 值 | 说明                                                  |
| :------------ | :---- | :----------------------------------------------------------- |
| 手动        | 0     | 用户手动选择了标签。                          |
| 自动     | 1     | 标签是由于策略条件而选择的。       |
| 建议   | 2     | 选择应用建议的标签。                    |
| policyDefault | 3     | 用户未执行任何操作，并且应用了策略默认标签。 |
| 强制性     | 4     | 用户在被迫选择后选择了标签。         |

### <a name="contentalignment-values"></a>contentAlignment 值

| 成员 | 值 | 说明                         |
| :----- | :---- | :---------------------------------- |
| left   | 0     | 将内容标记对齐到左侧。  |
| 对  | 1     | 将内容标记对齐到右侧。 |
| 中心 | 2     | 中心内容标记。             |

### <a name="watermarklayout-values"></a>watermarkLayout 值

| 成员     | 值 | 说明                 |
| :--------- | :---- | :-------------------------- |
| 水平 | 0     | 使用水平水印。 |
| 对角   | 1     | 使用对角线水印。   |

### <a name="conditionalaccesspolicystate-values"></a>conditionalAccessPolicyState 值

|成员|
|:---|
|enabled|
|禁用|
|enabledForReportingButNotEnforced|

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

### <a name="conditionalaccessrule-values"></a>conditionalAccessRule 值 

|成员|
|:---|
|allApps|
|firstPartyApps|
|office365|
|appId|
|Acr|
|appFilter|
|allUsers|
|客人|
|groupId|
|roleId|
|userId|
|allDevicePlatforms|
|devicePlatform|
|allLocations|
|insideCorpnet|
|allTrustedLocations|
|locationId|
|allDevices|
|deviceFilter|
|deviceState|
|unknownFutureValue|
|deviceFilterIncludeRuleNotMatched|
|allDeviceStates|

### <a name="signinaccesstype-values"></a>signInAccessType 值 

|成员|
|:---|
|无|
|b2bCollaboration|
|b2bDirectConnect|
|microsoftSupport|
|serviceProvider|
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

### <a name="conditionalaccessdeviceplatform-values"></a>conditionalAccessDevicePlatform 值

| 成员       |
|:--------------|
|Android|
|iOS|
|windows|
|windowsPhone|
|macOS|
|所有|
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
| 块   | 1     | 应阻止威胁。     |
| 疏通 | 2     | 不应阻止威胁。 |

### <a name="threatcategory-values"></a>threatCategory 值

| 成员             | 值 | 说明        |
|:-------------------|:------|:-------------------|
| 垃圾邮件 (spam)               | 1     | 垃圾邮件威胁。       |
| 仿冒           | 2     | 网络钓鱼威胁。   |
| 恶意软件 (malware)            | 3     | 恶意软件威胁。    |
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
| autoPurgeToJunk       | 10     | TimeTravel 将消息移动到垃圾邮件。    |
| autoPurgeToDeleted    | 11    | 要删除的 TimeTravel 移动消息。 |
| 出境              | 12     | 出站邮件。                      |
| notJunk               | 13    | 允许由于不是垃圾。              |
| 垃圾                  | 14     | 因垃圾而被阻止。                |
| unknownFutureValue    | 15     | 一个 sentinel 成员。                  |

### <a name="threatassessmentrequestpivotproperty-values"></a>threatAssessmentRequestPivotProperty 值

| 成员                       | 值 | 说明                                                            |
|:-----------------------------|:------|:-----------------------------------------------------------------------|
| threatCategory               | 1     | 按 `threatCategory` a0/a0> 聚合威胁评估请求。               |
| mailDestinationRoutingReason | 2     | 按 `mailDestinationRoutingReason` a0/a0> 聚合威胁评估请求。 |

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

### <a name="openidconnectresponsemode-values"></a>openIdConnectResponseMode 值

| 成员
|:----------------------
| form_post
| 查询
| unknownFutureValue

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
|选择 | choice 列 |
|multichoice | multichoice 列。 |
|number | 数字列。 |
|货币 | 货币列。 |
|dateTime | dateTime 列。 |
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
|unknownFutureValue | unknownFuturevalue |

### <a name="connectedorganizationstate-values"></a>connectedOrganizationState 值

| 成员                | 值 | 说明                                                                                                                                                                                                        |
|:----------------------| :-----|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 配置            | 0     | 具有此状态值的已连接组织包含在具有请求者范围类型的 `AllConfiguredConnectedOrganizationSubjects`分配策略中。                                                          |
| 提出              | 1     | 系统自动创建的已连接组织具有此状态值。 它们不包括在具有请求者范围类型的 `AllConfiguredConnectedOrganizationSubjects`分配策略中。   |
| unknownFutureValue    | 2     | 一个 sentinel 成员。                                                                                                                                                                                                 |

### <a name="identityuserflowattributedatatype-values"></a>identityUserFlowAttributeDataType 值

| 成员                | 值 | 说明                         |
|:----------------------|:------|:------------------------------------|
| string                | 1     | String 数据类型                    |
| boolean               | 2     | Boolean 数据类型                   |
| int64                 | 3     | Int 数据类型                       |
| stringCollection      | 4     | 字符串收集数据类型         |
|dateTime|5||
| unknownFutureValue    | 6      | 一个 sentinel 成员。                  |

### <a name="identityuserflowattributetype-values"></a>identityUserFlowAttributeType 值

| 成员                | 值 | 说明                                                        |
|:----------------------|:------|:-------------------------------------------------------------------|
| 内置               | 1     | 此用户流属性类型表示它是由系统创建的 |
| 自 定义                | 2     | 此用户流属性类型表示它是由用户创建的   |
|必需|3||
| unknownFutureValue    | 4     | 一个 sentinel 成员。                                                 |

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

| 成员
|:---
| entityUrl
| text

### <a name="cloudpcprovisioningpolicyimagetype-values"></a>cloudPcProvisioningPolicyImageType 值

|成员|
|:---|
|自 定义|
|库|

### <a name="chattype-values"></a>chatType 值

| 成员             | 值 | 说明               |
| :----------------- | :---- | :------------------------ |
|oneOnOne            | 0     | 指示聊天是 1：1 聊天。 对于这种类型的聊天，名册大小是固定的，无法删除/添加该成员。                  |
|组               | 1     | 指示聊天是群组聊天。 可以针对此类聊天更新至少 2 人) 的名册大小 (。 可以稍后删除/添加成员。   |
|会议             | 2     | 指示聊天是会议聊天，这是创建 OnlineMeeting 的副作用。  |
|unknownFutureValue  | 3     | 用于指示未来值的 Sentinel 值。 |

### <a name="singlesignonmode-values"></a>singleSignOnMode 值

|成员|
|:---|
|无|
|onPremisesKerberos|
|aadHeaderBased|
|pingHeaderBased|

### <a name="plannercontainertype-values"></a>plannerContainerType 值

|成员|
|:---|
|组|
|unknownFutureValue|
|名册|

### <a name="plannerplancontexttype-values"></a>plannerPlanContextType 值

|成员|
|:---|
|teamsTab|
|sharePointPage|
|meetingNotes|
|其他|
|unknownFutureValue|

### <a name="plannercontextstate-values"></a>plannerContextState 值

|成员             |
|:------------------|
|积极             |
|已取消链接           |
|unknownFutureValue |  


### <a name="policyscope-values"></a>policyScope 值

|成员|
|:---|
|无|
|所有|
|选择|

### <a name="teamsappinstallationscope-values"></a>teamsAppInstallationScope 值

|成员    |值    |说明 |
|:---------|:--------|:----------- |
|团队      |0        |指示可在团队中安装Teams应用，并有权访问该团队的数据。|
|groupChat |1        |指示可以在群聊中安装Teams应用，并有权访问该组聊天的数据。|
|personal  |2        |指示可在用户的个人范围内安装Teams应用，并有权访问该用户的数据。|

### <a name="roleassignmentschedulerequestfilterbycurrentuseroptions-values"></a>roleAssignmentScheduleRequestFilterByCurrentUserOptions 值

|成员|
|:---|
|主要|
|createdBy|
|审批者|
|unknownFutureValue|

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

### <a name="roleeligibilityschedulerequestfilterbycurrentuseroptions-values"></a>roleEligibilityScheduleRequestFilterByCurrentUserOptions 值

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

### <a name="cloudpcauditactivityoperationtype-values"></a>cloudPcAuditActivityOperationType 值

|成员|
|:---|
|create|
|delete|
|补丁|
|其他|

### <a name="cloudpcauditactivityresult-values"></a>cloudPcAuditActivityResult 值

|成员|
|:---|
|success|
|clientError|
|失败|
|timeout|
|其他|

### <a name="cloudpcauditactortype-values"></a>cloudPcAuditActorType 值

|成员|
|:---|
|itPro|
|应用程序|
|伙伴|
|unknown|

### <a name="cloudpcauditcategory-values"></a>cloudPcAuditCategory 值

|成员|
|:---|
|cloudPC|
|其他|

### <a name="posttype-values"></a>postType 值

|成员|
|:---|
|定期|
|快速|
|战略|
|unknownFutureValue|

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

### <a name="teamworktagtype-values"></a>teamworkTagType 值

|成员| 值 | 说明               |
|:---|:---- | :------------------------ |
|标准| 0     |标记的默认类型。 类型标准的标记可由拥有权限的成员在团队中管理。|

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

### <a name="callrecordingstatus-values"></a>callRecordingStatus 值

|成员|
|:---|
|success|
|失败|
|初始|
|chunkFinished|
|unknownFutureValue|

### <a name="payloaddeliveryplatform-values"></a>payloadDeliveryPlatform 值

|成员|
|:---|
|unknown|
|短信|
|电子邮件|
|团队|
|unknownFutureValue|

### <a name="trainingstatus-values"></a>trainingStatus 值

|成员|
|:---|
|unknown|
|分配|
|inProgress|
|完成|
|过期|
|unknownFutureValue|

### <a name="teamworkcalleventtype-values"></a>teamworkCallEventType 值

|成员|
|:---|
|通话|
|会议|
|screenShare|
|unknownFutureValue|

### <a name="binaryoperator-values"></a>binaryOperator 值 

|成员|
|:---|
|或|
|和|

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

### <a name="answerinputtype-values"></a>answerInputType 值

|成员|值|说明|
|:---|:---|:---|
|text|0|文本。|
|radioButton|1|RadioButton。|
|unknownFutureValue|2|UnknownFutureValue。|

### <a name="taskstatus_v2-values"></a>taskStatus_v2值

|成员|
|:---|
|notStarted|
|inProgress|
|完成|
|unknownFutureValue|


### <a name="wellknownlistname_v2-values"></a>wellKnownListName_v2值

|成员|
|:---|
|无|
|defaultList|
|flaggedEmail|
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

### <a name="bookingstaffrole-values"></a>bookingStaffRole 值 

|成员|
|:---|
|客人|
|管理员|
|观众|
|externalGuest|
|unknownFutureValue|

### <a name="bookingreminderrecipients-values"></a>bookingReminderRecipients 值 

|成员|
|:---|
|allAttendees|
|员工|
|客户|
|unknownFutureValue|

### <a name="teamworkconnectionstatus-values"></a>teamworkConnectionStatus 值

| 成员 |
|:--------|
|unknown|
|连接|
|断开|
|unknownFutureValue|

### <a name="teamworkdeviceactivitystate-values"></a>teamworkDeviceActivityState 值

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|unknown|0|未知状态。|
|忙|1|设备正忙。|
|闲置|2|设备处于空闲状态。|
|无法|3|设备不可用。|
|unknownFutureValue|4|可变枚举 sentinel 值。 请勿使用。|

### <a name="teamworkdeviceoperationtype-values"></a>teamworkDeviceOperationType 值

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|deviceRestart|0|重启设备。|
|configUpdate|1|更新设备配置。|
|deviceDiagnostics|2|获取设备日志。|
|softwareUpdate|3|更新设备上的软件。|
|deviceManagementAgentConfigUpdate|4|更新设备代理配置。|
|remoteLogin|5|设备远程登录。|
|remoteLogout|6 |设备远程注销。|
|unknownFutureValue|7 |可变枚举 sentinel 值。 请勿使用。|

### <a name="teamworksoftwarefreshness-values"></a>teamworkSoftwareFreshness 值

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|unknown|0|未知值。|
|最新|1|指示设备组件是否运行最新版本的软件。|
|updateAvailable|2|指示软件更新可用于设备组件。|
|unknownFutureValue|3|可变枚举 sentinel 值。 请勿使用。|

### <a name="teamworksoftwaretype-values"></a>teamworkSoftwareType 值

| 成员 |
|:---------------|
|adminAgent|
|operatingSystem|
|teamsClient|
|固件|
|partnerAgent|
|companyPortal|
|unknownFutureValue|

### <a name="teamworksupportedclient-values"></a>teamworkSupportedClient 值

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|unknown|0|未知值。|
|skypeDefaultAndTeams|1|同时支持这两者`Skype`。`Teams` 默认值为“`Skype`”。|
|teamsDefaultAndSkype|2|同时支持这两者`Skype`。`Teams` 默认值为“`Teams`”。|
|skypeOnly|3|仅 `Skype`支持 。|
|teamsOnly|4|仅 `Teams`支持 。|
|unknownFutureValue|5|可变枚举 sentinel 值。 请勿使用。|

### <a name="longrunningoperationstatus-values"></a>longRunningOperationStatus 值

| 成员|
|:-----------------|
|notStarted|
|运行|
|成功|
|失败|
|unknownFutureValue|

### <a name="delegatedadminaccessassignmentstatus-values"></a>delegatedAdminAccessAssignmentStatus 值 

|成员|
|:---|
|等待|
|积极|
|删除|
|deleted|
|error|
|unknownFutureValue|

### <a name="delegatedadminaccesscontainertype-values"></a>delegatedAdminAccessContainerType 值 

|成员|
|:---|
|securityGroup|
|unknownFutureValue|

### <a name="delegatedadminrelationshipoperationstatus-values"></a>delegatedAdminRelationshipOperationStatus 值 

|成员|
|:---|
|notStarted|
|运行|
|complete|
|失败|
|unknownFutureValue|

### <a name="delegatedadminrelationshipoperationtype-values"></a>delegatedAdminRelationshipOperationType 值 

|成员|
|:---|
|delegatedAdminAccessAssignmentUpdate|
|unknownFutureValue|

### <a name="delegatedadminrelationshiprequestaction-values"></a>delegatedAdminRelationshipRequestAction 值 

|成员|
|:---|
|lockForApproval|
|终止|
|unknownFutureValue|

### <a name="delegatedadminrelationshiprequeststatus-values"></a>delegatedAdminRelationshipRequestStatus 值 

|成员|
|:---|
|已创建|
|等待|
|complete|
|失败|
|unknownFutureValue|

### <a name="delegatedadminrelationshipstatus-values"></a>delegatedAdminRelationshipStatus 值 

|成员|
|:---|
|激活|
|积极|
|approvalPending|
|批准|
|已创建|
|过期|
|到期|
|终止|
|终止|
|terminationRequested|
|unknownFutureValue|
